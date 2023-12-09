## `postgres:15-bullseye`

```console
$ docker pull postgres@sha256:7fbb339ebd2f9069135ff9892d1b2b7d22b4215c3a14d43be29e1525996839a2
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
$ docker pull postgres@sha256:34b8af2230642c52c812d1a7164640e71415cadaf8e0af89510a72c665d54178
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138838236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef2d12cec0bf93382594bf7ba36fe6a25d7d8e19df4466920a8f77319b1817ac`
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
ENV PG_MAJOR=15
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PG_VERSION=15.5-1.pgdg110+1
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
	-	`sha256:248e0d69e1bcd5c38fb75e28f4470b54efc910fe5f2c710b45d3ca5ac608c5dc`  
		Last Modified: Fri, 08 Dec 2023 22:12:38 GMT  
		Size: 1.7 KB (1690 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b2bcc2edce61edbbad86b96d5a743bcbd32cbd2d7961425b82e711be717b4413`  
		Last Modified: Fri, 08 Dec 2023 22:12:38 GMT  
		Size: 4.2 MB (4207449 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f69cebe2baada4ead56f487d8efe3e6ecb095628e5f44986e672f92843f11e77`  
		Last Modified: Fri, 08 Dec 2023 22:12:39 GMT  
		Size: 1.5 MB (1472454 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0bfbe76cd7fb6ef7dbbaacb84413e8418a29407ca4a0d85c76338dcb277c3a52`  
		Last Modified: Fri, 08 Dec 2023 22:12:39 GMT  
		Size: 8.0 MB (8045208 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f552543882608ceef7ffe1524ce188b1489b95fd7bbddcaa6431e34d5d7da78c`  
		Last Modified: Fri, 08 Dec 2023 22:12:40 GMT  
		Size: 1.0 MB (1037453 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4fb00ef0c9a0b9e696e56574bb1e9cb1be03f7102d7ef7a99e833213973c39a5`  
		Last Modified: Fri, 08 Dec 2023 22:12:39 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6f943ed996a8abf1b51f57027e14fcd7d58a83bf002b2b360805ec064542d4e7`  
		Last Modified: Fri, 08 Dec 2023 22:12:39 GMT  
		Size: 3.1 KB (3143 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d6c8c612d8ae5e4cd09ffaac177090073a505e6d757b3b6a928690f260d33526`  
		Last Modified: Fri, 08 Dec 2023 22:12:41 GMT  
		Size: 92.6 MB (92638030 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e3d8d9240f3fb4f35236edb96df098c957c0f1539e554fd3f44abcab8d134d6b`  
		Last Modified: Fri, 08 Dec 2023 22:12:40 GMT  
		Size: 9.8 KB (9784 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5f9d9d7a4fb011b089d6f27944b1661e720d7646a4722caa426e470f6bed71c0`  
		Last Modified: Fri, 08 Dec 2023 22:12:41 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7d8032a9d33b7f2577e22cf190ca036317360b4407ae36a0d48f58400da62482`  
		Last Modified: Fri, 08 Dec 2023 22:12:41 GMT  
		Size: 171.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a112dc2517ce4b4995b6a7870e5110781db712888146c9d7fb71d61b80486403`  
		Last Modified: Fri, 08 Dec 2023 22:12:41 GMT  
		Size: 4.8 KB (4786 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:15-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:f1a7974c172975c3a862ffc21cee791f4418e97c344b16e3cea9c3df7c55f6ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5052238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8515e88c8d2a0db6fcffa6febfea31f9e068be84f7b1d556f13af0a12b1bc29`

```dockerfile
```

-	Layers:
	-	`sha256:c930798b87cb966e817644d448664cf36e64a48915c352c028ad84c63f3ba113`  
		Last Modified: Fri, 08 Dec 2023 22:12:38 GMT  
		Size: 5.0 MB (5002081 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:20ab0b27b33bee95bf9f4af372ba79fcf156ac15a81126c9024ae5e127160156`  
		Last Modified: Fri, 08 Dec 2023 22:12:38 GMT  
		Size: 50.2 KB (50157 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:15-bullseye` - linux; arm variant v5

```console
$ docker pull postgres@sha256:cd9a4fd3fcae3aa8837a10c002d6d273d3d91d7a3bd5167d19d81225e05cf760
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.1 MB (132059557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a6ffd5f66d305124e01f92aeb026357bb8773712b6cae4a033aec9d05507385`
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
ENV PG_MAJOR=15
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PG_VERSION=15.5-1.pgdg110+1
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
	-	`sha256:d74ef9892fc15cadc0a7a936f4d2cf44c60804135d2bbbbc2c9177fcfb4a67b6`  
		Last Modified: Sat, 09 Dec 2023 00:47:19 GMT  
		Size: 88.7 MB (88700160 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ac350103f07bb52e53a8e937fc0ba2fd4bec1f0b36a5d2fc82c1e5534de1c76`  
		Last Modified: Sat, 09 Dec 2023 00:47:17 GMT  
		Size: 9.8 KB (9785 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5796f1a4772fb6d9f36a34a2f4075b0e60c6cab953ab76dd21cd425cbcc43530`  
		Last Modified: Sat, 09 Dec 2023 00:47:16 GMT  
		Size: 127.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6a9087a7384a8fafc2125155c8ef7516cd62cf466910c8097992a5f9bec1bc81`  
		Last Modified: Sat, 09 Dec 2023 00:47:17 GMT  
		Size: 171.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d8da18df4e8ef240adbf4e60f94ccce985fd8d31bd27e7adfe737df89f38440a`  
		Last Modified: Sat, 09 Dec 2023 00:47:18 GMT  
		Size: 4.8 KB (4784 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:15-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:efee3bf2d6f8a4e7092f52e6728bbeeaaa4a2e56a14c772979a21387fbc0928f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.0 KB (49959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcdeb579117f16bd7de60da587d1cd1cf1ff5efa4e0fb0b5daea3d88d8c9038d`

```dockerfile
```

-	Layers:
	-	`sha256:6dad7c0e9a930fc6057134bc7382bbe23e09035ea2b5360f2519dcd5a6741c03`  
		Last Modified: Sat, 09 Dec 2023 00:47:16 GMT  
		Size: 50.0 KB (49959 bytes)  
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
$ docker pull postgres@sha256:bdef5ba054ed1ab465221ae026c9123043f58ab65f53cd0667734bc901d2ea0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.9 MB (147929304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:470c35fef128d07913e6679fcd02b0b0c3360574952509799675d8cd3dc3c9cf`
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
ENV PG_MAJOR=15
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PG_VERSION=15.5-1.pgdg110+1
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
	-	`sha256:6cc6cd7538640db49f978f32f06b6e378875ee9bd6eececf3730410afc7895ce`  
		Last Modified: Sat, 09 Dec 2023 04:51:47 GMT  
		Size: 97.0 MB (96963559 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1319d0220f7a88b44ae3cc2d24dfaff517244987af155418da6f7d515a23fdaf`  
		Last Modified: Sat, 09 Dec 2023 04:51:44 GMT  
		Size: 9.8 KB (9780 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5320ec87f41734d9273dce3eb5aef88498d7511b5cd3b12839de0713f8c2af34`  
		Last Modified: Sat, 09 Dec 2023 04:51:44 GMT  
		Size: 127.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:29b3dfc882e3d474ed9b05f3552f0bd3993632b143c66ad111fb390491cddb72`  
		Last Modified: Sat, 09 Dec 2023 04:51:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a27db81cc493792241d93a2e14d619b5b8c81970fe0136eb8c096fbead57a1bf`  
		Last Modified: Sat, 09 Dec 2023 04:51:45 GMT  
		Size: 4.8 KB (4787 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:15-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:4bf7b1814c4d961a19ada0a8646733ba9584639c0c523ba4a41158fb66375f9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5059251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:515d9b34918a5fb91d3baffdeaaaa8501dda8c918d59fd65e2d3f4985b76acf1`

```dockerfile
```

-	Layers:
	-	`sha256:2db34f3c64f3be2015bc7900267d77be9fcbdfaa3c362ad02c694252514f98b9`  
		Last Modified: Sat, 09 Dec 2023 04:51:44 GMT  
		Size: 5.0 MB (5009215 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:68a78d9c3fbfbe4bb3829c874f92873cd6ffa6b9841c31786e0bd37054bbdd16`  
		Last Modified: Sat, 09 Dec 2023 04:51:43 GMT  
		Size: 50.0 KB (50036 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:15-bullseye` - linux; s390x

```console
$ docker pull postgres@sha256:92041481732f61af7391bfb3764b181c0bb76cf03d9d6ed5090f3f18b5995155
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.5 MB (142450262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4088466a9ecaa52e60d88d32634a5e706e6465a6552c8124014cc373d27b6c4`
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
ENV PG_MAJOR=15
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Thu, 07 Dec 2023 22:39:53 GMT
ENV PG_VERSION=15.5-1.pgdg110+1
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
	-	`sha256:fad8ecce80efc016fa3fb0f9a1e4e07f0daa48941d019905f74931e30187103f`  
		Last Modified: Sat, 09 Dec 2023 02:08:16 GMT  
		Size: 98.1 MB (98125638 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b82b1d3e0e028743dcdcc148e8eedf7a566d4e6afdb31dfcbe0aa3db5b29452`  
		Last Modified: Sat, 09 Dec 2023 02:08:14 GMT  
		Size: 9.8 KB (9776 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ed8a740a924a889b43a8a9d5229b3536f85898627b791779281522050d15a16b`  
		Last Modified: Sat, 09 Dec 2023 02:08:14 GMT  
		Size: 127.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c7c21b13eff4d6edf543ba54a3d0147b7fe4ea815622eb542c29bf659d12adcd`  
		Last Modified: Sat, 09 Dec 2023 02:08:14 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c5ba57dc007ff4a2f413c0c63d15b0f001308f0c48b006b4d7a48f010dc88593`  
		Last Modified: Sat, 09 Dec 2023 02:08:15 GMT  
		Size: 4.8 KB (4785 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:15-bullseye` - unknown; unknown

```console
$ docker pull postgres@sha256:92ae1c3ed20b6c26b9ea8bba4d791118d94629f580b682814620102353deba66
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5051050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69f3ae1980e06f274f9525a11f589937ad466d6140092311525dcbacd596c7d9`

```dockerfile
```

-	Layers:
	-	`sha256:59d0f2e420c5923ecda222fce062ad20c1f0d094a2109d20cd352d5b04a7dc90`  
		Last Modified: Sat, 09 Dec 2023 02:08:14 GMT  
		Size: 5.0 MB (5001060 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7f3a70451cc19dee38dd653f0405aa8e2401fefdd3deaf639bc22cdb2975a634`  
		Last Modified: Sat, 09 Dec 2023 02:08:13 GMT  
		Size: 50.0 KB (49990 bytes)  
		MIME: application/vnd.in-toto+json
