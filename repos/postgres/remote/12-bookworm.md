## `postgres:12-bookworm`

```console
$ docker pull postgres@sha256:802b83e49f9fb79618dab8bca32c825982e516723c9a45911ed67f09ac89e07a
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
$ docker pull postgres@sha256:e907922c47bdbaa67f210578ee8af3272c08853059916bcf56bc54b6d550f5d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.9 MB (147938062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4a7b5d790eb0b98d3954538d46245b6033202b14e441a89495a6771e2810e83`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 11 Dec 2023 18:58:54 GMT
ADD file:ac3cd70031d35e46d86b876934946ffc8756de4de065fbc926dce642dac07ff3 in / 
# Mon, 11 Dec 2023 18:58:54 GMT
CMD ["bash"]
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV GOSU_VERSION=1.16
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	echo 'en_US.UTF-8 UTF-8' >> /etc/locale.gen; 	locale-gen; 	locale -a | grep 'en_US.utf8' # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV LANG=en_US.utf8
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_MAJOR=12
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_VERSION=12.17-1.pgdg120+1
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 11 Dec 2023 18:58:54 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 11 Dec 2023 18:58:54 GMT
COPY docker-entrypoint.sh docker-ensure-initdb.sh /usr/local/bin/ # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN ln -sT docker-ensure-initdb.sh /usr/local/bin/docker-enforce-initdb.sh # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Dec 2023 18:58:54 GMT
STOPSIGNAL SIGINT
# Mon, 11 Dec 2023 18:58:54 GMT
EXPOSE map[5432/tcp:{}]
# Mon, 11 Dec 2023 18:58:54 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:af107e978371b6cd6339127a05502c5eacd1e6b0e9eb7b2f4aa7b6fc87e2dd81`  
		Last Modified: Tue, 19 Dec 2023 01:24:59 GMT  
		Size: 29.1 MB (29125963 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:161c4a1c9e47b029f2cc04e9eddc636470a684db6f6da8d31474225fa244c342`  
		Last Modified: Tue, 19 Dec 2023 03:49:21 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:068ec7aef1c0475eb9208aef89043283f82b8c0a65010bc0874d110fca2bd213`  
		Last Modified: Tue, 19 Dec 2023 03:49:21 GMT  
		Size: 4.4 MB (4422568 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:84cb495413f5df78e343e0cddc9a037c95053122c83cc9c8c02e0dea4f22842f`  
		Last Modified: Tue, 19 Dec 2023 03:49:21 GMT  
		Size: 1.4 MB (1445246 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b9c266e38bb6c0bc9deb9d1d14e4ac29e72d3387b7d808f87ca9145aa3218d1`  
		Last Modified: Tue, 19 Dec 2023 03:49:21 GMT  
		Size: 8.1 MB (8065463 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:abf3132b55e359d68af11fea94492f932e41913b601b2fa3a662878a7f5099d6`  
		Last Modified: Tue, 19 Dec 2023 03:49:22 GMT  
		Size: 1.2 MB (1195102 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:61755c2bbafa90e77b0b8d5e29e4ffa8c052cceca38a07ddc7f6fa275168076d`  
		Last Modified: Tue, 19 Dec 2023 03:49:22 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dcc6b87767cd2725ebc5fc83d74bed259c2c6fa0b390fb56b122e7f5b4c9523a`  
		Last Modified: Tue, 19 Dec 2023 03:49:22 GMT  
		Size: 3.1 KB (3141 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:844bb6ff3ef2b1f81c2e2730e4e13372370a6b26003a6b18c2f23ed82de383cd`  
		Last Modified: Tue, 19 Dec 2023 03:49:24 GMT  
		Size: 103.7 MB (103664455 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee304895c401e9d2e1484a5c556770814b423401e3c250060b4f129c5f8de685`  
		Last Modified: Tue, 19 Dec 2023 03:49:23 GMT  
		Size: 9.0 KB (9021 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a107841a059993d8eaf0a3fdc22449ec6c6db286c5bd296cd16940e5e31438b`  
		Last Modified: Tue, 19 Dec 2023 03:49:23 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69b04a3aa9642f1881758da6ab97638f97d44c969b0216afa0b409d1c14f1f29`  
		Last Modified: Tue, 19 Dec 2023 03:49:23 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ea1f902e0429bc7bcbba9e62fc8959b44001ed26e6c453e89f77fadcbeba3cf`  
		Last Modified: Tue, 19 Dec 2023 03:49:24 GMT  
		Size: 5.3 KB (5339 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d36a0d8fbcc1cf9a46299d9110d3d33b2b97ffc0785d2127761f08ec3d857083`  
		Last Modified: Tue, 19 Dec 2023 03:49:23 GMT  
		Size: 185.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:9e19ff7cd5abe9596384fe14739f63e3ed9d3c8210fde23ccf4e6c89c2464262
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4872824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0895bec4e69ac2af1f1183c466a465d14c29a4bb3b6e936b6e6c7c0622c6ae95`

```dockerfile
```

-	Layers:
	-	`sha256:384f6e773da38dac22313b003800ed0b2d2de21952cd87763a5dabaf22f6a2aa`  
		Last Modified: Tue, 19 Dec 2023 03:49:21 GMT  
		Size: 4.8 MB (4818755 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:89dffef0b53b43bd34244d9c5e53db9b6f0b57e1e8ac01db4df3a7812f533eb7`  
		Last Modified: Tue, 19 Dec 2023 03:49:21 GMT  
		Size: 54.1 KB (54069 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:12-bookworm` - linux; arm variant v5

```console
$ docker pull postgres@sha256:5117520b46521f579027cb205db31a0efd4f6d8ca300a23d1fb28dfe6f02a981
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.7 MB (140664852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4019c95d532e7cc4e6a20e7bbe78791e6b561e08f891ef7c606ba5b53a9227b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 11 Dec 2023 18:58:54 GMT
ADD file:9503ab966c9dd707eeccc7c2f633bccc94c199f8714ec4ff2c8b54dde3dbabf9 in / 
# Mon, 11 Dec 2023 18:58:54 GMT
CMD ["bash"]
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV GOSU_VERSION=1.16
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	echo 'en_US.UTF-8 UTF-8' >> /etc/locale.gen; 	locale-gen; 	locale -a | grep 'en_US.utf8' # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV LANG=en_US.utf8
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_MAJOR=12
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_VERSION=12.17-1.pgdg120+1
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 11 Dec 2023 18:58:54 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 11 Dec 2023 18:58:54 GMT
COPY docker-entrypoint.sh docker-ensure-initdb.sh /usr/local/bin/ # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN ln -sT docker-ensure-initdb.sh /usr/local/bin/docker-enforce-initdb.sh # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Dec 2023 18:58:54 GMT
STOPSIGNAL SIGINT
# Mon, 11 Dec 2023 18:58:54 GMT
EXPOSE map[5432/tcp:{}]
# Mon, 11 Dec 2023 18:58:54 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:1ae9a2844c8c70942d2220553689b62e841cc706d77284fbfedbd770080fd699`  
		Last Modified: Tue, 19 Dec 2023 01:58:33 GMT  
		Size: 26.9 MB (26885440 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8562258818e323a73ddb0c31f9aad6745d00db79840d539c874bbe443ae0cb0b`  
		Last Modified: Tue, 19 Dec 2023 16:26:27 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:49f4ae0ebcef3a24a1c7aa8bcccd14716057287082db75d3aedc37080803cc1d`  
		Last Modified: Tue, 19 Dec 2023 16:26:28 GMT  
		Size: 4.0 MB (4040554 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:18c0d447effabeb85c059668474bc364967fc416cc6a4d3ba8c090b415ceb457`  
		Last Modified: Tue, 19 Dec 2023 16:26:28 GMT  
		Size: 1.4 MB (1422861 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:99854b875aacbbf2a16f6731d087ffe2d0b84954569e0c122f04909d943e3939`  
		Last Modified: Tue, 19 Dec 2023 16:26:28 GMT  
		Size: 8.1 MB (8065640 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:782fd948b1e3069939f324a104c412ea1910036f8eb13f230cca450c5ba9cdd0`  
		Last Modified: Tue, 19 Dec 2023 16:26:29 GMT  
		Size: 1.2 MB (1193959 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fa79161bb2d9691a29e379f6b2eb196735dd890ab77403002bb96f59beacb4be`  
		Last Modified: Tue, 19 Dec 2023 16:26:29 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0d3255b24598010853a039785388b60e37ff974670724c6e0e7c42bee395330c`  
		Last Modified: Tue, 19 Dec 2023 16:26:29 GMT  
		Size: 3.1 KB (3142 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d21e54eec7f00cd4462bf7dfbff83affd30d7c9a66aee8abfa52fab93b32dc16`  
		Last Modified: Tue, 19 Dec 2023 18:50:38 GMT  
		Size: 99.0 MB (99037120 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c6ff5df2a9ba32424407ffd3179edf8f51b2413cf7f69c4d9bdd8b467e2db833`  
		Last Modified: Tue, 19 Dec 2023 18:50:35 GMT  
		Size: 9.0 KB (9028 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e14d8f2ce2a42751d5d72fbd9e86b20d40a98a6795c116e8815f69d76478c6d`  
		Last Modified: Tue, 19 Dec 2023 18:50:35 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3cdb861d31800c5a2dab9ebde3dfb8271a126753d2f148aeff90f94a45beb837`  
		Last Modified: Tue, 19 Dec 2023 18:50:35 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:23e67e3d785fdaa7728787475b29b1014de5ed1286b2adcce96ab74df89ff5ad`  
		Last Modified: Tue, 19 Dec 2023 18:50:36 GMT  
		Size: 5.3 KB (5343 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4bfc71f04c122a990e20ac38584920ddf9e6f195eccde0ff2551919d34af68ca`  
		Last Modified: Tue, 19 Dec 2023 18:50:36 GMT  
		Size: 185.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:4d6f31831198efbfced778326c0342931ec4088e533ffe3b7b51694056626226
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.9 KB (53894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3555dc69401ddc3f3e173e528d0c1cf3fc1ff61925c5201d9fb37b35df18dbf`

```dockerfile
```

-	Layers:
	-	`sha256:4f41dc1595252b909ba2f16b70e5937558c64b58821b829d0adb86f18d228900`  
		Last Modified: Tue, 19 Dec 2023 18:50:35 GMT  
		Size: 53.9 KB (53894 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:12-bookworm` - linux; arm variant v7

```console
$ docker pull postgres@sha256:ae53da578b04a13afc8093e2024710d2208d70ae4326970cc0611ed63b9d0852
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.7 MB (135688566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e3eb7fd0d369f3975efcd221b9fa1a3ef6dbea2e968c06fb29aac5885eee2ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:43 GMT
ADD file:b693944382a95fa47622fde77eb98f0cdeafa40261e7334bd355e00f650b6632 in / 
# Tue, 21 Nov 2023 03:57:43 GMT
CMD ["bash"]
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV GOSU_VERSION=1.16
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	echo 'en_US.UTF-8 UTF-8' >> /etc/locale.gen; 	locale-gen; 	locale -a | grep 'en_US.utf8' # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV LANG=en_US.utf8
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_MAJOR=12
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_VERSION=12.17-1.pgdg120+1
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 11 Dec 2023 18:58:54 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 11 Dec 2023 18:58:54 GMT
COPY docker-entrypoint.sh docker-ensure-initdb.sh /usr/local/bin/ # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN ln -sT docker-ensure-initdb.sh /usr/local/bin/docker-enforce-initdb.sh # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Dec 2023 18:58:54 GMT
STOPSIGNAL SIGINT
# Mon, 11 Dec 2023 18:58:54 GMT
EXPOSE map[5432/tcp:{}]
# Mon, 11 Dec 2023 18:58:54 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:b4ce590529bbcf84326048a22fce76fcfcb5c60af5519debd7935a74c1e9126e`  
		Last Modified: Tue, 21 Nov 2023 04:01:50 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a21f4aebb739ffe9e0940e28d247a8da2f821a7f31a7802ddbeec56c29d382fe`  
		Last Modified: Wed, 22 Nov 2023 01:33:09 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ec8cff5cb7280b5e856a5c26b4275967808fa3cd8f286358a620731f3890ddf5`  
		Last Modified: Wed, 22 Nov 2023 01:33:09 GMT  
		Size: 3.6 MB (3645045 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1afbab58653c806dee1842134bc232fc8cc4443e53a1fe16a5c8e0585e94bce`  
		Last Modified: Wed, 22 Nov 2023 01:33:09 GMT  
		Size: 1.4 MB (1416140 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:86b3f0fa04d232a3c3ce72e77065c901b3902f976c0029d8a166a9035f5c3bb2`  
		Last Modified: Sat, 09 Dec 2023 05:37:40 GMT  
		Size: 8.1 MB (8067932 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4e59493675a5375d463b6e5328bd150d0f19c59eb446ca5a1fcc643d0210d59a`  
		Last Modified: Sat, 09 Dec 2023 05:37:39 GMT  
		Size: 1.1 MB (1065978 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:99e280b4019edf92089c2093350fcc13ea707026f191d4b42dc860f3c8d08874`  
		Last Modified: Sat, 09 Dec 2023 05:37:39 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f16f8fa83f99c03bc7c7e540ed27c4ed91ffd63085a00fe5dafad7d2fec0db7e`  
		Last Modified: Sat, 09 Dec 2023 05:37:39 GMT  
		Size: 3.1 KB (3145 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a37e3530825c49b308e93f782e17adfbec208eefe7797b0bc351dcb15f085735`  
		Last Modified: Sat, 09 Dec 2023 07:59:27 GMT  
		Size: 96.7 MB (96725262 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5dbf8e048f714ecf6ef6f22e001c04a5670ca428e9fd91f3a8d4dcb85fc1c93e`  
		Last Modified: Sat, 09 Dec 2023 07:59:24 GMT  
		Size: 9.0 KB (9030 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:981b660d30f696f623267dc904242dee53645a1bcaba1a195d92c4e5ab921377`  
		Last Modified: Sat, 09 Dec 2023 07:59:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8f61a930c9baa32c090e06a18a41161cb7080f8bbf96bc13d350b5ff520a1da8`  
		Last Modified: Sat, 09 Dec 2023 07:59:24 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e23827b70bc4c39916b31aabaa5a40fa4a8c043c77be40eba8810a1ffa8ecff4`  
		Last Modified: Thu, 14 Dec 2023 19:32:41 GMT  
		Size: 5.3 KB (5341 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c6469d8572ebcf992c361966395a6ee2d6bfcdff653112f61e22f292629e584`  
		Last Modified: Thu, 14 Dec 2023 19:32:41 GMT  
		Size: 187.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:5801e9a4317b7fedf1f15b4ee0f407189ad3445747acd33e3691e58a07a684e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4884806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a65b3c04923adbad156f6d606e44080ce58ddb1a9c9b90be655046476f3eabcd`

```dockerfile
```

-	Layers:
	-	`sha256:ec234a95cbcdd3645e443ac725402d386dfcfd1363b1efcecbc44bb6ca0f4381`  
		Last Modified: Thu, 14 Dec 2023 19:32:41 GMT  
		Size: 4.8 MB (4830697 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:89857587445bd0da7c6c8ba8a5d281f41eb1028288adabd9dab5d483762895dd`  
		Last Modified: Thu, 14 Dec 2023 19:32:41 GMT  
		Size: 54.1 KB (54109 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:12-bookworm` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:d57977c59a6d6be8b5eea97610c93d89cd655741658063bc71e80e94c5be366c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.5 MB (148483462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:933f0cc466d5aa969c7bd8e478f3d2fe08668cb1f083acaf833fa09abbae58f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV GOSU_VERSION=1.16
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	echo 'en_US.UTF-8 UTF-8' >> /etc/locale.gen; 	locale-gen; 	locale -a | grep 'en_US.utf8' # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV LANG=en_US.utf8
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_MAJOR=12
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_VERSION=12.17-1.pgdg120+1
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 11 Dec 2023 18:58:54 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 11 Dec 2023 18:58:54 GMT
COPY docker-entrypoint.sh docker-ensure-initdb.sh /usr/local/bin/ # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN ln -sT docker-ensure-initdb.sh /usr/local/bin/docker-enforce-initdb.sh # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Dec 2023 18:58:54 GMT
STOPSIGNAL SIGINT
# Mon, 11 Dec 2023 18:58:54 GMT
EXPOSE map[5432/tcp:{}]
# Mon, 11 Dec 2023 18:58:54 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cd877d542a822f9ecce74f11c6a6d6bc2512458fd5c9ae59e80bf253e8f4503d`  
		Last Modified: Thu, 14 Dec 2023 20:18:12 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ef4dec12b244d9ba0626e42c85cbca029218dd4c7fc7c43a5ecaca223a077097`  
		Last Modified: Thu, 14 Dec 2023 20:18:12 GMT  
		Size: 4.4 MB (4383850 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b4793e74422cf7be3ab549d686371ef745d4b3bc244d5e527b87a50553aa95ef`  
		Last Modified: Thu, 14 Dec 2023 20:18:12 GMT  
		Size: 1.4 MB (1380705 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:12f6bc37ee294e1b784512aff3d6208f2740302f512c4905f5438b63b5295611`  
		Last Modified: Thu, 14 Dec 2023 20:18:13 GMT  
		Size: 8.1 MB (8067957 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd9c37dc95ed39c1b71fa1969d8b622c00a382b2e6162d370d038bdae0b64d94`  
		Last Modified: Thu, 14 Dec 2023 20:18:13 GMT  
		Size: 1.1 MB (1107714 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:413b8cf9d665aba3d2b78b1c797c55d20d845d66adb615ea29e11c53c3368637`  
		Last Modified: Thu, 14 Dec 2023 20:18:13 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1c95e694bd99f3ff824cef87cf028c51806719d87e1a0c74d756b275eaabfaf2`  
		Last Modified: Thu, 14 Dec 2023 20:18:13 GMT  
		Size: 3.1 KB (3142 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4193a4794446470c4b9edfe0a779928a2469445201183b4daad02e37872f432e`  
		Last Modified: Thu, 14 Dec 2023 20:29:14 GMT  
		Size: 104.3 MB (104344680 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6880f3cd15d131cf178682b919d81b352948c440cb26217ac9dcf437708c656c`  
		Last Modified: Thu, 14 Dec 2023 20:29:11 GMT  
		Size: 9.0 KB (9026 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f503fa6b25cc641615180c3dde197fbc565852c411bcc3fc804068ea77c71ccd`  
		Last Modified: Thu, 14 Dec 2023 20:29:11 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ea13eb863a9f1fde16d062b2803008d1cb2fcbb413d6d306edca885a444c53e4`  
		Last Modified: Thu, 14 Dec 2023 20:29:11 GMT  
		Size: 171.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:abe780abf455f93ed6140fd51d5c35634ef9895a610a9c87c32a1b4808728bfd`  
		Last Modified: Thu, 14 Dec 2023 20:29:12 GMT  
		Size: 5.3 KB (5342 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b0aa3f9736a681d01abe0265b72445c9c4cd073f4d7fc0b254432eb86c7f8454`  
		Last Modified: Thu, 14 Dec 2023 20:29:12 GMT  
		Size: 186.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:a02da573c2e6e6a3505e1834a792f329f53e6e56ef62e24aec764b7182b75225
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4878278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:629cd68ad298367d1c9979b55898938ad6c26682a697ea0a3cd9a2691fe9da63`

```dockerfile
```

-	Layers:
	-	`sha256:e5d66806f2aa7e87f194729a963f98642712012107e8f0e21babbe234e6f573a`  
		Last Modified: Thu, 14 Dec 2023 20:29:11 GMT  
		Size: 4.8 MB (4824367 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c74a84aa427dc459dc13caf320f9c91a0f273fba107b626a9b4fc20eb4019582`  
		Last Modified: Thu, 14 Dec 2023 20:29:11 GMT  
		Size: 53.9 KB (53911 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:12-bookworm` - linux; 386

```console
$ docker pull postgres@sha256:aa5e7e8ca2b41369eb7acb39bce3c6d9f8a1b7933cb2a28632d3b69eb9f80f5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.3 MB (158254209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1202d0acefd796995ae5fb2b2b905138912cae34650899a46eabd7283c96f74`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 04:39:53 GMT
ADD file:930e1b9d85b6927c4d3046f7c75de2f3bfc6ec29100c314d0ab2b780ea30e962 in / 
# Tue, 21 Nov 2023 04:39:53 GMT
CMD ["bash"]
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV GOSU_VERSION=1.16
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	echo 'en_US.UTF-8 UTF-8' >> /etc/locale.gen; 	locale-gen; 	locale -a | grep 'en_US.utf8' # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV LANG=en_US.utf8
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_MAJOR=12
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_VERSION=12.17-1.pgdg120+1
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 11 Dec 2023 18:58:54 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 11 Dec 2023 18:58:54 GMT
COPY docker-entrypoint.sh docker-ensure-initdb.sh /usr/local/bin/ # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN ln -sT docker-ensure-initdb.sh /usr/local/bin/docker-enforce-initdb.sh # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Dec 2023 18:58:54 GMT
STOPSIGNAL SIGINT
# Mon, 11 Dec 2023 18:58:54 GMT
EXPOSE map[5432/tcp:{}]
# Mon, 11 Dec 2023 18:58:54 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:c0734eabce8885d8904dbd11b77aa97c2d2b04bc8e2af9e89d47c4bda590dd8e`  
		Last Modified: Tue, 21 Nov 2023 04:44:34 GMT  
		Size: 30.2 MB (30164109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9ee62d9644d28e22c39700bdd552c43317ccf9063c662751ba013dd18dfe4726`  
		Last Modified: Thu, 14 Dec 2023 19:03:35 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8abe3928ea6fcdf8e11d11005140aad9a64a134ed9a9e1928ec1aebebe152f9e`  
		Last Modified: Thu, 14 Dec 2023 19:03:35 GMT  
		Size: 4.8 MB (4844537 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8bb20e6c4f1024e00c2fe59e3f1e81c28530fa98a4e85bf866f0ea9df2b24b54`  
		Last Modified: Thu, 14 Dec 2023 19:03:35 GMT  
		Size: 1.4 MB (1424543 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dfae30d0fdf96fbbd7cbf2e130e59efad8a3f06c79a48f16bee7f9de86129d66`  
		Last Modified: Thu, 14 Dec 2023 19:03:36 GMT  
		Size: 8.1 MB (8067912 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:54c7ccae1802a3013bb2bdaddeeff5fbfda4d6278ba741c4c2a981792117edb3`  
		Last Modified: Thu, 14 Dec 2023 19:03:36 GMT  
		Size: 1.1 MB (1136181 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3809ed386277055df03581005d66f4e1316e1a53cf52558e95e2f466ad7dc065`  
		Last Modified: Thu, 14 Dec 2023 19:02:06 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a8d4f21b7bda83a1d7d4eac5528a9ce9fcab16f6908253e7e128db836f80c758`  
		Last Modified: Thu, 14 Dec 2023 19:03:37 GMT  
		Size: 3.1 KB (3143 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ace5adb88fa3dd913ffce19a36f82134fc55432ad35938099fa2d6c912ac2b84`  
		Last Modified: Thu, 14 Dec 2023 19:03:41 GMT  
		Size: 112.6 MB (112597641 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:30b30e97950acaffa1d143093bcbc713bcaa3cd97c5f0b1bcbda050ec6b0bfc9`  
		Last Modified: Thu, 14 Dec 2023 19:03:37 GMT  
		Size: 9.0 KB (9026 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:32247fd6df5712ce935fa56de950f84ac0baa026d0b96f4bac0c920ef88138b1`  
		Last Modified: Thu, 14 Dec 2023 19:03:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50bdd6ce4cd37b760375ae0bf647e0e8b05d1949e0c0a72840d4a2ea12640005`  
		Last Modified: Thu, 14 Dec 2023 19:03:38 GMT  
		Size: 171.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e5efb8c47fee9ba4cf69bc72c30f0e264415da4c8e676a96b53505be2a01574e`  
		Last Modified: Thu, 14 Dec 2023 19:03:39 GMT  
		Size: 5.3 KB (5346 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5d5e9be0926622137bcb04f0d5ebab6e0e577923993634572336ec965751e188`  
		Last Modified: Thu, 14 Dec 2023 19:03:39 GMT  
		Size: 189.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:f41005d66c1080f871184282692e71fa7654d54862991ff85b38ee0893298b08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 KB (53803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec1d127c4c6b3074d44db8312119536b9c0ffc75f86ccc03d4f04bd8298e299a`

```dockerfile
```

-	Layers:
	-	`sha256:0136304ca887cb7221cde89368252265cda43d0e417880fcb8046057b1797f27`  
		Last Modified: Thu, 14 Dec 2023 19:03:35 GMT  
		Size: 53.8 KB (53803 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:12-bookworm` - linux; mips64le

```console
$ docker pull postgres@sha256:fd23603faa0ed796aaa947a168e8c0a7cceef5f27b8f622d10a11e5c083434d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.8 MB (146757930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07819ba72b331584d39e9fed7bea97846a8b4096d14051f16490f18cca224b89`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV GOSU_VERSION=1.16
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	echo 'en_US.UTF-8 UTF-8' >> /etc/locale.gen; 	locale-gen; 	locale -a | grep 'en_US.utf8' # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV LANG=en_US.utf8
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_MAJOR=12
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_VERSION=12.17-1.pgdg120+1
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 11 Dec 2023 18:58:54 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 11 Dec 2023 18:58:54 GMT
COPY docker-entrypoint.sh docker-ensure-initdb.sh /usr/local/bin/ # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN ln -sT docker-ensure-initdb.sh /usr/local/bin/docker-enforce-initdb.sh # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Dec 2023 18:58:54 GMT
STOPSIGNAL SIGINT
# Mon, 11 Dec 2023 18:58:54 GMT
EXPOSE map[5432/tcp:{}]
# Mon, 11 Dec 2023 18:58:54 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d4751a8f9b59a5399e8b7e17a8be8bd1625be1d6a0119af4e4f4deb6f4c3e856`  
		Last Modified: Thu, 14 Dec 2023 20:03:34 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c439e1dc19d9efa184022d403ffe5199332a3f236c9e3c9f931beffd070b6c17`  
		Last Modified: Thu, 14 Dec 2023 20:03:35 GMT  
		Size: 4.4 MB (4355741 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9891d8c32f1da206d01d7b8bde5296280f1be1832a5c938e8ad2405a66aeec7e`  
		Last Modified: Thu, 14 Dec 2023 20:03:35 GMT  
		Size: 1.3 MB (1335986 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b6c4f29ac4e15a964e96f7ded128008abe69fdc2ac40aafb04240722a3ae91e0`  
		Last Modified: Thu, 14 Dec 2023 20:03:35 GMT  
		Size: 8.1 MB (8068091 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:710ac456ce453f1bf35a8525549a6259c6b252a4ae9147e99118e79053b92bc5`  
		Last Modified: Thu, 14 Dec 2023 20:03:36 GMT  
		Size: 1.2 MB (1181602 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a4671931e28db772abb5ccf8c6ff2e9f6c6556bba599062db0869c9e54dbd4ca`  
		Last Modified: Thu, 14 Dec 2023 20:03:36 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bfc7cffc84f4bce14c6144f372f6d93cd140aac3c7d9495ae2d2b6e033d8bf56`  
		Last Modified: Thu, 14 Dec 2023 20:03:37 GMT  
		Size: 3.1 KB (3141 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e9afb6255148042567b22661885708c6481f23f948cc3af439c406299918a155`  
		Last Modified: Fri, 15 Dec 2023 06:23:51 GMT  
		Size: 102.7 MB (102655231 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3a9b421986d55ed89201f624876828ebddc55fdaecf97b6e7b6b4e5326b3d994`  
		Last Modified: Fri, 15 Dec 2023 06:23:41 GMT  
		Size: 9.0 KB (9028 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d371c7c319e1ef765ab7d7a5f6b0f233bcbda80cda96a1fc811116d0f40f25b3`  
		Last Modified: Fri, 15 Dec 2023 06:23:41 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:44f0bbb6877218b378f0b9a44ae96133c793516dd8955c4ecd7edcd269901a2b`  
		Last Modified: Fri, 15 Dec 2023 06:23:41 GMT  
		Size: 171.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cfe1d0c361d73b9d6ce67ce5323f6827008ccdc0bbb9ad8d12dbfdc47d026de5`  
		Last Modified: Fri, 15 Dec 2023 06:23:42 GMT  
		Size: 5.3 KB (5348 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7cd8beeed6394139118eaaa1b5fee062393bd0468a4007ce4a9e73678b365e55`  
		Last Modified: Fri, 15 Dec 2023 06:23:42 GMT  
		Size: 190.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:8c759e6d1e19f2015fc57b020380c017e2cf2e3af739351064fa244da4f04c82
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 KB (53777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ece86d9a8fedf48b38c437468d9b40b3a9f5de526d1280f7acdadc5b8059fb65`

```dockerfile
```

-	Layers:
	-	`sha256:a8f585fd8f096abbfc9a0cd86f2cb3e2d8fa0e453acc1ba0e354958244aa5538`  
		Last Modified: Fri, 15 Dec 2023 06:23:40 GMT  
		Size: 53.8 KB (53777 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:12-bookworm` - linux; ppc64le

```console
$ docker pull postgres@sha256:e72d7dafe83266dc515a6cbf55e53f25f40ae382cb1526a05b1939985a2e5a0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.1 MB (160066202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeba6a285030e41983283a821b3296bf8a587403c618b4bcb29533978995884a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV GOSU_VERSION=1.16
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	echo 'en_US.UTF-8 UTF-8' >> /etc/locale.gen; 	locale-gen; 	locale -a | grep 'en_US.utf8' # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV LANG=en_US.utf8
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_MAJOR=12
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_VERSION=12.17-1.pgdg120+1
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 11 Dec 2023 18:58:54 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 11 Dec 2023 18:58:54 GMT
COPY docker-entrypoint.sh docker-ensure-initdb.sh /usr/local/bin/ # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN ln -sT docker-ensure-initdb.sh /usr/local/bin/docker-enforce-initdb.sh # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Dec 2023 18:58:54 GMT
STOPSIGNAL SIGINT
# Mon, 11 Dec 2023 18:58:54 GMT
EXPOSE map[5432/tcp:{}]
# Mon, 11 Dec 2023 18:58:54 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c2e1444eb5768a9f1452aad0278ed3b46e23bd0ddcdd4834e4c0c3f04f7a564`  
		Last Modified: Tue, 21 Nov 2023 23:54:59 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5aa03b72cb005f7e4b1680abe9b55b766463104336988c455382e20b7bd83ffe`  
		Last Modified: Tue, 21 Nov 2023 23:54:59 GMT  
		Size: 5.2 MB (5239246 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a4cb219c2b2f2937086d88d617001b3022093e4bdb6b1b0f88c97f0800c1b221`  
		Last Modified: Tue, 21 Nov 2023 23:54:59 GMT  
		Size: 1.4 MB (1370020 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:53e462d13c06b51d7c908aa6cbc93b2bcde82212de9ccd7ad886f35c9d16c328`  
		Last Modified: Sat, 09 Dec 2023 04:38:48 GMT  
		Size: 8.1 MB (8068028 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a417abce6335440f9a1599a71d0db83ce4ffbbe505d6ff49ade43aef04ebc9f5`  
		Last Modified: Sat, 09 Dec 2023 04:38:47 GMT  
		Size: 1.3 MB (1282773 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a832690b60f7957430cfe884b1c46be35fefa8f118a01692c8d54479bf785db`  
		Last Modified: Sat, 09 Dec 2023 04:38:47 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f0b051ef9bdd2b6276bf8538b01573ca9ee44b7c0574696cb1f83ab2945c330`  
		Last Modified: Sat, 09 Dec 2023 04:38:47 GMT  
		Size: 3.1 KB (3144 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8f459554adcfc69808bd48876ebcbc08dfa75ecce8da007c23c5a182d400343c`  
		Last Modified: Sat, 09 Dec 2023 05:26:33 GMT  
		Size: 110.9 MB (110945246 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:476461733b3bb41e83a38288e480729aba384414f66d853b0e5461d4cdd0de40`  
		Last Modified: Sat, 09 Dec 2023 05:26:29 GMT  
		Size: 9.0 KB (9031 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9f386c5456e2af833d7a4a51a7392b67fd0ab7ee9b4b154eddcbd45f14286f00`  
		Last Modified: Sat, 09 Dec 2023 05:26:29 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19635ea9d35876b21fd52fb4c46a642cd06da6011e224da55fab3a0495ee6c4d`  
		Last Modified: Sat, 09 Dec 2023 05:26:29 GMT  
		Size: 171.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d625cb49ff86089cfdf6624fb1a86139532fb2de506b27b97fffaf0a468f8e5b`  
		Last Modified: Thu, 14 Dec 2023 19:26:48 GMT  
		Size: 5.3 KB (5340 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eed21c9a570bdb43b9ac8f6282fc7cf6b2a467e068319350d61b11c43c453d07`  
		Last Modified: Thu, 14 Dec 2023 19:26:48 GMT  
		Size: 186.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:83f3fe0ea11da40ac1ea7a3fec5516a8d160dc6ddabc53a9a99e3a2f555f71b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4879834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:120595759ba39518ed70595f25243721dc0214b1fd5ad222a8b62eda7d297ee8`

```dockerfile
```

-	Layers:
	-	`sha256:030037d04add075256c0becc05c678c03e6c91360dc5d30619cf823d12589a09`  
		Last Modified: Thu, 14 Dec 2023 19:26:48 GMT  
		Size: 4.8 MB (4825872 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:668463a04128bb36674a9e8b20d8026a09dc875cc589946b5ade6a5c28543e89`  
		Last Modified: Thu, 14 Dec 2023 19:26:48 GMT  
		Size: 54.0 KB (53962 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:12-bookworm` - linux; s390x

```console
$ docker pull postgres@sha256:967ffc69e0ba82199b6fa3a510f6f77461dabdb87bbe95b23f856386917a78e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.6 MB (153559416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:106c7330f29f02e8fa09e7695e21613563fb2919c02cf8622f3fd72c60cb1e4f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 11 Dec 2023 18:58:54 GMT
ADD file:f06f12fa5a93afc3a79ac4371d24b0a471a5a1818cf34c1d90004c8f410914b9 in / 
# Mon, 11 Dec 2023 18:58:54 GMT
CMD ["bash"]
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV GOSU_VERSION=1.16
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	echo 'en_US.UTF-8 UTF-8' >> /etc/locale.gen; 	locale-gen; 	locale -a | grep 'en_US.utf8' # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV LANG=en_US.utf8
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_MAJOR=12
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_VERSION=12.17-1.pgdg120+1
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 11 Dec 2023 18:58:54 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 11 Dec 2023 18:58:54 GMT
COPY docker-entrypoint.sh docker-ensure-initdb.sh /usr/local/bin/ # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
RUN ln -sT docker-ensure-initdb.sh /usr/local/bin/docker-enforce-initdb.sh # buildkit
# Mon, 11 Dec 2023 18:58:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Dec 2023 18:58:54 GMT
STOPSIGNAL SIGINT
# Mon, 11 Dec 2023 18:58:54 GMT
EXPOSE map[5432/tcp:{}]
# Mon, 11 Dec 2023 18:58:54 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:bc6b1888979d3ceb063da848b2034e980e2c2613642159c1e856550b79aa620c`  
		Last Modified: Tue, 19 Dec 2023 01:47:38 GMT  
		Size: 27.5 MB (27491874 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6967509bd16206b93c3024f4b68e0387925ab9e31847a1cbfcc4c1ff13958cce`  
		Last Modified: Tue, 19 Dec 2023 15:40:14 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7b029f3a94337efef121f2a62bcb3207d562255d93b008f938975d3e7341c028`  
		Last Modified: Tue, 19 Dec 2023 15:40:14 GMT  
		Size: 4.3 MB (4278319 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e0130828c9e9eb5f4fdc3f80ae613ce551343a40f3b3237bdfe57541e7adc158`  
		Last Modified: Tue, 19 Dec 2023 15:40:14 GMT  
		Size: 1.4 MB (1411097 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4772c8242ecee0922c4c63cbb8858ca706eef5887ba301ff848d1179d8ec52a0`  
		Last Modified: Tue, 19 Dec 2023 15:40:14 GMT  
		Size: 8.1 MB (8119621 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ec250ac8f0ae714c6024fa4447a831539d2ad20613d4987efe2d55c8064d0d37`  
		Last Modified: Tue, 19 Dec 2023 15:40:15 GMT  
		Size: 1.1 MB (1095673 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:25eb5ab009ec175249d042171d140b44d0e9692d98c60fcbf82f5e8690abb003`  
		Last Modified: Tue, 19 Dec 2023 15:40:15 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cd33cdca52e6775ff1c5ae66240871a35ccf4e9101f7d0c3b2d1b5b86ad52d6c`  
		Last Modified: Tue, 19 Dec 2023 15:40:15 GMT  
		Size: 3.1 KB (3144 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:97a04b33a4bd58ffda0317c50bacf801877dc47eeb5e0b97410bb1b532f23216`  
		Last Modified: Tue, 19 Dec 2023 15:50:05 GMT  
		Size: 111.1 MB (111143556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:966c281ffd6ccf199631a605772a37b9f2536e40934081a7d95b63f1c118d108`  
		Last Modified: Tue, 19 Dec 2023 15:50:03 GMT  
		Size: 9.0 KB (9025 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c2977f6a58e0cd1b4353470ef687a294c411c7f2c1f71e8a6a81a268e0454ff`  
		Last Modified: Tue, 19 Dec 2023 15:50:03 GMT  
		Size: 127.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9bfa26e7af83b15326422c7584c940def5b74b0631468be2b133832421d5ded1`  
		Last Modified: Tue, 19 Dec 2023 15:50:03 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d52af4101b36d83afaee924613cb59ca79b4e0c56019b29a2eede6f8892d95a8`  
		Last Modified: Tue, 19 Dec 2023 15:50:04 GMT  
		Size: 5.3 KB (5342 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5770fdf7d15b9b32814d03ed4a4583a405732bdf87e20ca7f8a112c66d36dc64`  
		Last Modified: Tue, 19 Dec 2023 15:50:04 GMT  
		Size: 186.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:12-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:4c4dae0f9d21603b31624ba4861435035ccc59d6c09a55c6c892a55c98049202
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4871839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2bd7428f2dec15494431099fd661b0b2ebd6b481f9e3670016038a16ac54df7`

```dockerfile
```

-	Layers:
	-	`sha256:5c1034b4475686a61f2dcdce9e8c430345f9ad21aceaa665582988b7bc18d099`  
		Last Modified: Tue, 19 Dec 2023 15:50:05 GMT  
		Size: 4.8 MB (4817937 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:404a86d424b98bd5a3bd31eac8afe5e743febfb6309608440f56f8fe90708ee2`  
		Last Modified: Tue, 19 Dec 2023 15:50:04 GMT  
		Size: 53.9 KB (53902 bytes)  
		MIME: application/vnd.in-toto+json
