## `postgres:12-bullseye`

```console
$ docker pull postgres@sha256:96a52e8b854304514790adcbd731032002146641dafc5b7732782e1c63f7071a
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

### `postgres:12-bullseye` - linux; amd64

```console
$ docker pull postgres@sha256:84a558c0b4f46347413bac529415b01a3658d5d90c9bef0bb1dcd34390401b05
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.3 MB (136278462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43dec67e8efe9a535d92be72ddfbdac833506a2b7e8c319908ee49273793cfdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 11:05:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 11:05:32 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 23 Mar 2023 11:05:32 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 11:05:40 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 11:05:47 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 23 Mar 2023 11:05:47 GMT
ENV LANG=en_US.utf8
# Thu, 23 Mar 2023 11:05:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 11:05:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Mar 2023 11:05:52 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 11:07:15 GMT
ENV PG_MAJOR=12
# Thu, 23 Mar 2023 11:07:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Thu, 23 Mar 2023 11:07:16 GMT
ENV PG_VERSION=12.14-1.pgdg110+1
# Thu, 23 Mar 2023 11:07:34 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 23 Mar 2023 11:07:35 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 23 Mar 2023 11:07:35 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Mar 2023 11:07:35 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Mar 2023 11:07:36 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Mar 2023 11:07:36 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 27 Mar 2023 22:30:16 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Mon, 27 Mar 2023 22:30:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Mar 2023 22:30:16 GMT
STOPSIGNAL SIGINT
# Mon, 27 Mar 2023 22:30:16 GMT
EXPOSE 5432
# Mon, 27 Mar 2023 22:30:16 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c04f8741265c9cb018d6e0dc852fa48d9ca605cc4a8b910701149c268b46c4c`  
		Last Modified: Thu, 23 Mar 2023 11:08:27 GMT  
		Size: 4.4 MB (4414969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffc353b86ebafc024e489eb30725dec939794c5c853d8c40e8a228061ef618d`  
		Last Modified: Thu, 23 Mar 2023 11:08:25 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c4a9e6c414bdb0cea88de7b9d555fb825bbbd7b3ceff82ac6de73109460c58`  
		Last Modified: Thu, 23 Mar 2023 11:08:26 GMT  
		Size: 1.5 MB (1471387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f47e7b385280253a608f12b70c590d831395a3efe2908bc3f1eb9f18ba06b6`  
		Last Modified: Thu, 23 Mar 2023 11:08:25 GMT  
		Size: 8.0 MB (8045374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e26c947960d4da4154c7610b237230df37598a1cc6fbcaf57e6aa25b10e7a9d`  
		Last Modified: Thu, 23 Mar 2023 11:08:24 GMT  
		Size: 1.3 MB (1261165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c3dc85e8c3b85d3f412d47e5e3091453f92a0ca1de2154fee0efd915202eb4`  
		Last Modified: Thu, 23 Mar 2023 11:08:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17df73636f012eaeb40d794735572017fd87f992aa4338ac562491cfcd3b8a6c`  
		Last Modified: Thu, 23 Mar 2023 11:08:23 GMT  
		Size: 3.2 KB (3201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05add2dd64c861381fece31e2f7ae8e575d5ac3d4d910fbb957b275ee3847cb7`  
		Last Modified: Thu, 23 Mar 2023 11:09:59 GMT  
		Size: 89.7 MB (89654882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8eca8be8b3c48e13878af35bd4fdf77967825ac255169926bc36c2d953da4e0`  
		Last Modified: Thu, 23 Mar 2023 11:09:47 GMT  
		Size: 9.0 KB (9023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf9a1dad65dc15e884baf8274967fde96ea4a9165804d624ab828a2c31c2edf`  
		Last Modified: Thu, 23 Mar 2023 11:09:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:194ad2944d69d6bd0e947d0bd5cfae92c486af9a23493fd9dc063a443dabcf1b`  
		Last Modified: Thu, 23 Mar 2023 11:09:47 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6fdfcde120cd26779680a9fcd264b674f2b85eb89d8f064ababd4a7172b77ca`  
		Last Modified: Mon, 27 Mar 2023 22:32:05 GMT  
		Size: 4.8 KB (4781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-bullseye` - linux; arm variant v5

```console
$ docker pull postgres@sha256:e37dc686df442b296b137ccc6de967b54633a91d863089273ce7be0fe1f32d8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129535892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:385b6bc806b90353214372b5f386b19d9e252a23ffd9e023d0ba943b1380fb57`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 23 Mar 2023 00:48:44 GMT
ADD file:7595c7bfa6b3741f57a3ec7790e3108bb526244e52bb4a54548b8b5541e66616 in / 
# Thu, 23 Mar 2023 00:48:44 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 05:41:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 05:41:44 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 23 Mar 2023 05:41:44 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 05:41:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 05:42:01 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 23 Mar 2023 05:42:01 GMT
ENV LANG=en_US.utf8
# Thu, 23 Mar 2023 05:42:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 05:42:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Mar 2023 05:42:09 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 25 Mar 2023 01:03:54 GMT
ENV PG_MAJOR=12
# Sat, 25 Mar 2023 01:03:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Sat, 25 Mar 2023 01:03:54 GMT
ENV PG_VERSION=12.14-1.pgdg110+1
# Sat, 25 Mar 2023 01:16:30 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Sat, 25 Mar 2023 01:16:31 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 25 Mar 2023 01:16:32 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 25 Mar 2023 01:16:32 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 25 Mar 2023 01:16:32 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 25 Mar 2023 01:16:32 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 07 Apr 2023 23:59:09 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Fri, 07 Apr 2023 23:59:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Apr 2023 23:59:10 GMT
STOPSIGNAL SIGINT
# Fri, 07 Apr 2023 23:59:10 GMT
EXPOSE 5432
# Fri, 07 Apr 2023 23:59:10 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:b83d345710cdef1626d1940689dd3160e5ce3e4f63b3154cf612c52b704baa66`  
		Last Modified: Thu, 23 Mar 2023 02:22:00 GMT  
		Size: 28.9 MB (28915852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b596a08513f5f10750e2615df1971bd90af28e28fac7ee07c14b2aeb3b7999d`  
		Last Modified: Sat, 25 Mar 2023 01:17:25 GMT  
		Size: 4.1 MB (4096504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648d61fe59a2d792ab82557840572e0e5f0109175839fdcd8c45456ae9a3285b`  
		Last Modified: Sat, 25 Mar 2023 01:17:24 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b13ffb35c1d1c6e3b0a43baa49961dc6b971b250f0fe9a4d63f558a59f30aa`  
		Last Modified: Sat, 25 Mar 2023 01:17:24 GMT  
		Size: 1.4 MB (1448662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0ab220b1e90dd4d594cd7c7ae5d8a7a7a455aa0b59dc50476e0ab77096991f`  
		Last Modified: Sat, 25 Mar 2023 01:17:24 GMT  
		Size: 8.0 MB (8045131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b781cef1e55785ae4f8dbdb8013b906a28cd5033f97d7c32d5bcb209b619588`  
		Last Modified: Sat, 25 Mar 2023 01:17:22 GMT  
		Size: 1.3 MB (1257266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0281e259b86d066ef1338563cdb0b418144d33fb5fd95b6de5424db6e694ae0`  
		Last Modified: Sat, 25 Mar 2023 01:17:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3b3c0d5ba475db73b0763716a29edcd77c0235c582caf9155089e0ff48bee1`  
		Last Modified: Sat, 25 Mar 2023 01:17:21 GMT  
		Size: 3.2 KB (3194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024cd2358238aece0a12345d9a80231249c2dfd22db96ccfaf22f76948153b6c`  
		Last Modified: Sat, 25 Mar 2023 01:18:59 GMT  
		Size: 85.8 MB (85753206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1221e08ad829f37f4fe97d9451f76814867d291ac8d75f9de5a50d573df57d`  
		Last Modified: Sat, 25 Mar 2023 01:18:46 GMT  
		Size: 9.0 KB (9030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628f9c5980dc188e9a3cf28e52e13bb37a89779fce93ff3c3e9eb08504b54da0`  
		Last Modified: Sat, 25 Mar 2023 01:18:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f72aaab675354ae138e88f070234d99eb843f0e3cdb3ac4e6804e635c1ddf3`  
		Last Modified: Sat, 25 Mar 2023 01:18:46 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7e7f163ade1831aa5ea065da7c350f7f76c51319385f4f48782d9306ef588f`  
		Last Modified: Fri, 07 Apr 2023 23:59:29 GMT  
		Size: 4.8 KB (4782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-bullseye` - linux; arm variant v7

```console
$ docker pull postgres@sha256:4a0a9078f72fef2a303ed3afd1bb204fc17739478ad4463487aa2004b262cd24
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124295265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82febb4996f3207ce3a1281f741f9b1bacd7719b9fbc21d4893c078732a15aa4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 10:58:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 10:58:17 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 23 Mar 2023 10:58:17 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 10:58:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 10:58:32 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 23 Mar 2023 10:58:32 GMT
ENV LANG=en_US.utf8
# Thu, 23 Mar 2023 10:58:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 10:58:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Mar 2023 10:58:38 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 11:36:06 GMT
ENV PG_MAJOR=12
# Thu, 23 Mar 2023 11:36:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Thu, 23 Mar 2023 11:36:06 GMT
ENV PG_VERSION=12.14-1.pgdg110+1
# Thu, 23 Mar 2023 11:47:31 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 23 Mar 2023 11:47:32 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 23 Mar 2023 11:47:33 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Mar 2023 11:47:33 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Mar 2023 11:47:33 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Mar 2023 11:47:34 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 27 Mar 2023 23:58:02 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Mon, 27 Mar 2023 23:58:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Mar 2023 23:58:02 GMT
STOPSIGNAL SIGINT
# Mon, 27 Mar 2023 23:58:02 GMT
EXPOSE 5432
# Mon, 27 Mar 2023 23:58:02 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3a8667968a2db1a4d8fdfe4de326db3f475b097b6bb67fd8c96aaf5aa1a1fa7`  
		Last Modified: Thu, 23 Mar 2023 11:59:17 GMT  
		Size: 3.7 MB (3717300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6bbc02bbbd7873d21e453b297a9054998edc6166c926089caa9bfee5a74f67`  
		Last Modified: Thu, 23 Mar 2023 11:59:16 GMT  
		Size: 1.8 KB (1791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe548cbd05be1647b4c58950c26d4ebc0b8d6715e97c8772b7eb1c803e8f6935`  
		Last Modified: Thu, 23 Mar 2023 11:59:16 GMT  
		Size: 1.4 MB (1438727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f5bdef234eb976f6da02f71c24a8ea2d93d64ce81699e9b92062a0c6efdd9c`  
		Last Modified: Thu, 23 Mar 2023 11:59:15 GMT  
		Size: 8.0 MB (8045293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517a1d4afc5c67eb89563508719ce343a997056a6aa3aeaf398487b6fac2881d`  
		Last Modified: Thu, 23 Mar 2023 11:59:14 GMT  
		Size: 1.1 MB (1131177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8069c9944fe98f6bd9941fc370d6728cc9e16e9c10739ad1cd2508adaf65a760`  
		Last Modified: Thu, 23 Mar 2023 11:59:14 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54b099283053085aa8d8acbd3366ee31e047486e58af6b8f02860f032e89adb`  
		Last Modified: Thu, 23 Mar 2023 11:59:14 GMT  
		Size: 3.2 KB (3200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9b52e68839ba8d1cae553f16edd5fbb90d8b9b9ec8931ed34b5781c0beafe5`  
		Last Modified: Thu, 23 Mar 2023 12:00:58 GMT  
		Size: 83.4 MB (83366159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7789a90241651156474e332450f9ee1940b96102e63e67e50b13c531dd28a0fc`  
		Last Modified: Thu, 23 Mar 2023 12:00:46 GMT  
		Size: 9.0 KB (9029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94078625a9838ed2de252fdae4b49a8d090170b104f6d82f40a64f29e854296a`  
		Last Modified: Thu, 23 Mar 2023 12:00:46 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0738388964847e23cc79a0e149023db9dd31c6cd6bbfb4dc2a5d5bf46ba81f61`  
		Last Modified: Thu, 23 Mar 2023 12:00:46 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82671a4b17d6a748e43cdf1e7ea6d05d02b44db6b388f55831882f4afb38bd43`  
		Last Modified: Tue, 28 Mar 2023 00:04:39 GMT  
		Size: 4.8 KB (4783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-bullseye` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:722cfe6b170650b9aaa17d8390e991da28c1d23ff4f0291ac89c0085de02c937
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131381141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa40ad5771b98d92924c0cdf82405328639da65dd8d074bc2a7561c28c1da206`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:28:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 13:28:19 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 23 Mar 2023 13:28:19 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 13:28:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 13:28:33 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 23 Mar 2023 13:28:33 GMT
ENV LANG=en_US.utf8
# Thu, 23 Mar 2023 13:28:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:28:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Mar 2023 13:28:38 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 13:29:58 GMT
ENV PG_MAJOR=12
# Thu, 23 Mar 2023 13:29:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Thu, 23 Mar 2023 13:29:58 GMT
ENV PG_VERSION=12.14-1.pgdg110+1
# Thu, 23 Mar 2023 13:30:11 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 23 Mar 2023 13:30:13 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 23 Mar 2023 13:30:14 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Mar 2023 13:30:14 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Mar 2023 13:30:14 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Mar 2023 13:30:14 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 28 Mar 2023 01:20:33 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Tue, 28 Mar 2023 01:20:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Mar 2023 01:20:33 GMT
STOPSIGNAL SIGINT
# Tue, 28 Mar 2023 01:20:33 GMT
EXPOSE 5432
# Tue, 28 Mar 2023 01:20:33 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4de29c30b99b39aed5a35ff544bb397a90bd47de48bcbd6555014b8a6f0b60c`  
		Last Modified: Thu, 23 Mar 2023 13:31:03 GMT  
		Size: 4.4 MB (4416207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e28158506a33fe300a3fabc8eeb43bb6afa873ac85c93eb56ea47b9c5f4b97f`  
		Last Modified: Thu, 23 Mar 2023 13:31:05 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53514e250b72009b86f4fb727db037d7bd0a3b2f9a5f1591e15fc13d4c0f7d8c`  
		Last Modified: Thu, 23 Mar 2023 13:31:02 GMT  
		Size: 1.4 MB (1403222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c081701961bb12cf06f601dfcdfa3f1ee1e2d1b009549600c0be0a51318323`  
		Last Modified: Thu, 23 Mar 2023 13:31:02 GMT  
		Size: 8.0 MB (8045308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33cfeaf50096d9814b4481c61121dfaf3e755f772974f3652841ce4eaaac768a`  
		Last Modified: Thu, 23 Mar 2023 13:31:00 GMT  
		Size: 1.2 MB (1249198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0a34468e21b167f0644c1d2af2e24967064548ded0d9bf90a29c7c3bb7dd82d`  
		Last Modified: Thu, 23 Mar 2023 13:31:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9edf60e692b4f0262a6a66c6d6a4e1bb9c4a4606b59d65377ce3e9775c781c4a`  
		Last Modified: Thu, 23 Mar 2023 13:31:00 GMT  
		Size: 3.2 KB (3198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e9e83b54dec923c0cf97149b320ed4f0d28c157fc5bb8459a7ee70f4f9aca6`  
		Last Modified: Thu, 23 Mar 2023 13:32:24 GMT  
		Size: 86.2 MB (86185222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bccadde54696b932bdb0d047108487240e31133f698ab3d0fce1e8d5e74984f9`  
		Last Modified: Thu, 23 Mar 2023 13:32:16 GMT  
		Size: 9.0 KB (9022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c1ac3577e862fab76f40382f5b86cd01315948209b238689340eabc3eafe5b`  
		Last Modified: Thu, 23 Mar 2023 13:32:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfca6411db40a3a1ea607728e4160988cac8d4202fab07321c43187ca7f8d096`  
		Last Modified: Thu, 23 Mar 2023 13:32:16 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eeedf287cc4b48447673f2e6c92f757b4b4b67ef6e487d29e7c7337ea9a9ae9`  
		Last Modified: Tue, 28 Mar 2023 01:22:18 GMT  
		Size: 4.8 KB (4782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-bullseye` - linux; 386

```console
$ docker pull postgres@sha256:4a315015098624a09fafea38d9a9670ccb856250e510f90419b342a2612d88f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.3 MB (138282550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:118751eea6557aca52e874ee3ed5bf7b45a47238919bc8814ee111164cdc24f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 23 Mar 2023 00:39:18 GMT
ADD file:315d843eefd4a8bb2345366dcd6bab00a06fca4a7970e220ae8946123d07d7ed in / 
# Thu, 23 Mar 2023 00:39:19 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 10:59:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 10:59:15 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 23 Mar 2023 10:59:15 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 10:59:24 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 10:59:31 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 23 Mar 2023 10:59:31 GMT
ENV LANG=en_US.utf8
# Thu, 23 Mar 2023 10:59:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 10:59:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Mar 2023 10:59:38 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 11:42:05 GMT
ENV PG_MAJOR=12
# Thu, 23 Mar 2023 11:42:05 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Thu, 23 Mar 2023 11:42:05 GMT
ENV PG_VERSION=12.14-1.pgdg110+1
# Thu, 23 Mar 2023 11:54:49 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 23 Mar 2023 11:54:50 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 23 Mar 2023 11:54:51 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Mar 2023 11:54:51 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Mar 2023 11:54:52 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Mar 2023 11:54:52 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 28 Mar 2023 02:38:17 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Tue, 28 Mar 2023 02:38:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Mar 2023 02:38:17 GMT
STOPSIGNAL SIGINT
# Tue, 28 Mar 2023 02:38:17 GMT
EXPOSE 5432
# Tue, 28 Mar 2023 02:38:17 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:3e638a975ea99fe8646002726dcb1ccdccc49ad33967b30337b9b2413e0619b5`  
		Last Modified: Thu, 23 Mar 2023 00:43:09 GMT  
		Size: 32.4 MB (32396277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b5efc39d67da7b52ec54a8ad72b8103590c4e63ab903d7ec703ab719c24fd2`  
		Last Modified: Thu, 23 Mar 2023 12:07:49 GMT  
		Size: 4.8 MB (4813530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba67f18258ea767381c586bbed5a3c15e7a488bfc2caa3b99ce1771ab9b7ef7`  
		Last Modified: Thu, 23 Mar 2023 12:07:47 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446760225b0f099934406c4f375ec245a5de5e8f6811146647baf0486d19cdfb`  
		Last Modified: Thu, 23 Mar 2023 12:07:47 GMT  
		Size: 1.4 MB (1446938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e560907e97a51eb7ba2276bbfff20c1db32c60f627fa2a03776df53c08391e19`  
		Last Modified: Thu, 23 Mar 2023 12:07:48 GMT  
		Size: 8.0 MB (8045241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27814b26385849b51a7063a8114af61e7342658147f027c5fc6c84aee576911c`  
		Last Modified: Thu, 23 Mar 2023 12:07:45 GMT  
		Size: 1.3 MB (1251648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100a5ac21d53d61c336bfca6501fc393b2c84eb7219b48f1a3372920e47fa318`  
		Last Modified: Thu, 23 Mar 2023 12:07:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7eb509452c7ea72442acea397c433e531f0fab32051a290ef62b2e508915e42`  
		Last Modified: Thu, 23 Mar 2023 12:07:45 GMT  
		Size: 3.2 KB (3198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9420118568ad4b97bc4109fbaeb0e965cc1edae5f4b1dc49e4e4f62df5891ac`  
		Last Modified: Thu, 23 Mar 2023 12:09:46 GMT  
		Size: 90.3 MB (90309636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d8e1cc0c5ed18436a41f7964890f70fa0085bf4f2cdd2275dcd9659b48f24e`  
		Last Modified: Thu, 23 Mar 2023 12:09:29 GMT  
		Size: 9.0 KB (9024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290359cee606582cb9bde11d1d113d3b6ddece1cbfd9346dc28043cad0c33d75`  
		Last Modified: Thu, 23 Mar 2023 12:09:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cd2bcea040275f1024a5d27591e30558a82bbbf3fef8d8c0cd1fc4355dff3e`  
		Last Modified: Thu, 23 Mar 2023 12:09:29 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6ee4afdc5c8faa9496fea203b9bafd32569d06b74be329161295f4dd11012c`  
		Last Modified: Tue, 28 Mar 2023 02:40:02 GMT  
		Size: 4.8 KB (4794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-bullseye` - linux; mips64le

```console
$ docker pull postgres@sha256:8518274577ee120808c207330f71a28ac461607732a8e847ebeaf1017fa79944
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130695331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:341cb1147db3188dad8d6c178a0914639ea2d1b29faecf2486fdb9cafaabc4ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 23 Mar 2023 05:17:57 GMT
ADD file:fd3a8eec4ae8f6058f522536ca9af1b391f3032504c085d8ddb6f4878ca478d5 in / 
# Thu, 23 Mar 2023 05:18:02 GMT
CMD ["bash"]
# Fri, 24 Mar 2023 00:01:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 24 Mar 2023 00:01:43 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 24 Mar 2023 00:01:45 GMT
ENV GOSU_VERSION=1.16
# Fri, 24 Mar 2023 00:02:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Mar 2023 00:02:45 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Fri, 24 Mar 2023 00:02:47 GMT
ENV LANG=en_US.utf8
# Fri, 24 Mar 2023 00:03:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Mar 2023 00:03:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Mar 2023 00:03:15 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 24 Mar 2023 03:03:37 GMT
ENV PG_MAJOR=12
# Fri, 24 Mar 2023 03:03:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Fri, 24 Mar 2023 03:03:42 GMT
ENV PG_VERSION=12.14-1.pgdg110+1
# Fri, 24 Mar 2023 03:58:38 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 24 Mar 2023 03:58:45 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 24 Mar 2023 03:58:51 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 24 Mar 2023 03:58:54 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 24 Mar 2023 03:58:59 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 24 Mar 2023 03:59:03 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 28 Mar 2023 01:11:26 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Tue, 28 Mar 2023 01:11:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Mar 2023 01:11:32 GMT
STOPSIGNAL SIGINT
# Tue, 28 Mar 2023 01:11:36 GMT
EXPOSE 5432
# Tue, 28 Mar 2023 01:11:39 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:735f9e60414e17ec59baef702f7013b7327899801df2ecf10123ce2727d8dea5`  
		Last Modified: Thu, 23 Mar 2023 05:25:53 GMT  
		Size: 29.6 MB (29634483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f99e1729f3fe396e54005c638a841adbc8d91d377d7477477beee661c93ab65`  
		Last Modified: Fri, 24 Mar 2023 04:54:15 GMT  
		Size: 4.2 MB (4196296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03cd6a7f7dbefc0d6edad4cac9d3305bb9b2e65e63694e81eb6ca68b8c2e0ecb`  
		Last Modified: Fri, 24 Mar 2023 04:54:11 GMT  
		Size: 1.7 KB (1655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09e8b2ec035b7d03a3d62bc303d0f4236caaeb19286e8ed719ba86c876bc99d`  
		Last Modified: Fri, 24 Mar 2023 04:54:12 GMT  
		Size: 1.4 MB (1358242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f194c2ef27189c68e61ca346b1dbbe915027f0043051c9328208db69b0d27f5`  
		Last Modified: Fri, 24 Mar 2023 04:54:15 GMT  
		Size: 8.0 MB (8043844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7f618231d553098705ab70a718b95b9fdcff585305e1bf045d247a0f4e39d1`  
		Last Modified: Fri, 24 Mar 2023 04:54:09 GMT  
		Size: 1.1 MB (1089515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f864e76dd744496c5e6df154192dcf1309ffd336f98a0359adbee0531586b236`  
		Last Modified: Fri, 24 Mar 2023 04:54:09 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d961bb093587b7196b7ba7d0fa06da37079b393d89ad7c544394d8ba070e4f22`  
		Last Modified: Fri, 24 Mar 2023 04:54:09 GMT  
		Size: 3.1 KB (3142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37302eab5e82fb934bf2239113932918e0a044807328ff42706c094b2caf057`  
		Last Modified: Fri, 24 Mar 2023 04:58:32 GMT  
		Size: 86.4 MB (86353921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d157a33cb65331346a5fff579881ec495443cdcaf4fe899b61577d84906281`  
		Last Modified: Fri, 24 Mar 2023 04:57:39 GMT  
		Size: 9.0 KB (9033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b6796a520a8f18c2c3ef3895c24cd4618affd061a65b69feb6c1dd625b88e2`  
		Last Modified: Fri, 24 Mar 2023 04:57:39 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1afcf48c602b1c8a55545c1549ba3796f647c42f5e356685a93753a8cd369ca1`  
		Last Modified: Fri, 24 Mar 2023 04:57:39 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3e8e08b5f3d784103b0be72c7a5a7bdfbe2d78e6ecf761a54632be68796989`  
		Last Modified: Tue, 28 Mar 2023 01:13:12 GMT  
		Size: 4.8 KB (4786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-bullseye` - linux; ppc64le

```console
$ docker pull postgres@sha256:1589fcce74f7ad49e1c24cf213deb8d37aa4b58f7ff5bdcff9326aa0e64de685
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.2 MB (145222564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efb44974301fbef5f41cb8d335e0e3d93a12b66fd35553762ac7a6447b19eeaa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 12 Apr 2023 00:08:20 GMT
ADD file:63eb52aaff02c15bceabb87a78eb1b36389066ff4774cf8a754160ca7d509816 in / 
# Wed, 12 Apr 2023 00:08:23 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 05:02:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 05:02:55 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 12 Apr 2023 05:02:55 GMT
ENV GOSU_VERSION=1.16
# Wed, 12 Apr 2023 05:03:15 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 12 Apr 2023 05:03:30 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 12 Apr 2023 05:03:31 GMT
ENV LANG=en_US.utf8
# Wed, 12 Apr 2023 05:03:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 05:03:43 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 12 Apr 2023 05:03:45 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 12 Apr 2023 05:08:07 GMT
ENV PG_MAJOR=12
# Wed, 12 Apr 2023 05:08:07 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Wed, 12 Apr 2023 05:08:08 GMT
ENV PG_VERSION=12.14-1.pgdg110+1
# Wed, 12 Apr 2023 05:09:00 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 12 Apr 2023 05:09:06 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 12 Apr 2023 05:09:08 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 12 Apr 2023 05:09:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 12 Apr 2023 05:09:10 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 12 Apr 2023 05:09:10 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 12 Apr 2023 05:09:10 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Wed, 12 Apr 2023 05:09:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Apr 2023 05:09:11 GMT
STOPSIGNAL SIGINT
# Wed, 12 Apr 2023 05:09:12 GMT
EXPOSE 5432
# Wed, 12 Apr 2023 05:09:12 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5b41d5ec640939cf684959234ad3b80909268a32bfd520a31c6720a91521c2fa`  
		Last Modified: Wed, 12 Apr 2023 00:13:13 GMT  
		Size: 35.3 MB (35291995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccb1ca2e8082d7f2e908c0f65ecfca3cb5a0e476d3fd37e81690608c036d044`  
		Last Modified: Wed, 12 Apr 2023 05:10:57 GMT  
		Size: 5.2 MB (5222909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3ecbb301ff302aec5f49ff035102a2f07531dbe1c21358695d166ab7a15658`  
		Last Modified: Wed, 12 Apr 2023 05:10:55 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508555663cada6c60557882d6189b4d045a4aa289ccf31dac997bd59b6387a9c`  
		Last Modified: Wed, 12 Apr 2023 05:10:55 GMT  
		Size: 1.4 MB (1393372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78a033a897e17a1245626e4ccaf84c5060086835b2f66bba8812cb8221a4afc`  
		Last Modified: Wed, 12 Apr 2023 05:10:56 GMT  
		Size: 8.0 MB (8045553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1d7d764d1b4a1e87a59e66a9cf5965f688361d41570c2ab5b26e7e69ac6fe6`  
		Last Modified: Wed, 12 Apr 2023 05:10:53 GMT  
		Size: 1.4 MB (1420262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e66b07f0bb7da9ebb8303127eb0799e5f983297c86857bfbba37e0b2b2d4a9b1`  
		Last Modified: Wed, 12 Apr 2023 05:10:53 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3262e34438ad23be530486ecba19d8e44ade415898517f06476504621b12bae2`  
		Last Modified: Wed, 12 Apr 2023 05:10:53 GMT  
		Size: 3.2 KB (3198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3471d62d5daa0ecfa29c41cdf195dbb66b0018266c9e2494164ed24f786b2a`  
		Last Modified: Wed, 12 Apr 2023 05:13:14 GMT  
		Size: 93.8 MB (93829178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285caa8b237724fe01e5841003c2d30acecfe8d40eac5c5470baad367bdce0ef`  
		Last Modified: Wed, 12 Apr 2023 05:12:52 GMT  
		Size: 9.0 KB (9029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92674a242cc11bd871c35dd2bac097e1625760c20f918f8aa21a16804f65723b`  
		Last Modified: Wed, 12 Apr 2023 05:12:52 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c040697e724bd9dcc7b768712c8a8d667854467a92fc7df2a7132b0bb1c60a`  
		Last Modified: Wed, 12 Apr 2023 05:12:52 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cc953f50268dfcdd6fb108e2783ac0b5663a4b15ea3f54b7baaaf3afe74df2`  
		Last Modified: Wed, 12 Apr 2023 05:12:52 GMT  
		Size: 4.8 KB (4785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-bullseye` - linux; s390x

```console
$ docker pull postgres@sha256:8483f57a59049b0c0ea7a110c0b306ed6b3b3d068b4f6850799115c5e0eb493d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.0 MB (140026554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e540c9b5c29f039b00a3bc1d368e88f0af832a9ddaa7224611bc624e544879c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 23 Mar 2023 00:44:06 GMT
ADD file:8b6d3f57adaa8af2e0599a6468c50b713d281165b4e61150850bedf587f7ad4f in / 
# Thu, 23 Mar 2023 00:44:08 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 11:21:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 11:21:04 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 23 Mar 2023 11:21:04 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 11:21:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 11:21:16 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 23 Mar 2023 11:21:16 GMT
ENV LANG=en_US.utf8
# Thu, 23 Mar 2023 11:21:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 11:21:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Mar 2023 11:21:21 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 11:47:00 GMT
ENV PG_MAJOR=12
# Thu, 23 Mar 2023 11:47:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Thu, 23 Mar 2023 11:47:01 GMT
ENV PG_VERSION=12.14-1.pgdg110+1
# Thu, 23 Mar 2023 11:55:52 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 23 Mar 2023 11:55:57 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 23 Mar 2023 11:55:57 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Mar 2023 11:55:57 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Mar 2023 11:55:58 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Mar 2023 11:55:58 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 28 Mar 2023 00:09:02 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Tue, 28 Mar 2023 00:09:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Mar 2023 00:09:02 GMT
STOPSIGNAL SIGINT
# Tue, 28 Mar 2023 00:09:02 GMT
EXPOSE 5432
# Tue, 28 Mar 2023 00:09:02 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:25d08e051bb75230bad82e3a7a054083beec6b4f6a46c8345c731582c297a408`  
		Last Modified: Thu, 23 Mar 2023 00:47:20 GMT  
		Size: 29.6 MB (29646820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e18e93532c47246c3e9d57ecb387990e7550eea2787dae7037142d19e01337a`  
		Last Modified: Thu, 23 Mar 2023 12:05:48 GMT  
		Size: 4.3 MB (4302258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73de5c12adebd6a7a0dc2589be59a06e4f17976c3866d76a38cf50445e545195`  
		Last Modified: Thu, 23 Mar 2023 12:05:47 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cfe3000adb28f647c1e4e0c03addef7c47e742a2afd401faabfc0e1e544f2d9`  
		Last Modified: Thu, 23 Mar 2023 12:05:47 GMT  
		Size: 1.4 MB (1436969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38bad433379bb95836e22787c14c0020c31aee2487d83ffd945b5830795ea25`  
		Last Modified: Thu, 23 Mar 2023 12:05:47 GMT  
		Size: 8.1 MB (8099253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a1552993a1e18aec49dbe9c1620df541b14ea8bae5854d1128d03a9b6a9804`  
		Last Modified: Thu, 23 Mar 2023 12:05:46 GMT  
		Size: 1.2 MB (1237928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4266bfab125be5fc09061853d0826b2efd8e64d56db2761f056141dfbcd572a`  
		Last Modified: Thu, 23 Mar 2023 12:05:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b05f15f4a85e9df955d88f52cdefc7820f61d84059d52cfe0a4aae9b90e94bc`  
		Last Modified: Thu, 23 Mar 2023 12:05:46 GMT  
		Size: 3.2 KB (3197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce20532725efa00b1878fd217eb96892d1d19ad1b66e7622477dc3f88205d878`  
		Last Modified: Thu, 23 Mar 2023 12:06:47 GMT  
		Size: 95.3 MB (95284037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4df7c1e3d6d141868234e0a00530778dca0b973f50c5219d276b4b68c73df44`  
		Last Modified: Thu, 23 Mar 2023 12:06:35 GMT  
		Size: 9.0 KB (9029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa4ad01f3e28a5b187a76ed7d0e3af5c0414907fd00163b9a00e05325de128a`  
		Last Modified: Thu, 23 Mar 2023 12:06:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e7d23a8ac9757e1c4fdad3122a5c3df75a91144a6a4cf9e7a699c65a012b47`  
		Last Modified: Thu, 23 Mar 2023 12:06:34 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43472336c48961193a86d7e1fc60b7da0912081b0b3d025948d64589ae9838d`  
		Last Modified: Tue, 28 Mar 2023 00:10:34 GMT  
		Size: 4.8 KB (4782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
