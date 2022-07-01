## `postgres:15beta2-bullseye`

```console
$ docker pull postgres@sha256:59bb12db3f7cb14eed6bd9911be4ad5a9adb073898c25454fd5d07953bbb1f40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `postgres:15beta2-bullseye` - linux; amd64

```console
$ docker pull postgres@sha256:74e5861966b113c2241b3eae710ba91b43f4dc8ff8c601856f4b220a25ca8c72
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.8 MB (139804012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67ca4432cec3780f92047fcab4917bec681ecaafdb4e42aee895a48b43a34107`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:27 GMT
ADD file:8adbbab04d6f84cd83b5f4205b89b0acb7ecbf27a1bb2dc181d0a629479039fe in / 
# Thu, 23 Jun 2022 00:20:27 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 14:26:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 14:26:14 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 23 Jun 2022 14:26:14 GMT
ENV GOSU_VERSION=1.14
# Thu, 23 Jun 2022 14:26:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Jun 2022 14:26:28 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 23 Jun 2022 14:26:28 GMT
ENV LANG=en_US.utf8
# Thu, 23 Jun 2022 14:26:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 14:26:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Jun 2022 14:26:34 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 23 Jun 2022 14:26:34 GMT
ENV PG_MAJOR=15
# Thu, 23 Jun 2022 14:26:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Fri, 01 Jul 2022 01:58:11 GMT
ENV PG_VERSION=15~beta2-1.pgdg110+1
# Fri, 01 Jul 2022 01:58:35 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 01 Jul 2022 01:58:36 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 01 Jul 2022 01:58:36 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 01 Jul 2022 01:58:36 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 01 Jul 2022 01:58:37 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 01 Jul 2022 01:58:37 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 01 Jul 2022 01:58:37 GMT
COPY file:925d466681c8349f58385c00a8caa567c76b695158aa04bf4ad2ac92604e11c7 in /usr/local/bin/ 
# Fri, 01 Jul 2022 01:58:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Jul 2022 01:58:37 GMT
STOPSIGNAL SIGINT
# Fri, 01 Jul 2022 01:58:38 GMT
EXPOSE 5432
# Fri, 01 Jul 2022 01:58:38 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:b85a868b505ffd0342a37e6a3b1c49f7c71878afe569a807e6238ef08252fcb7`  
		Last Modified: Thu, 23 Jun 2022 00:25:18 GMT  
		Size: 31.4 MB (31379408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53bada42f30af6cb05b321cd1476f8e7618dfcf89614107050a261436b1097c`  
		Last Modified: Thu, 23 Jun 2022 14:31:40 GMT  
		Size: 4.4 MB (4414594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303bde9620f54624dd5ac06c8d299c420b8f422d086bc30b5ad3728419ecf171`  
		Last Modified: Thu, 23 Jun 2022 14:31:38 GMT  
		Size: 1.8 KB (1801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c32c0c0a1b9965aeb753d022e0574c5c29890183dbd91a4409659c6b651802e`  
		Last Modified: Thu, 23 Jun 2022 14:31:39 GMT  
		Size: 1.4 MB (1418435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302630a57c0605eca44604de509d0c938ec26c3d5ed27f87c11b643b113873f4`  
		Last Modified: Thu, 23 Jun 2022 14:31:38 GMT  
		Size: 8.0 MB (8045420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfead4dfb390e7fdf514870fbbd258dc62ad3457eda7281a7f0e8d567c7d067`  
		Last Modified: Thu, 23 Jun 2022 14:31:37 GMT  
		Size: 1.3 MB (1261185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d9917b93099eb77b625877b1f755d24af442568a78fc0805c0b09e3d23cda1`  
		Last Modified: Thu, 23 Jun 2022 14:31:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb0d8ea11e0d46901df9f6d54845c7aa10fb73ac29b8c22648afa2a308808ac`  
		Last Modified: Thu, 23 Jun 2022 14:31:36 GMT  
		Size: 3.2 KB (3201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcd284804b1e3f22a35ca889c458f5cf253a0a99e03fb8393722bb10cc2afd0`  
		Last Modified: Fri, 01 Jul 2022 02:03:43 GMT  
		Size: 93.3 MB (93264989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9830de421a6f7c7398a17a2428424ae724866e0ae5a01fec6a1af3b467b6a7d`  
		Last Modified: Fri, 01 Jul 2022 02:03:30 GMT  
		Size: 9.8 KB (9795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39abfc956feffe2ac3b616a32aa139a26d5ad3b511a314c9b3ccbccff87d40e5`  
		Last Modified: Fri, 01 Jul 2022 02:03:30 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1992d7b42e1582489b9f7b673939fd11ce6d345c06a9f7aec2d266c90f6f60f`  
		Last Modified: Fri, 01 Jul 2022 02:03:30 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6fa5f2cbb4dd4e2092069332e1e265a4679afc45923379e0cbc94c337e8dae`  
		Last Modified: Fri, 01 Jul 2022 02:03:30 GMT  
		Size: 4.7 KB (4703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta2-bullseye` - linux; arm variant v5

```console
$ docker pull postgres@sha256:c05187a6ae743a062893cd60d66fa4ceb0715e6525d3b99e868ba24b493a23db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.5 MB (134490090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:456b83a9dcfe605517c08b13140f4e2dad4d68129ef57b1851c7b877f2acc856`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 23 Jun 2022 00:50:38 GMT
ADD file:839c0e211e2260f5d54f2633e53c817c1f59e2394ba4b12f60e01e46cee61011 in / 
# Thu, 23 Jun 2022 00:50:39 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 08:30:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 08:30:18 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 23 Jun 2022 08:30:19 GMT
ENV GOSU_VERSION=1.14
# Thu, 23 Jun 2022 08:30:41 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Jun 2022 08:31:04 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 23 Jun 2022 08:31:04 GMT
ENV LANG=en_US.utf8
# Thu, 23 Jun 2022 08:31:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 08:31:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Jun 2022 08:31:20 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 23 Jun 2022 08:31:20 GMT
ENV PG_MAJOR=15
# Thu, 23 Jun 2022 08:31:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Fri, 01 Jul 2022 01:19:52 GMT
ENV PG_VERSION=15~beta2-1.pgdg110+1
# Fri, 01 Jul 2022 01:59:27 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 01 Jul 2022 01:59:29 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 01 Jul 2022 01:59:30 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 01 Jul 2022 01:59:31 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 01 Jul 2022 01:59:32 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 01 Jul 2022 01:59:33 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 01 Jul 2022 01:59:33 GMT
COPY file:925d466681c8349f58385c00a8caa567c76b695158aa04bf4ad2ac92604e11c7 in /usr/local/bin/ 
# Fri, 01 Jul 2022 01:59:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Jul 2022 01:59:34 GMT
STOPSIGNAL SIGINT
# Fri, 01 Jul 2022 01:59:35 GMT
EXPOSE 5432
# Fri, 01 Jul 2022 01:59:35 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:bd2d3b4056bd1b0310082fc5d17c6d03348601456c4b9306d1a333f1cec561f9`  
		Last Modified: Thu, 23 Jun 2022 01:05:39 GMT  
		Size: 28.9 MB (28921550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1528a45687a21e84bfd794de80b4b48bed7b5cfee1e713005589cdd227f190f6`  
		Last Modified: Thu, 23 Jun 2022 13:02:42 GMT  
		Size: 4.1 MB (4096605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91dfe8b4a0d84f97547b3cd95a77325f39a56d7e09b5c6cada6a6899719eb86b`  
		Last Modified: Thu, 23 Jun 2022 13:02:39 GMT  
		Size: 1.8 KB (1792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b899e4f4c313fe9dd5851822686a2c01bab253137a24c2209e0363720e9a7c64`  
		Last Modified: Thu, 23 Jun 2022 13:02:39 GMT  
		Size: 1.4 MB (1382670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eecc13760e9f728491b83588c8efa1bad2e8459c690854d2b9dc4ce04a3d0c3f`  
		Last Modified: Thu, 23 Jun 2022 13:02:44 GMT  
		Size: 8.0 MB (8045435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4888133f250330d22c607a07094c1505f6226990a800434feb9417c27adb209d`  
		Last Modified: Thu, 23 Jun 2022 13:02:38 GMT  
		Size: 1.3 MB (1257360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7acb6160cb60f95794d4cb7491038bf35ae77a476da6f205d41690b29a636e84`  
		Last Modified: Thu, 23 Jun 2022 13:02:37 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a68e5a67bb9d626a7eb08a175139d61c94dbcaacf4208e54a69d28efc2cabb89`  
		Last Modified: Thu, 23 Jun 2022 13:02:37 GMT  
		Size: 3.2 KB (3201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd47d2f047f4f43c357e7a855545fcc0e086408736e51a9f51129fac92ac249`  
		Last Modified: Fri, 01 Jul 2022 02:03:51 GMT  
		Size: 90.8 MB (90766504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d0399013275c07ade0c4ed71d094eaf864bf73f141fc5a2e3decdc8e12a72f`  
		Last Modified: Fri, 01 Jul 2022 02:03:01 GMT  
		Size: 9.8 KB (9789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2467604a1dac5f9be94cc9786504912b360ffab9f150e30fbe921c01fb5fed`  
		Last Modified: Fri, 01 Jul 2022 02:03:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff4fe96654eaf564411b81715f8fae44dedeec405cafeba79fb563ba96f93d3`  
		Last Modified: Fri, 01 Jul 2022 02:03:01 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6edee4cbd485672033056f1b55e4576a3a3d7cd36950f1f3901fdcd9ca57767`  
		Last Modified: Fri, 01 Jul 2022 02:03:01 GMT  
		Size: 4.7 KB (4704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta2-bullseye` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:b5f9e100cda79ae2ea4177f7c2d47360e50a1085b1f8abf61f17b77c2269675b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.5 MB (134460856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad9354cba03aefcc85474baf531de0108f9be9c9afec8fcd60def23375c7778b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 08:47:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 08:47:15 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 23 Jun 2022 08:47:16 GMT
ENV GOSU_VERSION=1.14
# Thu, 23 Jun 2022 08:47:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Jun 2022 08:47:32 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 23 Jun 2022 08:47:33 GMT
ENV LANG=en_US.utf8
# Thu, 23 Jun 2022 08:47:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 08:47:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Jun 2022 08:47:40 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 23 Jun 2022 08:47:41 GMT
ENV PG_MAJOR=15
# Thu, 23 Jun 2022 08:47:42 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Fri, 01 Jul 2022 00:47:02 GMT
ENV PG_VERSION=15~beta2-1.pgdg110+1
# Fri, 01 Jul 2022 00:47:22 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 01 Jul 2022 00:47:23 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 01 Jul 2022 00:47:24 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 01 Jul 2022 00:47:25 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 01 Jul 2022 00:47:26 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 01 Jul 2022 00:47:27 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 01 Jul 2022 00:47:29 GMT
COPY file:925d466681c8349f58385c00a8caa567c76b695158aa04bf4ad2ac92604e11c7 in /usr/local/bin/ 
# Fri, 01 Jul 2022 00:47:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Jul 2022 00:47:30 GMT
STOPSIGNAL SIGINT
# Fri, 01 Jul 2022 00:47:31 GMT
EXPOSE 5432
# Fri, 01 Jul 2022 00:47:32 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d019bcaa13826cb59d653d18da03c778e4115b5f01bc14b348df2b7da19da06`  
		Last Modified: Thu, 23 Jun 2022 09:13:17 GMT  
		Size: 4.2 MB (4209041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c6496d90a8f53ba58fcd3b65b9aa02486e07875bd15d7c961fd40b48f8f715`  
		Last Modified: Thu, 23 Jun 2022 09:13:16 GMT  
		Size: 1.6 KB (1650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994bae8aa9406084a7d7b1db15a5048d915fd420f7879fe03ee823f43e07224f`  
		Last Modified: Thu, 23 Jun 2022 09:13:17 GMT  
		Size: 1.3 MB (1346184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:255bac0c560b70d77007723570b56c77164a7f1dc1568c0f93a456c4145ab462`  
		Last Modified: Thu, 23 Jun 2022 09:13:16 GMT  
		Size: 8.0 MB (8043612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f605281268d731048a8399f5c9e0082e88518d20d2ba64e0dd8215cd5667f447`  
		Last Modified: Thu, 23 Jun 2022 09:13:15 GMT  
		Size: 1.0 MB (1025848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0037c6d29459637d2c6a94812e6d4e0050cf7475c3a8c8e87d8956e8859e5e3`  
		Last Modified: Thu, 23 Jun 2022 09:13:14 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064e9138f07b410f97c672ead7ebdf37053caa5b019bafb4005a0ac8d3e30917`  
		Last Modified: Thu, 23 Jun 2022 09:13:14 GMT  
		Size: 3.1 KB (3141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2921d8faea2cc31b168254a8f8988b7db3cba697cbac0c9faf234428f39d4b6a`  
		Last Modified: Fri, 01 Jul 2022 00:54:19 GMT  
		Size: 89.8 MB (89750754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:557fe4b889490d5fd58cb67eb23dcc73ba6d72e0933cc1371b900f4ed78033c3`  
		Last Modified: Fri, 01 Jul 2022 00:54:07 GMT  
		Size: 9.8 KB (9790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141f2c02eb3d9b1fd3fd6aecaafd4e74560fc51850a7928c1dc0f2aeb0b585ff`  
		Last Modified: Fri, 01 Jul 2022 00:54:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:820544b467d7aeba4e4fd84a80a9e7ba7af624d15c7d71f27b444c593e99d508`  
		Last Modified: Fri, 01 Jul 2022 00:54:06 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d37070834a7d4228a5f3c4d29c8cef66b98261be4bed7c0552bb2bc43fc66b`  
		Last Modified: Fri, 01 Jul 2022 00:54:07 GMT  
		Size: 4.7 KB (4700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta2-bullseye` - linux; 386

```console
$ docker pull postgres@sha256:5cd644019c7866782ff3d4354667827390404c6dd1d4404849335a9043b472dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.2 MB (143186020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be67b791f7bcb753479251809423ab27a918cc20b4d61ffb8eb22beb2cc3c8a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 23 Jun 2022 00:39:33 GMT
ADD file:9d46d3f8fb63833a6dbd8dd796ad541d556046a48342d22e1fd3bffa3fb8e504 in / 
# Thu, 23 Jun 2022 00:39:33 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 10:03:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 10:03:55 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 23 Jun 2022 10:03:56 GMT
ENV GOSU_VERSION=1.14
# Thu, 23 Jun 2022 10:04:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Jun 2022 10:04:11 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 23 Jun 2022 10:04:11 GMT
ENV LANG=en_US.utf8
# Thu, 23 Jun 2022 10:04:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 10:04:17 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Jun 2022 10:04:19 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 23 Jun 2022 10:04:20 GMT
ENV PG_MAJOR=15
# Thu, 23 Jun 2022 10:04:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Fri, 01 Jul 2022 00:38:54 GMT
ENV PG_VERSION=15~beta2-1.pgdg110+1
# Fri, 01 Jul 2022 00:52:36 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 01 Jul 2022 00:52:36 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 01 Jul 2022 00:52:37 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 01 Jul 2022 00:52:38 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 01 Jul 2022 00:52:39 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 01 Jul 2022 00:52:40 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 01 Jul 2022 00:52:42 GMT
COPY file:925d466681c8349f58385c00a8caa567c76b695158aa04bf4ad2ac92604e11c7 in /usr/local/bin/ 
# Fri, 01 Jul 2022 00:52:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Jul 2022 00:52:43 GMT
STOPSIGNAL SIGINT
# Fri, 01 Jul 2022 00:52:44 GMT
EXPOSE 5432
# Fri, 01 Jul 2022 00:52:45 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:4870b12e407743816673c11cfb39974d80c1569d876287bef61f8c585954822f`  
		Last Modified: Thu, 23 Jun 2022 00:46:40 GMT  
		Size: 32.4 MB (32390198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a815fde110b4f4c5e4780320ba2daeaeabc65198ec76c379fa9151873da9ce`  
		Last Modified: Thu, 23 Jun 2022 11:22:59 GMT  
		Size: 4.6 MB (4606898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09de2f39d0d670d63cd25bbe33f6453594846285564fe7c0f2b607d246a63885`  
		Last Modified: Thu, 23 Jun 2022 11:22:57 GMT  
		Size: 1.6 KB (1643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a3d063d529ea34ce96c2e3efc157c3da42e5ad4cdbd1baa487f97eb71229fc`  
		Last Modified: Thu, 23 Jun 2022 11:22:58 GMT  
		Size: 1.4 MB (1385086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e23c1af65c34ab50691c50716b0f441ba60748bee864e64dabf37816defa04`  
		Last Modified: Thu, 23 Jun 2022 11:22:57 GMT  
		Size: 8.0 MB (8043636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea1501def2f9f08add48981469f79176afc475ecc7129015f3eae4f88b9e935`  
		Last Modified: Thu, 23 Jun 2022 11:22:56 GMT  
		Size: 1.0 MB (1027948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8158424953b3f8de3fcae5f292295443937338dd750f21fd60e91789310047a`  
		Last Modified: Thu, 23 Jun 2022 11:22:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6da7dc3bcf2c4a8e538b7d91bbc8cb0771db6deec73fd85d663acc42a520da`  
		Last Modified: Thu, 23 Jun 2022 11:22:55 GMT  
		Size: 3.1 KB (3141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098015e48d53263d2c908994404d42678583f7f3e4ea441d63188517a85a3430`  
		Last Modified: Fri, 01 Jul 2022 01:00:16 GMT  
		Size: 95.7 MB (95712556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9768b70dbe84272baa432cb9eed5555c76d69bdbe7be98f3c8427cc451110834`  
		Last Modified: Fri, 01 Jul 2022 01:00:04 GMT  
		Size: 9.8 KB (9793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7806e9f1c5c0e620c4f0fa3775c19c8f0cfdd9f4614d4af80209f96eb41b3116`  
		Last Modified: Fri, 01 Jul 2022 01:00:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044c36f4d1731309cb68f257bb7abaea53abdbce79168cbebb2e14051d120836`  
		Last Modified: Fri, 01 Jul 2022 01:00:04 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f240b38dbb45251512a985cb6004cfd0d1390c4a6b1d6d8e450e744fb51e24f7`  
		Last Modified: Fri, 01 Jul 2022 01:00:04 GMT  
		Size: 4.7 KB (4706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta2-bullseye` - linux; ppc64le

```console
$ docker pull postgres@sha256:cf40f317b5b2604e318a363b3aaeb0e3dc62f2152a8aad83c43654a058809e75
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.9 MB (148901600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61d851e0c5cd44209fbeb415ffc3b59b4ba4dbd70fb5dd617695a76dc3606d84`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 23 Jun 2022 02:02:32 GMT
ADD file:e18c13649ea1f145047652c8e171c4824f9b6b0dbc92127a914c7fca910acf96 in / 
# Thu, 23 Jun 2022 02:02:34 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 17:54:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 17:54:34 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 23 Jun 2022 17:54:36 GMT
ENV GOSU_VERSION=1.14
# Thu, 23 Jun 2022 17:55:04 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Jun 2022 17:55:26 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 23 Jun 2022 17:55:29 GMT
ENV LANG=en_US.utf8
# Thu, 23 Jun 2022 17:55:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 17:55:49 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Jun 2022 17:55:57 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 23 Jun 2022 17:56:00 GMT
ENV PG_MAJOR=15
# Thu, 23 Jun 2022 17:56:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Fri, 01 Jul 2022 01:26:27 GMT
ENV PG_VERSION=15~beta2-1.pgdg110+1
# Fri, 01 Jul 2022 01:28:09 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 01 Jul 2022 01:28:21 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 01 Jul 2022 01:28:27 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 01 Jul 2022 01:28:30 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 01 Jul 2022 01:28:36 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 01 Jul 2022 01:28:41 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 01 Jul 2022 01:28:44 GMT
COPY file:925d466681c8349f58385c00a8caa567c76b695158aa04bf4ad2ac92604e11c7 in /usr/local/bin/ 
# Fri, 01 Jul 2022 01:28:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Jul 2022 01:28:53 GMT
STOPSIGNAL SIGINT
# Fri, 01 Jul 2022 01:28:56 GMT
EXPOSE 5432
# Fri, 01 Jul 2022 01:29:01 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:7716f0df7ba06b6f1937cd664805984e25e386a4165f2c6acc65356686e35221`  
		Last Modified: Thu, 23 Jun 2022 02:15:20 GMT  
		Size: 35.3 MB (35286823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020126cd7adc35ddd83605444413437b17db388415b535e0e670d5f67b3c8776`  
		Last Modified: Thu, 23 Jun 2022 18:15:26 GMT  
		Size: 5.2 MB (5222957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c0042078ea251b9c7504ed2587c0d97526de4400c1002381d9bace80beb063`  
		Last Modified: Thu, 23 Jun 2022 18:15:25 GMT  
		Size: 1.8 KB (1801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338a832b4ece725ccbb232684fc1ffc9db30723713e5019c96663951c19346e1`  
		Last Modified: Thu, 23 Jun 2022 18:15:25 GMT  
		Size: 1.3 MB (1317569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b01978c049df34ee7f8ee387cf1249d65aa64aea142f3035e0da1c226341bc5`  
		Last Modified: Thu, 23 Jun 2022 18:15:24 GMT  
		Size: 8.0 MB (8045517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d546326ffb4c415f7422b2770cf361b11f292efe885edae9b8438fffa2b7f49`  
		Last Modified: Thu, 23 Jun 2022 18:15:21 GMT  
		Size: 1.4 MB (1420200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42e15537e0887b85aa436afa0f4bef0c566dd330c2b8d681bf9b1c07fb208562`  
		Last Modified: Thu, 23 Jun 2022 18:15:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:010ab4f9e2503ff2ff7bcff2a64696dfdd5d682faac053f4672e36550da10eb9`  
		Last Modified: Thu, 23 Jun 2022 18:15:21 GMT  
		Size: 3.2 KB (3201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d902157dacbbd00afa0ee66d9b4137aa73cd9e1857f4e6a30a0dcb148f0c1590`  
		Last Modified: Fri, 01 Jul 2022 01:38:17 GMT  
		Size: 97.6 MB (97588559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9556877d48ea3b51aa793f08a2fa54a25033a2978a25cde31f4f8c5d6959c5fc`  
		Last Modified: Fri, 01 Jul 2022 01:38:00 GMT  
		Size: 9.8 KB (9792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f6cb7b735f9d58c39da87d9f1ff3d4e5dbb7759bc835d6507614ffaf104ce4`  
		Last Modified: Fri, 01 Jul 2022 01:38:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437c8b35796ec23db8fc2f6a8ba8641f7f673468e225237c578d89c11161d476`  
		Last Modified: Fri, 01 Jul 2022 01:38:00 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0953f0b911e76ced1008bd82a27f38656caf2cc58b88fd54fde26429604bc77`  
		Last Modified: Fri, 01 Jul 2022 01:38:00 GMT  
		Size: 4.7 KB (4703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta2-bullseye` - linux; s390x

```console
$ docker pull postgres@sha256:64ada99c3161c8482932f9dd4fcafa622804c88cf6656a9a6236637e2dc0956d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87934041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aca3de1a5041cb12346e6cc96ffed80fae8f903c99adb5d13c764c40da9d6f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 23 Jun 2022 00:43:10 GMT
ADD file:0b511e3efd87267fb27161eae56c4d08f0fed733697da6ffe6ea96a4cb68e938 in / 
# Thu, 23 Jun 2022 00:43:15 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 08:08:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 08:08:59 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 23 Jun 2022 08:08:59 GMT
ENV GOSU_VERSION=1.14
# Thu, 23 Jun 2022 08:09:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Jun 2022 08:09:25 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 23 Jun 2022 08:09:28 GMT
ENV LANG=en_US.utf8
# Thu, 23 Jun 2022 08:09:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 08:09:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Jun 2022 08:09:39 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 23 Jun 2022 08:09:39 GMT
ENV PG_MAJOR=15
# Thu, 23 Jun 2022 08:09:40 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Fri, 01 Jul 2022 00:41:59 GMT
ENV PG_VERSION=15~beta2-1.pgdg110+1
# Fri, 01 Jul 2022 00:51:10 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 01 Jul 2022 00:51:17 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 01 Jul 2022 00:51:19 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 01 Jul 2022 00:51:19 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 01 Jul 2022 00:51:20 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 01 Jul 2022 00:51:21 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 01 Jul 2022 00:51:21 GMT
COPY file:925d466681c8349f58385c00a8caa567c76b695158aa04bf4ad2ac92604e11c7 in /usr/local/bin/ 
# Fri, 01 Jul 2022 00:51:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Jul 2022 00:51:22 GMT
STOPSIGNAL SIGINT
# Fri, 01 Jul 2022 00:51:23 GMT
EXPOSE 5432
# Fri, 01 Jul 2022 00:51:23 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:c547f465e0c8708ad0c57cf09caa52f4c2b5b295bf10ab1ce71ca17ff81ea36a`  
		Last Modified: Thu, 23 Jun 2022 00:51:59 GMT  
		Size: 29.7 MB (29655262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095780b4f3c40e915ed76f2089ae36b1cecb78fa3c87b5c0c904cbeee8298fe8`  
		Last Modified: Thu, 23 Jun 2022 09:17:41 GMT  
		Size: 4.3 MB (4302483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8a7df919000a6bd661a7ba6cd5438c045e1acc3a0783182de465bb0bdb3e98`  
		Last Modified: Thu, 23 Jun 2022 09:17:41 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a1e57d482182b54639d65add607526ee7afde0ff3d5f00eaa3e0d9d7a893c4`  
		Last Modified: Thu, 23 Jun 2022 09:17:41 GMT  
		Size: 1.4 MB (1381679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edaaa6c43b3581001bd0b12339d2fe654d4e7bb10d375cafa1d18596de945a1d`  
		Last Modified: Thu, 23 Jun 2022 09:17:41 GMT  
		Size: 8.1 MB (8099231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d2861463c88cc1e226d3e20ecbe08c3881b4326a427e2049a046351f0ce2f3`  
		Last Modified: Thu, 23 Jun 2022 09:17:39 GMT  
		Size: 1.2 MB (1238070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6c3240a377326867bf202f16784508362cee1b29faa3a9266c46134fcb57cd`  
		Last Modified: Thu, 23 Jun 2022 09:17:39 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d4b5cce3748d8838bda90cc17d89876c5ab51b0fec445dd6b7f484e5d60b3b`  
		Last Modified: Thu, 23 Jun 2022 09:17:39 GMT  
		Size: 3.2 KB (3191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3664b558cfb2e276c9dcafadbfdccfac6c275e8e8fbcd7fbf0b2e7492554c03`  
		Last Modified: Fri, 01 Jul 2022 00:59:25 GMT  
		Size: 43.2 MB (43237344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e2b6c30d6dac2c87ce1953e4dd9fe453f2dbf7d00c386386d52f4b753a5025`  
		Last Modified: Fri, 01 Jul 2022 00:59:19 GMT  
		Size: 9.8 KB (9797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1644abaceefde52823ef63ed7b37d3856c0f8c0364edc16fb27533d9c6f39d`  
		Last Modified: Fri, 01 Jul 2022 00:59:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58a4d4cf2c28042d28ed319b5889099ba1dd17cbd0158df53f6f685b54ab891`  
		Last Modified: Fri, 01 Jul 2022 00:59:20 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7260b4061ff25aee5564e1dcefc113b1705c2f881f42b93840eb412d5d43bf2`  
		Last Modified: Fri, 01 Jul 2022 00:59:20 GMT  
		Size: 4.7 KB (4704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
