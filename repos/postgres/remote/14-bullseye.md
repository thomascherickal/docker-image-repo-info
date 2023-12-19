## `postgres:14-bullseye`

```console
$ docker pull postgres@sha256:a15679f51ab1f89a7f59e2ef2303c2c42f5f01d73b0b52ed4f5d2eca6578a8e6
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

### `postgres:14-bullseye` - linux; amd64

```console
$ docker pull postgres@sha256:0e13e271d98d489e4e2664302c3962ee98399e5176d33cfc11535abb7e9ff229
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.7 MB (137704365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ccccaaa977e85500dbc563e5cc8ef7740b9a03986988d8882507e413fee4096`
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
ENV PG_MAJOR=14
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_VERSION=14.10-1.pgdg110+1
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:cfda79428ddd54935d1d2a4ee65b09c6d361d27adfa63a620b45bedce6b4fc48`  
		Last Modified: Tue, 19 Dec 2023 03:48:29 GMT  
		Size: 1.7 KB (1684 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:de4979af18a390bc0c38816f6458983ebd114a1f7d02ca4f00eeb5846d035fe4`  
		Last Modified: Tue, 19 Dec 2023 03:48:30 GMT  
		Size: 4.2 MB (4207492 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:def6df620c20542a06adc476f7c9696e3bf7ab2a1bdd24c0cdf03abceb1df841`  
		Last Modified: Tue, 19 Dec 2023 03:48:30 GMT  
		Size: 1.5 MB (1472465 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:82700b620cfd5b458f5edb7d0670f72b3d6528ce348a0a5f7796b34e9536802b`  
		Last Modified: Tue, 19 Dec 2023 03:48:30 GMT  
		Size: 8.0 MB (8045275 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1101f5ab8ed217eb7c8d602ef40692b1ad23b666692530817057d6140bca2710`  
		Last Modified: Tue, 19 Dec 2023 03:48:31 GMT  
		Size: 1.0 MB (1037446 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:443cdb0b30fa4cb4dac1cbff69fc86cefcc5e2b8d34d066fca0ed1583d23a0fa`  
		Last Modified: Tue, 19 Dec 2023 03:48:31 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e9219d8c93830f3e8ae98b22da4ea23d7c4d9ce51349495ef17bf5852664e9ba`  
		Last Modified: Tue, 19 Dec 2023 03:48:31 GMT  
		Size: 3.1 KB (3141 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:34064d088ec3323f285a96f171c126d10d903337287d99b0ffc1cd0850d2079e`  
		Last Modified: Tue, 19 Dec 2023 03:48:34 GMT  
		Size: 91.5 MB (91503518 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d114f4f65ea85f660ef892c0b529fd8ecf8156635c0e5bf6ccab675918e5d3e2`  
		Last Modified: Tue, 19 Dec 2023 03:48:32 GMT  
		Size: 9.5 KB (9532 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ca45e28205d3a1085e9605b7bd89f46cb56235d77a11c13aadfbd39a86688e89`  
		Last Modified: Tue, 19 Dec 2023 03:48:32 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:13df1989f70a4e3e3ab0843aac7c1126cdf87650d7111285e31fd1099b016a29`  
		Last Modified: Tue, 19 Dec 2023 03:48:32 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b5f4b909eda5b8def94af101bbaf3b92931b47743b4d271c58b50bfd54b2ce1a`  
		Last Modified: Tue, 19 Dec 2023 03:48:33 GMT  
		Size: 5.3 KB (5340 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dd4805fde52a8b62a5a75519635b567b59adc32502cb63e89c8fa3bcb8297d2b`  
		Last Modified: Tue, 19 Dec 2023 03:48:33 GMT  
		Size: 186.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:14-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:a575faf3691d4e78a85120b0f95584c718879f70dd61aec0c47ddb82ff170bfd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5013089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4476cdfc46df712f6ad2fa1707d4ca433cdeaf6dbc15eb3a18b0ba89d66d9a0`

```dockerfile
```

-	Layers:
	-	`sha256:6434275cf94e7583bde72f19e95e641df6ca35768a32510dd9f66453a5bfa8da`  
		Last Modified: Tue, 19 Dec 2023 03:48:30 GMT  
		Size: 5.0 MB (4959620 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:67191c14366f512e4246caeea5e80552468feb4e82184b1e7aed0e346979790a`  
		Last Modified: Tue, 19 Dec 2023 03:48:30 GMT  
		Size: 53.5 KB (53469 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:14-bullseye` - linux; arm variant v5

```console
$ docker pull postgres@sha256:59fdd16a0f7b923d23c765b2d01fc3a9f564d24643f085430edfdd6b86f71be4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130905493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ba85ae4024f23c4d757dbf6e20722b947b9e84d95f083e0530074e379cd6b13`
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
ENV PG_MAJOR=14
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_VERSION=14.10-1.pgdg110+1
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:20d7cfaef318f52c4db48e92344da25e52c349b706841ce754377dbaf8d0633b`  
		Last Modified: Tue, 19 Dec 2023 17:40:54 GMT  
		Size: 87.5 MB (87545572 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df7092f536407cb2212c66dd1f5f2af0b12dd2fc86b6f1e99347bfaeb30c7f5c`  
		Last Modified: Tue, 19 Dec 2023 17:40:47 GMT  
		Size: 9.5 KB (9536 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3000f7b161c4f1c604d02c23f7d59ab1131f9b6f1824b03f9150d084314c2568`  
		Last Modified: Tue, 19 Dec 2023 17:40:47 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5f8b60fb30cec611bb2f7b0f8042171670038936d4b5017a8e6bb0e1715c3da3`  
		Last Modified: Tue, 19 Dec 2023 17:40:46 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:24f1cd1b4edeb6918de31c1680101d66712c35099b5e9aec7d6929ba15136253`  
		Last Modified: Tue, 19 Dec 2023 17:40:48 GMT  
		Size: 5.3 KB (5343 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c57ff3564efaf50be4272565c98f443e2245038844e262c4a2de378509ed14cf`  
		Last Modified: Tue, 19 Dec 2023 17:40:48 GMT  
		Size: 186.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:14-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:7f237e3423c410e4ff489e684cef9c8e7b67c3681fc8510b160fac1f3df6f1f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 KB (53283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a60912af1bf418edb3c3fe63be27eff82676455142747add21a7e91b8e09142c`

```dockerfile
```

-	Layers:
	-	`sha256:e93409506ecf10160734378bf49f868d763e162ac7cc833859a26bdd12f14703`  
		Last Modified: Tue, 19 Dec 2023 17:40:46 GMT  
		Size: 53.3 KB (53283 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:14-bullseye` - linux; arm variant v7

```console
$ docker pull postgres@sha256:d9b063e918ed806f079388486614168693b31d857375b907a64b3642f9cb9fbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125549692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38e1d7c968063b5e4012ee2acfcaa499c642f44974f7bb6681460ffc87cd0cd7`
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
ENV PG_MAJOR=14
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_VERSION=14.10-1.pgdg110+1
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:e9285e6918a46e8fd50532ee3e605b7ccf03352ba052ad49fdf2c472c4ef16f6`  
		Last Modified: Sat, 09 Dec 2023 07:04:17 GMT  
		Size: 85.0 MB (85047455 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8927b4352f48172e6eef4359cde34a0e2a885d0f73b56ca0263ecd4aa9cd51ac`  
		Last Modified: Sat, 09 Dec 2023 07:04:14 GMT  
		Size: 9.5 KB (9534 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8ccc14d1c4c5a53a6e13eaf2d8f44dac33e19e904f00d88a0448e15b2797f6c9`  
		Last Modified: Sat, 09 Dec 2023 07:04:14 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aa8b4ff947c5bf316ae2b82d4be8dc85c759553ffac2a8f18860c05ba8c16d65`  
		Last Modified: Sat, 09 Dec 2023 07:04:14 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7425f33524c90b83911e731df42da67aa2552c28412341bb2963ff063e8dd15a`  
		Last Modified: Thu, 14 Dec 2023 19:29:35 GMT  
		Size: 5.3 KB (5335 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ec3681deb7d74d6b56745956b1c9b4cca8ac30c7540efdad19df5675933b22b6`  
		Last Modified: Thu, 14 Dec 2023 19:29:35 GMT  
		Size: 186.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:14-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:2c90c5dcf37645bd93b15c124900ed49f92e52a51c95e07a7b14c44142d3acd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5022093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a73933feeef1ed44a387295ba298b5b88bb9777dfb0269f9bba1e8d5fb8c1057`

```dockerfile
```

-	Layers:
	-	`sha256:6e2fd60dc6288a8bb362224742e380828a3b65e8ad7dccbd8bacbf782dc5daa3`  
		Last Modified: Thu, 14 Dec 2023 19:29:35 GMT  
		Size: 5.0 MB (4968603 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8e1a8ce545648afa0e5f2d96c8c0c17385b1ea73798474745c77cdc6e2c4f046`  
		Last Modified: Thu, 14 Dec 2023 19:29:34 GMT  
		Size: 53.5 KB (53490 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:14-bullseye` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:34450f0d5e228455b6ec0ccb20b519b6f0024ef3ea0e39b5a86b757bb0809068
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.8 MB (132799993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a974076c755bb2e8cdc9a57ae09dbcbd78e58346541dfc350b0393942d595ef`
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
ENV PG_MAJOR=14
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_VERSION=14.10-1.pgdg110+1
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:9075267ff24eab47b84b44f9c376dd1d51cacf93f6822df6f67657a125f18183`  
		Last Modified: Thu, 14 Dec 2023 20:24:34 GMT  
		Size: 88.0 MB (88030619 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:088cceee67d8cfb6f5ce3d6ef638f017496767e4046addfd05ce7941ae0027a6`  
		Last Modified: Thu, 14 Dec 2023 20:24:31 GMT  
		Size: 9.5 KB (9528 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c2b3e5bd72dc08f869d8c876a97e26d6d57bfd51e0cf7cc8ea3727c5d8b5160`  
		Last Modified: Thu, 14 Dec 2023 20:24:32 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fbb84d12eb8246d4eccd47f8857324ec5238763c44e625c4a18a4d99c661e3dd`  
		Last Modified: Thu, 14 Dec 2023 20:24:32 GMT  
		Size: 171.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3e59e462cd969ef8d120fa99e21284d3fdbcc655213d810a22a3b69a8f73e99e`  
		Last Modified: Thu, 14 Dec 2023 20:24:33 GMT  
		Size: 5.3 KB (5341 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ce4757117d2e4dc24fcd33e12e79ce7758fe9ce933d25d3ecfdecfaa25f1e2da`  
		Last Modified: Thu, 14 Dec 2023 20:24:33 GMT  
		Size: 185.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:14-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:2931aec716560e2eb15deab39673dd3f310c55e32ce6214047b8446e90fee9e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5018559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27ede4a9770228c24cd80a6dca7c1b5738b5ac4a6a3a17e406095f9889b96541`

```dockerfile
```

-	Layers:
	-	`sha256:eca24d61d72e57a1cdc1a048da87c6499705e0a4c41ae51cc343f6996100e88b`  
		Last Modified: Thu, 14 Dec 2023 20:24:31 GMT  
		Size: 5.0 MB (4965251 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1464ba5c561cb4f1d18ebec78caca849bace6b0e62b40556af5c0c9fd7c234cc`  
		Last Modified: Thu, 14 Dec 2023 20:24:31 GMT  
		Size: 53.3 KB (53308 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:14-bullseye` - linux; 386

```console
$ docker pull postgres@sha256:7b03a3a153c9c1557a36f95cfa5b0040cc4d2489c31eecc5c6c0cf5bfe66ba63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.7 MB (139680878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f80a292554d94243c8078a30f03eaaa81073f7fc017d5d269a0a5c1fa095a4ec`
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
ENV PG_MAJOR=14
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_VERSION=14.10-1.pgdg110+1
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:d0d0e546285e981d92c9530fd2a53105ddfc9d473045cc214afec193c78fa1af`  
		Last Modified: Thu, 14 Dec 2023 19:02:56 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6f377f4ffd5e470e73cc63281e787c6929062c1ed3753e40963b212756e9351a`  
		Last Modified: Thu, 14 Dec 2023 19:02:56 GMT  
		Size: 4.6 MB (4607442 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:010dc4f2311172ce595c3aad656caa9506d64170d9246489edfc62507cf104e3`  
		Last Modified: Thu, 14 Dec 2023 19:02:56 GMT  
		Size: 1.4 MB (1448292 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:647b124702b6a1601b98735b569f9c1a1ff44bfc851f6a16c8ebc1010ee75a01`  
		Last Modified: Thu, 14 Dec 2023 19:02:57 GMT  
		Size: 8.0 MB (8045161 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc4ea4e081d41de5ef9d1b9543d249af0b59efce6b58dc358ac755af8828fab2`  
		Last Modified: Thu, 14 Dec 2023 19:02:57 GMT  
		Size: 1.0 MB (1027970 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f44e80326555848738d3bc50c02063de326e80f4ca17bdbecd8d575154528731`  
		Last Modified: Thu, 14 Dec 2023 18:51:42 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a6b24a0d4e3ae68df4d093db6c66352b55b5a50a65dbbf65b732cc42ac613ab`  
		Last Modified: Thu, 14 Dec 2023 18:51:42 GMT  
		Size: 3.1 KB (3145 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3a16d8f60d8dfbe2caa47cf2e2525214f2c3af58e8090d73c3f658e828737ef8`  
		Last Modified: Thu, 14 Dec 2023 19:03:01 GMT  
		Size: 92.1 MB (92129080 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:588c4f625a37c33420cabaa5a9f7923f7aa4c55e79a42a0a2e8349b3ffde3888`  
		Last Modified: Thu, 14 Dec 2023 19:02:58 GMT  
		Size: 9.5 KB (9529 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ebae684a31272b4e4916f50b6193a3793ae88e96b77adbb981a23db281d4c62b`  
		Last Modified: Thu, 14 Dec 2023 19:02:59 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bd86268cbec3f2a5747c8101703453da16d89e33b0b3e4081c0e85b10a154c76`  
		Last Modified: Thu, 14 Dec 2023 19:02:59 GMT  
		Size: 171.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1148af6c76173108a106768101e5524995a66b5da19c6b66a6d56d7b45e76ca0`  
		Last Modified: Thu, 14 Dec 2023 19:02:59 GMT  
		Size: 5.3 KB (5347 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ff52e6a4b69e5b419b8ecc1ab300e5f23812583530d5c47d065c9919ac3a45c7`  
		Last Modified: Thu, 14 Dec 2023 19:03:00 GMT  
		Size: 188.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:14-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:b3fce2ba84d65d5a1eeaf5b04bb917f22eac7548cb5a80d6ad6f15d5d98c128b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 KB (53213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d443654ca79629d1ed4d3435c32805b565616f143b90d24cb1c844abcb3d035`

```dockerfile
```

-	Layers:
	-	`sha256:218066bea5663f24fd47677cda0bed8354148d66751785f15f64699e2a0ed7ff`  
		Last Modified: Thu, 14 Dec 2023 19:02:56 GMT  
		Size: 53.2 KB (53213 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:14-bullseye` - linux; mips64le

```console
$ docker pull postgres@sha256:5f39e3739341d01aa07e7c2121202decc12a8ac8dc6f0eea1c471b156f5e8b74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.4 MB (132446949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95edc37b8bdbb19a7650062836b9e7ab4e58034b9f77bd75ec00b4489bbd7f9b`
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
ENV PG_MAJOR=14
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_VERSION=14.10-1.pgdg110+1
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:4af99e4f578699cb0f9b18e718bca0b1e2c559bdafff3182478ea46686eabe68`  
		Last Modified: Fri, 15 Dec 2023 03:02:05 GMT  
		Size: 88.1 MB (88099151 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:33b43a3143017c4d9af5276e9012a7ae194db178d90226161b0670122a05d706`  
		Last Modified: Fri, 15 Dec 2023 03:01:56 GMT  
		Size: 9.5 KB (9535 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:14e9cba12f7d9f29c717dd546e9365e3fc6f6290ef7c3ae13bfb244ffcd48ed4`  
		Last Modified: Fri, 15 Dec 2023 03:01:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f49ead7f47e261af4a3bbb682a7fcffe2f4b26a41cab86c958b3f498e6a21fb9`  
		Last Modified: Fri, 15 Dec 2023 03:01:56 GMT  
		Size: 172.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:23cec1d151ea7b01eca0150171e6f0a97d80d9f7fd629caeedeb3c12706faba3`  
		Last Modified: Fri, 15 Dec 2023 03:01:58 GMT  
		Size: 5.3 KB (5344 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:96425fba0433fab89e8c0807a90329fbd959389aef9e9d14bd66e16eebc6a0d6`  
		Last Modified: Fri, 15 Dec 2023 03:01:58 GMT  
		Size: 185.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:14-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:d8cffdc68ae48731b597fa3cb2361f08ffd3e6776041f8a897060ba12b944548
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 KB (53159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5a1cfed9ab9a97dffebc9e18374b3e431e52fa0f032d1a3483b238e5fc47ba6`

```dockerfile
```

-	Layers:
	-	`sha256:e8e24323725e8c311e63b25b93b8b0c8a998e9720910f34f8e33ea506c0e2782`  
		Last Modified: Fri, 15 Dec 2023 03:01:56 GMT  
		Size: 53.2 KB (53159 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:14-bullseye` - linux; ppc64le

```console
$ docker pull postgres@sha256:0e2f5d1807a5361c419a4275f2e235b87da0b8121b73b59b085f0696264a24b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.8 MB (146767827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60af8f51dc0c32795ba04cd4898a5cda5160b13506a1ab51752b195e27f649a8`
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
ENV PG_MAJOR=14
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_VERSION=14.10-1.pgdg110+1
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:1a7141e58e5b544f55f4f781710829b5d0f96acd5ae5c73894bf92b7454194fb`  
		Last Modified: Sat, 09 Dec 2023 05:00:27 GMT  
		Size: 95.8 MB (95801586 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c45104ed46c19a8d3bd5d50ede7ba0e1fcae5cc370174824b4c98b459958981d`  
		Last Modified: Sat, 09 Dec 2023 05:00:23 GMT  
		Size: 9.5 KB (9533 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:956c2359f8afbbbb4d308ca81df99dd690a26924538a99f95446c0b1ff794ae4`  
		Last Modified: Sat, 09 Dec 2023 05:00:24 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc214b7aa0a710969a30f815e57175f0eafa35e3d664ad667dc9bee42ecc58a3`  
		Last Modified: Sat, 09 Dec 2023 05:00:24 GMT  
		Size: 172.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ff6bc3720ec39e7ec93be2267545cb70eff98899cd6bb625c1204e8e83193a92`  
		Last Modified: Thu, 14 Dec 2023 19:22:01 GMT  
		Size: 5.3 KB (5341 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:91de41d0224fc0452fd33ce636002c715a5664b81c74861b9b29c04f6bd9b4bd`  
		Last Modified: Thu, 14 Dec 2023 19:22:01 GMT  
		Size: 186.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:14-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:0be0833b116b20a170254ccafffae9f1d1c1c6811aed436d4e6cc676bb17e028
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5020103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:197d49f0217eb5bc2d21cc6eb34af8df25cc09a3126eecd931a15f043a0fa2b9`

```dockerfile
```

-	Layers:
	-	`sha256:fe479ea50248fa2898fabfdbf556bdd93efb79a702c4164c63ca47b48991de39`  
		Last Modified: Thu, 14 Dec 2023 19:22:01 GMT  
		Size: 5.0 MB (4966754 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a100bd2c6c28b79d918a004c8682c0805cba7c41b1d0cc6ab09c9e19c95b1979`  
		Last Modified: Thu, 14 Dec 2023 19:22:00 GMT  
		Size: 53.3 KB (53349 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:14-bullseye` - linux; s390x

```console
$ docker pull postgres@sha256:adecb9c7e72dc562b2f7ac56bab0551c1004e9b7502abf03090300c93063c61e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.3 MB (141344252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32e02d4a5827746fee3d8759440e443078c61399651e92baaf8e4186e2a489aa`
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
ENV PG_MAJOR=14
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Mon, 11 Dec 2023 18:58:54 GMT
ENV PG_VERSION=14.10-1.pgdg110+1
# Mon, 11 Dec 2023 18:58:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:ad07ac2457bf897db8bf2f5776a415dfa5b81af6670900e371a9dbc7c1595571`  
		Last Modified: Tue, 19 Dec 2023 15:46:41 GMT  
		Size: 97.0 MB (97019132 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dee5fc1b2eee43ddc72156066f254f5c96fa6d10267f835db006fc4170fd72f5`  
		Last Modified: Tue, 19 Dec 2023 15:46:39 GMT  
		Size: 9.5 KB (9532 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b33c4562d88fe2403bb6d5f5f75f08e5e3eac34e716ebcdc5fdcb10391b2e973`  
		Last Modified: Tue, 19 Dec 2023 15:46:39 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:62862b0484cf83d0712bd86fac97a1dd32aa2ef17b2232edb8d92e5ab89bbe8e`  
		Last Modified: Tue, 19 Dec 2023 15:46:39 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f9d0b1741651a356f175b462d10b632e1f1db2e243d6c7995e2289af40da3e4e`  
		Last Modified: Tue, 19 Dec 2023 15:46:40 GMT  
		Size: 5.3 KB (5342 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d60545d3140a8b2e1b4514573ca4b544ac6dfc4dedd622e1f2d8c869b5ab69a3`  
		Last Modified: Tue, 19 Dec 2023 15:46:40 GMT  
		Size: 185.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:14-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:5bdd8b5cd5335f4e803c93ab812b970733e85506e22df1113a37c1fa7296d244
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5011901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5797902c61c6b26ed557a27c19d7cf24206ec069ebe5fd423f725564f6140e4b`

```dockerfile
```

-	Layers:
	-	`sha256:687725ef0f9071e958e6f3a295140c1d83b800cde5eebf9b3a8a82a7facd776e`  
		Last Modified: Tue, 19 Dec 2023 15:46:38 GMT  
		Size: 5.0 MB (4958599 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:6818f91519f8e4667fd561d48778da2086070e9bf2ffbd631451f961b96c3d4c`  
		Last Modified: Tue, 19 Dec 2023 15:46:38 GMT  
		Size: 53.3 KB (53302 bytes)  
		MIME: application/vnd.in-toto+json
