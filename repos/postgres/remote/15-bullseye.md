## `postgres:15-bullseye`

```console
$ docker pull postgres@sha256:7a4d83a3ae2a9ce1eac86afad1a6386e723459780c2ff789d7c2bf7571540a17
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 16
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; mips64le
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `postgres:15-bullseye` - linux; amd64

```console
$ docker pull postgres@sha256:6c0adafe00348b840f5808ecc603fb2eb9b8eae51e41285d3c9c723575d1a4cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138838458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4349050e2552bb6a4ec3ffa9cd726cdfde0d2a02a4fe5d225b883c5bb1c66e9d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENV GOSU_VERSION=1.16
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8 # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENV LANG=en_US.utf8
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENV PG_MAJOR=15
# Thu, 30 Nov 2023 00:11:07 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Thu, 30 Nov 2023 00:11:07 GMT
ENV PG_VERSION=15.5-1.pgdg110+1
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Nov 2023 00:11:07 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Nov 2023 00:11:07 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Nov 2023 00:11:07 GMT
STOPSIGNAL SIGINT
# Thu, 30 Nov 2023 00:11:07 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 30 Nov 2023 00:11:07 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:841c394aa1c185c41ad415a96c41065e9f83188ec89e40c44c1604ec091f2e96`  
		Last Modified: Sat, 02 Dec 2023 12:40:05 GMT  
		Size: 1.7 KB (1690 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e185d652d1d8e3d2a959763b482aac7fb4892ea112cf5da1f42b2184ac448ead`  
		Last Modified: Sat, 02 Dec 2023 12:40:06 GMT  
		Size: 4.2 MB (4207517 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1d6ca2bb3722032eee56b28f34351aebdabcb5bf3dd2b80bdcc8be50d05e5035`  
		Last Modified: Sat, 02 Dec 2023 12:40:04 GMT  
		Size: 1.5 MB (1472464 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:25c61fd365c3cb601f1718aea55f9dde8e63d067f5346232c9ea6062ced3f7f9`  
		Last Modified: Sat, 02 Dec 2023 12:40:05 GMT  
		Size: 8.0 MB (8045279 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b1cf6f3a256e357abeddc48a56f9aeedcc97ecccd4e2262c8d46fd1ff61c4c80`  
		Last Modified: Sat, 02 Dec 2023 12:40:06 GMT  
		Size: 1.0 MB (1037453 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ee947e6e8c27f2740ca07a99e4a94cff3efd560a10210d8bb177bf0b51ae4b3`  
		Last Modified: Sat, 02 Dec 2023 12:40:06 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1839dcc9fa4029d3f83de34a72db1a990af4ae154482006bbfe074285601c586`  
		Last Modified: Sat, 02 Dec 2023 12:40:07 GMT  
		Size: 3.1 KB (3145 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:227e0b5b5affadfcfbb751a08e784252488c715fe03a30d45e91566d1f8f00ee`  
		Last Modified: Sat, 02 Dec 2023 12:40:10 GMT  
		Size: 92.6 MB (92638105 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a1a2902a167818626492fda925f7aa867c0560c1432675efab811e94288644e4`  
		Last Modified: Sat, 02 Dec 2023 12:40:07 GMT  
		Size: 9.8 KB (9780 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:04ef8ea127a876cb8fe6315da619c721ca3b2e33211a4255f275e16516a437c5`  
		Last Modified: Sat, 02 Dec 2023 12:40:07 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3b117d3ccf6e78241a34b7c41c6aca6cd8dcd8480ebdfe3f5884d78075227db9`  
		Last Modified: Sat, 02 Dec 2023 12:40:08 GMT  
		Size: 171.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b91f752265f7d276c2c45d4c6a244e7679e34e92c90fb6ba11e10c130bfce415`  
		Last Modified: Sat, 02 Dec 2023 12:40:08 GMT  
		Size: 4.8 KB (4786 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:15-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:c06d0825ae18a950384329febc92f552ce729da6abdbf44e8b467cb5703fa791
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5052077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:216057506a5e71c1351ac550a613dfccafaa0d9c8e9b1b43e637779f3b42bc12`

```dockerfile
```

-	Layers:
	-	`sha256:094f6c7e3cd11c9fed4bc8848b51c22e3ee6aeca94a7be494d55c13850591252`  
		Last Modified: Sat, 02 Dec 2023 12:40:06 GMT  
		Size: 5.0 MB (5002048 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:fc7a3f6b49bb54fac684ba0248ebb82e0998cf69db6bbc03cb67c193faa52c89`  
		Last Modified: Sat, 02 Dec 2023 12:40:04 GMT  
		Size: 50.0 KB (50029 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:15-bullseye` - linux; arm variant v5

```console
$ docker pull postgres@sha256:ae02a2b464b28597302db0078a50aabb45d6dd74ae7583381ca38454d46fa90a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.1 MB (132063389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5429dd351785ea322c03d2ba19abd28831b16bfe571892a2f0fb21ef183d1309`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 05:01:09 GMT
ADD file:f7d1d017cc4e588f213f4536967b8d58c50b8602fb8a10b786856c35a843f31e in / 
# Tue, 21 Nov 2023 05:01:09 GMT
CMD ["bash"]
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENV GOSU_VERSION=1.16
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8 # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENV LANG=en_US.utf8
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENV PG_MAJOR=15
# Thu, 30 Nov 2023 00:11:07 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Thu, 30 Nov 2023 00:11:07 GMT
ENV PG_VERSION=15.5-1.pgdg110+1
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Nov 2023 00:11:07 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Nov 2023 00:11:07 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Nov 2023 00:11:07 GMT
STOPSIGNAL SIGINT
# Thu, 30 Nov 2023 00:11:07 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 30 Nov 2023 00:11:07 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:d051266714ac5508b442ebbe5911d353bfacddc64f657eeba14a993cced96358`  
		Last Modified: Tue, 21 Nov 2023 05:04:38 GMT  
		Size: 28.9 MB (28921267 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ece1beb92cce2ac06ca58cdf90840eefcd484ca3a322e1ede41adbd2aa5af81`  
		Last Modified: Tue, 21 Nov 2023 20:02:31 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b626f1f20e2d8180138b585029d4c234ef8f68fce1ea4de209c15160a571570`  
		Last Modified: Tue, 21 Nov 2023 20:02:31 GMT  
		Size: 3.9 MB (3889265 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:848c2a7661551b2883b51208a362b26b127489d0d144f9726925dfcb6c8f296c`  
		Last Modified: Tue, 21 Nov 2023 20:02:31 GMT  
		Size: 1.4 MB (1449946 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4fa10149f3fedf3623013ea4617c0347bf1d5e1018a20c3acb3089fe3f16c201`  
		Last Modified: Tue, 21 Nov 2023 20:02:33 GMT  
		Size: 8.0 MB (8045273 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:20f01ea795e7f5f05e14920788c8357f1db83187f8933ca15bf4b6818312e40b`  
		Last Modified: Tue, 21 Nov 2023 20:02:33 GMT  
		Size: 1.0 MB (1033914 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0a65ccf4e087845b4aaf62c24b518eb775f6e8ab3080d62030cde1e5890bf51e`  
		Last Modified: Tue, 21 Nov 2023 20:02:32 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c0f312b2560772e07297fec490d54bb2c01a653ed43b44a32d9845e7993b5c7`  
		Last Modified: Tue, 21 Nov 2023 20:02:33 GMT  
		Size: 3.1 KB (3143 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ac2a6b29f537bae5177de7e823b2d2de2479df230655a6f07d3adef927e3d0f`  
		Last Modified: Tue, 21 Nov 2023 20:32:11 GMT  
		Size: 88.7 MB (88703918 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cd07bc6bced7c0cd678fa4df3bc38fe7daf23ce42936bff5e1463e6a35ce55fb`  
		Last Modified: Tue, 21 Nov 2023 20:32:08 GMT  
		Size: 9.8 KB (9784 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2d48f969dc7cb885bc35d2a2fcc5762f1ec2c7519f414670132c70150c22790d`  
		Last Modified: Fri, 01 Dec 2023 22:16:17 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:db6f8f29954b6eb2bb87a59731408e915739feaa4e7709bb188c68282c48cc1a`  
		Last Modified: Fri, 01 Dec 2023 22:16:17 GMT  
		Size: 175.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3024b82c0ba8fca50c1c9a7e378e23f71cf5e356767b19e8e6ee7686d44b5e85`  
		Last Modified: Fri, 01 Dec 2023 22:16:17 GMT  
		Size: 4.8 KB (4784 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:15-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:b45402a1345d779cf05a1a47214216a1a9d13d992fafa5cf43aa2e24113a28a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.8 KB (49831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d871d8fa5f0e7be6f8b97bbe0aa47cb8180dcc786df77da931d9b058dfca9e0c`

```dockerfile
```

-	Layers:
	-	`sha256:8089af006da30ab887df9f24dcb90969d0e0a934a233bca59f3df06f2386cb49`  
		Last Modified: Fri, 01 Dec 2023 22:16:17 GMT  
		Size: 49.8 KB (49831 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:15-bullseye` - linux; arm variant v7

```console
$ docker pull postgres@sha256:614f3e98a698509d3cc3a10e228de58cd244b421d2790ecdf50d5be43c08ac9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.7 MB (126696443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b49ab39438784ce1467417608eb82d9e44fc411d4d6fc2a6a93f9ef5be9df9b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 03:58:04 GMT
ADD file:c4afced274aaa80ab3018b368ed739c1c55e49b41e9637ac44d63e61344fe865 in / 
# Tue, 21 Nov 2023 03:58:04 GMT
CMD ["bash"]
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENV GOSU_VERSION=1.16
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8 # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENV LANG=en_US.utf8
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENV PG_MAJOR=15
# Thu, 30 Nov 2023 00:11:07 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Thu, 30 Nov 2023 00:11:07 GMT
ENV PG_VERSION=15.5-1.pgdg110+1
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Nov 2023 00:11:07 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Nov 2023 00:11:07 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Nov 2023 00:11:07 GMT
STOPSIGNAL SIGINT
# Thu, 30 Nov 2023 00:11:07 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 30 Nov 2023 00:11:07 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:6dc4ed5513793308b8e30b08e03f97fa54025c3d3f3172c6edccb1dbbc7ff139`  
		Last Modified: Tue, 21 Nov 2023 04:02:35 GMT  
		Size: 26.6 MB (26579014 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:03cc7941b400f3bf57e88ca53cd8f503b865c5758c4a78c8b4c7a8e328530196`  
		Last Modified: Wed, 22 Nov 2023 01:48:04 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ac4a88703271fa81c161e06205d8313b2f8f0af319f9e0b3ad8c61257ecf43a8`  
		Last Modified: Wed, 22 Nov 2023 01:48:05 GMT  
		Size: 3.5 MB (3509868 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:78a39292d0ae527985471598a74ca795bbde210667b000f267cd16afcf4db4df`  
		Last Modified: Wed, 22 Nov 2023 01:48:05 GMT  
		Size: 1.4 MB (1440036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6c9409bab78ee01b73d472aa8b928ed37ba03e08bb0b9a13dea577c13c60654b`  
		Last Modified: Wed, 22 Nov 2023 01:48:07 GMT  
		Size: 8.0 MB (8045202 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:22395ce5acb8645b4427e09aae3b58c5cc849b5d6a5a2a825396e15ac23a11d2`  
		Last Modified: Wed, 22 Nov 2023 01:48:06 GMT  
		Size: 907.8 KB (907774 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:681b290bd10a5aa1e8c51ba74de59868cb4d847b7e121c7b9363e822124e4772`  
		Last Modified: Wed, 22 Nov 2023 01:48:06 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f8dca2bf4cee3e9a783c855ca659a8048dcfcd8982a97eaa0f090e14a1ba182c`  
		Last Modified: Wed, 22 Nov 2023 01:48:06 GMT  
		Size: 3.1 KB (3140 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:95e4283f704a12e038a95423808dd439114b96c8a2fea7b081abf7eba763d22d`  
		Last Modified: Wed, 22 Nov 2023 02:19:34 GMT  
		Size: 86.2 MB (86194743 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:052f52400f34132cf8aac10d8f595941f864e28d0000d528e3303ea5179d7e91`  
		Last Modified: Wed, 22 Nov 2023 02:19:31 GMT  
		Size: 9.8 KB (9784 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7adb328d7e22a4f1e6da64a43b161a8891e7dab218036e83f632b1e0d834e68e`  
		Last Modified: Fri, 01 Dec 2023 22:32:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:639adb8c10e49f0ca32d8323991d624d8a34c7259a734ec259277fd4f3596f8c`  
		Last Modified: Fri, 01 Dec 2023 22:32:55 GMT  
		Size: 175.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6eecec9b782ce3a2dff6f0e64c0833b69080b558c5b149f67e4f9e6c31f9c057`  
		Last Modified: Fri, 01 Dec 2023 22:32:55 GMT  
		Size: 4.8 KB (4784 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:15-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:39cc8c43f744221b76887bc025b87f09aa7ec16c99015370b3bb140c56983c1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5062425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:897e55efea46d59d03564d8fbadaa6837d359927ce1a096683c14469860420fd`

```dockerfile
```

-	Layers:
	-	`sha256:6aee59680d558bdbb705bb75f1e184d266e0a62b3cddfb171185d4433bd5ae1a`  
		Last Modified: Fri, 01 Dec 2023 22:32:55 GMT  
		Size: 5.0 MB (5012387 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9d6c74aa427db6c42e84ef91404abbae6c62f9be2e4eb321e723889cf1a96eb6`  
		Last Modified: Fri, 01 Dec 2023 22:32:55 GMT  
		Size: 50.0 KB (50038 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:15-bullseye` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:804787d150c81b5665f87afb4df25e3491a8c499b60c361a55de4149e303bd7b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133920851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f51e45b06f998117038d2852b4d2a22fc2e172df27316e9d577a58eee3dee417`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENV GOSU_VERSION=1.16
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8 # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENV LANG=en_US.utf8
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENV PG_MAJOR=15
# Thu, 30 Nov 2023 00:11:07 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Thu, 30 Nov 2023 00:11:07 GMT
ENV PG_VERSION=15.5-1.pgdg110+1
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Nov 2023 00:11:07 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Nov 2023 00:11:07 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Nov 2023 00:11:07 GMT
STOPSIGNAL SIGINT
# Thu, 30 Nov 2023 00:11:07 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 30 Nov 2023 00:11:07 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3d499610b7b67a680fc82a27625cc3960384326345a873ab3729091fde96c2d4`  
		Last Modified: Wed, 22 Nov 2023 11:52:59 GMT  
		Size: 1.7 KB (1683 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:16b9d08385de13134ad8df9d9c5a6603d462b4040c8aed8a540ce5c6bbea37e8`  
		Last Modified: Wed, 22 Nov 2023 11:53:00 GMT  
		Size: 4.2 MB (4209368 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5cd9b1488b80fd9988b0d188f94dbfb975e022a376c386cb265ffe5c3b768bdf`  
		Last Modified: Wed, 22 Nov 2023 11:53:00 GMT  
		Size: 1.4 MB (1404352 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:05093a7fd59075e84a24aa46c2310864ff48fd4dd26e8257c36529acd6f93514`  
		Last Modified: Wed, 22 Nov 2023 11:53:00 GMT  
		Size: 8.0 MB (8045185 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb6e913704ba9c6cb18a563dc9c85e201f5cf9c09dfe06f2c1532537258b76e9`  
		Last Modified: Wed, 22 Nov 2023 11:53:01 GMT  
		Size: 1.0 MB (1025874 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c5fcd4f567dd99db4cd906a4ef25247ec80783aeacd0b6482f58884caebadfda`  
		Last Modified: Wed, 22 Nov 2023 11:53:01 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bda47adbeb1f61f09d98831d05acf423d1d07ddb6ec1677bfe37ab19c5c07e0d`  
		Last Modified: Wed, 22 Nov 2023 11:53:01 GMT  
		Size: 3.1 KB (3141 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ded628e4be603de0e3a44eddb0eceb35db9535cec4aaece989f1a186682e6f57`  
		Last Modified: Wed, 22 Nov 2023 11:54:42 GMT  
		Size: 89.2 MB (89152148 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9857e0d640a62d20b56188d147716671cf508957a5a63cc7dcfe22479772a06b`  
		Last Modified: Wed, 22 Nov 2023 11:54:39 GMT  
		Size: 9.8 KB (9775 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:57d1762f26e4858f91a67adb16314375b9a80036e00d9b2b3f7aaa9924066f96`  
		Last Modified: Fri, 01 Dec 2023 22:29:45 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:db0ab1fc88b355a06730ce36ab5036690c15091757b861f9ff6f90186b7957af`  
		Last Modified: Fri, 01 Dec 2023 22:29:45 GMT  
		Size: 174.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1951b29154c4686d09ad01b13a708ca79efae26ec22cca8b2edcac9b446e0e92`  
		Last Modified: Fri, 01 Dec 2023 22:29:45 GMT  
		Size: 4.8 KB (4784 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:15-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:b414f6d807dfac5d91105598a2218e5886af4046f6825aa722e3c1e3e92fa69d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5057547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5707b1c2533cc64afee67ff9bcd38303e5a2afa342ddaa9e2685a855b83409f0`

```dockerfile
```

-	Layers:
	-	`sha256:7ffba7437e70f2de6524d1425423cc42056c69bf30dd417c4608bfe6b9b5f4d1`  
		Last Modified: Fri, 01 Dec 2023 22:29:45 GMT  
		Size: 5.0 MB (5007679 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:e59fc5b8400948c9f10dcf8a7f84d76f3d878196d625317c9e244bce3cb5dad9`  
		Last Modified: Fri, 01 Dec 2023 22:29:45 GMT  
		Size: 49.9 KB (49868 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:15-bullseye` - linux; 386

```console
$ docker pull postgres@sha256:55b4266b9a9e47d76f9769cc0e4b934d4c5e68c36988f7b746dbb9d9a4c1a58a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.7 MB (140672240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d25753eb3feb5751de76ae9b810e2968453972f9fcc0c3efd66fb8c35960e9d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 14 Sep 2023 18:02:56 GMT
ADD file:67f223c9c48e525a23fb110e4c105d7128dcac0c10f32c38f98ea84a21d2bd00 in / 
# Thu, 14 Sep 2023 18:02:56 GMT
CMD ["bash"]
# Thu, 14 Sep 2023 18:02:56 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 14 Sep 2023 18:02:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 14 Sep 2023 18:02:56 GMT
ENV GOSU_VERSION=1.16
# Thu, 14 Sep 2023 18:02:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 14 Sep 2023 18:02:56 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8 # buildkit
# Thu, 14 Sep 2023 18:02:56 GMT
ENV LANG=en_US.utf8
# Thu, 14 Sep 2023 18:02:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 14 Sep 2023 18:02:56 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 14 Sep 2023 18:02:56 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 14 Sep 2023 18:02:56 GMT
ENV PG_MAJOR=15
# Thu, 14 Sep 2023 18:02:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Thu, 14 Sep 2023 18:02:56 GMT
ENV PG_VERSION=15.4-2.pgdg110+1
# Thu, 14 Sep 2023 18:02:56 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 14 Sep 2023 18:02:56 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 14 Sep 2023 18:02:56 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql # buildkit
# Thu, 14 Sep 2023 18:02:56 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 14 Sep 2023 18:02:56 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA" # buildkit
# Thu, 14 Sep 2023 18:02:56 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 14 Sep 2023 18:02:56 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 14 Sep 2023 18:02:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Sep 2023 18:02:56 GMT
STOPSIGNAL SIGINT
# Thu, 14 Sep 2023 18:02:56 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 14 Sep 2023 18:02:56 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:bc6810e8fe9346a3caaff984163b789d12b6964a15a2029e384143ca19fef5ad`  
		Last Modified: Wed, 01 Nov 2023 00:44:14 GMT  
		Size: 32.4 MB (32402692 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4079e286e13e666ced278e631e538141761f143229e5133dd9468586727cc000`  
		Last Modified: Wed, 01 Nov 2023 01:23:24 GMT  
		Size: 1.7 KB (1674 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7466494e1b18909c6eb143c44e93f95ba5395cbea44fe76ca5c78917855516b5`  
		Last Modified: Wed, 01 Nov 2023 01:23:25 GMT  
		Size: 4.6 MB (4607425 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6bf3a859cea4b1dbcb2f006419627892fff38294ec7adc3ae69d2c798db88322`  
		Last Modified: Wed, 01 Nov 2023 01:23:24 GMT  
		Size: 1.4 MB (1448290 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9b5e3540d5a0ede8679728900616d27779000ad577d33ddd4fae7da4a20cda15`  
		Last Modified: Wed, 01 Nov 2023 01:23:25 GMT  
		Size: 8.0 MB (8045170 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ce89ff79412c6462360c788bb58bec84dc900d718bfd727669b01d94579daae`  
		Last Modified: Wed, 01 Nov 2023 01:23:25 GMT  
		Size: 1.0 MB (1027939 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:269aa20944684c7b30e23735f91d98c3bdffccdc0f84d17577a5d98c0801cc11`  
		Last Modified: Wed, 01 Nov 2023 01:23:25 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ae5b83958cc8a61a0aa48a2a90d6558ed61623f69d6b71aa6d4840a50b23524`  
		Last Modified: Wed, 01 Nov 2023 01:23:26 GMT  
		Size: 3.1 KB (3142 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c5fc0539d21e5616f6a8d255a110e57d48cc040389b23a65301f3c290dea2708`  
		Last Modified: Wed, 01 Nov 2023 01:23:31 GMT  
		Size: 93.1 MB (93120921 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b4b53152299c17b35a347a270c9fae45f05f4fa8bdf95d13deaa83bc22be9c82`  
		Last Modified: Wed, 01 Nov 2023 01:23:26 GMT  
		Size: 9.8 KB (9784 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ec2f55babc9b98e27e30c009841a379cefb5252727d606b2b514288088ef2206`  
		Last Modified: Wed, 01 Nov 2023 01:23:27 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4cd9425d5a7f675fe65af1ec2250861bcfcdeabea25df26443189ab8b92f57d6`  
		Last Modified: Wed, 01 Nov 2023 01:23:27 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:757698ce662b02d6953431ca02a3c14fdf48a62430e600ce92ddacc2388233d5`  
		Last Modified: Wed, 01 Nov 2023 01:23:27 GMT  
		Size: 4.8 KB (4789 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:15-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:a4ba3acb45fce42e28bea3b1c082c2da66e60c0903dd72269f98715183481e12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.8 KB (49770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a39b7ed5585612aacfb44be1b15449c30ba9942127ff847a85a540f290998c9`

```dockerfile
```

-	Layers:
	-	`sha256:a9c736c0fc945b7ca923f6292368d01c49c5011dcbeea6b2cb4cea498f965b84`  
		Last Modified: Wed, 01 Nov 2023 01:23:24 GMT  
		Size: 49.8 KB (49770 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:15-bullseye` - linux; mips64le

```console
$ docker pull postgres@sha256:f55be29640bc405481455df07fb39cbfc0c6128ec060de7a061deff45046a7df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.6 MB (133573536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ae68112081950947ad0ab6a956b22849d0610728bf2db072a63ca46af7f0969`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 04:11:02 GMT
ADD file:09d1c4f0f5b78b81f635498ee58f6ab1843bca8a18549ecc39686f1c60b1951d in / 
# Tue, 21 Nov 2023 04:11:06 GMT
CMD ["bash"]
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENV GOSU_VERSION=1.16
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8 # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENV LANG=en_US.utf8
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENV PG_MAJOR=15
# Thu, 30 Nov 2023 00:11:07 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Thu, 30 Nov 2023 00:11:07 GMT
ENV PG_VERSION=15.5-1.pgdg110+1
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Nov 2023 00:11:07 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Nov 2023 00:11:07 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Nov 2023 00:11:07 GMT
STOPSIGNAL SIGINT
# Thu, 30 Nov 2023 00:11:07 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 30 Nov 2023 00:11:07 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:a157b7f5d72df9473d33b22278cb42e4e06e22b99ac1864b7b586f36671f15bb`  
		Last Modified: Tue, 21 Nov 2023 04:22:02 GMT  
		Size: 29.6 MB (29636034 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:785f51b53d1db400472f15ec096a7ee4b64d3c08b994759b18049124438c4010`  
		Last Modified: Thu, 23 Nov 2023 03:33:57 GMT  
		Size: 1.7 KB (1687 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3778165671f234b7363ec027202183f74d772e1950d82cc3f6278f678dee79d8`  
		Last Modified: Thu, 23 Nov 2023 03:33:57 GMT  
		Size: 4.2 MB (4196358 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d8ffc22c0ea9927329be3519bab2180352190f8f23bd689c2bf7ae7728a4b58d`  
		Last Modified: Thu, 23 Nov 2023 03:33:57 GMT  
		Size: 1.4 MB (1360004 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b06695751e19c683fa07fd1965155895afddce123ca9e7c3692385a156fed23f`  
		Last Modified: Thu, 23 Nov 2023 03:33:58 GMT  
		Size: 8.0 MB (8045542 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4edf0bee40de56418f9a87800e244e08967f4a60cb290bafe31b3a6dda9924f1`  
		Last Modified: Thu, 23 Nov 2023 03:33:58 GMT  
		Size: 1.1 MB (1089550 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e4184426f7fc37d1def27fcf0df1f7857cfc9719ef315d62071070a32836371e`  
		Last Modified: Thu, 23 Nov 2023 03:33:58 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d171f5a3c657f88f3ab962f218611f594098b65259f3aad13e26350d1d4be229`  
		Last Modified: Thu, 23 Nov 2023 03:33:58 GMT  
		Size: 3.1 KB (3144 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c2dc9b49cf853476e951c32eb4f904a511212bd3330565ef98605e3a05f845c6`  
		Last Modified: Thu, 23 Nov 2023 05:48:26 GMT  
		Size: 89.2 MB (89226234 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b18c3e1dfa98a09c1d3160dfa288002b23426f69cf055ce1744a4d33445e397`  
		Last Modified: Thu, 23 Nov 2023 05:48:17 GMT  
		Size: 9.8 KB (9787 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9f6fc324528f3740138fb8414c0e15af0a2250d5a7d363be1c77ffd316aaa511`  
		Last Modified: Fri, 01 Dec 2023 22:18:55 GMT  
		Size: 127.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd8527b4f01b2d5fa18f0e182ff6c9aff2215fe066fd9c70b9a1a688d4f97170`  
		Last Modified: Fri, 01 Dec 2023 22:18:55 GMT  
		Size: 174.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:faef280d2ba56eedcbc504ec2f420fa609b96d18d9c3e12739417a1b0b4b90bc`  
		Last Modified: Fri, 01 Dec 2023 22:18:55 GMT  
		Size: 4.8 KB (4779 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:15-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:cae7fe6c4a4674e871dc2de4df8a4f1994bd7c4d24d1b377d6320e6af435c164
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.7 KB (49716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a321a68709ce2fcea19dfb8fcb685cee19de94fcd75acd73ca0b5390045c2a2`

```dockerfile
```

-	Layers:
	-	`sha256:b17b4d3eeadea61164a8a58525063d495e117904a98193068bd0771a1657e8da`  
		Last Modified: Fri, 01 Dec 2023 22:18:54 GMT  
		Size: 49.7 KB (49716 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:15-bullseye` - linux; ppc64le

```console
$ docker pull postgres@sha256:3b9516a2c5d3153e0e1b7867a2e7a13feaa16e200fe2b29c5dd7dc21a0220f63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.9 MB (147928662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90a28301053766be34118647880bf90da8946a4faab406a0c428f507bc69f58d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:43 GMT
ADD file:b0d18f2d04821eb50d1faecc1a64916f5c63dd386ae71a3b2cb1d6c4aac6e1c4 in / 
# Tue, 21 Nov 2023 04:24:46 GMT
CMD ["bash"]
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENV GOSU_VERSION=1.16
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8 # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENV LANG=en_US.utf8
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENV PG_MAJOR=15
# Thu, 30 Nov 2023 00:11:07 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Thu, 30 Nov 2023 00:11:07 GMT
ENV PG_VERSION=15.5-1.pgdg110+1
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Nov 2023 00:11:07 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Nov 2023 00:11:07 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Nov 2023 00:11:07 GMT
STOPSIGNAL SIGINT
# Thu, 30 Nov 2023 00:11:07 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 30 Nov 2023 00:11:07 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:60239a74847cd7e9a928353188f3cf096ca8cf648e2b27c765058e169d568fd9`  
		Last Modified: Tue, 21 Nov 2023 04:29:47 GMT  
		Size: 35.3 MB (35293727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:16de6da61666e950a5b7b529f3038a00b9f2c676c778ce6877c9554fdd36857c`  
		Last Modified: Tue, 21 Nov 2023 23:56:59 GMT  
		Size: 1.7 KB (1690 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a8c98567766a405ce84a0be0e02e7cf9914d6d4691dffc5496c760a347867228`  
		Last Modified: Tue, 21 Nov 2023 23:56:59 GMT  
		Size: 5.0 MB (5015948 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6c61a8652eea248c5219212393f2a552f9493c1642d9219671579c1ee733f77d`  
		Last Modified: Tue, 21 Nov 2023 23:56:59 GMT  
		Size: 1.4 MB (1394026 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bbdb4e3c161d5532d076597f8745f34a6f37d4c07e3b0e6b813a8739f23e1417`  
		Last Modified: Tue, 21 Nov 2023 23:57:00 GMT  
		Size: 8.0 MB (8045122 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e02ed0182f1b78eec622706c1ce7e2e3a5db1a8ff2f9e72219ed5427a3cfa888`  
		Last Modified: Tue, 21 Nov 2023 23:57:00 GMT  
		Size: 1.2 MB (1196901 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4862e5122b808ebe059b3ed3a9d62dbbcfcfd0a4ee79f3185115cb2be9eb5889`  
		Last Modified: Tue, 21 Nov 2023 23:57:00 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5f110a1ad0cf91d66fa9f7495dcf0d900b6a19805cca2e349d646c9211a38e3d`  
		Last Modified: Tue, 21 Nov 2023 23:57:00 GMT  
		Size: 3.1 KB (3140 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b6907f14acb378b64be96dd54543b99c5669a755e131d3299f47efcab031219f`  
		Last Modified: Tue, 21 Nov 2023 23:59:40 GMT  
		Size: 97.0 MB (96963127 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ff2b4711167f148f9d5b532e4e60f19d88bf7d1ec059fe2fac7fe0b5e923f461`  
		Last Modified: Tue, 21 Nov 2023 23:59:37 GMT  
		Size: 9.8 KB (9780 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d71dd2b8d4c3ee438800037cd0501893481525328661e13235e534da8403b419`  
		Last Modified: Fri, 01 Dec 2023 22:29:02 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b868983d324acd9e7571e1deb1de089ccda1820abfcfeee26ababddeac5d6722`  
		Last Modified: Fri, 01 Dec 2023 22:29:02 GMT  
		Size: 174.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7a2c19a21017c95c3abbadb68c3048e6582b04a41df477627cb633dccdbc5a06`  
		Last Modified: Fri, 01 Dec 2023 22:29:02 GMT  
		Size: 4.8 KB (4783 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:15-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:f3681fdaf51f91dfcbf4fdd0f5b78b212cda6c41c8f0d3b63cade9a7593464ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5059090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06b663dcdc51ed139d3ba67e240287f95c7baefcf24775c5bb5d0540ec44e5a2`

```dockerfile
```

-	Layers:
	-	`sha256:97ef6f23a369a5a98eaf64c82a777d8003ac061591d3c6fef114c0c5164be37c`  
		Last Modified: Fri, 01 Dec 2023 22:29:01 GMT  
		Size: 5.0 MB (5009182 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ff7ff0cf6cbed15b427dde60d992a1b62709db2d8371d8ed239786ad8295a81d`  
		Last Modified: Fri, 01 Dec 2023 22:29:01 GMT  
		Size: 49.9 KB (49908 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:15-bullseye` - linux; s390x

```console
$ docker pull postgres@sha256:f8f1e56f37cf37cae6410d1c65c060cec2b0313bba8991b72698c82186c9f047
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.5 MB (142450246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:877953cec82538317c3cd300267b79d73ea60156f08dda52ab2bbdb2e54bcfd6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 05:05:18 GMT
ADD file:a545f27075704ce13e33e539170d3f47007424d2cc2bea5aecfd2608a5194151 in / 
# Tue, 21 Nov 2023 05:05:22 GMT
CMD ["bash"]
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENV GOSU_VERSION=1.16
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8 # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENV LANG=en_US.utf8
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENV PG_MAJOR=15
# Thu, 30 Nov 2023 00:11:07 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Thu, 30 Nov 2023 00:11:07 GMT
ENV PG_VERSION=15.5-1.pgdg110+1
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Nov 2023 00:11:07 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Nov 2023 00:11:07 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 30 Nov 2023 00:11:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Nov 2023 00:11:07 GMT
STOPSIGNAL SIGINT
# Thu, 30 Nov 2023 00:11:07 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 30 Nov 2023 00:11:07 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:b114072f1cab66b7376d690985b12816aebab2e4e41fc170e32f111df27951dc`  
		Last Modified: Tue, 21 Nov 2023 05:10:48 GMT  
		Size: 29.7 MB (29656938 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6c14abe39e5d7af1af3f169efac214a4f5188f9cf0b1eeff4aa56e29edadb83e`  
		Last Modified: Tue, 21 Nov 2023 18:48:13 GMT  
		Size: 1.7 KB (1685 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cda7c74bb621b77965678f0178a83d5ab3be51a08a147477342ecbce0570474b`  
		Last Modified: Tue, 21 Nov 2023 18:48:13 GMT  
		Size: 4.1 MB (4096138 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c24e48d76c2c7273893bb9fdadd72210e42e08d97d83c1951ece2885024a7ddf`  
		Last Modified: Tue, 21 Nov 2023 18:48:13 GMT  
		Size: 1.4 MB (1438342 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:907bad315ef26db29b2f1d30476df3623e928037f4f1245879d0acefc7d51fee`  
		Last Modified: Tue, 21 Nov 2023 18:48:14 GMT  
		Size: 8.1 MB (8099088 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:932751c91c6f7fde288cdfb18a762883255568a6d26c4bab31952f47a2412095`  
		Last Modified: Tue, 21 Nov 2023 18:48:14 GMT  
		Size: 1.0 MB (1014332 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:51466198f57f994776e57e10129e6e8b2e9e80ceda50f34cfddfd8c226e6a9e1`  
		Last Modified: Tue, 21 Nov 2023 18:48:14 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:68f4ed0154dba5579cb0fe28fe0064fd32f637f29598866ce370d1f8641be866`  
		Last Modified: Tue, 21 Nov 2023 18:48:15 GMT  
		Size: 3.1 KB (3140 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5ba4aa7c026edb3ca79083ad2114e3c870f80dc95347d607fcee27077c3fec87`  
		Last Modified: Tue, 21 Nov 2023 18:50:38 GMT  
		Size: 98.1 MB (98125608 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1da978850e162968ab549692c476232df0d8697747bd15e8a2bcdc43761afbd0`  
		Last Modified: Tue, 21 Nov 2023 18:50:36 GMT  
		Size: 9.8 KB (9779 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7d73410d148d449d25ef851aaa92ff5a36cabbcd9950df1e8e21cbe7207e467b`  
		Last Modified: Fri, 01 Dec 2023 22:21:44 GMT  
		Size: 126.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:45ca4364828f25a8b9fb91718443c92d3f6435db83e5e0f38705933d20502854`  
		Last Modified: Fri, 01 Dec 2023 22:21:44 GMT  
		Size: 173.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2b2b5c71a1c67e66975f2d599adeb66e2f3bb5f8e50bad89a53cd02cbc90a7d1`  
		Last Modified: Fri, 01 Dec 2023 22:21:44 GMT  
		Size: 4.8 KB (4781 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:15-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:dc3b8b7fab200ee94ac0a563c19488c37a194f2b2ddc3d2487bbf36f089e18aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5050889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fed2104691db47b3d8bac22d5cfd148d19603c13500e9aad2eda52fc6e897976`

```dockerfile
```

-	Layers:
	-	`sha256:5c7241e804f5245c0d066a35fa82701670df0dae4cb17375740543958d866ac4`  
		Last Modified: Fri, 01 Dec 2023 22:21:44 GMT  
		Size: 5.0 MB (5001027 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8eabd5298a7fdd52c12d82d7191223f8bf21ba7db1f1e4f98fa3cbedff2c88b1`  
		Last Modified: Fri, 01 Dec 2023 22:21:43 GMT  
		Size: 49.9 KB (49862 bytes)  
		MIME: application/vnd.in-toto+json
