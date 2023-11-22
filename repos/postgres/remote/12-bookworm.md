## `postgres:12-bookworm`

```console
$ docker pull postgres@sha256:b7da969734af311c7cce36d92727b8cbde02321c208a87bef0d076cac9cbcd33
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

### `postgres:12-bookworm` - linux; amd64

```console
$ docker pull postgres@sha256:a58017754bc5e03892047b1169d7123e50d29ae475043507ef5ebaa5b75df781
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.0 MB (147959560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d56839ac0df4898dcfe760cb23e5f726dd62585d602385ed15bd16359f13089`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 09 Nov 2023 19:16:09 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Thu, 09 Nov 2023 19:16:09 GMT
CMD ["bash"]
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENV GOSU_VERSION=1.16
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8 # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENV LANG=en_US.utf8
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENV PG_MAJOR=12
# Thu, 09 Nov 2023 19:16:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Thu, 09 Nov 2023 19:16:09 GMT
ENV PG_VERSION=12.17-1.pgdg120+1
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 09 Nov 2023 19:16:09 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA" # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 09 Nov 2023 19:16:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Nov 2023 19:16:09 GMT
STOPSIGNAL SIGINT
# Thu, 09 Nov 2023 19:16:09 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 09 Nov 2023 19:16:09 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b276ad3ec71680df28d405fb44314fb75db4a1f53da1449f77a49099c1fa1659`  
		Last Modified: Tue, 21 Nov 2023 06:17:33 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5594500286b92f970fbf74e321e094661699c13979fd7a9d7c6cc4ee438d7f97`  
		Last Modified: Tue, 21 Nov 2023 06:17:34 GMT  
		Size: 4.4 MB (4422657 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d346ff68d011fcb4aeeca5bcc8df20d318812faef3f6cf4705ca64dacaf7cd6e`  
		Last Modified: Tue, 21 Nov 2023 06:17:33 GMT  
		Size: 1.4 MB (1448522 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a517466f4964e23ed7a999019764741eb18698a467871e312fb973206a6841f1`  
		Last Modified: Tue, 21 Nov 2023 06:17:34 GMT  
		Size: 8.1 MB (8067886 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fa27853c360b25dff4f81884f6345f2d9bd52841615d894dbb2e87040225e000`  
		Last Modified: Tue, 21 Nov 2023 06:17:34 GMT  
		Size: 1.2 MB (1195077 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bca5b88435a36b34efb4960d378a12bb0b0923ad22281cdd3896f42dcc2775c1`  
		Last Modified: Tue, 21 Nov 2023 06:17:34 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7438bf8c221d37b989171c9f0476f2103320d438d2df400cd550ce7b446d262f`  
		Last Modified: Tue, 21 Nov 2023 06:17:34 GMT  
		Size: 3.1 KB (3141 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7f77650e50b4aedbd5a6913db730117843e23716d08a7e603b999f8620b3b4cd`  
		Last Modified: Tue, 21 Nov 2023 06:17:37 GMT  
		Size: 103.7 MB (103656983 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:965fca7fd5c99fc98ff69d248ea6b70f0f585934d55653c22ef01d836b437e32`  
		Last Modified: Tue, 21 Nov 2023 06:17:35 GMT  
		Size: 9.0 KB (9022 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:964c1bc5b9f0de37bfeb8dae44da79204ae70cbf6e5efa53c72f9e2c51fa0c2f`  
		Last Modified: Tue, 21 Nov 2023 06:17:35 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8ae8bfd81aea8ff26f1887b46eb52f6d7fa991da829d4f8ecf74058c2d3b0e96`  
		Last Modified: Tue, 21 Nov 2023 06:17:35 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:878a93acb8c9c0743545b35b9e83c791e0934310697414160601636d4416f431`  
		Last Modified: Tue, 21 Nov 2023 06:17:36 GMT  
		Size: 4.8 KB (4783 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:1c95d6839d0df7f6903fc54fcab6d66c414582b97e5d99791ebcc637ba9ad940
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4869238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40b078756ebe2d7b4210adab614033772d6e0148442ad676ebd3be25b1a7ceaa`

```dockerfile
```

-	Layers:
	-	`sha256:b2c8994c974347780a31a1d8d3f98fb54446b26afd9a394361adcdd69bb8393c`  
		Last Modified: Tue, 21 Nov 2023 06:17:34 GMT  
		Size: 4.8 MB (4818610 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ff3bc0b85613405761afbf8ca4512980783a2b7aa8d35babda3020708f298c8f`  
		Last Modified: Tue, 21 Nov 2023 06:17:33 GMT  
		Size: 50.6 KB (50628 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:12-bookworm` - linux; arm variant v5

```console
$ docker pull postgres@sha256:512df42a227c4f7a1379d3dd93aabe69c4cdb404ebb44b345b9974fafd080743
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.8 MB (140764670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a7d466d700afadb194758fa078c8028b158aba00a705a5a7a468455634df1a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 09 Nov 2023 19:16:09 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Thu, 09 Nov 2023 19:16:09 GMT
CMD ["bash"]
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENV GOSU_VERSION=1.16
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8 # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENV LANG=en_US.utf8
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENV PG_MAJOR=12
# Thu, 09 Nov 2023 19:16:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Thu, 09 Nov 2023 19:16:09 GMT
ENV PG_VERSION=12.17-1.pgdg120+1
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 09 Nov 2023 19:16:09 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA" # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 09 Nov 2023 19:16:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Nov 2023 19:16:09 GMT
STOPSIGNAL SIGINT
# Thu, 09 Nov 2023 19:16:09 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 09 Nov 2023 19:16:09 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c863ca7dc37cc9d54f09d80f7efc95fc0178e7b263ee207d87b3e389318d50b`  
		Last Modified: Tue, 21 Nov 2023 19:33:50 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ae7dffa6f88c3231ae065b2ac8a5761d4fb2714fc9b620e0ce18c6a4e117c180`  
		Last Modified: Tue, 21 Nov 2023 19:33:51 GMT  
		Size: 4.0 MB (4040458 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:618ddb4421135e804b37d405cea3e86e469b42c704021086f6ee0061670f7084`  
		Last Modified: Tue, 21 Nov 2023 19:33:51 GMT  
		Size: 1.4 MB (1426029 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:455859c961c410c425f9371753d5cbd993096afe0f87500c5f1e96e07048815f`  
		Last Modified: Tue, 21 Nov 2023 19:33:51 GMT  
		Size: 8.1 MB (8067930 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eca058b52570a9e9b7bb7b375680edb208b96c6638aadcef52ed9cfa232f0743`  
		Last Modified: Tue, 21 Nov 2023 19:33:52 GMT  
		Size: 1.2 MB (1193943 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a38ac683c54e9d588bab738d12f1697b58ada140b9d7b6341cfbfcb39542d9d9`  
		Last Modified: Tue, 21 Nov 2023 19:33:52 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:851553c31be3fb45927fad8181b4d58067a5c9a020f90c5f984c4720cfb297fb`  
		Last Modified: Tue, 21 Nov 2023 19:33:52 GMT  
		Size: 3.1 KB (3141 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4e0c1e1ff8fd1c307c15c268e64b6e88c77c1090564be4bcb6b42a6b2220d8a4`  
		Last Modified: Tue, 21 Nov 2023 21:44:22 GMT  
		Size: 99.1 MB (99095622 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:238bb612cbe0ceeede5151c64cecf1696a567530a65e4db2ff02c33d804fd989`  
		Last Modified: Tue, 21 Nov 2023 21:44:19 GMT  
		Size: 9.0 KB (9025 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a63002f803af2fa4d6c6d91689f4048b8ee62a59387b894964371a72ddadc8a7`  
		Last Modified: Tue, 21 Nov 2023 21:44:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a3247720f5b3d417b103f0e7c4899dfd2fbdc7ce86fe93434273f8b0db03ebd8`  
		Last Modified: Tue, 21 Nov 2023 21:44:19 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c7f5d2e9f49d8166ec29f3ca3dc80321a82f3f85a736fb48c99338704939a425`  
		Last Modified: Tue, 21 Nov 2023 21:44:20 GMT  
		Size: 4.8 KB (4789 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:d80cbfa56241f48b1c72b36a9f6aff5fc8926b6b18458c3c1fdc4f167bbace40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 KB (50442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6704a94be1771ab5deeaa9599447628955b76dd279a5a621538c0a0e0414c0a2`

```dockerfile
```

-	Layers:
	-	`sha256:17304059d80a573107249ae3d79f08d8498eb9448fe10df029d038f77ef94524`  
		Last Modified: Tue, 21 Nov 2023 21:44:19 GMT  
		Size: 50.4 KB (50442 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:12-bookworm` - linux; arm variant v7

```console
$ docker pull postgres@sha256:1b497efd282b886e528546d1244c5017ec28e0cd0a69b307647aa3b374cdc705
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.7 MB (135689869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaf9df28c71d5493bdfe58d14ca2b98142d8578cbed48f25e6a7feabe97c2c1f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 01 Nov 2023 00:57:53 GMT
ADD file:fbe34fcf46c7cb91e83b67f7381d8971c97842aadd3e081994eaee4c08043106 in / 
# Wed, 01 Nov 2023 00:57:53 GMT
CMD ["bash"]
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENV GOSU_VERSION=1.16
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8 # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENV LANG=en_US.utf8
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENV PG_MAJOR=12
# Thu, 09 Nov 2023 19:16:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Thu, 09 Nov 2023 19:16:09 GMT
ENV PG_VERSION=12.17-1.pgdg120+1
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 09 Nov 2023 19:16:09 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA" # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 09 Nov 2023 19:16:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Nov 2023 19:16:09 GMT
STOPSIGNAL SIGINT
# Thu, 09 Nov 2023 19:16:09 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 09 Nov 2023 19:16:09 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:0a684901cedc28e6abb4cde4579d23d26345d871acd708a5bf266c562fe15b4d`  
		Last Modified: Wed, 01 Nov 2023 01:02:13 GMT  
		Size: 24.7 MB (24748900 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fbdf18656e8dc32c6bf84e2d712de9ae100a6d55ef304456701841a2e0356e52`  
		Last Modified: Wed, 01 Nov 2023 21:55:44 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6344a37e392af0d1fa4e388b695397daf2e8dd1dcdc06a1350194ada02b72c6a`  
		Last Modified: Wed, 01 Nov 2023 21:55:45 GMT  
		Size: 3.6 MB (3645034 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4acec71bc7f0d33db8c92c8e3c358e40e4dbff630fc752901512194e1984b060`  
		Last Modified: Wed, 01 Nov 2023 21:55:45 GMT  
		Size: 1.4 MB (1416144 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1e5230a03a21c4ed6d28bcda0049797f9ff0a600e82608b0408f1b5ff74c6c6`  
		Last Modified: Wed, 01 Nov 2023 21:55:45 GMT  
		Size: 8.1 MB (8067856 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9ec0ef3666ff187be863a6a7cfb8df5fc73fd620f23a70135a92e1d3f32224a1`  
		Last Modified: Wed, 01 Nov 2023 21:55:46 GMT  
		Size: 1.1 MB (1065947 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9ba47644b5f59ad9acdc66f0ee9bd264d698dd4df2e006b85f00b31b8b51f1ef`  
		Last Modified: Wed, 01 Nov 2023 21:55:46 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2d8130b13a1e83af85be2bc271b0d2465d9cabcd8b32e85cac10f52efeb47f08`  
		Last Modified: Wed, 01 Nov 2023 21:55:46 GMT  
		Size: 3.1 KB (3144 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7274d1df14ed7e3900fa7e89cae94082df10f92857670b3c3265720f0cf388e9`  
		Last Modified: Tue, 14 Nov 2023 04:42:30 GMT  
		Size: 96.7 MB (96727458 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:265f2a842300c2be6238e1d7f5c3e5a30cce94d2c055e4800a43ed011d0056ca`  
		Last Modified: Tue, 14 Nov 2023 04:42:27 GMT  
		Size: 9.0 KB (9021 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fcae968f3d141441ac794e561cacad794ea580a4e3a34df5f5af1cc2425a9ac8`  
		Last Modified: Tue, 14 Nov 2023 04:42:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:59cefa259f07e093839d77e0957a920021e2889ad486b19f5d83bddb26ef6d14`  
		Last Modified: Tue, 14 Nov 2023 04:42:27 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb2c22487abf1d5d149f42b8e09fb415ed0e85470557c76b7bf54b2b0a45b33b`  
		Last Modified: Tue, 14 Nov 2023 04:42:28 GMT  
		Size: 4.8 KB (4786 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:f5d21a2df1a6b4dda10c1c66a50577c16b7db00b3a44a0c4c88720838d100cdb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4880709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5efdaeda092a9c9b9896222d54f24776f1e0c3b7f92516f2fade42f91dcb0d8`

```dockerfile
```

-	Layers:
	-	`sha256:4ee50256b9abffcb66c26be8e38b9ea76b7707ded1ef36a9f857f2d589e35eac`  
		Last Modified: Tue, 14 Nov 2023 04:42:27 GMT  
		Size: 4.8 MB (4830052 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b6c65e11bc84c84c801d0a5523f0be5f41073c3b1073dc64753c6b87a449fccc`  
		Last Modified: Tue, 14 Nov 2023 04:42:27 GMT  
		Size: 50.7 KB (50657 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:12-bookworm` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:2b3bf31a240c5695b50c8949fee6d212bfde72b83f6b9bcec827fa9b9f7f5293
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.2 MB (146209044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c2bea28dc6413c7e3a640963383e087d5e172199d5d57cfa0eb897a81ea9aff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:41 GMT
ADD file:c58f86cd28b3a97f884e2a46f8fe60a2c5c1f443e198bd10e3277b4f3653736a in / 
# Wed, 01 Nov 2023 00:39:41 GMT
CMD ["bash"]
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENV GOSU_VERSION=1.16
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8 # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENV LANG=en_US.utf8
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENV PG_MAJOR=12
# Thu, 09 Nov 2023 19:16:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Thu, 09 Nov 2023 19:16:09 GMT
ENV PG_VERSION=12.17-1.pgdg120+1
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 09 Nov 2023 19:16:09 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA" # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 09 Nov 2023 19:16:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Nov 2023 19:16:09 GMT
STOPSIGNAL SIGINT
# Thu, 09 Nov 2023 19:16:09 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 09 Nov 2023 19:16:09 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:31ce7ceb6d443e2ab4ae91695fea10e1443417fd94c40a46994d5a96940ea1ca`  
		Last Modified: Wed, 01 Nov 2023 00:43:07 GMT  
		Size: 29.2 MB (29179119 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:28caef79f6eda62a2701ef8a65f2b7d831768c16d8a68e9b1f9d9cdf425bd7d1`  
		Last Modified: Wed, 01 Nov 2023 13:57:30 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:be24e278ddaad2d55a37b4bdbc7eb73194fceeafedcd70c268bafc55c385b8db`  
		Last Modified: Wed, 01 Nov 2023 13:57:30 GMT  
		Size: 4.4 MB (4383804 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dfdbb4d6f9a3bcfc8a4be67d1377969401d918889680a7c6b03049ea8699c9cd`  
		Last Modified: Wed, 01 Nov 2023 13:57:30 GMT  
		Size: 1.4 MB (1380679 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ebb06cfd45ecccc5e0239a087529125b8341766a2b42155b493d2a46ac62647c`  
		Last Modified: Wed, 01 Nov 2023 13:57:31 GMT  
		Size: 8.1 MB (8067936 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9738a56db3f94a601e623ff2ab30b771a53c00fbba904218f19fae742a30eba8`  
		Last Modified: Wed, 01 Nov 2023 13:57:31 GMT  
		Size: 1.1 MB (1107703 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:87cb08d2765cc07029f40344159144191287e4517518a2d578d765bfe0b268f0`  
		Last Modified: Wed, 01 Nov 2023 13:57:31 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d99960ffd545e8c2574f78896a028a84c1c70e91e2e475589403b80d2ece6d75`  
		Last Modified: Wed, 01 Nov 2023 13:57:32 GMT  
		Size: 3.1 KB (3141 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:21a03120b5e8ff92ef51f3bb337ac5d7f0e1e91e42b302438dfbcb5d16760fe1`  
		Last Modified: Tue, 14 Nov 2023 02:20:19 GMT  
		Size: 102.1 MB (102071277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1c7dcb9c7acbab6623105e95859730918e5cbbaafdce2e4970d4a107bd0693d0`  
		Last Modified: Tue, 14 Nov 2023 02:20:14 GMT  
		Size: 9.0 KB (9021 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ac0a7bac2b3a0e84a0b7729fb0a70610e3c4f022fd4ba31153a5859bac63aca3`  
		Last Modified: Tue, 14 Nov 2023 02:20:14 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7508b7bb43d3da8acdd0f8fd201d5cf65a5bc5386eb8ba5906cc4b1509045aed`  
		Last Modified: Tue, 14 Nov 2023 02:20:14 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6982b84c0351ee65772e44729546bc90504c196134203ce1c955a0ad1b2c2b0c`  
		Last Modified: Tue, 14 Nov 2023 02:20:15 GMT  
		Size: 4.8 KB (4785 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:b0de0bc8b54a5b410775d9af4f64817dddb778976a12319b90a86030564e0a68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4874130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0541d69414cb67e083f9e61f801435bc1e473ac7e61ab0f30a6f7a4e1e63d931`

```dockerfile
```

-	Layers:
	-	`sha256:8b675f427d868e3fcf0487a53d01166bec5510a34524597ba81da2f7e4334ba2`  
		Last Modified: Tue, 14 Nov 2023 02:20:15 GMT  
		Size: 4.8 MB (4823658 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f22567b27af076c1c1929df8ff071d3a3a1ca4b5294980c4a294af50dd16a5ec`  
		Last Modified: Tue, 14 Nov 2023 02:20:14 GMT  
		Size: 50.5 KB (50472 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:12-bookworm` - linux; 386

```console
$ docker pull postgres@sha256:6c1779f6e441b3654657722fb5a6d224d40518b056c2097030354ee6a7a1faac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.9 MB (152881737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9da2533d6eb45a3912724ecb705a79984523ddcdcdce012a15f8381aefa0f206`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 10 Aug 2023 18:14:30 GMT
ADD file:0c94521fdd9c0a4fdeeb9aad23e68cd053fba0dcd7c3af550aefa79377816e31 in / 
# Thu, 10 Aug 2023 18:14:30 GMT
CMD ["bash"]
# Thu, 10 Aug 2023 18:14:30 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 10 Aug 2023 18:14:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 10 Aug 2023 18:14:30 GMT
ENV GOSU_VERSION=1.16
# Thu, 10 Aug 2023 18:14:30 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 10 Aug 2023 18:14:30 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8 # buildkit
# Thu, 10 Aug 2023 18:14:30 GMT
ENV LANG=en_US.utf8
# Thu, 10 Aug 2023 18:14:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 10 Aug 2023 18:14:30 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 10 Aug 2023 18:14:30 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 10 Aug 2023 18:14:30 GMT
ENV PG_MAJOR=12
# Thu, 10 Aug 2023 18:14:30 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Thu, 10 Aug 2023 18:14:30 GMT
ENV PG_VERSION=12.16-1.pgdg120+1
# Thu, 10 Aug 2023 18:14:30 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 10 Aug 2023 18:14:30 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 10 Aug 2023 18:14:30 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql # buildkit
# Thu, 10 Aug 2023 18:14:30 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 10 Aug 2023 18:14:30 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA" # buildkit
# Thu, 10 Aug 2023 18:14:30 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 10 Aug 2023 18:14:30 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 10 Aug 2023 18:14:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Aug 2023 18:14:30 GMT
STOPSIGNAL SIGINT
# Thu, 10 Aug 2023 18:14:30 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 10 Aug 2023 18:14:30 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:98bdfce9af831c2a0d0bfcca812d0039cd1666986550f552b4b4c625bd5aa31c`  
		Last Modified: Wed, 01 Nov 2023 00:43:26 GMT  
		Size: 30.2 MB (30164042 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4582fba6a6b8ce4dadabfa190b174287f71e0b58bfb68c7f036606832f06c701`  
		Last Modified: Wed, 01 Nov 2023 01:17:38 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3b8774ce1dc14705e3c1a21e6ac84664103dcad7ba1c85e200c204621cb818af`  
		Last Modified: Wed, 01 Nov 2023 01:17:39 GMT  
		Size: 4.8 MB (4844493 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cef83864c3baddfdaaa53e412071ab6a7862c1822cefe3760e7e84749f486ebb`  
		Last Modified: Wed, 01 Nov 2023 01:17:39 GMT  
		Size: 1.4 MB (1424509 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:691a973fb62e325092ec5794cffc332292265318a03bfa7cc92af6bd29ab2f6f`  
		Last Modified: Wed, 01 Nov 2023 01:17:39 GMT  
		Size: 8.1 MB (8067907 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d0fd2a5e5f5224a66448158a89a9b3c061fe5cb4fa9e2cc52ad4c9affd8c4e6d`  
		Last Modified: Wed, 01 Nov 2023 01:17:40 GMT  
		Size: 1.1 MB (1136158 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:86abc5998037db54717a1627c6707283ce4f8825d26301b94ecc10ea9ec57b22`  
		Last Modified: Wed, 01 Nov 2023 01:17:40 GMT  
		Size: 114.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:844a7bd861321febe7d4fc6bd74d7d52d82b303b5c637c60602610ad7a968c3f`  
		Last Modified: Wed, 01 Nov 2023 01:17:40 GMT  
		Size: 3.1 KB (3144 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a84062cf214d619ffbf0b6c9ea4fbf2cde3b8443eb834d4af25c991f1db150dc`  
		Last Modified: Wed, 01 Nov 2023 01:17:47 GMT  
		Size: 107.2 MB (107226093 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:11fc1f3609e42b70433a1dace8bfe9411f5d455e794c87cb9b63107d1224dfa8`  
		Last Modified: Wed, 01 Nov 2023 01:17:41 GMT  
		Size: 9.0 KB (9031 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7a433f6b76fbe1613cebbee247f55a48dfa4a9f254a28f7fa53d124821678e30`  
		Last Modified: Wed, 01 Nov 2023 01:17:41 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:740bac833c4f1fccf7c9c40e1a47c6da7b30a1d13843e55822bdaf6a69da8bb3`  
		Last Modified: Wed, 01 Nov 2023 01:17:41 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cc40f7ba26a6fa2d6efc8fe8336d48bfd99436a9259befaebd721c78440bbcf9`  
		Last Modified: Wed, 01 Nov 2023 01:17:42 GMT  
		Size: 4.8 KB (4786 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:9854212405666bf9991e01b7d42b758bcabdf5ae4c586290b78f7ca795781eb3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 KB (50365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba39ec182cfe99409e0f6c92f68ec3955134d0cea8664e8487cd6c84b842c493`

```dockerfile
```

-	Layers:
	-	`sha256:0fb1322b6fec20881cee8c239e93c8ac3ef1410a63aaa344712980aa91733180`  
		Last Modified: Wed, 01 Nov 2023 01:17:38 GMT  
		Size: 50.4 KB (50365 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:12-bookworm` - linux; mips64le

```console
$ docker pull postgres@sha256:71888887ea62a4e7274cc7f2981f901a5e07d2df19d53880771aef3ecaf503ec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.1 MB (144061218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2876b24f78cc15543b822667c0132d4adca9e9758cc020ca43eec7901498abd7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 01 Nov 2023 01:09:01 GMT
ADD file:902f83a7b431527b044dd807bec38e30f5402c6a655e71f1c8addec0f384768f in / 
# Wed, 01 Nov 2023 01:09:05 GMT
CMD ["bash"]
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENV GOSU_VERSION=1.16
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8 # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENV LANG=en_US.utf8
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENV PG_MAJOR=12
# Thu, 09 Nov 2023 19:16:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Thu, 09 Nov 2023 19:16:09 GMT
ENV PG_VERSION=12.17-1.pgdg120+1
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 09 Nov 2023 19:16:09 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA" # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 09 Nov 2023 19:16:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Nov 2023 19:16:09 GMT
STOPSIGNAL SIGINT
# Thu, 09 Nov 2023 19:16:09 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 09 Nov 2023 19:16:09 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:0d679670615aaadf144eccb296137109a3362efe18b995cdfda7614231abd659`  
		Last Modified: Wed, 01 Nov 2023 01:19:46 GMT  
		Size: 29.1 MB (29141870 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e26dc7a88cd94a47dcdf46dd8941a8ba20f07c145d4dc40204f981480ab4df7c`  
		Last Modified: Thu, 02 Nov 2023 07:51:30 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f3870d7d2753e51b333afe5ed9ac1a7efc30bdf39fa1d3fbb8a982f4a70b9c6c`  
		Last Modified: Thu, 02 Nov 2023 07:51:31 GMT  
		Size: 4.4 MB (4355736 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:679f01e71a1f1723f5afebe16e6d33b071ebad0d05a28fc91292789d0b39c480`  
		Last Modified: Thu, 02 Nov 2023 07:51:31 GMT  
		Size: 1.3 MB (1335964 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:963c26d03998a51743c509b01a4b57806a7ae842771baff863c77a33367515da`  
		Last Modified: Thu, 02 Nov 2023 07:51:32 GMT  
		Size: 8.1 MB (8068075 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8e261c38676ca25c35cdb358ac9a8f86859b54ef18d83c7ec43c80ff4216118f`  
		Last Modified: Thu, 02 Nov 2023 07:51:32 GMT  
		Size: 1.2 MB (1181574 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6f6bd5cafaf2ee33a9f182395567084dd7a49771595fbb0d79aba13c9e652589`  
		Last Modified: Thu, 02 Nov 2023 07:51:33 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:25fc4a78d2b1d6620076aac432f0a2036b3bcdfa6438b8f0c5deb7ba0d8b471a`  
		Last Modified: Thu, 02 Nov 2023 07:51:32 GMT  
		Size: 3.1 KB (3144 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a737176673f6c1ad5d0c53f79ea11b99cbea964b94379e58a54f676df1eea1f0`  
		Last Modified: Tue, 14 Nov 2023 11:14:17 GMT  
		Size: 100.0 MB (99959463 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:843821859e2305d25c8c41bd45bf81b39454b06e04b135db87866e37c2a6d239`  
		Last Modified: Tue, 14 Nov 2023 11:14:07 GMT  
		Size: 9.0 KB (9027 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7aa030f09e92ecd678a63cb6d2e8d3b3bf1bc14bfd53de1101ab16535c32973d`  
		Last Modified: Tue, 14 Nov 2023 11:14:07 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da78b072fb6ada281101da54567c52087f0ca7c678e969dfa27dbd3d9e163f15`  
		Last Modified: Tue, 14 Nov 2023 11:14:07 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d500c3ee8cb61ee45c29819e47a7bb7d03e797304439cf63184ff9d4a922003b`  
		Last Modified: Tue, 14 Nov 2023 11:14:08 GMT  
		Size: 4.8 KB (4788 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:ad48ba17becadf5d659dd34437a30f0e172f25a5950d10122597f896f0076eaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 KB (50329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24f7c4e920a2396437d270a1fc69f59e84ce33fc08a26129c4b7bbd4f0ba2822`

```dockerfile
```

-	Layers:
	-	`sha256:46c85ac073ac3527f37bbb6c90de126aea46d48c4ea9b14737c825f442d8536b`  
		Last Modified: Tue, 14 Nov 2023 11:14:07 GMT  
		Size: 50.3 KB (50329 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:12-bookworm` - linux; ppc64le

```console
$ docker pull postgres@sha256:57a4c777e14fab269eb796afcac5ba4ddf758500a36c769400f2d61456ea82c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.1 MB (160064805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e689f8a988a15c8927b10d4b9f821cde28b3b4d4eb4f16947d315fe934e87766`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:39 GMT
ADD file:f36d600ab8508979b5763875a75f35555fa0a83d2656cbcdfa50978c6ae97353 in / 
# Wed, 01 Nov 2023 00:21:41 GMT
CMD ["bash"]
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENV GOSU_VERSION=1.16
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8 # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENV LANG=en_US.utf8
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENV PG_MAJOR=12
# Thu, 09 Nov 2023 19:16:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Thu, 09 Nov 2023 19:16:09 GMT
ENV PG_VERSION=12.17-1.pgdg120+1
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 09 Nov 2023 19:16:09 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA" # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 09 Nov 2023 19:16:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Nov 2023 19:16:09 GMT
STOPSIGNAL SIGINT
# Thu, 09 Nov 2023 19:16:09 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 09 Nov 2023 19:16:09 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:e56c8f20d7d119ff87eb044f21bfd5a4b30bf8436fc5fac12871095a6bd1517c`  
		Last Modified: Wed, 01 Nov 2023 00:26:10 GMT  
		Size: 33.1 MB (33141482 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:10492c076a5482ef3ee20f8ae7f3e9f32b8b077620de814be68cbf66942f34da`  
		Last Modified: Thu, 02 Nov 2023 00:52:34 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9275155c01fdde71c05227748bc502803cf4154c0248cb63c6d52d8829a39c39`  
		Last Modified: Thu, 02 Nov 2023 00:52:35 GMT  
		Size: 5.2 MB (5239263 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e20bf10779df26266aa42f231a654459176eec7565c25692f2f3d190983155b7`  
		Last Modified: Thu, 02 Nov 2023 00:52:35 GMT  
		Size: 1.4 MB (1370000 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b3fd8e907e8a12a5bb5b3e1bad3b5c9f20d2a33b3865db73f4975810b967278d`  
		Last Modified: Thu, 02 Nov 2023 00:52:36 GMT  
		Size: 8.1 MB (8067981 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6368a98230e1f08b09679b2c4349acb80892e96a442f105a42e0dad0ffbaea0a`  
		Last Modified: Thu, 02 Nov 2023 00:52:36 GMT  
		Size: 1.3 MB (1282767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:37f44d82a127013872334d7d0adc56feaedcfb24c18b57ac82938a20fd6c85df`  
		Last Modified: Thu, 02 Nov 2023 00:52:36 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ff0cdb2e4019174bd3e36693c000523c31a0c33f61759262e15e5cdfd169e52`  
		Last Modified: Thu, 02 Nov 2023 00:52:36 GMT  
		Size: 3.1 KB (3144 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0707436c434e7bbf2dbadb68ed46224a863219dd2f2f809508c233ddb52c44b1`  
		Last Modified: Tue, 14 Nov 2023 02:33:45 GMT  
		Size: 110.9 MB (110944782 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a5b59d9adbba59fd06c1fe591456ecb85e69148b3f11a07b92a24018afbd64b1`  
		Last Modified: Tue, 14 Nov 2023 02:33:41 GMT  
		Size: 9.0 KB (9025 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:17028b306a1f5844745ec2b4b0436bc626464f997384107a96fa8152350af0c7`  
		Last Modified: Tue, 14 Nov 2023 02:33:40 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b53a717b2608eae039b969ba15f4b5533eddc59aff7ce11ff7b533709dfc5317`  
		Last Modified: Tue, 14 Nov 2023 02:33:41 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5cf4ff912538d74960b5b7da417818dd870838e6aebcd920193418149dc57aed`  
		Last Modified: Tue, 14 Nov 2023 02:33:41 GMT  
		Size: 4.8 KB (4783 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:1126ba5d204b7e071788910d1186f2aaff6c2c7611350c6a44603f592b7f6154
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4875746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7a71daac0730d14e76d85eba6444d3200963bba38b4b4a3cdcc09b2368d40a6`

```dockerfile
```

-	Layers:
	-	`sha256:47297370f57610b90e304d188681648fd13c977f82ad079d5639c9ac624c4991`  
		Last Modified: Tue, 14 Nov 2023 02:33:41 GMT  
		Size: 4.8 MB (4825227 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ae39f70643d2577db930188d59259ca6aa9661de5c5bc892bd95cf14bf431001`  
		Last Modified: Tue, 14 Nov 2023 02:33:40 GMT  
		Size: 50.5 KB (50519 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:12-bookworm` - linux; s390x

```console
$ docker pull postgres@sha256:918a8ed2542dcb58e52f037d1e47f4c63f090ce2f9257ef9af67cc9a7513dee5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.6 MB (153591063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b619b77aeec123d6a404c66e1b01e6a7d5a36237c89a51819952e1f597645f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 09 Nov 2023 19:16:09 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Thu, 09 Nov 2023 19:16:09 GMT
CMD ["bash"]
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENV GOSU_VERSION=1.16
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8 # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENV LANG=en_US.utf8
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENV PG_MAJOR=12
# Thu, 09 Nov 2023 19:16:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Thu, 09 Nov 2023 19:16:09 GMT
ENV PG_VERSION=12.17-1.pgdg120+1
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 09 Nov 2023 19:16:09 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA" # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 09 Nov 2023 19:16:09 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 09 Nov 2023 19:16:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Nov 2023 19:16:09 GMT
STOPSIGNAL SIGINT
# Thu, 09 Nov 2023 19:16:09 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 09 Nov 2023 19:16:09 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89216ae53f720b4da9522deb1c8896d66a743dbc83d0ab5356ccf6bf6c0ad8e4`  
		Last Modified: Tue, 21 Nov 2023 18:22:46 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8bd1123ed4c50e7e0d7ff3fb10d11792421107339b8201d7dea2bde635cf5d86`  
		Last Modified: Tue, 21 Nov 2023 18:22:46 GMT  
		Size: 4.3 MB (4278291 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:86d8142ebc194d7418f51ad332e0a79f3e1a575f2503f46b4f93cb085d5812f4`  
		Last Modified: Tue, 21 Nov 2023 18:22:46 GMT  
		Size: 1.4 MB (1414350 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:06692ba87c4c56ba5fa93bef232b01a7087875351540daebfdff46dd5c3bc834`  
		Last Modified: Tue, 21 Nov 2023 18:22:46 GMT  
		Size: 8.1 MB (8122208 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6068c51b298204ad2608f4a906160c9749c057bc056e26b1ba79715761b391c0`  
		Last Modified: Tue, 21 Nov 2023 18:22:47 GMT  
		Size: 1.1 MB (1095680 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a2b031c4de2d2726bdaa88b1fb2ff2bef864e96adb293b76faaa47facd0235ea`  
		Last Modified: Tue, 21 Nov 2023 18:22:47 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d2508545e1ea1dbe7e27a83463f8337ac42fcfb626c048a9e6364b34354a0a24`  
		Last Modified: Tue, 21 Nov 2023 18:22:47 GMT  
		Size: 3.1 KB (3141 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c27f497f611b4ce7cbaff45e0ca2ec55d44980788e4aca7a71d22900416f5ab0`  
		Last Modified: Tue, 21 Nov 2023 18:56:51 GMT  
		Size: 111.1 MB (111149116 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ae352b5955e44d0abf66d860d20d389b3cdad22168b7c529efa15dde72ab3e3`  
		Last Modified: Tue, 21 Nov 2023 18:56:48 GMT  
		Size: 9.0 KB (9026 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c8f18fcb9921b9b49f2196fc42ca913fe6f96fb1c43152059901a2c4894077d9`  
		Last Modified: Tue, 21 Nov 2023 18:56:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c916b05369ee71c947a28b448b5988c2aa78f269555329b3fa502b0164e02823`  
		Last Modified: Tue, 21 Nov 2023 18:56:48 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b832505f7a46535d9ac6e1932e685f0a4612c656b6da16536285dc2440a7293d`  
		Last Modified: Tue, 21 Nov 2023 18:56:49 GMT  
		Size: 4.8 KB (4785 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:50de068c0b7ff25acbea0d563f4478e07c630fe6326043ba3ac3e2724203a0ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4868254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edca3186babd419df6a14f3ac7bfcff92f95ca2b725b8fe7f1165feebe3b7627`

```dockerfile
```

-	Layers:
	-	`sha256:494f72a99a90cd6cf22acdc893b18a94eb68d805df16badb8e9fe4900259cabb`  
		Last Modified: Tue, 21 Nov 2023 18:56:48 GMT  
		Size: 4.8 MB (4817792 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a3347e1dcbcbd678b86207a2742e0cc368cf25439712c0dad12b49bd2b417d99`  
		Last Modified: Tue, 21 Nov 2023 18:56:48 GMT  
		Size: 50.5 KB (50462 bytes)  
		MIME: application/vnd.in-toto+json
