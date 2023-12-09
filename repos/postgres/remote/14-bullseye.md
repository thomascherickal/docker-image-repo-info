## `postgres:14-bullseye`

```console
$ docker pull postgres@sha256:178c1e6796b68424095f9693348f64a6d71185311e98a01fd0cb7ac165fe13db
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
$ docker pull postgres@sha256:c46db363978642ed46cbd2f1043338df7ae38786a291e7e00d2fda72f6950a32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.7 MB (137703266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fe8611ba4e0b2352631df709f2c095b3956b00d34b68986f43f9c62a5ffbe7d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENV GOSU_VERSION=1.16
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	echo 'en_US.UTF-8 UTF-8' >> /etc/locale.gen; 	locale-gen; 	locale -a | grep 'en_US.utf8' # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENV LANG=en_US.utf8
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PG_MAJOR=14
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PG_VERSION=14.10-1.pgdg110+1
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 07 Dec 2023 22:39:53 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 07 Dec 2023 22:39:53 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 22:39:53 GMT
STOPSIGNAL SIGINT
# Thu, 07 Dec 2023 22:39:53 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 07 Dec 2023 22:39:53 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50032b5657dba5015de710a0b23eb7694f0994f4acaaffaedfc6a69749728b2e`  
		Last Modified: Fri, 08 Dec 2023 22:12:39 GMT  
		Size: 1.7 KB (1688 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1ccd4cb1bcec34b21639d4b5c8235392c2a06c805ff1f446c31118421438dd84`  
		Last Modified: Fri, 08 Dec 2023 22:12:39 GMT  
		Size: 4.2 MB (4207465 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:88475882f64fe45f821adefe700e33a6dfb7795665f6193ced533d9af5bb0640`  
		Last Modified: Fri, 08 Dec 2023 22:12:39 GMT  
		Size: 1.5 MB (1472451 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dc4095b51b59a29136a2b979e18867eed41c00d20d5a9363ddd6afef44b45078`  
		Last Modified: Fri, 08 Dec 2023 22:12:39 GMT  
		Size: 8.0 MB (8045287 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d49f21699e16d8476806735871a221d2c4058982e01656662d58af16ac4fd1c9`  
		Last Modified: Fri, 08 Dec 2023 22:12:40 GMT  
		Size: 1.0 MB (1037441 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bb8fb522edb2f4804c49f4be8ff7100af59d5fba5d0d6a2192cf36dba6c1dc0d`  
		Last Modified: Fri, 08 Dec 2023 22:12:40 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d83898b9620b400282ae41a7eb442fba3a4f1e54557fb0c1f40bf31bc5eeb2be`  
		Last Modified: Fri, 08 Dec 2023 22:12:40 GMT  
		Size: 3.1 KB (3144 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aad476cbc41227ab78ab988d37134c133f1e2492744cdf68491ce98339ceab52`  
		Last Modified: Fri, 08 Dec 2023 22:12:41 GMT  
		Size: 91.5 MB (91503238 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ec05a6974b369ee42509d96efac9785bfe312a5be73c33256b1f7aca0069abd6`  
		Last Modified: Fri, 08 Dec 2023 22:12:41 GMT  
		Size: 9.5 KB (9529 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:511fcfca995812d0d7d780ba3993db283babd39dae0c2f12140173384549e846`  
		Last Modified: Fri, 08 Dec 2023 22:12:41 GMT  
		Size: 127.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:48068573d79a52dfe19691e913f636fa907455d1765fdd3936c9e867d96ba8e9`  
		Last Modified: Fri, 08 Dec 2023 22:12:41 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee287363678335b715d2ea245db065fc681363e0bf7e675e5d416c8454a285ad`  
		Last Modified: Fri, 08 Dec 2023 22:12:42 GMT  
		Size: 4.8 KB (4786 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:14-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:10cdc12584640ff4dd7334cd46c8f0996f7c51b93b9f8146a24abcacfda5ea6d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5009786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:396babd33c6bb6e69cfe715477ee3dd0abd8c2817eee5fc63f034d1c1693a107`

```dockerfile
```

-	Layers:
	-	`sha256:7aa21c1ddfb3512fecc2fac5feaba79a77d69fab9f70c025d0ef88b8634fd24a`  
		Last Modified: Fri, 08 Dec 2023 22:12:39 GMT  
		Size: 5.0 MB (4959620 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c9e854ac0f3ca8f505e831ed67f7ffec12744a47d3fddfb4b39e02c999e41076`  
		Last Modified: Fri, 08 Dec 2023 22:12:39 GMT  
		Size: 50.2 KB (50166 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:14-bullseye` - linux; arm variant v5

```console
$ docker pull postgres@sha256:792cc6f81c37588a79c071054f5e1ce470829c06aece02d66fa60f4a74c0b9f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.9 MB (130904821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77763508f51aa8e1f7565fe7e000163ad2768cafd90fd391a62d74c5f468c7fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 05:01:09 GMT
ADD file:f7d1d017cc4e588f213f4536967b8d58c50b8602fb8a10b786856c35a843f31e in / 
# Tue, 21 Nov 2023 05:01:09 GMT
CMD ["bash"]
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENV GOSU_VERSION=1.16
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	echo 'en_US.UTF-8 UTF-8' >> /etc/locale.gen; 	locale-gen; 	locale -a | grep 'en_US.utf8' # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENV LANG=en_US.utf8
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PG_MAJOR=14
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PG_VERSION=14.10-1.pgdg110+1
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 07 Dec 2023 22:39:53 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 07 Dec 2023 22:39:53 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 22:39:53 GMT
STOPSIGNAL SIGINT
# Thu, 07 Dec 2023 22:39:53 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 07 Dec 2023 22:39:53 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:d051266714ac5508b442ebbe5911d353bfacddc64f657eeba14a993cced96358`  
		Last Modified: Tue, 21 Nov 2023 05:04:38 GMT  
		Size: 28.9 MB (28921267 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b3539638f1fab92d51a0d14c2cee8920328a304f5c7633216f54ed0aa88e4731`  
		Last Modified: Sat, 09 Dec 2023 00:14:34 GMT  
		Size: 1.7 KB (1681 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b807d78336669cfc685fc00aff0760d705474f2ebe57214f98bc754d4ba75fb6`  
		Last Modified: Sat, 09 Dec 2023 00:14:35 GMT  
		Size: 3.9 MB (3889269 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:57a6525a1166519faebe70be9e1098704ef475dd60a7be3b63e21b3e6e63fc84`  
		Last Modified: Sat, 09 Dec 2023 00:14:34 GMT  
		Size: 1.4 MB (1449953 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3035251b772a3224764f5364fcbbd519fe38469cc29c1cbad295274c10204ef2`  
		Last Modified: Sat, 09 Dec 2023 00:14:35 GMT  
		Size: 8.0 MB (8045195 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f560faffc18a1397b5b0da7ad53e47c5532e4f256d2bea3b6ed88fb15ed09ef5`  
		Last Modified: Sat, 09 Dec 2023 00:14:36 GMT  
		Size: 1.0 MB (1033904 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e197de1d191dba1e6028d28d426ed0c939239ae88559636d0d465e46cdff1306`  
		Last Modified: Sat, 09 Dec 2023 00:14:35 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69ed1100a18f4ca66fbf732cc710d06e01cfa8e87b9bbdad478c0c9f4e31895f`  
		Last Modified: Sat, 09 Dec 2023 00:14:36 GMT  
		Size: 3.1 KB (3145 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b0f20f840216d03674ae9f2c173a6e0c4e5fff9306576e4dc7f512124b29ef95`  
		Last Modified: Sat, 09 Dec 2023 01:16:49 GMT  
		Size: 87.5 MB (87545671 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:61382ea5933a9f2ec081d7e78c07c89eb6ec2eefc152c11bcee203da211de95a`  
		Last Modified: Sat, 09 Dec 2023 01:16:45 GMT  
		Size: 9.5 KB (9537 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:70dd74bd3c8b3ba5ba7c14c695412175d75a129c375e7fd49aca81bbde58bce4`  
		Last Modified: Sat, 09 Dec 2023 01:16:46 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fd4f502f0f20488f8b26ff378a94850ee4c1bab1b0b344cb3a7691960a0e4c15`  
		Last Modified: Sat, 09 Dec 2023 01:16:46 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:358d9cea02d44c03598622b90e30a71313774b1db1781a9539c52c9c8925d94c`  
		Last Modified: Sat, 09 Dec 2023 01:16:46 GMT  
		Size: 4.8 KB (4785 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:14-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:0aee615483eacec48b0de2b659350f0945e2e782cf8b6d4918d8c1adf461ed90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.0 KB (49968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96d43ef93ffc1d0f2e4f7f91814e034c1a0f4cbfad021f89301916063639fe53`

```dockerfile
```

-	Layers:
	-	`sha256:c6ff48eb8d1a7e7655d332b75460cf1afda4c628b0b80821141691e28d7b62ae`  
		Last Modified: Sat, 09 Dec 2023 01:16:45 GMT  
		Size: 50.0 KB (49968 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:14-bullseye` - linux; arm variant v7

```console
$ docker pull postgres@sha256:1f9fa1ed170a2666a18188ed0059c9c10a025a77c1115733839123e88de80b78
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.5 MB (125548956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59a3d6cd66a8b0eda1fbe4855e07d894c184f562be3f84a3761dddfdeb28e199`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 03:58:04 GMT
ADD file:c4afced274aaa80ab3018b368ed739c1c55e49b41e9637ac44d63e61344fe865 in / 
# Tue, 21 Nov 2023 03:58:04 GMT
CMD ["bash"]
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENV GOSU_VERSION=1.16
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	echo 'en_US.UTF-8 UTF-8' >> /etc/locale.gen; 	locale-gen; 	locale -a | grep 'en_US.utf8' # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENV LANG=en_US.utf8
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PG_MAJOR=14
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PG_VERSION=14.10-1.pgdg110+1
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 07 Dec 2023 22:39:53 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 07 Dec 2023 22:39:53 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 22:39:53 GMT
STOPSIGNAL SIGINT
# Thu, 07 Dec 2023 22:39:53 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 07 Dec 2023 22:39:53 GMT
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
	-	`sha256:ae6c70103bba9579b70d208939bf763c2e174d288783d1a4e840a53fc5a90bd4`  
		Last Modified: Sat, 09 Dec 2023 07:04:15 GMT  
		Size: 4.8 KB (4785 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:14-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:80264368d1712160ffa3a184cad3b75d5ee7be051f7e6680bd1d5840935117d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5018779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d784da66d74caadc210ac5c933aa140c411a1e34839a9a70b3304f426894e58e`

```dockerfile
```

-	Layers:
	-	`sha256:848bd10b463f815dbdcd4c26a5d46382e9d68bbb9c46983a48fcf430d465dae5`  
		Last Modified: Sat, 09 Dec 2023 07:04:14 GMT  
		Size: 5.0 MB (4968603 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8483d1a5f0d84565f2234a66347a2a665f5267c5f873431846b81dff3e9f7c70`  
		Last Modified: Sat, 09 Dec 2023 07:04:13 GMT  
		Size: 50.2 KB (50176 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:14-bullseye` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:2983dc757704d9bc05060439fa1079588b8c7eadac94fabed178638c5d100bf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.8 MB (132799722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:702ecc822af38b1e4d841b2b9694b2ef05027bce8891973180c7174a1e61ffa5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENV GOSU_VERSION=1.16
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	echo 'en_US.UTF-8 UTF-8' >> /etc/locale.gen; 	locale-gen; 	locale -a | grep 'en_US.utf8' # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENV LANG=en_US.utf8
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PG_MAJOR=14
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PG_VERSION=14.10-1.pgdg110+1
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 07 Dec 2023 22:39:53 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 07 Dec 2023 22:39:53 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 22:39:53 GMT
STOPSIGNAL SIGINT
# Thu, 07 Dec 2023 22:39:53 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 07 Dec 2023 22:39:53 GMT
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
	-	`sha256:9e6072b26e353ce98b326ed9576c5d4876a7bd7243aff6c342deeba1552b38fb`  
		Last Modified: Sat, 09 Dec 2023 06:34:28 GMT  
		Size: 8.0 MB (8045205 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cc1422f0626700c1d722e8fc82ff92ca588a95ebd0f6193c8f335efaf7281eb5`  
		Last Modified: Sat, 09 Dec 2023 06:34:28 GMT  
		Size: 1.0 MB (1025908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6156fa106fc8d40f1220f2f23933bf7eecbfc62a16c5e4e9a0e3b5cda8d17af4`  
		Last Modified: Sat, 09 Dec 2023 06:34:28 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2442bf731203a26fe675a291696ba53beaa7f3865c8652ef69eb3330fe903067`  
		Last Modified: Sat, 09 Dec 2023 06:34:28 GMT  
		Size: 3.1 KB (3145 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a011c69b1965f8d39217056646646f32f4d1517009f942134ca8580296543885`  
		Last Modified: Sat, 09 Dec 2023 06:43:24 GMT  
		Size: 88.0 MB (88031213 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7a8cad0f85d2d9fe9ede6d8fbf4825d29c957dda8b6364a341232f458d2ed48e`  
		Last Modified: Sat, 09 Dec 2023 06:43:21 GMT  
		Size: 9.5 KB (9528 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7b29f0e3ff017e1f1a3ccbc23f5a8029acd477ada157b39a584e310f31556226`  
		Last Modified: Sat, 09 Dec 2023 06:43:21 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:22caf781611f9d46787b9cfad2e05dfdc6421fd2e73f6177e191df7929d570c5`  
		Last Modified: Sat, 09 Dec 2023 06:43:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7cda8b9aa60d4cb91fe91d8af19fab64a362e9042c992aa5c9d8c700d8b5471`  
		Last Modified: Sat, 09 Dec 2023 06:43:22 GMT  
		Size: 4.8 KB (4783 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:14-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:983b23d800607752887f3f88eee58a00ab65358f2565722cea60eef6dc448056
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5015256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f9201f59defc1a9aeeeaa1bd3d3673ab2b2725eb1aeca86b390b230f4704abe`

```dockerfile
```

-	Layers:
	-	`sha256:e8daccba47cc222470704ae8e484a7df0ef185b78e2a0515032d4ead43517a50`  
		Last Modified: Sat, 09 Dec 2023 06:43:21 GMT  
		Size: 5.0 MB (4965251 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1467bb9a1e40e1411d97976c7cd801bad8ca6ac490a2afa786c7fa9134716637`  
		Last Modified: Sat, 09 Dec 2023 06:43:21 GMT  
		Size: 50.0 KB (50005 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:14-bullseye` - linux; 386

```console
$ docker pull postgres@sha256:68a8181396927db516b062d2a1d1f398847c609c7c94ee91fb13df0bacd8e17b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.7 MB (139667281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7e900a53459a5392c1d434932267bfce2189c87144ae046a1d95037f91e5558`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 10 Aug 2023 18:35:14 GMT
ADD file:67f223c9c48e525a23fb110e4c105d7128dcac0c10f32c38f98ea84a21d2bd00 in / 
# Thu, 10 Aug 2023 18:35:14 GMT
CMD ["bash"]
# Thu, 10 Aug 2023 18:35:14 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENV GOSU_VERSION=1.16
# Thu, 10 Aug 2023 18:35:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8 # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENV LANG=en_US.utf8
# Thu, 10 Aug 2023 18:35:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PG_MAJOR=14
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PG_VERSION=14.9-1.pgdg110+1
# Thu, 10 Aug 2023 18:35:14 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 10 Aug 2023 18:35:14 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA" # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 10 Aug 2023 18:35:14 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 10 Aug 2023 18:35:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Aug 2023 18:35:14 GMT
STOPSIGNAL SIGINT
# Thu, 10 Aug 2023 18:35:14 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 10 Aug 2023 18:35:14 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:bc6810e8fe9346a3caaff984163b789d12b6964a15a2029e384143ca19fef5ad`  
		Last Modified: Wed, 01 Nov 2023 00:44:14 GMT  
		Size: 32.4 MB (32402692 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df2f34d3d1879059604b84ca41095d534093e5f1d564c1185086ca61ea597e09`  
		Last Modified: Wed, 01 Nov 2023 01:17:49 GMT  
		Size: 1.7 KB (1674 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a3d5050df9eba3c8ae72d70bc4d791230b77835e7ee9114d597cafb55b90c378`  
		Last Modified: Wed, 01 Nov 2023 01:17:50 GMT  
		Size: 4.6 MB (4607411 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:99ac2ef827cc18c98da75368e0fcf2a5bd91e2611668fbadbfe1736f471ab9f4`  
		Last Modified: Wed, 01 Nov 2023 01:17:49 GMT  
		Size: 1.4 MB (1448292 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:61ffb44518182588da9f01eaa1165b5d52a7f900801c24e45d1b8943a014bc6c`  
		Last Modified: Wed, 01 Nov 2023 01:17:50 GMT  
		Size: 8.0 MB (8045152 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7f07239071614ce9b68aac9789be2d851643f3809ebca60c33622b448091b89`  
		Last Modified: Wed, 01 Nov 2023 01:17:51 GMT  
		Size: 1.0 MB (1027957 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:850361112d2dbd5463f55cc99b0c048aee5e34166a04043ca9df1bc65c8008f8`  
		Last Modified: Wed, 01 Nov 2023 01:17:51 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7368f6002ec30136dd0aeaec84f4df3dbd01e0a5e0614fc1a1d8748669eca2e`  
		Last Modified: Wed, 01 Nov 2023 01:17:51 GMT  
		Size: 3.1 KB (3140 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c55de30cac4e487c3c17e344f6e346d08ed0b044dd228adc157c5b8d67e3bc54`  
		Last Modified: Wed, 01 Nov 2023 01:17:55 GMT  
		Size: 92.1 MB (92116227 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c5cb6efcdc7d94a1b08d36ed88293584e636e6920b81fb2534f721f495503447`  
		Last Modified: Wed, 01 Nov 2023 01:17:52 GMT  
		Size: 9.5 KB (9535 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:939ff3dfa98a44e0d7883b8ebe23101c9d5e290a85fc8b14204d1907ab130c74`  
		Last Modified: Wed, 01 Nov 2023 01:17:52 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:66e67758df867579e9cb9f7750c99745ecc2010c91fa3c1d369ee0126a0625f3`  
		Last Modified: Wed, 01 Nov 2023 01:17:52 GMT  
		Size: 169.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:057fd3636848344376f73142d0296dd77b7d5856af66e91e5f1e0fc0e95c6134`  
		Last Modified: Wed, 01 Nov 2023 01:17:53 GMT  
		Size: 4.8 KB (4788 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:14-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:0d72b6e5829c3dd34ba112d25e6b879b8b756f4a2100e181e4e4d3fc511075ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.8 KB (49770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b86e2c724dccda5626b541bfdb945752d772d3f97630dbb61a088ac4ec084ce3`

```dockerfile
```

-	Layers:
	-	`sha256:c9cf8cc6f58eca7c614dadf199d0ad0466e98b055e635af80605d62d698a44e0`  
		Last Modified: Wed, 01 Nov 2023 01:17:49 GMT  
		Size: 49.8 KB (49770 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:14-bullseye` - linux; mips64le

```console
$ docker pull postgres@sha256:a690dfee3e1f310ed67b73788b64d034d1e3cc3349e209cd5b8fb785956f5878
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.4 MB (132446955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a26c4308fc473724278c18f976e8d3738681e5a2f7d6f702b3aab0427d08873`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 04:11:02 GMT
ADD file:09d1c4f0f5b78b81f635498ee58f6ab1843bca8a18549ecc39686f1c60b1951d in / 
# Tue, 21 Nov 2023 04:11:06 GMT
CMD ["bash"]
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENV GOSU_VERSION=1.16
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	echo 'en_US.UTF-8 UTF-8' >> /etc/locale.gen; 	locale-gen; 	locale -a | grep 'en_US.utf8' # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENV LANG=en_US.utf8
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PG_MAJOR=14
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PG_VERSION=14.10-1.pgdg110+1
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 07 Dec 2023 22:39:53 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 07 Dec 2023 22:39:53 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 22:39:53 GMT
STOPSIGNAL SIGINT
# Thu, 07 Dec 2023 22:39:53 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 07 Dec 2023 22:39:53 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:a157b7f5d72df9473d33b22278cb42e4e06e22b99ac1864b7b586f36671f15bb`  
		Last Modified: Tue, 21 Nov 2023 04:22:02 GMT  
		Size: 29.6 MB (29636034 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2f200f5675741a01979a21c59687bdf670196b64f5501d814775250da5e3e851`  
		Last Modified: Sat, 09 Dec 2023 08:06:42 GMT  
		Size: 1.7 KB (1691 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a740b666e6e2cd43021e5f1ed6d6f2e6734ef1868ba1978f0a6f8f3812bfbb7f`  
		Last Modified: Sat, 09 Dec 2023 08:06:43 GMT  
		Size: 4.2 MB (4196371 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6f89e303a5c4dbc07c22346b687d7932c1b557eb314f45abc6f51ae37b1048c4`  
		Last Modified: Sat, 09 Dec 2023 08:06:43 GMT  
		Size: 1.4 MB (1360016 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0eff5bc0f71093b3e64d30bfa8e0e0130ac754c41c03241ff2b41ca0d5082365`  
		Last Modified: Sat, 09 Dec 2023 08:06:43 GMT  
		Size: 8.0 MB (8045516 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c7f4d80e1fc8ced29ba7c1a472607498a6ca12c670e1c79cdef5b5247c809c28`  
		Last Modified: Sat, 09 Dec 2023 08:06:43 GMT  
		Size: 1.1 MB (1089543 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1cc8f130ec200be7dd83fdbbc9a82bc82737222859bc69c853dadd1a16622f13`  
		Last Modified: Sat, 09 Dec 2023 08:06:44 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b20231e1f450db754f60eacee6b2462ab1180eeb3ae009891ab27c17816b282e`  
		Last Modified: Sat, 09 Dec 2023 08:06:44 GMT  
		Size: 3.1 KB (3143 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6c16e41b77e57efe2b1cbc86f6cf9d82e795118a0cfad9785625b63027b98608`  
		Last Modified: Sat, 09 Dec 2023 12:33:00 GMT  
		Size: 88.1 MB (88099907 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:de31e0da47eb130d1b89f40b68da740fa235fcb51d7b117bc3bcfd7aac494c6e`  
		Last Modified: Sat, 09 Dec 2023 12:32:52 GMT  
		Size: 9.5 KB (9536 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5e10f14cfb9ad2d1fece8223205be2c7f547345993b2e2b7eacb9d5b56214f12`  
		Last Modified: Sat, 09 Dec 2023 12:32:51 GMT  
		Size: 127.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cf271d62c7a8754b621b1264ff673dae8ebcd181d7f6bf5e8230038b7fb30bbf`  
		Last Modified: Sat, 09 Dec 2023 12:32:52 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8cce0a2343ec29f3f4815027f0dca5412d0131c12524cb03a804462ec30c0e6`  
		Last Modified: Sat, 09 Dec 2023 12:32:53 GMT  
		Size: 4.8 KB (4785 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:14-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:a87cc5b59d62ab914b2ecb0dad04d555495b8df906b243765dab485d88d4a844
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 KB (49854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:599cfe569b58b2acf2d27f90c014927d3354e916350210784c92b38cb86c48fc`

```dockerfile
```

-	Layers:
	-	`sha256:ee2a68a69af8d336b020989bc61efb1b24d04f82b42acb33e5815c348ef8be0a`  
		Last Modified: Sat, 09 Dec 2023 12:32:51 GMT  
		Size: 49.9 KB (49854 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:14-bullseye` - linux; ppc64le

```console
$ docker pull postgres@sha256:b0cabf61ab42eacfc8abb40a4a5cecf4e10f8e392be4263c34e1b5347dff9cc5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.8 MB (146767085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdb93d14ef0bf1b08435475d5366869f6829b078333ce9010a62d72564fb6a3d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:43 GMT
ADD file:b0d18f2d04821eb50d1faecc1a64916f5c63dd386ae71a3b2cb1d6c4aac6e1c4 in / 
# Tue, 21 Nov 2023 04:24:46 GMT
CMD ["bash"]
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENV GOSU_VERSION=1.16
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	echo 'en_US.UTF-8 UTF-8' >> /etc/locale.gen; 	locale-gen; 	locale -a | grep 'en_US.utf8' # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENV LANG=en_US.utf8
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PG_MAJOR=14
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PG_VERSION=14.10-1.pgdg110+1
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 07 Dec 2023 22:39:53 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 07 Dec 2023 22:39:53 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 22:39:53 GMT
STOPSIGNAL SIGINT
# Thu, 07 Dec 2023 22:39:53 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 07 Dec 2023 22:39:53 GMT
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
	-	`sha256:f2956af0e2f80964cb94fad1113da8feff801aba2630e605c46c980d7ac1e958`  
		Last Modified: Sat, 09 Dec 2023 05:00:25 GMT  
		Size: 4.8 KB (4785 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:14-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:5d81abfcd3752a92836985131163088fddeee25a21be8d2b3b6a313a4a6ae509
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5016799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bfeb6860c00a97afdb1f6d98cf2bab8142275fb4a869a3f92a37f93f387c505`

```dockerfile
```

-	Layers:
	-	`sha256:1a495edecb3c158329f8a9977d3106fd90723378d443a5db42a740da9146f255`  
		Last Modified: Sat, 09 Dec 2023 05:00:24 GMT  
		Size: 5.0 MB (4966754 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4379e663c2137def0581d7636deef6b5b247e81635b6736ecea690e2f837a120`  
		Last Modified: Sat, 09 Dec 2023 05:00:23 GMT  
		Size: 50.0 KB (50045 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:14-bullseye` - linux; s390x

```console
$ docker pull postgres@sha256:51ddb9c23a68dd291e8f3d1c9ac0253f493cd1d104cffea5317555262998ba85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.3 MB (141343763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50c9b4df789cb23bbfc0f81840934cfe36d7c1c691b4989778add290ebf28e99`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 05:05:18 GMT
ADD file:a545f27075704ce13e33e539170d3f47007424d2cc2bea5aecfd2608a5194151 in / 
# Tue, 21 Nov 2023 05:05:22 GMT
CMD ["bash"]
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENV GOSU_VERSION=1.16
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	echo 'en_US.UTF-8 UTF-8' >> /etc/locale.gen; 	locale-gen; 	locale -a | grep 'en_US.utf8' # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENV LANG=en_US.utf8
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN mkdir /docker-entrypoint-initdb.d # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PG_MAJOR=14
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PG_VERSION=14.10-1.pgdg110+1
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 3777 /var/run/postgresql # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 07 Dec 2023 22:39:53 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 1777 "$PGDATA" # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 07 Dec 2023 22:39:53 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 07 Dec 2023 22:39:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 22:39:53 GMT
STOPSIGNAL SIGINT
# Thu, 07 Dec 2023 22:39:53 GMT
EXPOSE map[5432/tcp:{}]
# Thu, 07 Dec 2023 22:39:53 GMT
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
	-	`sha256:6732892b01a43f904783c199df2bae5ab175a930b87fe3f41c21d3ef3a05f6ae`  
		Last Modified: Sat, 09 Dec 2023 02:00:44 GMT  
		Size: 8.1 MB (8099051 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f77a5e4d5d326f748adafe6031eb23a9f8a24dfd082cd27a78725c140d7f70a3`  
		Last Modified: Sat, 09 Dec 2023 02:00:44 GMT  
		Size: 1.0 MB (1014354 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:666a1f7d7b8f503067398637105430ec484972cf2da519b16278da55e126ebf4`  
		Last Modified: Sat, 09 Dec 2023 02:00:44 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c50e5c34c42386c7e2b49988d81f9464ff0322939e02adf58b8b6b54c1eb452`  
		Last Modified: Sat, 09 Dec 2023 02:00:44 GMT  
		Size: 3.1 KB (3142 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:99982fc6b7ebe618b3ab5ffde71b55c0db3356554c4cdfa8c639824d8aee1563`  
		Last Modified: Sat, 09 Dec 2023 02:19:04 GMT  
		Size: 97.0 MB (97019384 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dff16c61fbf17f0a79f96e480a6fd3897dd84cdfd6c8866316da6920ff400425`  
		Last Modified: Sat, 09 Dec 2023 02:19:02 GMT  
		Size: 9.5 KB (9531 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:37f137c67f40ce25ff5686a6317267d2271b48669e463d6688d7d0a6cbb32826`  
		Last Modified: Sat, 09 Dec 2023 02:19:02 GMT  
		Size: 127.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:510719173db9d3213c7d30f8b3e15402ed06457d4c771fb8a08c699e64c4d5b8`  
		Last Modified: Sat, 09 Dec 2023 02:19:03 GMT  
		Size: 171.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:280a0b399dc9fcf699d30a018dbfd1a931ae76d28264bbf6dd4b9ac103021bf1`  
		Last Modified: Sat, 09 Dec 2023 02:19:04 GMT  
		Size: 4.8 KB (4784 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:14-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:5a0d14f5a7811d678a2e04a6511a56121e0bb55534bf0c6d089c492d36cf294b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5008597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa1b5d2a4fa2e76c173c1b0bba80af7bda850ca04eb48e8bc441d36015952f4b`

```dockerfile
```

-	Layers:
	-	`sha256:3eafa98c896d88b9837bc44cacd650ef01272d6b14276960ad122574ee48361c`  
		Last Modified: Sat, 09 Dec 2023 02:19:03 GMT  
		Size: 5.0 MB (4958599 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:919d582ef8e3872ae7598c2642e01abdecc91e0ad27d039645c8528a920dcd01`  
		Last Modified: Sat, 09 Dec 2023 02:19:02 GMT  
		Size: 50.0 KB (49998 bytes)  
		MIME: application/vnd.in-toto+json
