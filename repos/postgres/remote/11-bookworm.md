## `postgres:11-bookworm`

```console
$ docker pull postgres@sha256:5c3c4daa567181f6a387d85a3d86aa9e6ae0e47062f0f05b6813e03e1e317fb6
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

### `postgres:11-bookworm` - linux; amd64

```console
$ docker pull postgres@sha256:6e8c8d27bb47aaf58221cfba78cb5886cc6e7f3315a2ee188b507975cdb1b317
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.9 MB (144948784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65bfdecde9f8076b8b9555591da4c2e6c3e903df07f4942ba62b81f669fe2653`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 10 Aug 2023 18:02:22 GMT
ADD file:fbd8521c24ed758023728505c18d7a0d6d101bc77fd772a4af9b65049b943864 in / 
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
ENV PG_VERSION=11.21-1.pgdg120+1
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:578acb154839e9d0034432e8f53756d6f53ba62cf8c7ea5218a2476bf5b58fc9`  
		Last Modified: Wed, 01 Nov 2023 00:25:30 GMT  
		Size: 29.1 MB (29149836 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0be9e2ccda0647b01d766dbd03b56365a9e36751fd2d9a219bfe9fcf2c5bd542`  
		Last Modified: Wed, 01 Nov 2023 01:03:30 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9068004ed21eae12afa6be5b17c8ff847c2a0092b152893f56981ccbce259685`  
		Last Modified: Wed, 01 Nov 2023 01:03:30 GMT  
		Size: 4.4 MB (4422639 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d161147ec16da58cee7705e27fcc3735d0e8e22a7df0ae1047210a63cf5a71bf`  
		Last Modified: Wed, 01 Nov 2023 01:03:30 GMT  
		Size: 1.4 MB (1448503 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6d98b5f862799b13592aa88ab2b4605cbad33bcd5ca9d1ea92cd6a6d280a7de8`  
		Last Modified: Wed, 01 Nov 2023 01:03:31 GMT  
		Size: 8.1 MB (8067880 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f7ff7bdddb17f1cc55cb43114c545abe94ab11e0857c83181a3b7c1638a66cd9`  
		Last Modified: Wed, 01 Nov 2023 01:03:31 GMT  
		Size: 1.2 MB (1195064 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c3d98522c1bb2ebcccbe1831694ac73f11620a2baef381cf041a1ab76f0d1011`  
		Last Modified: Wed, 01 Nov 2023 01:03:31 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:25ae3bb25aee4c2536f1721fbca0f5eff941fd355532ef7b1748cf349cf1b193`  
		Last Modified: Wed, 01 Nov 2023 01:03:31 GMT  
		Size: 3.1 KB (3144 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da49379c0c4a5a3aeb2a8c1bb6561a3b2c6f0cc88f5b8bf2f6e02fa4d0824565`  
		Last Modified: Wed, 01 Nov 2023 01:03:36 GMT  
		Size: 100.6 MB (100647028 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ba26a50158ced3fe97506c0c6ef3a580f6ca3222511b15dede95b0b52cc48298`  
		Last Modified: Wed, 01 Nov 2023 01:03:32 GMT  
		Size: 8.3 KB (8327 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0cb60f90dcf1fbfc71b800a7f9ef2a7085b56104376b09cb29703fdd4417b57d`  
		Last Modified: Wed, 01 Nov 2023 01:03:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f9784114b6f4eac9ba2a25e8c69bc3566411e3f74674b60b93043d82b38c77d4`  
		Last Modified: Wed, 01 Nov 2023 01:03:32 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bfe862c0397e57714dcc70d945334fbb98e289ce7fc849efffadc19f48051de6`  
		Last Modified: Wed, 01 Nov 2023 01:03:33 GMT  
		Size: 4.8 KB (4783 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:11-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:5567f7424d8b9632cfc1518176fdbace01f2ac10c327e2bb46956fde2deeebcf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4877106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fb1b1ebc157dee66e2a637f7958f8ce009cb772c64ed3ea301e400fb2bf0bc6`

```dockerfile
```

-	Layers:
	-	`sha256:e6f8cce164537d2670cf2114e66702e1ecf5e9f8cfd187a33397511104791ba8`  
		Last Modified: Wed, 01 Nov 2023 01:03:30 GMT  
		Size: 4.8 MB (4827071 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b91ac520c079f0c54f104ac6537ae1c6dc5f720c88c173d45a2743d6e3c40891`  
		Last Modified: Wed, 01 Nov 2023 01:03:30 GMT  
		Size: 50.0 KB (50035 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:11-bookworm` - linux; arm variant v5

```console
$ docker pull postgres@sha256:63e3860632e0a846cc948f0b5617639169a8db77d683c0009afe24d2efaaa320
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137787358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77ebace766fe5e6e8c64e799edc8494d7ae8ef9f4e4e93b47ec1d97db8daf3a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 10 Aug 2023 18:02:22 GMT
ADD file:c00ddcb556a3791b020308012fd4d7749535c34d372bac47f6ff687a7652b25f in / 
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
ENV PG_VERSION=11.21-1.pgdg120+1
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:8d7feeb74478e4770869563dfee6adf560c449e1ac037f4250fde21517f75323`  
		Last Modified: Wed, 01 Nov 2023 00:51:29 GMT  
		Size: 26.9 MB (26921998 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89b5a536e45e35b41624cccc437f0f695abc425b1887dc4b74c72a9350ef986b`  
		Last Modified: Wed, 01 Nov 2023 15:22:32 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bff87197f909d3be7056fd3215aa32dae47740e01bbf77e71c3567a46ff44424`  
		Last Modified: Wed, 01 Nov 2023 15:22:33 GMT  
		Size: 4.0 MB (4040511 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:87eabc6e2c6dd9d78109daec613ac057322988bcb6fd44264a8b296d35e02de0`  
		Last Modified: Wed, 01 Nov 2023 15:22:33 GMT  
		Size: 1.4 MB (1426100 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a1ae65e68105571ef51f1f396a40f8100e984cedcf19b34908afd2d1730baa18`  
		Last Modified: Wed, 01 Nov 2023 15:22:33 GMT  
		Size: 8.1 MB (8067978 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ab9b0aaf386768fdb8427bd92a8598a13f64f73070106ad98d3a096c2f17d3b0`  
		Last Modified: Wed, 01 Nov 2023 15:22:34 GMT  
		Size: 1.2 MB (1193961 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1620d77715374f5ab6218905bc8171d43e7058c90c5682bd5233420ad47a0814`  
		Last Modified: Wed, 01 Nov 2023 15:22:34 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:525c99de099fca984f184b228db45e17dcbf3498fe6c09740103f2d1cb3b6347`  
		Last Modified: Wed, 01 Nov 2023 15:22:34 GMT  
		Size: 3.1 KB (3144 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:be1bed42929fb0898aaa5351bdc2d02a4011235235e17152b367f67a274c45b5`  
		Last Modified: Wed, 01 Nov 2023 17:55:19 GMT  
		Size: 96.1 MB (96118974 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:70711f2674a075c3bff627307ebf8753524048d3fb2d7c3f0c758349ae0e4963`  
		Last Modified: Wed, 01 Nov 2023 17:55:13 GMT  
		Size: 8.3 KB (8327 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:84693467bf08881036ab8ba5a11f83dd6489f40185769ee4ca77895011d2bc5a`  
		Last Modified: Wed, 01 Nov 2023 17:55:13 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8d5c3f4aeefee9c21f159190c2b2f111cd181111001b90d128b9bb5808ebd0dc`  
		Last Modified: Wed, 01 Nov 2023 17:55:13 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f8851a7f2d3d64796f5c4f42b13a85b093266b365881aecd0bd2168b49945413`  
		Last Modified: Wed, 01 Nov 2023 17:55:14 GMT  
		Size: 4.8 KB (4788 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:11-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:116b006c6ba403f65fa7c320701d54fd7deb2e1c8c093e116b6b2370aee91b38
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.8 KB (49832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d30c0c9c63d66c9aff1b41d6313605fc21b5253c05eb11e6c465c95b02309091`

```dockerfile
```

-	Layers:
	-	`sha256:bc78a4bc711db782c3d4481055dd11365fa9355324bed8fc22b1b7965b6e5537`  
		Last Modified: Wed, 01 Nov 2023 17:55:13 GMT  
		Size: 49.8 KB (49832 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:11-bookworm` - linux; arm variant v7

```console
$ docker pull postgres@sha256:d1bf8fe5b7631df2a757bfeaff50b576334af826c004f26489fdac61d60806ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.8 MB (132838634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daaa101a093032b3101394684e839312681444c9a98b031471144e5d089fce3a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 10 Aug 2023 18:02:22 GMT
ADD file:da08fed31a161a2210fd920a1b5e43aa3f4199985cdeaa0d5d24c0a0f19044aa in / 
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
ENV PG_VERSION=11.21-1.pgdg120+1
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:2f11c34abc7b59f09b58bb6e2cf54f260f4b4142ecf8023a114e281ea4b532d1`  
		Last Modified: Wed, 11 Oct 2023 17:46:22 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4facd2c5d70bef63b1727bfe365696e532d93d0145656abb5b85dfc98d3c4ff2`  
		Last Modified: Thu, 12 Oct 2023 18:31:09 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a288cbebc25a18896833b9fe8265e63fd16f6c4ae66ed753923ace0a4ba1a7e`  
		Last Modified: Thu, 12 Oct 2023 18:31:10 GMT  
		Size: 3.6 MB (3645072 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cbd523fa6ed2803288ee2b88ca856071e8d3b66d068500baf2aad2100f6601d3`  
		Last Modified: Thu, 12 Oct 2023 18:31:10 GMT  
		Size: 1.4 MB (1416108 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:46aef7cb74bca24cf91b0e3dbccfc09f6daf0a1936582604b80e55decf7d6d2c`  
		Last Modified: Thu, 12 Oct 2023 18:31:12 GMT  
		Size: 8.1 MB (8067860 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5fe39abc25ccc279d632d452f7b627924cd67f4ea7eccc23fc15eac3a378e2df`  
		Last Modified: Thu, 12 Oct 2023 18:31:12 GMT  
		Size: 1.1 MB (1065952 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6252d2603645fcf1989fb21a2e6569032a52ae3525dc923674b1bb728f1348b9`  
		Last Modified: Thu, 12 Oct 2023 18:31:12 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:782679c4564086aea7f6579c4d34d6a767a38b325cfc234e5d107dfe75aa99ba`  
		Last Modified: Thu, 12 Oct 2023 18:31:13 GMT  
		Size: 3.1 KB (3141 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b5e5ab97431eeace0708a291a584626a418d2f3634b5fb821ea883b81c17365f`  
		Last Modified: Thu, 12 Oct 2023 21:25:49 GMT  
		Size: 93.9 MB (93876882 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1123f76aad15b0cc6d099287e94c19c2d3d5c442bc745e5756fad3f9232a14e3`  
		Last Modified: Thu, 12 Oct 2023 21:25:43 GMT  
		Size: 8.3 KB (8326 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4eb137ee519a40d1636dadb76e9150ba6edc2a1808b581d8e2f44ea6240d6cff`  
		Last Modified: Thu, 12 Oct 2023 21:25:43 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c7ec1880b424eeb5c336d32d4aa06ec70b705b068c7141b38790aa8b765e12bd`  
		Last Modified: Thu, 12 Oct 2023 21:25:43 GMT  
		Size: 168.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:99dc5eb79619a61bbee0945de33dce39cdae34e639cc787f9ef4f554c24921b6`  
		Last Modified: Thu, 12 Oct 2023 21:25:44 GMT  
		Size: 4.8 KB (4789 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:11-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:8946d1e533d71f51fdea591264de953364a8be151528daa66b07dda0590edb51
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4838215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b158a528dc64545654e5b93d4fd9c1667b7749832b327d8deeb8c1314ee0ee5`

```dockerfile
```

-	Layers:
	-	`sha256:7f3444a394758831811aa923baa880dfd73e4079872ebc2d83968ad3a740552a`  
		Last Modified: Thu, 12 Oct 2023 21:25:43 GMT  
		Size: 4.8 MB (4788168 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f89e271d6c13109caf399662df36fb0b0e9155d320cfcc0899f5befee313c0e9`  
		Last Modified: Thu, 12 Oct 2023 21:25:43 GMT  
		Size: 50.0 KB (50047 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:11-bookworm` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:4885591c1b3caed18cb91cfcb2d08f5035144d448a6330ebfb283521e3711dc7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.9 MB (142923480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da73bdc4a2353071f3c3397b1f20df59b9e5ccab0fb94ef695bd689c8b0a62b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 10 Aug 2023 18:02:22 GMT
ADD file:5c81bfc00a28feb4079c0daa743f829a6a5bbc1a9d40a890cb49e420539a7f15 in / 
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
ENV PG_VERSION=11.21-1.pgdg120+1
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:1bc163a14ea6a886d1d0f9a9be878b1ffd08a9311e15861137ccd85bb87190f9`  
		Last Modified: Wed, 11 Oct 2023 18:28:28 GMT  
		Size: 29.2 MB (29179284 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fe7eaee44872e599ccb8d0e447402f7620ec0f4959af25b499945231225505d4`  
		Last Modified: Thu, 12 Oct 2023 10:42:26 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e13ff0d3a0490b3bd4494019ac4808203b77d5727d0b04f02f39d9a1d53d4543`  
		Last Modified: Thu, 12 Oct 2023 10:42:27 GMT  
		Size: 4.4 MB (4383854 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4d16fa05eefee762c2f5abd2ad414208de704a0aad4686e459138bc1c169829e`  
		Last Modified: Thu, 12 Oct 2023 10:42:27 GMT  
		Size: 1.4 MB (1380716 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d86be54291050ce5b8614bc6fa7ac0bc7c5d97dd5800f9c4a68ea052d04433e3`  
		Last Modified: Thu, 12 Oct 2023 10:42:28 GMT  
		Size: 8.1 MB (8067971 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b9908c218b14658b8acf70ba82d5bb1dc8a3d0e1d06114fb79a50c754173434`  
		Last Modified: Thu, 12 Oct 2023 10:42:28 GMT  
		Size: 1.1 MB (1107712 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:07683d534ecbf8b15ec0289f3fcd4d7381e7ae622bad17a08c00bc927912c1c0`  
		Last Modified: Thu, 12 Oct 2023 10:42:28 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c5194879a0212b77a2125adef410f2e3b8ad74c6d8900342a8ad53ee12a4aed`  
		Last Modified: Thu, 12 Oct 2023 10:42:29 GMT  
		Size: 3.1 KB (3143 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eb3a2d31a1f19b9ca86bcc5d94dee279914bcad2409c6add397c2e8d7b002404`  
		Last Modified: Thu, 12 Oct 2023 10:42:36 GMT  
		Size: 98.8 MB (98786102 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:16d182f56e9a02c859a0078db5c5606f75e7fa1137c5932f4d9edb5ad5a18f95`  
		Last Modified: Thu, 12 Oct 2023 10:42:29 GMT  
		Size: 8.3 KB (8328 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2e5c0efa5a656f2ea7d027c7dfb8a604b9d6b3ea8b9c76ade40977b9d65b3beb`  
		Last Modified: Thu, 12 Oct 2023 10:42:29 GMT  
		Size: 127.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e54bd28ae20eac81574ad6576f6f528fc53ce1af23dc09d8263b0aa7eea698be`  
		Last Modified: Thu, 12 Oct 2023 10:42:30 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ac1252ac287179ab5d268e967f037d836380d5634a785a0bb18a911bba651da7`  
		Last Modified: Thu, 12 Oct 2023 10:42:30 GMT  
		Size: 4.8 KB (4790 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:11-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:7fbe8a94b5fc275293a30c5fc0ad12bd01017e7507adc65b1b65aa105d1c1424
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4826758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7a20e3d845ea35ff704eb8b0feb4be15ebf585299e368de072b150df57421e2`

```dockerfile
```

-	Layers:
	-	`sha256:e0ebf18463a50970821ad1904e7c89ca1451e15b79c28bf260113de02133b6e3`  
		Last Modified: Thu, 12 Oct 2023 10:42:27 GMT  
		Size: 4.8 MB (4776722 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:43615cafc53513c3be2ffb65e9d3a03de8658e39242b5a2e8e5e8397cb87b3cc`  
		Last Modified: Thu, 12 Oct 2023 10:42:26 GMT  
		Size: 50.0 KB (50036 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:11-bookworm` - linux; 386

```console
$ docker pull postgres@sha256:0f337e9e49e853a4eb654ec0ee16a6cab9f4515a24f41eb37849694293a222a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.9 MB (151888720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d160a7ca1cd2ea64b27e0051c1af408b2e13d587bf0b0df3aa2326a2fa9356f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 10 Aug 2023 18:02:22 GMT
ADD file:0c94521fdd9c0a4fdeeb9aad23e68cd053fba0dcd7c3af550aefa79377816e31 in / 
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
ENV PG_VERSION=11.21-1.pgdg120+1
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:98bdfce9af831c2a0d0bfcca812d0039cd1666986550f552b4b4c625bd5aa31c`  
		Last Modified: Wed, 01 Nov 2023 00:43:26 GMT  
		Size: 30.2 MB (30164042 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9558ee1456705c9615d7bf9c503ae3fdd5e9feafb05984a63937fe44f2882020`  
		Last Modified: Wed, 01 Nov 2023 01:17:46 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:634f1bbbcc1566951b5f05beda10c6942d75edbb370d6da1792f88ab5251f3f2`  
		Last Modified: Wed, 01 Nov 2023 01:17:46 GMT  
		Size: 4.8 MB (4844468 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1c3296367646b1479375e970f55175c8a74fb76f06408b44a2444b8bf62e32f7`  
		Last Modified: Wed, 01 Nov 2023 01:17:46 GMT  
		Size: 1.4 MB (1424522 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:db8246c8f037dac021106e169a69786ac9da8a188ea7e4945a1dd7d6aba054f5`  
		Last Modified: Wed, 01 Nov 2023 01:17:47 GMT  
		Size: 8.1 MB (8067913 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a3b0c9ea2d500556dd33a654d00a7ca49d20321a109f745dbdaaf44145f1180e`  
		Last Modified: Wed, 01 Nov 2023 01:17:47 GMT  
		Size: 1.1 MB (1136169 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:51c8520fea571d4a3e4ab6ea2691d34e345d8951c93069f567c9f50ea77b6388`  
		Last Modified: Wed, 01 Nov 2023 01:03:25 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:357ab8271670fdb088e878280ba276cb22ef7a469b10ed3075e62a1466186ad7`  
		Last Modified: Wed, 01 Nov 2023 01:03:25 GMT  
		Size: 3.1 KB (3144 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2b3f3e369112a524bf1108403be70c53fcf9c2f8edb0be1f594f343d7546be69`  
		Last Modified: Wed, 01 Nov 2023 01:17:53 GMT  
		Size: 106.2 MB (106233767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d0f0dee1523ce477616fc8208ff36719d49dde727fcac00cc81c01fe1eb869f`  
		Last Modified: Wed, 01 Nov 2023 01:17:47 GMT  
		Size: 8.3 KB (8330 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9614500eaa762668548f296b0d8de2f13b1affd3e927f96ac2f1221245802623`  
		Last Modified: Wed, 01 Nov 2023 01:17:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1bbe48076aa39434d5591c5905f31680da98de8380342117ce2eb1f37a307ec2`  
		Last Modified: Wed, 01 Nov 2023 01:17:48 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b45fd9ed1a177a7334cc9190c55b1a68d14fe0978140dbe24dc27f7bb36d95e`  
		Last Modified: Wed, 01 Nov 2023 01:17:48 GMT  
		Size: 4.8 KB (4786 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:11-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:162372cb34cc3defeef916ae280a9e2c585cfd8ab5112e1964238003d7c01989
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.8 KB (49781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:345b2e4b1ce55f4ef094844941f57e1b1decddaced3bc8be48151f6243776d84`

```dockerfile
```

-	Layers:
	-	`sha256:81ccb1656562910b484c747e621308530f2b33b0e87f03099fd01fa25ea7ea83`  
		Last Modified: Wed, 01 Nov 2023 01:17:45 GMT  
		Size: 49.8 KB (49781 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:11-bookworm` - linux; mips64le

```console
$ docker pull postgres@sha256:6691d6d3de9a5018347dbbc6a19cfece0bf29f7c05eb3315a73a435737fdb4fa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.1 MB (141129389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d10786554244ab246c4fe4978d11c2f0680f6a4662d44ac7232a8ce051fa84cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 10 Aug 2023 18:02:22 GMT
ADD file:2abda0a72972a417d4f7f530ca8fa1ee7e85e25d4015fd4e70acf903cfd96d3d in / 
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
ENV PG_VERSION=11.21-1.pgdg120+1
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:f11870ec99d788b4b160d9f3f4c0a79904290083d8930b26e5d13579226e07f0`  
		Last Modified: Wed, 11 Oct 2023 18:00:43 GMT  
		Size: 29.1 MB (29142026 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b37824221b719661a665dbf0e19aec4a57008e056fab2f3de51a3f58fa68ad74`  
		Last Modified: Fri, 13 Oct 2023 10:36:46 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b90cadd652a0e0bf7f0d5b8df0e371544c97d7781cedea13730fc55dd2e1f58d`  
		Last Modified: Fri, 13 Oct 2023 10:36:47 GMT  
		Size: 4.4 MB (4355792 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1c9ce2e72082369681df18caabc15ba0663cb5d9f0af63dfecb25898ba16dcb1`  
		Last Modified: Fri, 13 Oct 2023 10:36:47 GMT  
		Size: 1.3 MB (1336004 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0c0b171f54ef2143f543b5a3d471a644423c5f6d62c0a4a78262533cb02b0f8a`  
		Last Modified: Fri, 13 Oct 2023 10:36:48 GMT  
		Size: 8.1 MB (8068088 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5fab6a8207afea9019c72eb0b82d28b69968f1ee5df6c038566544651016190a`  
		Last Modified: Fri, 13 Oct 2023 10:36:48 GMT  
		Size: 1.2 MB (1181567 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b0249c365c791cbd32d712c972f178a5e23beb01af4525ab65d3feada22bfc29`  
		Last Modified: Fri, 13 Oct 2023 10:36:48 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:79c1265289be673dab55108553ea56588d26470891f5b6c355d1366eef9fdce0`  
		Last Modified: Fri, 13 Oct 2023 10:36:48 GMT  
		Size: 3.1 KB (3144 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:81ac537dc75903e0af197e34550fa174b0f7e5523e85573c4692c7ee6a9d6455`  
		Last Modified: Sat, 14 Oct 2023 02:11:04 GMT  
		Size: 97.0 MB (97028061 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8f17807484dc964953c2926efc49bef17a31c5dd398ec06afa68face4ddef770`  
		Last Modified: Sat, 14 Oct 2023 02:10:54 GMT  
		Size: 8.3 KB (8332 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9010dc558874aa4f48e19620367d80880a15ed5bf6c562702d3433f10bbc8405`  
		Last Modified: Sat, 14 Oct 2023 02:10:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:322413676dd2bc2c4b83ab26d2544439921c7dfc496dd4e6f84e8b182ee62b65`  
		Last Modified: Sat, 14 Oct 2023 02:10:55 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ab4b673b1a24e9870a52a9382a99ed5cda333bfb20b760ea5da7cee0e2c0a16c`  
		Last Modified: Sat, 14 Oct 2023 02:10:56 GMT  
		Size: 4.8 KB (4790 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:11-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:2b5df3b25d22c3f63862ca5de0caf0e60b20c94996374d32304de0d6473164d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.7 KB (49717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad7296c2f3cde429cfdd74860dd9cad6c5eddfcc5e5b3b7f14f71cc9d6517209`

```dockerfile
```

-	Layers:
	-	`sha256:03a5e888145b50718d575452d4182fb653ec105048842088ba31359df31df28b`  
		Last Modified: Sat, 14 Oct 2023 02:10:54 GMT  
		Size: 49.7 KB (49717 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:11-bookworm` - linux; ppc64le

```console
$ docker pull postgres@sha256:f6ce7466b316912264544bec89a458d2f4ac4157f1cff2a7a07ec35ee63cd4ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.5 MB (156516079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e24ecf59ba085bf74e060f9292b6d6d69082f198591aa1a9e21effb9fb357be5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 10 Aug 2023 18:02:22 GMT
ADD file:53c83bdd58e7c4003ae769596cc2f8e6b72c0bbb854dbe7f006a39f273848b1b in / 
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
ENV PG_VERSION=11.21-1.pgdg120+1
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:54813908ce8a5d8a81f2db88ad0366eb5266484c7c402e5e93ef26e764f7a0e2`  
		Last Modified: Wed, 11 Oct 2023 17:49:58 GMT  
		Size: 33.1 MB (33141653 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c1d64a898f51bd59910434d75b5421e466556e6189d7c429f3409210fd40bdc9`  
		Last Modified: Fri, 13 Oct 2023 01:08:44 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a22cdf1ed46ac99577690807f680edfad9a8f60b561b56dc2ed6a4663dac263`  
		Last Modified: Fri, 13 Oct 2023 01:08:45 GMT  
		Size: 5.2 MB (5239267 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:118e8d21fcde53aff7add1b1fc59183b24a8f3d059264dd2bae23114a758b366`  
		Last Modified: Fri, 13 Oct 2023 01:08:44 GMT  
		Size: 1.4 MB (1370043 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:be5afdd73aa12fec9cca2a6418b381afbfe8755ff6e49e6dc6898afd7d8e5fcf`  
		Last Modified: Fri, 13 Oct 2023 01:08:45 GMT  
		Size: 8.1 MB (8068045 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:860d0a9f288b61b3d55aac1d41314e8223eb4ef4eda8688f3a8f7de9aecf8bb4`  
		Last Modified: Fri, 13 Oct 2023 01:08:45 GMT  
		Size: 1.3 MB (1282781 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4730b799559ef181d60866ce28543d85c1d184dab0c68a0272310ced70629fff`  
		Last Modified: Fri, 13 Oct 2023 01:08:45 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf82148d68620142dd018dfa25bce557571f445b5c19184d7309db51ab48bd69`  
		Last Modified: Fri, 13 Oct 2023 01:08:46 GMT  
		Size: 3.1 KB (3143 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:de598d124fa3a03c57a550c289d01a311b7bff04a0296d1b52e16e173a56183e`  
		Last Modified: Fri, 13 Oct 2023 04:54:52 GMT  
		Size: 107.4 MB (107396453 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aca87cc91a164ef0ca2a83bc699326bec097e35e9064a8b62842c6fea48f5c55`  
		Last Modified: Fri, 13 Oct 2023 04:54:47 GMT  
		Size: 8.3 KB (8327 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:579d743a5c06b34d4bab6f2efd6e0c0e49d5faf213883d6f646a082ed1974032`  
		Last Modified: Fri, 13 Oct 2023 04:54:47 GMT  
		Size: 127.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:91c9acde129f53d2e52a147a908cc156f47c3cfa29773c4f3d22784a36f4a073`  
		Last Modified: Fri, 13 Oct 2023 04:54:47 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:97c425269696c385549e9f797e84db2778fed59d3bb601b3d1f06d811feea2f0`  
		Last Modified: Fri, 13 Oct 2023 04:54:48 GMT  
		Size: 4.8 KB (4788 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:11-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:363371efdeb04e4b5425ea89fd45e67a90b029a551e33380a073877e1ea75bfa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4840309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:257710d22bb37aef7143f775177068fe8d66af986080777d34589c849fb2bf4e`

```dockerfile
```

-	Layers:
	-	`sha256:8e9cc24e91c504651a9bd17dffb242bd766e97fde3496196cd4f641c6b9055c3`  
		Last Modified: Fri, 13 Oct 2023 04:54:47 GMT  
		Size: 4.8 MB (4790395 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:fadbdc0b962e8a44f78d2a84a5e6d28a918766305079ca3dc8e206e8492d78a5`  
		Last Modified: Fri, 13 Oct 2023 04:54:46 GMT  
		Size: 49.9 KB (49914 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:11-bookworm` - linux; s390x

```console
$ docker pull postgres@sha256:2c18eae1cc7ceca591d2b80fbc2dc0eaa5c9eac33ae0de9fd5a295d1127f5564
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.1 MB (150114763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f411f431d54686975b514ff006be95a9e917d49174217872fe4d073e2788e301`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 10 Aug 2023 18:02:22 GMT
ADD file:2764e93c5bba50564937cce7bcaa7c7d3bdc3fd0d53a7bb09e6955e6fda8d7c2 in / 
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
ENV PG_VERSION=11.21-1.pgdg120+1
# Thu, 10 Aug 2023 18:02:22 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:ac72f5406002214602d5a625a21b606af78a78e99e377d3140a83021f7edd666`  
		Last Modified: Wed, 01 Nov 2023 00:48:04 GMT  
		Size: 27.5 MB (27512766 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:07d6b9d43a4b35250440297979532ab3515a8ec8ab1ea35b44a008ebc3f144de`  
		Last Modified: Wed, 01 Nov 2023 01:07:34 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:db86f81e0b1af776a51011ad5f55068e76ab77d1f31dcbc040b0702b20427472`  
		Last Modified: Wed, 01 Nov 2023 01:07:34 GMT  
		Size: 4.3 MB (4278300 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb27c3d28b808be1f030e4e0b57ca98e671647aa84a5847b54c864bb3ba15c80`  
		Last Modified: Wed, 01 Nov 2023 01:07:34 GMT  
		Size: 1.4 MB (1414349 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2836a8b7da48e1c618312914de1439f84f5cdebc8620b3d736fc7d17bbac1e55`  
		Last Modified: Wed, 01 Nov 2023 01:07:34 GMT  
		Size: 8.1 MB (8122241 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b54461755a1570db9ea9dc984f138fb768669ae71ee1f9b5ba18d437f5428b89`  
		Last Modified: Wed, 01 Nov 2023 01:07:35 GMT  
		Size: 1.1 MB (1095685 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d88e40a02f754960ee9d61cbd6cc19b1d7905ac1449ccdc33013d91187808559`  
		Last Modified: Wed, 01 Nov 2023 01:07:35 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e1e0534e50eb8e5cb8e9d40c713fb6ed11bc6a548e5c6b5585015561efe58318`  
		Last Modified: Wed, 01 Nov 2023 01:07:35 GMT  
		Size: 3.1 KB (3144 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:33857500f78dbc647a465e1ed93ab6c8a10f52c2249f392070e82891934f3171`  
		Last Modified: Wed, 01 Nov 2023 17:13:42 GMT  
		Size: 107.7 MB (107673584 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0fd1fc05ab490b18cfbe399443da22e9c6d2439b6625a152386e1cb856a842be`  
		Last Modified: Wed, 01 Nov 2023 17:13:37 GMT  
		Size: 8.3 KB (8329 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da587d97798736533e2c90f8d418a97aa132b58d774c5b5765be18528dc12fbe`  
		Last Modified: Wed, 01 Nov 2023 17:13:37 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:23e80446c297c06ea2938c1da0c03230ccd692858c1cc85e95bf1376e4c4b893`  
		Last Modified: Wed, 01 Nov 2023 17:13:37 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f4242f6f7872d7a8cd1f443172f74397a11338ad7bf77ce617208fe5232c3a11`  
		Last Modified: Wed, 01 Nov 2023 17:13:38 GMT  
		Size: 4.8 KB (4786 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:11-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:7854c4a64a3382a602d0b817e38cdd895c126195e08934bc5da143172a665718
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4876121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63b8289591dc6d74824b179a79d369b23e60e7cc54ab04e30325dc73a225ec38`

```dockerfile
```

-	Layers:
	-	`sha256:60bf97d4e5aae846771c8a3eae2ce8fa516350d4cec5b2e18eaa5bad58ae5412`  
		Last Modified: Wed, 01 Nov 2023 17:13:37 GMT  
		Size: 4.8 MB (4826253 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:af99d3088e3686dc7e9c69b1a5d2d9f3c8753678e8f90d3e4b8f7b65760c4aa5`  
		Last Modified: Wed, 01 Nov 2023 17:13:37 GMT  
		Size: 49.9 KB (49868 bytes)  
		MIME: application/vnd.in-toto+json
