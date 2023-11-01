## `postgres:11-bullseye`

```console
$ docker pull postgres@sha256:9bfba8fe10100654eaa4c0ef7e9211ff74e42b1cf001fb4a2cd34cfaadc72a3b
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

### `postgres:11-bullseye` - linux; amd64

```console
$ docker pull postgres@sha256:02f54b4914cfff280b78f4dfd44ee3d7780bab7f8a7330dc161ed35960dd4937
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.0 MB (135006965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966b2c40225f6bb4fe7fa756c49fe59411989a612372c7c4960d42b3bec96401`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 10 Aug 2023 18:02:22 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Thu, 10 Aug 2023 18:02:22 GMT
CMD ["bash"]
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV GOSU_VERSION=1.16
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8 # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV LANG=en_US.utf8
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PG_MAJOR=11
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PG_VERSION=11.21-1.pgdg110+1
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 10 Aug 2023 18:02:22 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA" # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 10 Aug 2023 18:02:22 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Aug 2023 18:02:22 GMT
STOPSIGNAL SIGINT
# Thu, 10 Aug 2023 18:02:22 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 10 Aug 2023 18:02:22 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f8a7879327c18cd3947968cc733e368934189c884cf448ed7f252b6bdfc9cdc5`  
		Last Modified: Wed, 01 Nov 2023 01:03:28 GMT  
		Size: 1.7 KB (1682 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8aa893d93b829ca3d266e44c22774bec2d75b5d66fa07fb8525f49b36e038692`  
		Last Modified: Wed, 01 Nov 2023 01:03:29 GMT  
		Size: 4.2 MB (4207470 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7ef5a925d7f51db0ad5bcb9715de218ffa199ced5019da00325147158e131b6b`  
		Last Modified: Wed, 01 Nov 2023 01:03:28 GMT  
		Size: 1.5 MB (1472436 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:641caf1b0ebd8c649ffd29e436f4962075e47fce1ea534dc2eb7d414dc64bc30`  
		Last Modified: Wed, 01 Nov 2023 01:03:29 GMT  
		Size: 8.0 MB (8045195 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9cdeea50967feb3941b8e42c85bd9e5e4346e0859876006e17d2fff38afe2138`  
		Last Modified: Wed, 01 Nov 2023 01:03:30 GMT  
		Size: 1.0 MB (1037447 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e3a5e528f780129af6b6cce51901362105d6dd546e6d5c300270570cf141cf86`  
		Last Modified: Wed, 01 Nov 2023 01:03:29 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ea4de275d17c25c78a3b9524792e3cab0cfbcd291a3313341a40ee81ffd8fa7f`  
		Last Modified: Wed, 01 Nov 2023 01:03:30 GMT  
		Size: 3.1 KB (3143 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc7536ca3d531f02fb1bd2d99ce3ef7b4ed7c52217a3f1db30f69111aaf09c1b`  
		Last Modified: Wed, 01 Nov 2023 01:03:35 GMT  
		Size: 88.8 MB (88808149 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:63a3cc372a5779a6bd68556535a3b4daaebed5fe57936d9e3d339969c6e67da5`  
		Last Modified: Wed, 01 Nov 2023 01:03:31 GMT  
		Size: 8.3 KB (8330 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:97cac53df0404e8770772b84a3ec73c25367be5835c99abbfd80fe546c8a3ce4`  
		Last Modified: Wed, 01 Nov 2023 01:03:31 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b0d3e5d8ad0859aa0bb436881d18b810209fc4fd73ab7cc4bc131c48681dc472`  
		Last Modified: Wed, 01 Nov 2023 01:03:31 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:467d8717d5dd9ad9b6765d5babeb4015785606bd306581b3f739c3e6a600706e`  
		Last Modified: Wed, 01 Nov 2023 01:03:32 GMT  
		Size: 4.8 KB (4784 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:11-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:7c06f52ebcca72f66691ebdb0279d5579a21ea0833f0a6bbdb4c17e6bff7b393
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4989569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd78176b12be6da6a6eb76bb5741f2c644b8176f13b001518cc3d4259595b995`

```dockerfile
```

-	Layers:
	-	`sha256:14fb37d46169fc140fd8e3574ccd8b3caeb9fa1c6a6da681540c18b46b8cf05d`  
		Last Modified: Wed, 01 Nov 2023 01:03:29 GMT  
		Size: 4.9 MB (4939539 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c52809fe360c9ada8a8a5235fba46f9fefd9714610a5a3878dcaa6a7ccd9fa94`  
		Last Modified: Wed, 01 Nov 2023 01:03:28 GMT  
		Size: 50.0 KB (50030 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:11-bullseye` - linux; arm variant v5

```console
$ docker pull postgres@sha256:281d6b9ced9d5a957646724ff764acad6bbb6a470b7724c5f35007b6e440fd00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128147889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39c93ad9305d113756141cd132b3298ba5589f6ae769aa58aafba6be9001cbd6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 10 Aug 2023 18:02:22 GMT
ADD file:ccc4159f30855826069fec59b14fe886384e5373119e7f382b6faf66f22fb6c6 in / 
# Thu, 10 Aug 2023 18:02:22 GMT
CMD ["bash"]
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV GOSU_VERSION=1.16
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8 # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV LANG=en_US.utf8
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PG_MAJOR=11
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PG_VERSION=11.21-1.pgdg110+1
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 10 Aug 2023 18:02:22 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA" # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 10 Aug 2023 18:02:22 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Aug 2023 18:02:22 GMT
STOPSIGNAL SIGINT
# Thu, 10 Aug 2023 18:02:22 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 10 Aug 2023 18:02:22 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:42b20947607fb3d0005c8f3e1da41d53f7e4b3187e4a4bed890c7e9207a1ae03`  
		Last Modified: Wed, 01 Nov 2023 00:52:14 GMT  
		Size: 28.9 MB (28921182 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aca79d7b5a878d424f8e4b98a3653b61982a3ff799e22346d449a0fa142a22ff`  
		Last Modified: Wed, 01 Nov 2023 15:43:07 GMT  
		Size: 1.7 KB (1673 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bbbaf4735053d700117bc69fad778fe7b19ef63c50a2e83aec7450ad921bd119`  
		Last Modified: Wed, 01 Nov 2023 15:43:08 GMT  
		Size: 3.9 MB (3889332 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c04cba7638d886f5fd351e10f9c10445b5eaa957cf4ff108d649b4d2a477f8e6`  
		Last Modified: Wed, 01 Nov 2023 15:43:07 GMT  
		Size: 1.4 MB (1449969 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:80555810c8e1719c745976929ca0bf24a03ce94b83519bfe6e3d028034ec23c0`  
		Last Modified: Wed, 01 Nov 2023 15:43:09 GMT  
		Size: 8.0 MB (8045207 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5d698bab96a97122f53a734a664a94978d14f7eaab72962e709598fc6da18b7d`  
		Last Modified: Wed, 01 Nov 2023 15:43:09 GMT  
		Size: 1.0 MB (1033905 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3607618f7a584ff7868a5c1b78bda8b8403707e25074bac81a4a7458c4455816`  
		Last Modified: Wed, 01 Nov 2023 15:43:09 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e624724f61cd2066b09ea30cc988d2b13f93a128481a4b5a858f6b89d3253485`  
		Last Modified: Wed, 01 Nov 2023 15:43:10 GMT  
		Size: 3.1 KB (3141 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c3e06615619de63a201689aa7a5e460bfec80fb309ea7cb119af35587ccb3bf1`  
		Last Modified: Wed, 01 Nov 2023 18:08:11 GMT  
		Size: 84.8 MB (84789958 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:181bb0525725facf5bffc58e57bf9b47e571908fca143db1d980ef94e5f81a4d`  
		Last Modified: Wed, 01 Nov 2023 18:08:06 GMT  
		Size: 8.3 KB (8322 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4603281f5179326c6e3e6d7985ce48119a97645a4f311be54cf39c9a1911e15b`  
		Last Modified: Wed, 01 Nov 2023 18:08:06 GMT  
		Size: 127.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:508c0530d47cf60734f46de04859f8c50b3d8c0de84c3eb52d51dada316d3eb7`  
		Last Modified: Wed, 01 Nov 2023 18:08:06 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9561982a2f67386c3b21bb92dcce216d2b93e5c279198eaaa93afc5e1c99f423`  
		Last Modified: Wed, 01 Nov 2023 18:08:07 GMT  
		Size: 4.8 KB (4788 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:11-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:0256dbe16004da84f321b60f922bb2b971bd8b7eaf3d1ed5f3930c57dfd469a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.8 KB (49832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e36fe7283b05f91210aeca094f90c91833fd247e463e0a261b73f58216f5fadd`

```dockerfile
```

-	Layers:
	-	`sha256:05fbd542ad0e33fb2de50445c57bc2fff25a44c3f54090f6e0477b029edebf56`  
		Last Modified: Wed, 01 Nov 2023 18:08:05 GMT  
		Size: 49.8 KB (49832 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:11-bullseye` - linux; arm variant v7

```console
$ docker pull postgres@sha256:9c28f0190722d7d922c613db7aa809f70d0b99f47eb4d7620a23952a066b3c66
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123001639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:231626e66ec7502321201eb256c56d332833ec2c309a5254455e170e9724ab7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 10 Aug 2023 18:02:22 GMT
ADD file:0d1753bfedd7193184780166819d0407867a22d82804c0045274f1f13afecac0 in / 
# Thu, 10 Aug 2023 18:02:22 GMT
CMD ["bash"]
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV GOSU_VERSION=1.16
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8 # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV LANG=en_US.utf8
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PG_MAJOR=11
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PG_VERSION=11.21-1.pgdg110+1
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 10 Aug 2023 18:02:22 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA" # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 10 Aug 2023 18:02:22 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Aug 2023 18:02:22 GMT
STOPSIGNAL SIGINT
# Thu, 10 Aug 2023 18:02:22 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 10 Aug 2023 18:02:22 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:bb9c59b28e9fb9c31ffdb002ca9a6656677eee093c8093fcbea8818e927df70a`  
		Last Modified: Wed, 11 Oct 2023 17:47:06 GMT  
		Size: 26.6 MB (26579008 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9068411873aad6400bd295ce3c9c7615bb6257f3b060c0f1fc34bcb50f8bf21d`  
		Last Modified: Thu, 12 Oct 2023 19:10:06 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f4750f4a9686081f92d8054512c1471329d5326ef79ed1c5efe80edca386cd44`  
		Last Modified: Thu, 12 Oct 2023 19:10:07 GMT  
		Size: 3.5 MB (3509896 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:44fe86832a3034209b008abcdb414302ec2070eda610180c13f76f530190fdec`  
		Last Modified: Thu, 12 Oct 2023 19:10:07 GMT  
		Size: 1.4 MB (1440047 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:13825c0974702ea42928129106f722061873a4abc5a7fcf312f3a89ad56fce38`  
		Last Modified: Thu, 12 Oct 2023 19:10:09 GMT  
		Size: 8.0 MB (8045175 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15702f5c7849e612b622235b1a9a828d2774452e6970b395b7a04f51998945dd`  
		Last Modified: Thu, 12 Oct 2023 19:10:08 GMT  
		Size: 907.8 KB (907773 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a1d313a66e66cb3c84dd849228ca8ce662d61f4d66e252f1beb4119fe71b9211`  
		Last Modified: Thu, 12 Oct 2023 19:10:08 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:02e37a96c90f46ce7575d15e600aa2987758b2c5db2b8a9e4fd30b9c070c5673`  
		Last Modified: Thu, 12 Oct 2023 19:10:10 GMT  
		Size: 3.1 KB (3143 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9cd913fb2e7833119298c65d3e5324dc708f8f2d29d30ebbe6baeee11e412d99`  
		Last Modified: Thu, 12 Oct 2023 21:37:41 GMT  
		Size: 82.5 MB (82501387 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:358843dd2d9a120dce88d9eb26e90e81669abfddcc51305f60b534ab3d2543c4`  
		Last Modified: Thu, 12 Oct 2023 21:37:36 GMT  
		Size: 8.3 KB (8330 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c89c55ed218ef92e999070f2328ec281f78a8369a52f2c7a87c6262a4910a14a`  
		Last Modified: Thu, 12 Oct 2023 21:37:35 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4556ec1c7ecdaa3b4752697112af51297ae2aa8b856f8ca932ff839c5c2cd4e1`  
		Last Modified: Thu, 12 Oct 2023 21:37:35 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3e60b783d4d4e235504f93a73e523cd752c4cf52c763f5e62f18f5c584ed8ab7`  
		Last Modified: Thu, 12 Oct 2023 21:37:37 GMT  
		Size: 4.8 KB (4789 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:11-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:20e5ae96d22c8ee0067b4f9c3f44f30be15caf59df7e7572a61266dc068e228a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4999366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfcda20ce8a7642ce929cd4c5447271e4c55b7bbfd175cfaf9300126abe09e48`

```dockerfile
```

-	Layers:
	-	`sha256:169626af28b1fe07f35a6d161f2dcb20925240e0ff28889d2a8fc67c4a768a75`  
		Last Modified: Thu, 12 Oct 2023 21:37:36 GMT  
		Size: 4.9 MB (4949327 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a0537ab55119e4586d961b0c731fef1f3328ed40caf4b5341e13e64039e724ef`  
		Last Modified: Thu, 12 Oct 2023 21:37:35 GMT  
		Size: 50.0 KB (50039 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:11-bullseye` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:52326b2f5b42c014cb705dea1baca04be8a1ac5fb9b099d6bf1ad49134eaa94e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.1 MB (130102962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0c254aa8bfca9db0f963e55dc05fb2ba1cd13bd32e3754af2dd092a0972de7f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 10 Aug 2023 18:02:22 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Thu, 10 Aug 2023 18:02:22 GMT
CMD ["bash"]
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV GOSU_VERSION=1.16
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8 # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV LANG=en_US.utf8
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PG_MAJOR=11
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PG_VERSION=11.21-1.pgdg110+1
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 10 Aug 2023 18:02:22 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA" # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 10 Aug 2023 18:02:22 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Aug 2023 18:02:22 GMT
STOPSIGNAL SIGINT
# Thu, 10 Aug 2023 18:02:22 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 10 Aug 2023 18:02:22 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ce3ff771def927f093d5cc616091c5539f37a8b0de84b60aaa56c91249fcf525`  
		Last Modified: Thu, 12 Oct 2023 16:58:45 GMT  
		Size: 1.7 KB (1688 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7317a2026c07cdafdc60688a261cdcfc8df77cb91c3e3c20842df1cbeee7ba5b`  
		Last Modified: Thu, 12 Oct 2023 16:58:46 GMT  
		Size: 4.2 MB (4209380 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fe90c16a41a91765b7306289bce9c685bd727bd0f070a33c93b9c89cb91fbc62`  
		Last Modified: Thu, 12 Oct 2023 16:58:45 GMT  
		Size: 1.4 MB (1404387 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dd2891aa9a8d9ed3643130aabdab4999c4b8d141e76951f1c3bfeec15982db5d`  
		Last Modified: Thu, 12 Oct 2023 16:58:47 GMT  
		Size: 8.0 MB (8045182 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:03cdd3e15684a5ee8e3d3603b87a72c606be98a36e41e3032dc3bb09b343a831`  
		Last Modified: Thu, 12 Oct 2023 16:58:47 GMT  
		Size: 1.0 MB (1025926 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:621ae45f35e5a9a2017b0cbdffe8a2f82a266900c8e0008be54d9c19d9ee369b`  
		Last Modified: Thu, 12 Oct 2023 16:58:47 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cdf98eff2f6bbd9d2c42178020852f6be97591005572dd2eb2f4917b91e0e388`  
		Last Modified: Thu, 12 Oct 2023 16:58:48 GMT  
		Size: 3.1 KB (3143 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:053aee1a9e6b1f9ce847df2c173156624e4ac52939c68c43461b1834d4e087c2`  
		Last Modified: Thu, 12 Oct 2023 16:58:53 GMT  
		Size: 85.3 MB (85335644 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bca8d65219962a72ae711877ddd931e44b269ff88f9e31dea3b55caa7dd3ccd3`  
		Last Modified: Thu, 12 Oct 2023 16:58:48 GMT  
		Size: 8.3 KB (8325 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:33913210da60b39ffd2713d98a60fe0babe4c44b5e71bc707eb4207f1c86cb0a`  
		Last Modified: Thu, 12 Oct 2023 16:58:48 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:685e9db5842bcbeebc1d828eb32134a3cc34b5c17f0bffe725aebcf9d599bcab`  
		Last Modified: Thu, 12 Oct 2023 16:58:49 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:70aa3a68cc3badabfecf46445dc69f38f5e1a3bef344335e006d5c5597829e15`  
		Last Modified: Thu, 12 Oct 2023 16:58:49 GMT  
		Size: 4.8 KB (4788 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:11-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:2d7c1f643b16a0a9c9bc6bb506e4c6722de94c7b9c2579e95da313cd595ec81d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4988429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1925d917ae7b1af0c3bbe0b8da5b225f3fcd4ab53ede7b74e6a30bd8b7b35746`

```dockerfile
```

-	Layers:
	-	`sha256:1646e5cc1ca531c6c0e264f976923dd2086b11fae21975da653c7543e29bfeb6`  
		Last Modified: Thu, 12 Oct 2023 16:58:45 GMT  
		Size: 4.9 MB (4938393 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:580c35f350249d852796b31879baa731d5f357806cf1bdb104bcfaafb85243a4`  
		Last Modified: Thu, 12 Oct 2023 16:58:45 GMT  
		Size: 50.0 KB (50036 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:11-bullseye` - linux; 386

```console
$ docker pull postgres@sha256:52242a28e513810d0e4a3d1bffdd4c9482b3e278777becd4cbcb04206ce41ead
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.9 MB (136889137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4a348b3f7d6273b246408f75a4ffe1999e3c472d172715234510932a7851581`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 10 Aug 2023 18:02:22 GMT
ADD file:67f223c9c48e525a23fb110e4c105d7128dcac0c10f32c38f98ea84a21d2bd00 in / 
# Thu, 10 Aug 2023 18:02:22 GMT
CMD ["bash"]
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV GOSU_VERSION=1.16
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8 # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV LANG=en_US.utf8
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PG_MAJOR=11
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PG_VERSION=11.21-1.pgdg110+1
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 10 Aug 2023 18:02:22 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA" # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 10 Aug 2023 18:02:22 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Aug 2023 18:02:22 GMT
STOPSIGNAL SIGINT
# Thu, 10 Aug 2023 18:02:22 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 10 Aug 2023 18:02:22 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:bc6810e8fe9346a3caaff984163b789d12b6964a15a2029e384143ca19fef5ad`  
		Last Modified: Wed, 01 Nov 2023 00:44:14 GMT  
		Size: 32.4 MB (32402692 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:de62efeb2d2c08236797932bbdac574a323b4fb7b9c5f873c16162a2ddb33f82`  
		Last Modified: Wed, 01 Nov 2023 01:19:30 GMT  
		Size: 1.7 KB (1674 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:302615dd6a87911f035908c5715c9f7c60f34b5e65aeabc01d9b1137b3d4293c`  
		Last Modified: Wed, 01 Nov 2023 01:19:30 GMT  
		Size: 4.6 MB (4607440 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d5ac126b9ac03dbd29ca86d0e6a4151fb7f1aa921334c6963a13dc5e262d2588`  
		Last Modified: Wed, 01 Nov 2023 01:19:30 GMT  
		Size: 1.4 MB (1448292 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:41ec8bbe9c52ed17c8cc6a00e6ad0d03f3c17ce86f08938b526db6cc6cb5aec6`  
		Last Modified: Wed, 01 Nov 2023 01:19:31 GMT  
		Size: 8.0 MB (8045178 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b3222de05b2bf2610d6394d9c15ba10d48c06f801f570bbcb4e4d099cef2138`  
		Last Modified: Wed, 01 Nov 2023 01:19:31 GMT  
		Size: 1.0 MB (1027977 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e3a5e528f780129af6b6cce51901362105d6dd546e6d5c300270570cf141cf86`  
		Last Modified: Wed, 01 Nov 2023 01:03:29 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ea4de275d17c25c78a3b9524792e3cab0cfbcd291a3313341a40ee81ffd8fa7f`  
		Last Modified: Wed, 01 Nov 2023 01:03:30 GMT  
		Size: 3.1 KB (3143 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d274ce0d2ded81e4c0d360c0f105c2b535d15e44bc5241eb01a02f79e6b8239f`  
		Last Modified: Wed, 01 Nov 2023 01:19:35 GMT  
		Size: 89.3 MB (89339211 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:42fe33feb8a61ac2fa9a89d276824cfd81fbdfded08c37da6cda4071ab21dc8b`  
		Last Modified: Wed, 01 Nov 2023 01:19:32 GMT  
		Size: 8.3 KB (8325 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:763238a31591cba2e6d192f23d35dbcd6e3d2d7f6a9599aa5414a50b2b6fdd61`  
		Last Modified: Wed, 01 Nov 2023 01:19:32 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ec661614d00bba3b1d59ffda56ab9f8ee601410c229fcf61177f4f16bd8d0b2`  
		Last Modified: Wed, 01 Nov 2023 01:19:32 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:be68a41dc00a010a239fab41bcee83f878355c86f9342fb57475242a5bcf34b1`  
		Last Modified: Wed, 01 Nov 2023 01:19:33 GMT  
		Size: 4.8 KB (4791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:11-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:00628b59067022e8115af0ff3576d4cf890fa04afb525bf78dbefdbe248dffad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.8 KB (49774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e061ee21bd29278ca4037d3ec142c1032561e888a0a743bb31530a6f7d81fdb`

```dockerfile
```

-	Layers:
	-	`sha256:3d8c832051aba75b546356933b70f62b6c995ef9693def6b0bbc5e59f1c44c92`  
		Last Modified: Wed, 01 Nov 2023 01:19:30 GMT  
		Size: 49.8 KB (49774 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:11-bullseye` - linux; mips64le

```console
$ docker pull postgres@sha256:903a1b782f0fc11b596a1297f95b86f3159c03f142c81f5c9754c91295c51230
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.8 MB (129763608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5a95615f57d37dab2a7d19eafa659df04795f3f63032db91f6e1d36b3f79919`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 10 Aug 2023 18:02:22 GMT
ADD file:86abe5722ef15fa073bf5b38a44ec0524e99a0cf1a6dbf0c6510fb1926c7abf8 in / 
# Thu, 10 Aug 2023 18:02:22 GMT
CMD ["bash"]
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV GOSU_VERSION=1.16
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8 # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV LANG=en_US.utf8
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PG_MAJOR=11
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PG_VERSION=11.21-1.pgdg110+1
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 10 Aug 2023 18:02:22 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA" # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 10 Aug 2023 18:02:22 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Aug 2023 18:02:22 GMT
STOPSIGNAL SIGINT
# Thu, 10 Aug 2023 18:02:22 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 10 Aug 2023 18:02:22 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:7ed8396e400b964776cd6b7c617ad90d450d2ece3dbd9e26e9c264e98e7145ea`  
		Last Modified: Wed, 11 Oct 2023 18:02:07 GMT  
		Size: 29.6 MB (29636021 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b008e488c7d4ee897ad11bd699878f86490e0474f62c64ac40471668858e050b`  
		Last Modified: Fri, 13 Oct 2023 11:54:19 GMT  
		Size: 1.7 KB (1689 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:94f03a676413bb8d48d9d914e8d87292411e808f14348b534310007cb2b5fad9`  
		Last Modified: Fri, 13 Oct 2023 11:54:20 GMT  
		Size: 4.2 MB (4196256 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0f41f2a2594d3c210d1d53011b1edc77aaac0404df9a1799a76d4d65178a099d`  
		Last Modified: Fri, 13 Oct 2023 11:54:20 GMT  
		Size: 1.4 MB (1359938 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:585a591333b0a0f53fc80eb815fdd55339e9075bb02c03c630bcd56da6283f3a`  
		Last Modified: Fri, 13 Oct 2023 11:54:22 GMT  
		Size: 8.0 MB (8045432 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:47563d4a845a70efccd2fa326ec2f84ae675602956b4fa6841c7cd1808eac7e4`  
		Last Modified: Fri, 13 Oct 2023 11:54:21 GMT  
		Size: 1.1 MB (1089514 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7d93f4c0c4d8842fc172b1b64e352a70e544455d64575be0f4c240c4b2dfe361`  
		Last Modified: Fri, 13 Oct 2023 11:54:21 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0795e78108b2b9b204f919bbd8c91454c083917772fc2b8e4286e06299246c12`  
		Last Modified: Fri, 13 Oct 2023 11:54:23 GMT  
		Size: 3.1 KB (3144 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9dbd8e746ac6698614543bf59d11fcf5d688751f28d4bcc6252b657ec8d27bb8`  
		Last Modified: Sat, 14 Oct 2023 05:39:32 GMT  
		Size: 85.4 MB (85418079 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ff236a297fa789dfcf50e8afdf145e9766a59e45bd0d8a1a8c9648cba694477f`  
		Last Modified: Sat, 14 Oct 2023 05:39:23 GMT  
		Size: 8.3 KB (8332 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7f67b02358f809000869eea52ae07f4c03946514c84ac20670e6ab30dc2f0ea0`  
		Last Modified: Sat, 14 Oct 2023 05:39:23 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:49b324acbdf0828789b379417e6b99f0c34211acdb969641ce4c5d07c841b181`  
		Last Modified: Sat, 14 Oct 2023 05:39:23 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:407361d038517f36494b09cb00686bd01f52d70f9d9005777138ae24aa6f18b5`  
		Last Modified: Sat, 14 Oct 2023 05:39:24 GMT  
		Size: 4.8 KB (4790 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:11-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:8c7bcafd3f2ebfe5b7553d84c83fec0b29a900dd85751aa008422f43cb013ac0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.7 KB (49717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75ba725304473e689ced018823e34cbe181f711e97faf72f86b1c1f61a20fe22`

```dockerfile
```

-	Layers:
	-	`sha256:36149a8a7d0c2e2576cf583060d3f803cd4267e36c9512cf1a756353ab15f404`  
		Last Modified: Sat, 14 Oct 2023 05:39:23 GMT  
		Size: 49.7 KB (49717 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:11-bullseye` - linux; ppc64le

```console
$ docker pull postgres@sha256:9da404f39a4f9634721cc0b3f51d2668eba554be802746674356a9f74a926ec6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.9 MB (143907862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e435b3a8d9df381d961a8152170246497cc867df9b6fe81441c00564f20ab9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 10 Aug 2023 18:02:22 GMT
ADD file:96450fb62af4cd68105cbbf612cb5d2f79139cc9416835b6c2fdf40727635939 in / 
# Thu, 10 Aug 2023 18:02:22 GMT
CMD ["bash"]
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV GOSU_VERSION=1.16
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8 # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV LANG=en_US.utf8
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PG_MAJOR=11
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PG_VERSION=11.21-1.pgdg110+1
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 10 Aug 2023 18:02:22 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA" # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 10 Aug 2023 18:02:22 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Aug 2023 18:02:22 GMT
STOPSIGNAL SIGINT
# Thu, 10 Aug 2023 18:02:22 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 10 Aug 2023 18:02:22 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:cde4df93466f96fbb1bbc513d09d354ea1e58d3e619c19fcf9120dbba87405ea`  
		Last Modified: Wed, 11 Oct 2023 17:50:55 GMT  
		Size: 35.3 MB (35293715 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b9accccc56d67302b8282298cf43134bf1b6b22e19aa37eac676d9a26722bfc`  
		Last Modified: Fri, 13 Oct 2023 01:17:28 GMT  
		Size: 1.7 KB (1685 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1089fd3e26d899e532efbef9567a350913ebb264c3ba51e0373d090b5afdc19`  
		Last Modified: Fri, 13 Oct 2023 01:17:29 GMT  
		Size: 5.0 MB (5016026 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f057edb42f8a0e92b99ef76189c94833e644d8fa34a000bc93747f36bf04972d`  
		Last Modified: Fri, 13 Oct 2023 01:17:29 GMT  
		Size: 1.4 MB (1394092 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f5da68b7d5d20015c8ca7a56e22763f89fb058d4103aa6fcec648b387de37d44`  
		Last Modified: Fri, 13 Oct 2023 01:17:30 GMT  
		Size: 8.0 MB (8045327 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b6f4b040ea332c453b7edbdd6aaec76217214034d2c9246c7405facacbd9e5f`  
		Last Modified: Fri, 13 Oct 2023 01:17:31 GMT  
		Size: 1.2 MB (1196970 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9c9904b269eb0444c7988db66c03e1de71b34aabfcabff07fc5d1b41ee5ba931`  
		Last Modified: Fri, 13 Oct 2023 01:17:30 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:25e9270c34e21ccc313eaa1cca93c472787b31139910b55ca4a415772ef8e43f`  
		Last Modified: Fri, 13 Oct 2023 01:17:31 GMT  
		Size: 3.1 KB (3144 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee5da275335ea8b46cf0ff1c8b4f0e4ca46dff3c5cf87273a7b57c83cbe19255`  
		Last Modified: Fri, 13 Oct 2023 04:57:23 GMT  
		Size: 92.9 MB (92943375 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5d427622802753b07d8ba256ed7e06bee7765b4dfd6d9a5fa0476601f4f3def8`  
		Last Modified: Fri, 13 Oct 2023 04:57:17 GMT  
		Size: 8.3 KB (8329 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:13473910f45d8833e64c8d405ee585cd96c00d30bff98b91e40f9cf42207cd5f`  
		Last Modified: Fri, 13 Oct 2023 04:57:17 GMT  
		Size: 127.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2807a01f43fffe8174fa332468069b33634814f012474c2aa7c645a0a26a15cc`  
		Last Modified: Fri, 13 Oct 2023 04:57:17 GMT  
		Size: 171.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b27a5afd03df7617228e4e64093e061d38f57318246537ce92ae47ef71103dd0`  
		Last Modified: Fri, 13 Oct 2023 04:57:18 GMT  
		Size: 4.8 KB (4785 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:11-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:72136ca3b3ab0c57b0b3c07d282f7b0b2ab170f6fdac5ff604ad6612e3fe2789
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5001761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89dfe87d83582b1a7677eec00f19599d2b5e75deea8723b43b67473866e97004`

```dockerfile
```

-	Layers:
	-	`sha256:03ac8cc03279d2877ef6fa70dcd5554118eb38053787fb512a110354c2ad14bc`  
		Last Modified: Fri, 13 Oct 2023 04:57:17 GMT  
		Size: 5.0 MB (4951852 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:e5fc3a73b0c62f44adfc589677a411b681f0a31321d349f4b596212ebc39d629`  
		Last Modified: Fri, 13 Oct 2023 04:57:16 GMT  
		Size: 49.9 KB (49909 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:11-bullseye` - linux; s390x

```console
$ docker pull postgres@sha256:d399d4a10cb7187dd7c3d3d90c70baf9fe1bbb6c8e7667734edd5127332f52b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138518559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:856cbdb7779547ed449eef62fac5e66ceae5ee516d43e0064ab5a3f68ebed9b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 10 Aug 2023 18:02:22 GMT
ADD file:0cfc89fea6da8404b2bccfb0c408dde9e7497e8a93304c4ced9e51bd2b3a319a in / 
# Thu, 10 Aug 2023 18:02:22 GMT
CMD ["bash"]
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV GOSU_VERSION=1.16
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8 # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV LANG=en_US.utf8
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PG_MAJOR=11
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PG_VERSION=11.21-1.pgdg110+1
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 10 Aug 2023 18:02:22 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA" # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 10 Aug 2023 18:02:22 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 10 Aug 2023 18:02:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Aug 2023 18:02:22 GMT
STOPSIGNAL SIGINT
# Thu, 10 Aug 2023 18:02:22 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 10 Aug 2023 18:02:22 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:a12df18f4c86c0f825c6b30eb023dc9f30ba0de34f6b97dca708a7247f4f6c49`  
		Last Modified: Wed, 11 Oct 2023 17:57:36 GMT  
		Size: 29.7 MB (29656917 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:029f80cb736850ba17c8026acafbb79cd0ddd66e3d7ecdd91eefc30b3e359e83`  
		Last Modified: Fri, 13 Oct 2023 05:43:27 GMT  
		Size: 1.7 KB (1688 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3d0a7fbd651b88fdf1017a8c6220522452d9ed292c58aac9d726bda66d557517`  
		Last Modified: Fri, 13 Oct 2023 05:43:28 GMT  
		Size: 4.1 MB (4096084 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:be05afd754a3c2077dd01a515f3b1d7d8eea22ed5b706533acbe8ff12dfd3446`  
		Last Modified: Fri, 13 Oct 2023 05:43:28 GMT  
		Size: 1.4 MB (1438315 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:71150d0671d9f12bb6d2f72185f0ec0589c215aee42448de141aa48444e77522`  
		Last Modified: Fri, 13 Oct 2023 05:43:29 GMT  
		Size: 8.1 MB (8099085 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a9d403e04c732c69e65a56717b3c095d9cacca3f12c6bfbce08470a4f1828334`  
		Last Modified: Fri, 13 Oct 2023 05:43:29 GMT  
		Size: 1.0 MB (1014304 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d5dc7504ba64f3f021e874f79dd38345c182aafc7918a92fe011c9a23b0c4afb`  
		Last Modified: Fri, 13 Oct 2023 05:43:29 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:24420643e53f95befbb6422c897e9f105fa2b8cfea3279e8de078153e7d22a85`  
		Last Modified: Fri, 13 Oct 2023 05:43:30 GMT  
		Size: 3.1 KB (3144 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:327429f19b4372fccfd4cd6f9359d770841a1434f25302413d29edaa20152c07`  
		Last Modified: Fri, 13 Oct 2023 06:09:18 GMT  
		Size: 94.2 MB (94195493 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d06704e831d486b37d176c0dae414268711c88afc96b6a11edf2bb0e958afd15`  
		Last Modified: Fri, 13 Oct 2023 06:09:12 GMT  
		Size: 8.3 KB (8329 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d8661ae185197e694a3328571af43dc95d739b7fa4d4237d02edc3f11448e413`  
		Last Modified: Fri, 13 Oct 2023 06:09:12 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0e500cca7469bc25664d243b457ccaa6dce5d667280c3dc9d794b672bf8d3db8`  
		Last Modified: Fri, 13 Oct 2023 06:09:13 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:adc7cd0dfff6880091ab91d4ab439b717a1e8cd17d9f733876c8c898a5400abf`  
		Last Modified: Fri, 13 Oct 2023 06:09:13 GMT  
		Size: 4.8 KB (4785 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:11-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:2f481553eb8e1703f755b556b7637685c8b50301a63ac7643b18a0c6d0591756
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4976092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1dbc7bb85cddf815893dbebc910e6435b5a40bc8a6e6c17e80cb1ce6e0d12423`

```dockerfile
```

-	Layers:
	-	`sha256:a2ae9b5a084c8397151eb36d6a7240149b4d16ec3e9c404594987fdee045e634`  
		Last Modified: Fri, 13 Oct 2023 06:09:12 GMT  
		Size: 4.9 MB (4926229 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a404b99aa25fc877100acdb6a10d32ed27257d406251726f58003a9ec0f2373b`  
		Last Modified: Fri, 13 Oct 2023 06:09:12 GMT  
		Size: 49.9 KB (49863 bytes)  
		MIME: application/vnd.in-toto+json
