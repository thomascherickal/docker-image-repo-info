## `postgres:13-bullseye`

```console
$ docker pull postgres@sha256:5312b55d12bc1aa78b1e63d9c3ab0ecc01d65ff8060c40f05e34d5afefe34263
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

### `postgres:13-bullseye` - linux; amd64

```console
$ docker pull postgres@sha256:8aea50c8f8385adac864292a20c5412a555c06b95b68bb6ab4f06210e151fd1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.4 MB (136429293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd2812c2792738ca0e346cfd49b1bbfbc83c52e44264771789d1dbf583e44df3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 11 Dec 2023 18:58:54 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
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
ENV PG_MAJOR=13
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_VERSION=13.13-1.pgdg110+1
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0fe1b92edc640f55dc9a72138ebc39aecdcf93292c3f6d2e4d62accac3179447`  
		Last Modified: Tue, 19 Dec 2023 03:49:21 GMT  
		Size: 1.7 KB (1683 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7a49bf42f0e475d059fe31999719c53d48a6d6ef6d272eb8e89a8f983bafd2e9`  
		Last Modified: Tue, 19 Dec 2023 03:49:22 GMT  
		Size: 4.2 MB (4207467 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:960a285d0ff19795952263ebd3fbb7caa8e22326985cd079c71c758fd6c2da6d`  
		Last Modified: Tue, 19 Dec 2023 03:49:22 GMT  
		Size: 1.5 MB (1472471 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3d8f89f5c9a03546d9e116fc26f95d86bdd4f67be23b85b89c3df64f73f96f66`  
		Last Modified: Tue, 19 Dec 2023 03:49:22 GMT  
		Size: 8.0 MB (8045248 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e30d77dec428c4e17626ca04131250a9fa7fb50d72aaee84d8db99b02cff1f81`  
		Last Modified: Tue, 19 Dec 2023 03:49:22 GMT  
		Size: 1.0 MB (1037444 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2cce8f7e2b8202cd6c00772aefce3e762f2783be357669cfe9212e60f4589ae5`  
		Last Modified: Tue, 19 Dec 2023 03:49:23 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0c3ba98d35a065bcab6e297246e9cd88e90bac1c6bb04f29d8bf75570c602908`  
		Last Modified: Tue, 19 Dec 2023 03:49:23 GMT  
		Size: 3.1 KB (3145 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:45b1f3780c7163b2391c62f7f3141eb8ff7d4657700ae0955042fbfa07c1d1be`  
		Last Modified: Tue, 19 Dec 2023 03:49:24 GMT  
		Size: 90.2 MB (90228667 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:36df9c91975cf4e0a2f8e932f6edf88914f7e9e21dfc2422e13bb95f67950f18`  
		Last Modified: Tue, 19 Dec 2023 03:49:23 GMT  
		Size: 9.4 KB (9353 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6641e3cdab3c1b3c1e7ee788d3667a8e6752633af15e8880c6a8a62c221f2c6c`  
		Last Modified: Tue, 19 Dec 2023 03:49:23 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d30fc99f00266bd2d513e7b8455a1f2734f2530a24c6b1da2de5882f469dc1b8`  
		Last Modified: Tue, 19 Dec 2023 03:49:24 GMT  
		Size: 172.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:db8d60b03c11e7e51bead57b286bd924484feeffb22a297e152ef2c69821b2e7`  
		Last Modified: Tue, 19 Dec 2023 03:49:24 GMT  
		Size: 5.3 KB (5340 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4896a60985e77abace7c0e6e7ee673c49fd026ae06c7dd4cd299488ae265615c`  
		Last Modified: Tue, 19 Dec 2023 03:49:24 GMT  
		Size: 186.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:13-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:ab75255a63ce8773b67f25164fb43feff5910380a5c3817e5ff181e0d0f75285
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4980039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d479ab5f16458737909a86c11ebb5203aa96e19ff9ae34fd874bf04ee5fd56e6`

```dockerfile
```

-	Layers:
	-	`sha256:b6758e4de63900658fd54851d6bec1b289088c4deb68436ae982c80c9262350e`  
		Last Modified: Tue, 19 Dec 2023 03:49:21 GMT  
		Size: 4.9 MB (4926185 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:81ea75c68d148f5736382207802d0732ae0cf8ff4b35cc3939ea762a73ab3e50`  
		Last Modified: Tue, 19 Dec 2023 03:49:21 GMT  
		Size: 53.9 KB (53854 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:13-bullseye` - linux; arm variant v5

```console
$ docker pull postgres@sha256:84115ef537fbebc60851622f08e0ee75bc97febd0710de156655f9f7c7f25177
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129587389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:812d91a3ef4d27bb942e3b093e3b540430b592da13a52bd1dce2850039129ff3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 11 Dec 2023 18:58:54 GMT
ADD file:831966ecbc1ad85566dda1f3580cd9306cc099069cd418506e8befd03c296d1c in / 
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
ENV PG_MAJOR=13
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_VERSION=13.13-1.pgdg110+1
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:fdebea600ba5b47ddd94c41d9d687679a030fdad563a3490945a5433dae01d54`  
		Last Modified: Tue, 19 Dec 2023 01:59:22 GMT  
		Size: 28.9 MB (28921283 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c8b17a06ffa3320ccfe76e7d2b9f21b851cfc9dcccfd09f4cfc8096e66f5bd4f`  
		Last Modified: Tue, 19 Dec 2023 16:42:05 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:64af0b841280455247d46812890d54321f384070b68408a18d4d02da7e6bb5d3`  
		Last Modified: Tue, 19 Dec 2023 16:42:06 GMT  
		Size: 3.9 MB (3889288 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d9602b7a047953422b7834698dc7d5b4452af629e6e1b92b8bbb01c6e6f7190a`  
		Last Modified: Tue, 19 Dec 2023 16:42:06 GMT  
		Size: 1.4 MB (1449972 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:54be4f2ae1ebdf3ddb038261842efa004884d3e4e9b77d26369bd500cda63f41`  
		Last Modified: Tue, 19 Dec 2023 16:42:06 GMT  
		Size: 8.0 MB (8045165 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50185ddccbcfb827a990b0eeed0c750ac97f28036caaabb8a704b4d67b877807`  
		Last Modified: Tue, 19 Dec 2023 16:42:07 GMT  
		Size: 1.0 MB (1033916 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1ca75026c18e4b6ac67ce24fb9e13a24d957d8f63bda67ae7df31c9ac2652638`  
		Last Modified: Tue, 19 Dec 2023 16:42:07 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6a2b3931718a446aa856ab8719ed141597d7c66baebe8e141de92192607131ff`  
		Last Modified: Tue, 19 Dec 2023 16:42:07 GMT  
		Size: 3.1 KB (3141 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c92bbf4784ec8c0a9d09b54e58790eed400d1012f14100a1f7110583b14ff5b7`  
		Last Modified: Tue, 19 Dec 2023 18:33:42 GMT  
		Size: 86.2 MB (86227644 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:44a8bb6954064a345144cf15fbc01fd553b71290e6d4d161c80b3f7772595a09`  
		Last Modified: Tue, 19 Dec 2023 18:33:40 GMT  
		Size: 9.4 KB (9361 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3bf113bc8d0d5847f6595ac009bbc783f7d07e36019d71d15dff8a8f6426d1b9`  
		Last Modified: Tue, 19 Dec 2023 18:33:39 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:300bd8be56c51dfbf32a440729872bd8ef8ab3d88fd9cfaec12b9aeb9a5dfbf5`  
		Last Modified: Tue, 19 Dec 2023 18:33:39 GMT  
		Size: 168.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f3b8b979592bd5ad0da0ec1724df657a677cc10ecfaf27845c9279bb0d5f226f`  
		Last Modified: Tue, 19 Dec 2023 18:33:40 GMT  
		Size: 5.3 KB (5344 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:97513aa794a2f3eee1d94f41163b68fe0e88686ec31db6ac5df82b005bf37ec3`  
		Last Modified: Tue, 19 Dec 2023 18:33:40 GMT  
		Size: 185.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:13-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:1a2f15a739eef8f783cfbfb269733b3dfc6c752bc913921b72d6603ededb7c1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 KB (53669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3098d26ef6d50047d2e7f28a3d2673d5af549270a626ee4640ead2c0fa1f876`

```dockerfile
```

-	Layers:
	-	`sha256:30cb384a9c9c2eada8c355074c7b63e5bc0dac276deb02a025277035840fc08e`  
		Last Modified: Tue, 19 Dec 2023 18:33:38 GMT  
		Size: 53.7 KB (53669 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:13-bullseye` - linux; arm variant v7

```console
$ docker pull postgres@sha256:6f6d88d904b7c8d4651aaa515b208b681489b69fab748010675645923fca0729
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124324378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad1d65f93cf6b4774fe2d3818fd1d60ad46c309c350ced13d5e9bfc76151af95`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 03:58:04 GMT
ADD file:c4afced274aaa80ab3018b368ed739c1c55e49b41e9637ac44d63e61344fe865 in / 
# Tue, 21 Nov 2023 03:58:04 GMT
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
ENV PG_MAJOR=13
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_VERSION=13.13-1.pgdg110+1
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:5c39cf341d428ea9188d777cab5a4c94f1fc12fdc6a2425d05e625d850bcdca0`  
		Last Modified: Sat, 09 Dec 2023 05:52:42 GMT  
		Size: 8.0 MB (8045236 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b01a7f4c370ad80689b166441d3514666eb75428c26502c76f9caab498bf4d0e`  
		Last Modified: Sat, 09 Dec 2023 05:52:42 GMT  
		Size: 907.8 KB (907792 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c253d539777978d21acf514a003973e041e5c27a2082162d21eeb75b62920c17`  
		Last Modified: Sat, 09 Dec 2023 05:52:41 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2478ae0a2a54ce75a8c09f32ad4ad8a31abcc5e51be714fd015a32539f175f1c`  
		Last Modified: Sat, 09 Dec 2023 05:52:41 GMT  
		Size: 3.1 KB (3145 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:46c85fc48278b97bd717bd76448f759b6317e7c48ac9994a0a9fd3c638a2b468`  
		Last Modified: Sat, 09 Dec 2023 07:42:25 GMT  
		Size: 83.8 MB (83822315 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:489c95a332ace6f3c68a2e390d5ceb0b41ff0b8dde2b054a4f4efd09d58683c0`  
		Last Modified: Sat, 09 Dec 2023 07:42:22 GMT  
		Size: 9.4 KB (9359 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:67d8a14463578585982ec20230b0edbe8437dff129f4d119b9adc334c9beb6b9`  
		Last Modified: Sat, 09 Dec 2023 07:42:22 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:af0d9b16a9dbd4ea20429650a7a1dcfa9be59bfd79c7a11f76b648905c9c527b`  
		Last Modified: Sat, 09 Dec 2023 07:42:23 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e6ea91e3ee615d6a3afadc1c05a1df74dfeb452faecb01271301f2da6b08ccf9`  
		Last Modified: Thu, 14 Dec 2023 19:31:20 GMT  
		Size: 5.3 KB (5337 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fc5dc46dac499791af4e7f5ab685017eaa06dd5826facd98eb256b12c80663d1`  
		Last Modified: Thu, 14 Dec 2023 19:31:20 GMT  
		Size: 185.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:13-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:8b267e86e3f2f13f37a212f2e710aaa44e5d854080bcd0a961a475e963c560c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4989736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3980ac2dcfed74eb438a506d55742afca9d04019ad4ae82737fd22a72c97192b`

```dockerfile
```

-	Layers:
	-	`sha256:3a85ddfd57353cb5a09c55e4af6a28de9a1996330bb9640df742bdcc5918a710`  
		Last Modified: Thu, 14 Dec 2023 19:31:20 GMT  
		Size: 4.9 MB (4935861 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:64d1c1392b049f4c3eccac79a171d5f4c8b0ad7c8def44903b6808d67cbe8c3b`  
		Last Modified: Thu, 14 Dec 2023 19:31:19 GMT  
		Size: 53.9 KB (53875 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:13-bullseye` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:a2d072c13a15538a7b61ce653d75873ca9f27770c5da41d16831fcc07b372a65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131517940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:093771f3ba05792deff516742b3dcfde6939f0938e3d699b1228457239919eb2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
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
ENV PG_MAJOR=13
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_VERSION=13.13-1.pgdg110+1
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26d8e35e025ba18d00a023f73a42e9fef69bf9a5fcf9319d2052ebdadb0ed180`  
		Last Modified: Thu, 14 Dec 2023 20:19:28 GMT  
		Size: 1.7 KB (1689 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:621f8729ccee11c1ad3afd9e43d8c0f0b2e3d77fd6e2ac604e79a7fc12f1b7cb`  
		Last Modified: Thu, 14 Dec 2023 20:19:29 GMT  
		Size: 4.2 MB (4209460 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8a8d15bfa3ddaea50b8bd5effcd822ec1d82508e16f15d93bae78c12057398d9`  
		Last Modified: Thu, 14 Dec 2023 20:19:29 GMT  
		Size: 1.4 MB (1404403 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e012f0d3b92f8148be3aca422ff924c9e9815eac7a6ab2770f380a38fe3f6e8`  
		Last Modified: Thu, 14 Dec 2023 20:19:29 GMT  
		Size: 8.0 MB (8045202 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cab050646091b33fcad866f3fc875216b9ced730086a864c47258b5d159f4c45`  
		Last Modified: Thu, 14 Dec 2023 20:19:29 GMT  
		Size: 1.0 MB (1025884 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b881b0bb9f8c7e6b117860de9150285128d36c5b002bd9e2e8dcf56549228044`  
		Last Modified: Thu, 14 Dec 2023 20:19:30 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:caac159a555aceb06a6dfc1a6b7e5d718c4e9a4da7255f5509a77b92061d0c86`  
		Last Modified: Thu, 14 Dec 2023 20:19:30 GMT  
		Size: 3.1 KB (3144 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:53a51ebbdaec2b54817d9505c109484268ced2a81f77dafb64fc36194f3acb22`  
		Last Modified: Thu, 14 Dec 2023 20:27:45 GMT  
		Size: 86.7 MB (86748735 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9c4c0a1dc3dc1cdbde7b8d9ad6104c6aeb353d24587df0786cfd203685215e41`  
		Last Modified: Thu, 14 Dec 2023 20:27:42 GMT  
		Size: 9.4 KB (9360 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7585f6c86e1d430c47a3cb31bf286aff0637c61f4184d7af21cd51ced4dac58d`  
		Last Modified: Thu, 14 Dec 2023 20:27:42 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ab81b1c391fec2caecaf41c1555e69f76f32b150448c0989abb2bb2eb1308a8`  
		Last Modified: Thu, 14 Dec 2023 20:27:42 GMT  
		Size: 171.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e1fa97b94e20b13bd68abbfd77c426ec25e4c64d0c67f5ca81954f451a8e8fb5`  
		Last Modified: Thu, 14 Dec 2023 20:27:44 GMT  
		Size: 5.3 KB (5340 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3e1ecc27e190ce0d3695220132f85a37ff56e214e85b3561cc200e9f572e0706`  
		Last Modified: Thu, 14 Dec 2023 20:27:43 GMT  
		Size: 185.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:13-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:96d67d745a315dbacc0281bddb83a319087362c10b7dcf9d5522ef161ebfe5cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4985509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f16cb27ab4dc5d22c45d5055d71ef4c07ee68bbc2b06e290865c5f9b0e2cc82`

```dockerfile
```

-	Layers:
	-	`sha256:957df0b5137e7f6b5dde3c85346a53bada44f7f3568f7509742e73ddb9124519`  
		Last Modified: Thu, 14 Dec 2023 20:27:42 GMT  
		Size: 4.9 MB (4931816 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1a3ae799a627ce7ca18019e12b6a063c35ed003a1938823ed2490f08173ede2a`  
		Last Modified: Thu, 14 Dec 2023 20:27:42 GMT  
		Size: 53.7 KB (53693 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:13-bullseye` - linux; 386

```console
$ docker pull postgres@sha256:0894f499a67192d7325c2cd809d9209383c3ddaccae9f1d962a350e6fc88bf04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.4 MB (138398536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82365c76516da1a8e5b654c024a410872dde72ef69bc0e4140a26cb4c18f04a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 04:40:15 GMT
ADD file:7de881b584405a880c4d02778056aaa81bb5dd5d1af65b3086d66aed9ff0ad4b in / 
# Tue, 21 Nov 2023 04:40:16 GMT
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
ENV PG_MAJOR=13
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_VERSION=13.13-1.pgdg110+1
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:75c11612678b54e79a38118fe66e532c61b3d0798afb741007b4cd3209c0ec4e`  
		Last Modified: Tue, 21 Nov 2023 04:45:24 GMT  
		Size: 32.4 MB (32402632 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e46ae5d5094cbf10e4766adf49327569e78191cd470369e32ebc9bb4dba0ae1e`  
		Last Modified: Thu, 14 Dec 2023 19:02:17 GMT  
		Size: 1.7 KB (1679 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:839181cd324a9eccb2950a7379a0bc2d9ddff6ef5aae917a9a06b94a8586ce70`  
		Last Modified: Thu, 14 Dec 2023 19:02:17 GMT  
		Size: 4.6 MB (4607437 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:010def1053f162351f42422860fa939e1e8d42fbb791a2b8c357387c2bead458`  
		Last Modified: Thu, 14 Dec 2023 19:02:17 GMT  
		Size: 1.4 MB (1448289 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:43339a645c12ed0239b4861ddfcf7bfcf16aebe85087bd3512c5e381a978d2dc`  
		Last Modified: Thu, 14 Dec 2023 19:02:17 GMT  
		Size: 8.0 MB (8045157 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc9b2fd30a5681960ddd06df97536714c62192e3a3a77a3fdacca4d032be331a`  
		Last Modified: Thu, 14 Dec 2023 19:02:18 GMT  
		Size: 1.0 MB (1027968 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d1b2206f0ee1d520e727e75c9a0ba1b543b880ddccb9d183d2dfbc481a000a6a`  
		Last Modified: Thu, 14 Dec 2023 19:02:18 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:85d5fd8ebf54ea5ef00ffb868fe7c62b93db9f22f011fe9ac8f25827c9dd020b`  
		Last Modified: Thu, 14 Dec 2023 19:02:18 GMT  
		Size: 3.1 KB (3142 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b855eb90cb84d1ad380aa5ca4f1cf523068f50bd477705c943f2abb7c88f398`  
		Last Modified: Thu, 14 Dec 2023 19:02:21 GMT  
		Size: 90.8 MB (90846922 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8471cf8966ae5cdad2c927b5691ccfc85014f5cd18d5270cdeb9f22baa400323`  
		Last Modified: Thu, 14 Dec 2023 19:02:19 GMT  
		Size: 9.4 KB (9360 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb2b4c05d4f4d8937654cd7d978015b059738f3b79577af064af3f0fe95df3d3`  
		Last Modified: Thu, 14 Dec 2023 19:02:19 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cbe04c68a7f999c81293d04b8d4b23b76f91b47314001298a1233ddbc9797329`  
		Last Modified: Thu, 14 Dec 2023 19:02:19 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:782d53f84335c408e37d21548b67f23ddb9056264666a6c69f50da134d90e790`  
		Last Modified: Thu, 14 Dec 2023 19:02:20 GMT  
		Size: 5.3 KB (5347 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:984960d224d048b5ca666322cafc73be69f901a97d234ab8f267e7cdc40ad77c`  
		Last Modified: Thu, 14 Dec 2023 19:02:20 GMT  
		Size: 188.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:13-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:a7077b1bf5ca2dcd4a52825e45b241f0a4de9fed5bfa2509e87614b7cc4d7e4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 KB (53597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc6f8f803b76e98ee04af7a263fe9b6e585b92032757dea1eef7e2041e428ad4`

```dockerfile
```

-	Layers:
	-	`sha256:d6c03bba353da8933809d0f05d5ae3bedb39d569acf150aa52f16de08df7adc6`  
		Last Modified: Thu, 14 Dec 2023 19:02:17 GMT  
		Size: 53.6 KB (53597 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:13-bullseye` - linux; mips64le

```console
$ docker pull postgres@sha256:c66227a36edcde6e6842d6119099892d656f594d72ea7d0bbc33be8995ed2265
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.2 MB (131172138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bd75ce38f32028d78b2efc264ff4a50f3310d5c32b08575e4866d25f2652d57`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 04:11:02 GMT
ADD file:09d1c4f0f5b78b81f635498ee58f6ab1843bca8a18549ecc39686f1c60b1951d in / 
# Tue, 21 Nov 2023 04:11:06 GMT
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
ENV PG_MAJOR=13
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_VERSION=13.13-1.pgdg110+1
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:a157b7f5d72df9473d33b22278cb42e4e06e22b99ac1864b7b586f36671f15bb`  
		Last Modified: Tue, 21 Nov 2023 04:22:02 GMT  
		Size: 29.6 MB (29636034 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da4f8a086f8ee2ae344567ef2236a8449ccd5d922d507e0b100f752d3d832ad7`  
		Last Modified: Thu, 14 Dec 2023 21:15:23 GMT  
		Size: 1.7 KB (1700 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c9598b461dfba72d8cea81900061cc0a770753537a3d21181d04234fe20baec7`  
		Last Modified: Thu, 14 Dec 2023 21:15:24 GMT  
		Size: 4.2 MB (4196376 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9e8785524799966281da638a9eae6592091c22cf6809bdb30c5317f8ba4d1384`  
		Last Modified: Thu, 14 Dec 2023 21:15:24 GMT  
		Size: 1.4 MB (1359980 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da4c7a02d1de3ff39c2c81809ae917a73c2d379816f761509c4d26c366b6c05e`  
		Last Modified: Thu, 14 Dec 2023 21:15:24 GMT  
		Size: 8.0 MB (8045536 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c7a9a8c8efeb9396dd3d08f9d1597b6e64dff16cddde8a8b3af24fe3382efa3`  
		Last Modified: Thu, 14 Dec 2023 21:15:26 GMT  
		Size: 1.1 MB (1089547 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a62a850af8981d83db60c8b09075c5df562171378fcb56af1094b6831b1d95d`  
		Last Modified: Thu, 14 Dec 2023 21:15:25 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ee6ae6b998a33975bb7023e4ffe338e6c1d8419ece17204023e454e057903ec`  
		Last Modified: Thu, 14 Dec 2023 21:15:26 GMT  
		Size: 3.1 KB (3144 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f75dabfc91470734832ed8e27b897a56bd469acf9afad5d8f0e0d18e93fb9d4b`  
		Last Modified: Fri, 15 Dec 2023 05:17:40 GMT  
		Size: 86.8 MB (86824514 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f2e5d028d56a2049f1058cecefa5741f27952c1ebd51860db21124bc8ea98c84`  
		Last Modified: Fri, 15 Dec 2023 05:17:31 GMT  
		Size: 9.4 KB (9363 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a2b6fe76cfb35aaa9f6349b4ea35d8982482fdd5b13713b32d5bf51f77441323`  
		Last Modified: Fri, 15 Dec 2023 05:17:31 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:01e560aaf6855cb7edd3f44c2cc644de3d87b114a6221389288543ca8c3a8d06`  
		Last Modified: Fri, 15 Dec 2023 05:17:31 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9f5c702d2eafe6930acea2dc602be56ad20b075c7cf24631b09d68e5c77acc7f`  
		Last Modified: Fri, 15 Dec 2023 05:17:32 GMT  
		Size: 5.3 KB (5344 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fffa3d0f8dba9da9dc546bb9da507f9a3b7c13d2ba5ab6d05b872e77400afc39`  
		Last Modified: Fri, 15 Dec 2023 05:17:32 GMT  
		Size: 186.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:13-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:001f642a17ffc9344dddbb64baac9af75ca4d6e745cb6ca1a303ae5dfd55ac56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 KB (53544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d53f38fcc43cbb8d7ea8b941a75573c692f0023de907f0ce9c0856505e9a31a`

```dockerfile
```

-	Layers:
	-	`sha256:4ff8e8fc458ab2ebe7d8d3d6db8855135440ccb78d2c9bcb13db037fc7484039`  
		Last Modified: Fri, 15 Dec 2023 05:17:31 GMT  
		Size: 53.5 KB (53544 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:13-bullseye` - linux; ppc64le

```console
$ docker pull postgres@sha256:054bc2330b47a3b3c5de40d67dd1bc765a2b65903868c320c9f3c5d3e3861e0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.4 MB (145398175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64bfed10e003794f9a7963f6f84003d74453abd4618fcfe26cb3559d460771de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:43 GMT
ADD file:b0d18f2d04821eb50d1faecc1a64916f5c63dd386ae71a3b2cb1d6c4aac6e1c4 in / 
# Tue, 21 Nov 2023 04:24:46 GMT
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
ENV PG_MAJOR=13
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_VERSION=13.13-1.pgdg110+1
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:73f0bb7ed372db4d48b74acd2118a3deda5f5ba3aa65ce0959175af09972c66e`  
		Last Modified: Sat, 09 Dec 2023 04:41:36 GMT  
		Size: 8.0 MB (8045283 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ece094dfff02923d81739960771851eea79691d4742db2fcffa0b3a70e7af537`  
		Last Modified: Sat, 09 Dec 2023 04:41:36 GMT  
		Size: 1.2 MB (1196947 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1959736e1a786070d635066f1f7fe6028923556c8300f9e1324a0a3e9d44cb72`  
		Last Modified: Sat, 09 Dec 2023 04:41:36 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c37575ac82b06eae8d223e3fc598801a6e8897416c399ad1a95ecc5542523cc0`  
		Last Modified: Sat, 09 Dec 2023 04:41:36 GMT  
		Size: 3.1 KB (3144 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6ef46f2c4327f0eeaead976e9f5045f9e79e251ae076556779bb4e6dc367a22d`  
		Last Modified: Sat, 09 Dec 2023 05:09:41 GMT  
		Size: 94.4 MB (94432108 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:accd234c35d43e3f32ac479465000c14df97e649d8d9c19525f83191c9759931`  
		Last Modified: Sat, 09 Dec 2023 05:09:37 GMT  
		Size: 9.4 KB (9360 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:057daa53c32acc53c6ee60644e1eaeabef00e94de5f091163aacfe0941257d87`  
		Last Modified: Sat, 09 Dec 2023 05:09:37 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f44b2bb4ce9025d0e29da146fcf6fc90f06e08fc13f0a8e114be09f7db131b96`  
		Last Modified: Sat, 09 Dec 2023 05:09:37 GMT  
		Size: 172.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eb2872eff63f4ac9d4d81769274111cd0d549328b9c23a5c496c08954364ff6d`  
		Last Modified: Thu, 14 Dec 2023 19:24:42 GMT  
		Size: 5.3 KB (5340 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cffff7c9af3d53fe31a2721163443266e26e171449370f14f7a72476fcfbbdae`  
		Last Modified: Thu, 14 Dec 2023 19:24:42 GMT  
		Size: 186.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:13-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:e8a16fec54fe2a096e2110669fc71bcdd5b7a85420a1c433d5f29d8794408bcd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4987053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4ddb4ef7c3b345b9bda480a7fbbcc22f46672b27fd9f9bbcbc9304d00c408a1`

```dockerfile
```

-	Layers:
	-	`sha256:d5c7cb29933e8afec6ab2539da714fe8972ce1275c715bccc7a31be082824381`  
		Last Modified: Thu, 14 Dec 2023 19:24:42 GMT  
		Size: 4.9 MB (4933319 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:67c7e16bd96501d19fe5a744f006cfdc2197506f7cc9918ff9bd7afb7c890bfd`  
		Last Modified: Thu, 14 Dec 2023 19:24:41 GMT  
		Size: 53.7 KB (53734 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:13-bullseye` - linux; s390x

```console
$ docker pull postgres@sha256:0c4129d010f0400898575e9610c40978e6a3a9454797249146a395bddf7c0b18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.9 MB (139944118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20883af73d818953e598ee48aaade65ddb678d5aba8754d0a61a05a2933f2ce4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 11 Dec 2023 18:58:54 GMT
ADD file:36a070457acddafcd6cdda22a3c41efcbd4e2b1694831eb74c8143520ebf1cf2 in / 
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
ENV PG_MAJOR=13
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_VERSION=13.13-1.pgdg110+1
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:eff2a4367cf88d5103011eba9299da2b4d173b0bde5dc0455020febf72b9b1c4`  
		Last Modified: Tue, 19 Dec 2023 01:48:08 GMT  
		Size: 29.7 MB (29657006 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:369b891674da655514f0ac3404da121a3bec6700dd18315ffb5d91ed3da8be9a`  
		Last Modified: Tue, 19 Dec 2023 15:41:43 GMT  
		Size: 1.7 KB (1688 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:064d665dd7d5609c5bf35ea85d4109596b6642b979180ff8c81bc53c3af9ae12`  
		Last Modified: Tue, 19 Dec 2023 15:41:44 GMT  
		Size: 4.1 MB (4096145 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2e215fdd056d05b8a8144d5a854967c5f8580132804acb57abf6ddac7c22b635`  
		Last Modified: Tue, 19 Dec 2023 15:41:44 GMT  
		Size: 1.4 MB (1438319 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a9abe21501bcb9dbf5ee5b994d9a12fcf5c3460a2c01f3df43da24861e7c70dd`  
		Last Modified: Tue, 19 Dec 2023 15:41:44 GMT  
		Size: 8.1 MB (8099036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c7ba4a580fa6aa550dde22a6c2076af1f668a977d7be7d6053854f434207f058`  
		Last Modified: Tue, 19 Dec 2023 15:41:44 GMT  
		Size: 1.0 MB (1014312 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f365b225a06eaf8e3d4fc6ea1cc6a0c176cd7e7264a8e8f00df8416989c89823`  
		Last Modified: Tue, 19 Dec 2023 15:41:44 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5df5d1b90ef8f9b0489460d1e48b13f72bfee611d29c5cb9d9da167cace54921`  
		Last Modified: Tue, 19 Dec 2023 15:41:45 GMT  
		Size: 3.1 KB (3141 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e3eaa86c96971d0188eca2197e1554f826fa25ee65ce52e7f5ee5a3a4e41f918`  
		Last Modified: Tue, 19 Dec 2023 15:48:59 GMT  
		Size: 95.6 MB (95619176 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:13c7740e2a0641bac30881f9b48837b6a7dfa8c0c1b7684cbdd9e284a2484cdd`  
		Last Modified: Tue, 19 Dec 2023 15:48:56 GMT  
		Size: 9.4 KB (9355 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eabadf42ebb2fdf7f3ea7b07b8e118e3a6eb487b1ca62112e7277787dab35f7d`  
		Last Modified: Tue, 19 Dec 2023 15:48:56 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dbc7df2e21cb871ab6c43e954793a3b06d822ed402547ddfa36a6fc8ddbdfd67`  
		Last Modified: Tue, 19 Dec 2023 15:48:56 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:573b51629927d4081cd4825a5ea1cfa424c6a47c0a24a2e5c0bf80965ebfed9b`  
		Last Modified: Tue, 19 Dec 2023 15:48:57 GMT  
		Size: 5.3 KB (5340 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0cf10f4d082f6c3f6458493cebde51f6ffb9df381e95b1c398c106d5e049b7f1`  
		Last Modified: Tue, 19 Dec 2023 15:48:57 GMT  
		Size: 186.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:13-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:9c383a572093260a80ea75c1ac8486c4bf33f0be9cb1cf9e957da8d8396652fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4978851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d58c475605169aace8d66deee56b7c1d19a90071899071b924e831ba2733dbf`

```dockerfile
```

-	Layers:
	-	`sha256:710b1141419ba6b976210afb93437064827f13b6216a377a670d172328a93895`  
		Last Modified: Tue, 19 Dec 2023 15:48:56 GMT  
		Size: 4.9 MB (4925164 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9c11bb363cd280d7688b3224c4ef52c7189d311b77e82e5d4e38fde42b121298`  
		Last Modified: Tue, 19 Dec 2023 15:48:56 GMT  
		Size: 53.7 KB (53687 bytes)  
		MIME: application/vnd.in-toto+json
