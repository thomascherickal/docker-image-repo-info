## `postgres:15-bookworm`

```console
$ docker pull postgres@sha256:2918cd09f56b6f864994313adf7fd7b370e995f47e01959e35215de84434ad0c
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

### `postgres:15-bookworm` - linux; amd64

```console
$ docker pull postgres@sha256:6cb3b06966a9f3ec18680d5362d0f7ba8bab748bdb4380fcf400afdf69086830
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.8 MB (150848065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16e9af8ba3fae07e3ce4c1ce35ec2d15581f9d31870230b1bb60b196935ff49a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
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
ENV PG_VERSION=15.5-1.pgdg120+1
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:90fbd05a6c64c308dbaca6fc1e43864575e07f853c3eab179f258b9800991a95`  
		Last Modified: Fri, 08 Dec 2023 22:12:40 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c107a494d63c013517c1eb0470fad84601fe596e9aa3981fe63c2831a2c670a2`  
		Last Modified: Fri, 08 Dec 2023 22:12:45 GMT  
		Size: 4.4 MB (4422621 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b1f93317ded148aa5d59afec862b9ed159e082c8cfbe656ccdd62d8245d1118`  
		Last Modified: Fri, 08 Dec 2023 22:12:44 GMT  
		Size: 1.4 MB (1448547 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b4e0db51dfb9dd299216bc35d221a3b84efed2d8cc0990a459dc455bbe9a47de`  
		Last Modified: Fri, 08 Dec 2023 22:12:45 GMT  
		Size: 8.1 MB (8067864 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ffcd2018dc44e9a0d458879102bfb9e68cebe98ddaf3d085a585aa0beb16bcd8`  
		Last Modified: Fri, 08 Dec 2023 22:12:45 GMT  
		Size: 1.2 MB (1195084 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bb8fb522edb2f4804c49f4be8ff7100af59d5fba5d0d6a2192cf36dba6c1dc0d`  
		Last Modified: Fri, 08 Dec 2023 22:12:40 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d83898b9620b400282ae41a7eb442fba3a4f1e54557fb0c1f40bf31bc5eeb2be`  
		Last Modified: Fri, 08 Dec 2023 22:12:40 GMT  
		Size: 3.1 KB (3144 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7c74348418e9c86f7509f120115e37df99d8a404de386a9f10ebf6335336b2ff`  
		Last Modified: Fri, 08 Dec 2023 22:12:49 GMT  
		Size: 106.5 MB (106544746 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a56b24ebf9935e0b8dc17e561955e06201669cae82275dd6ab3afe0605275fe8`  
		Last Modified: Fri, 08 Dec 2023 22:12:46 GMT  
		Size: 9.8 KB (9782 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aa48b46b9cdbaf7c0ed6c9153ac9cca4c008743382ba8aa4ef4e7ff07fd2ca39`  
		Last Modified: Fri, 08 Dec 2023 22:12:43 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:be71efae0c173879a0c511dfa62171cbad2b93ac245d0c0bf42cf1810e82d221`  
		Last Modified: Fri, 08 Dec 2023 22:12:43 GMT  
		Size: 171.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:22902c020f47357a4ccbb59fecd3aaca3c98a33994a506b6712609c4e0b7b864`  
		Last Modified: Fri, 08 Dec 2023 22:12:46 GMT  
		Size: 4.8 KB (4786 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:15-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:8d0a94bdf28cebb6bf3c7e2968924fd1a3c4e6bd01bbb0e93ef1ec417ff2dd6e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4940961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f19eb0b5a469fcee41b630b2f86b2deac5d71dffbe4d854b59d12210e9de958`

```dockerfile
```

-	Layers:
	-	`sha256:a7f5b54e246845a5c290d5813b7d62f96fb979a4e19fae546fca995eee98d6f4`  
		Last Modified: Fri, 08 Dec 2023 22:12:45 GMT  
		Size: 4.9 MB (4890207 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:25dbb523837fe899942a1609b292b450a9ec13328943e19bdb90057c146140a1`  
		Last Modified: Fri, 08 Dec 2023 22:12:44 GMT  
		Size: 50.8 KB (50754 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:15-bookworm` - linux; arm variant v5

```console
$ docker pull postgres@sha256:9f090cdc49431810f1e5b1cf53e11df143a2086631749759aeda13c994b1550b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.6 MB (143587836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cca49fcb6282d0bed23b809b4eb9af2d4998ae68307d4008e0c01fe21a5187b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:51 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Tue, 21 Nov 2023 05:00:52 GMT
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
ENV PG_VERSION=15.5-1.pgdg120+1
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:749be5ef15818a6d009a4eeb567fd6b3341f668dbd0778f344ba9ac1c3434090`  
		Last Modified: Fri, 08 Dec 2023 23:49:50 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:16cfc5a4bde01ce112826bedc5094d77282fddbd8697063c504bb035e5a7ffe1`  
		Last Modified: Fri, 08 Dec 2023 23:49:50 GMT  
		Size: 4.0 MB (4040489 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c818e7cc03f89d1edf7b7dcac145dffa73298e87bc608f0d0ced470844da8c2b`  
		Last Modified: Fri, 08 Dec 2023 23:49:50 GMT  
		Size: 1.4 MB (1426052 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bacdb34348a9747d38a6db8c6fc635b82fcd09258f03a97cc16f830544eb4c1c`  
		Last Modified: Fri, 08 Dec 2023 23:49:51 GMT  
		Size: 8.1 MB (8067982 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dd985847be75937a28a261fb141a6b83f7a3a2869d7cb9802a97e494b1206bf2`  
		Last Modified: Fri, 08 Dec 2023 23:49:51 GMT  
		Size: 1.2 MB (1193963 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e0ede3e8380dbd67add822320acc1014151fd90bd8285565e2e4b17b21adbab`  
		Last Modified: Fri, 08 Dec 2023 23:49:52 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69cc4363f64d85c4f58f7ab91a533f7153e4b8a7707c5ce1495298d29bb76468`  
		Last Modified: Fri, 08 Dec 2023 23:49:52 GMT  
		Size: 3.1 KB (3144 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2854998af74d48503b92498a2a5afb2f067fe2d3c251474965213c6088c35a5e`  
		Last Modified: Sat, 09 Dec 2023 00:32:53 GMT  
		Size: 101.9 MB (101917899 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8cd41984809f6b834ceb3e164b9783ff3899056150d5393845e2c1d3246c462b`  
		Last Modified: Sat, 09 Dec 2023 00:32:49 GMT  
		Size: 9.8 KB (9785 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:27107e2d671978bae422d0dcb8f382f50da67d6505865a8a7014f6b84ab3ad2e`  
		Last Modified: Sat, 09 Dec 2023 00:32:49 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4d56bace631b8a4e313f3027bfe434e3c4e12ecbc00c29d9b0ff8c2750d0da6f`  
		Last Modified: Sat, 09 Dec 2023 00:32:49 GMT  
		Size: 171.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bee7a035acf6c1fda37a4ece9158aeee5b72398ad62adb359ccb31b3832c0a8b`  
		Last Modified: Sat, 09 Dec 2023 00:32:50 GMT  
		Size: 4.8 KB (4787 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:15-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:941576d2d2cb6a20fa1536b03d5698645af84b4840d2742a481a0b4fdb07a615
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.6 KB (50572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b5907aed121a37da0ec6e3f5fb801b7315fa4a7cbc07dad33bf2958d58c9ceb`

```dockerfile
```

-	Layers:
	-	`sha256:ae9b0240d1d05a4540c7eaa01c5b8a33a1e6f1b47a06b48e4570e860b2a0d3d2`  
		Last Modified: Sat, 09 Dec 2023 00:32:48 GMT  
		Size: 50.6 KB (50572 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:15-bookworm` - linux; arm variant v7

```console
$ docker pull postgres@sha256:82467f3f72c7af96b429771cbf778545971959ffc95460e1e7e852b1aa2242e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.4 MB (138430840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c94be80dbf94b1115c69aa4f6c2e81283fb0d4f8526c00841bc29dabeabdf2ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:43 GMT
ADD file:b693944382a95fa47622fde77eb98f0cdeafa40261e7334bd355e00f650b6632 in / 
# Tue, 21 Nov 2023 03:57:43 GMT
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
ENV PG_VERSION=15.5-1.pgdg120+1
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:e223d57922c86fb53eee7a89d66e8928409562d66b276b2a7fb121c997054dc0`  
		Last Modified: Wed, 22 Nov 2023 01:33:10 GMT  
		Size: 8.1 MB (8067889 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:326ab74a3f8493265ec860fd62d15f34dbf491c787bbc030c214ee3e35cbdfc7`  
		Last Modified: Wed, 22 Nov 2023 01:33:10 GMT  
		Size: 1.1 MB (1065924 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:85273e10b04abf86fdd4cfd58839d0457c8a52b94927a0085fda8527a7eb8eba`  
		Last Modified: Wed, 22 Nov 2023 01:33:10 GMT  
		Size: 114.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d759abb828279091b19672436eedd188e080b8f24632d0f84c9a990f293319a`  
		Last Modified: Wed, 22 Nov 2023 01:33:10 GMT  
		Size: 3.1 KB (3143 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6b3116ca7d560e3843b505eeb6305e210889ca6e89068acc19ec3caf065093e7`  
		Last Modified: Wed, 22 Nov 2023 02:04:13 GMT  
		Size: 99.5 MB (99467625 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19ece263c3b82b0f03a1cb9f82db0f96ef988fb719d8c0cede7024db3ebfd130`  
		Last Modified: Wed, 22 Nov 2023 02:04:10 GMT  
		Size: 9.8 KB (9786 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c454084698dd5fd585494a5c791e5186b151d41b4d1360f45a35150cbf7b4d64`  
		Last Modified: Fri, 01 Dec 2023 22:32:24 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b533863cb21e2b08f274b3019eeec5249c5f06fd581696f9c68188759aa04a60`  
		Last Modified: Fri, 01 Dec 2023 22:32:24 GMT  
		Size: 176.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:99f383eccf895de3a5518791ccc2ca650b1e63006964ea9d885d47b9e50c3d93`  
		Last Modified: Fri, 01 Dec 2023 22:32:24 GMT  
		Size: 4.8 KB (4779 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:15-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:6fdaac49c4dd27ff97bbcf96cae67944eda0b878dd145e6b3dcc101b031cfb4b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4951205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7aed84dd0f6dc946c9cf803aa81b56be9e55239fcbe922e30508adf423c2cbaf`

```dockerfile
```

-	Layers:
	-	`sha256:5f4537068bec6c786ecdeaa42171b3faa943bee12a63038adb95a601d322cf27`  
		Last Modified: Fri, 01 Dec 2023 22:32:24 GMT  
		Size: 4.9 MB (4900552 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c8cbd80e27c2a5a0b30913fe34010ac7f15ab2f71dfb6bdee7a6af2f04edd628`  
		Last Modified: Fri, 01 Dec 2023 22:32:23 GMT  
		Size: 50.7 KB (50653 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:15-bookworm` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:4164cf6c1755caa0c3bba8b9436618837fdac9aef50cace7c25e5c3fb5ed7914
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.0 MB (149039851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abba7927bfee206642fce490af39d2f257186fee95d0a8bace961eefcf39c0b2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
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
ENV PG_VERSION=15.5-1.pgdg120+1
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1cceff339129572dbb692e7aa1ed4221a7ffc75cf59151c83b04ff8dc59e069c`  
		Last Modified: Wed, 22 Nov 2023 11:51:51 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:205f857684f5cbc32a359894eac031b9e3228e9e600f87a016db9921226bf202`  
		Last Modified: Wed, 22 Nov 2023 11:51:51 GMT  
		Size: 4.4 MB (4383844 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0cba82cb23b34b9baa62d2db06ae15164a9877c18aa858187007c9aecdc11f25`  
		Last Modified: Wed, 22 Nov 2023 11:51:51 GMT  
		Size: 1.4 MB (1380715 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:98bdcf4e4d625179b6cdca8bb63f4f22cd4a04becdd488d4e41a6c7b51bd494b`  
		Last Modified: Wed, 22 Nov 2023 11:51:51 GMT  
		Size: 8.1 MB (8067935 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b3ce7bf87298edf9a9cebc92c39207f310cf48d21dd2388090285ae757661b73`  
		Last Modified: Wed, 22 Nov 2023 11:51:52 GMT  
		Size: 1.1 MB (1107732 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:53521cca1206cc645107b20f50b6613f0f282e10b9ed7d885ebdbe839004eeb1`  
		Last Modified: Wed, 22 Nov 2023 11:51:52 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:58d4091d2a8b6ee3356c1da8b550408ef9e6c726ab9e69d2f82f867407cfa1b2`  
		Last Modified: Wed, 22 Nov 2023 11:51:52 GMT  
		Size: 3.1 KB (3145 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:47a313de8a1c50ce51387358bbc9a79c3812d467c668329c46d6b3dd9acbced1`  
		Last Modified: Wed, 22 Nov 2023 11:53:56 GMT  
		Size: 104.9 MB (104901061 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bda5115d9194c753701d7645485b5df1bcdb83c163ed83cc26dbd62011e47240`  
		Last Modified: Wed, 22 Nov 2023 11:53:52 GMT  
		Size: 9.8 KB (9779 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a218c73ab1f3f00af8f5787205313daafe92df465904da736d07d7af9e7e157f`  
		Last Modified: Fri, 01 Dec 2023 22:29:20 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:29262dedcc99ecf91f179a0bf645021a141dfa009041f2a40b48f9ed81466879`  
		Last Modified: Fri, 01 Dec 2023 22:29:20 GMT  
		Size: 175.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ffe0db4f9729b54129f2b1d5879888c86ba3036fc5ebebdbcfa16a7736976e71`  
		Last Modified: Fri, 01 Dec 2023 22:29:21 GMT  
		Size: 4.8 KB (4780 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:15-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:0d6c318639b5e72eece21aceac00336b249f8feb23a0bc129b9291209d4e2caf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4946303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6434f3199806a0ee74cd4f1d52f41110337ed2a48565172f7f9675da8d98b918`

```dockerfile
```

-	Layers:
	-	`sha256:f2167bd1e19ca12f3861c2bddc1d510abb2203ce850b20a44f25945fce0eb39e`  
		Last Modified: Fri, 01 Dec 2023 22:29:20 GMT  
		Size: 4.9 MB (4895834 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:fbce103a9929025a8e9a3d6c64d8c4bd953afaf2a9971750252f0b2368fb12e7`  
		Last Modified: Fri, 01 Dec 2023 22:29:20 GMT  
		Size: 50.5 KB (50469 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:15-bookworm` - linux; 386

```console
$ docker pull postgres@sha256:c325fffa9c49f08bce9bfc3c9fda171e4bff15092d1f4ec8cf977b44dd5ba8f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.7 MB (155665049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14f739ab9be3eef3f5468b435dc826b1336fbb41eb818d12115fd1b80314737b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 14 Sep 2023 18:02:56 GMT
ADD file:0c94521fdd9c0a4fdeeb9aad23e68cd053fba0dcd7c3af550aefa79377816e31 in / 
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
ENV PG_VERSION=15.4-2.pgdg120+1
# Thu, 14 Sep 2023 18:02:56 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:98bdfce9af831c2a0d0bfcca812d0039cd1666986550f552b4b4c625bd5aa31c`  
		Last Modified: Wed, 01 Nov 2023 00:43:26 GMT  
		Size: 30.2 MB (30164042 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3b7b26f0bf3f50ed8910541a15f4789297f42b5ccb39ae9d55d268822abd6836`  
		Last Modified: Wed, 01 Nov 2023 01:18:19 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fe61326bd39802a069c5b859f6f2fbe6afb5bffea50931e39ba801baeb515936`  
		Last Modified: Wed, 01 Nov 2023 01:18:20 GMT  
		Size: 4.8 MB (4844483 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7c7ee73442cfae0bfa6b701e7a87c9b61905cd305734c2b1ec339181e70c858b`  
		Last Modified: Wed, 01 Nov 2023 01:18:19 GMT  
		Size: 1.4 MB (1424517 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f27d52cf56c1b73d719679b97c7049de0a4248844ed0829210114660c8fc6a71`  
		Last Modified: Wed, 01 Nov 2023 01:18:20 GMT  
		Size: 8.1 MB (8067932 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:672c476995e895d65445f5074f4df21d7f6a776d676937166813257ba54ae592`  
		Last Modified: Wed, 01 Nov 2023 01:18:20 GMT  
		Size: 1.1 MB (1136174 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:38f6a0eb82a0b789eacf11421bf98934782d2067b3d03ba774ddeeb2c21dc867`  
		Last Modified: Wed, 01 Nov 2023 01:18:20 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b256bb2fe43e3dfb5cac055202b39c60394feb9ddb9dadb00e8c96a448811adf`  
		Last Modified: Wed, 01 Nov 2023 01:18:21 GMT  
		Size: 3.1 KB (3143 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bcc0e59cf67e735575053d85c6b0b7be63d57e63ba39f08cd0ce8f2d3910e964`  
		Last Modified: Wed, 01 Nov 2023 01:18:26 GMT  
		Size: 110.0 MB (110008609 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5deafcd2b6f2f1508ae9f390dd4b120b5c9c86f093abe93807bbf0db537b98eb`  
		Last Modified: Wed, 01 Nov 2023 01:18:21 GMT  
		Size: 9.8 KB (9785 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b785c5551a7aa5363191fbb6a075b51455149e95314f5f06c0540ef047bfb816`  
		Last Modified: Wed, 01 Nov 2023 01:18:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eaac617c9ef57506e99825e75976ff92ff143e537c21977e5ee12b0a3a4f79d2`  
		Last Modified: Wed, 01 Nov 2023 01:18:22 GMT  
		Size: 170.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b850c1be51861dea1a06973b03234333ae7a6c4424e88cfd3ce8fb8d357033df`  
		Last Modified: Wed, 01 Nov 2023 01:18:22 GMT  
		Size: 4.8 KB (4786 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:15-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:6c59d114f76c70edff1108466fc0fb55236176cd80798ab6dcdb66cd08e7c7c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 KB (50357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:798f3493d1ecf3744ce603a5bd47d389848b7910a1a1808e31133cb0301cea7a`

```dockerfile
```

-	Layers:
	-	`sha256:0bd1f44d90ac235be1a11302365295a6d43ec09f0a68f70e794d9f5883de1b2b`  
		Last Modified: Wed, 01 Nov 2023 01:18:20 GMT  
		Size: 50.4 KB (50357 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:15-bookworm` - linux; mips64le

```console
$ docker pull postgres@sha256:b726184e9dd3bdab435b3a8db240de6294e250c23dc75add851d1c56b2962aa6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.8 MB (146819308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2fb735768f3429c48cf94052e61300a97dfe231e094af2881c6bb895511382f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
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
ENV PG_VERSION=15.5-1.pgdg120+1
# Thu, 30 Nov 2023 00:11:07 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:871b96f8117e597e34b3c42046e069e9a9853742b6dc729e7b535c28bfc6779d`  
		Last Modified: Thu, 23 Nov 2023 02:23:22 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2c7fcc8f2d432d7771d17e625701b453db95c7027f1032834c3a62ab676cf317`  
		Last Modified: Thu, 23 Nov 2023 02:23:23 GMT  
		Size: 4.4 MB (4355757 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:83300bed39f72a033140a846a97f7266adf45bd0b6d84e37ed437a40d612bb9b`  
		Last Modified: Thu, 23 Nov 2023 02:23:23 GMT  
		Size: 1.3 MB (1335999 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8d7e2fba0bdd77ec3166ca923dd6a279b53177ac4c996eff47553411057f6458`  
		Last Modified: Thu, 23 Nov 2023 02:23:24 GMT  
		Size: 8.1 MB (8068141 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ce0bdd1562b4671180c14ee1f065b11fddaef70c8b3ed2d93183195153c4a39`  
		Last Modified: Thu, 23 Nov 2023 02:23:24 GMT  
		Size: 1.2 MB (1181570 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bcca17a3e4955db19e17fbaf970a3515578cc080fa3dc9498e054766268c96ff`  
		Last Modified: Thu, 23 Nov 2023 02:23:24 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6169d401417f1a1c36c835cfdfc41d14fa36b4866061a4d54a76ae67690f828f`  
		Last Modified: Thu, 23 Nov 2023 02:23:24 GMT  
		Size: 3.1 KB (3142 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:62a95d2be9982aa3801ebd141369f3ae9b9ff75435ef86473e2844169f61c7fd`  
		Last Modified: Thu, 23 Nov 2023 04:42:39 GMT  
		Size: 102.7 MB (102716548 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8568698a7b26fdf1df854996c4e3e83311e40a163bab2af27fcb0483162374fc`  
		Last Modified: Thu, 23 Nov 2023 04:42:29 GMT  
		Size: 9.8 KB (9784 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eaac3d72c10fcfa240e03db6d94de44615e9f51b1fb39d9076d95a14cc101797`  
		Last Modified: Fri, 01 Dec 2023 22:17:54 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fa96ced42ad07c55ae5d3cd7ff85b05b91537efb4329d410dcd9f61b36f0b4e5`  
		Last Modified: Fri, 01 Dec 2023 22:17:54 GMT  
		Size: 174.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5dc21ffd10ae9fb3973d6f4cc04868ba1ebbd0305ef5f2f9ca8d784b49d17d01`  
		Last Modified: Fri, 01 Dec 2023 22:17:55 GMT  
		Size: 4.8 KB (4793 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:15-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:cd05b2e0086d44f84191a91bfbdea0fd6ffbdaa197a6f673214c402492694aa3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 KB (50331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51c54a58b005a39127be08016ead76edc32ca92089efb2411f66c866856f0d3a`

```dockerfile
```

-	Layers:
	-	`sha256:a4b04c6030cff87a0cbeae40b55cfbaccdc31d9286b39f34844fd1e31c588b8c`  
		Last Modified: Fri, 01 Dec 2023 22:17:54 GMT  
		Size: 50.3 KB (50331 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:15-bookworm` - linux; ppc64le

```console
$ docker pull postgres@sha256:bcf15450cbc37cbb858b096194b2606f1d3cd41d960f3b720f580c26abcba5b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.1 MB (163131136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6beb94512a97039daa4211efce9ede19417b69c217e05e2a2c2571fff253248`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
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
ENV PG_VERSION=15.5-1.pgdg120+1
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:315990094206abeaeb5d46d599ef4bb0e1007672173f67455f81cbcf17d870a7`  
		Last Modified: Sat, 09 Dec 2023 04:49:35 GMT  
		Size: 114.0 MB (114010164 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e4a34086aeb58bef33cfdcd53a6c3fcd8bbf8f1e2b229632c1e48b11d2b4c08a`  
		Last Modified: Sat, 09 Dec 2023 04:49:31 GMT  
		Size: 9.8 KB (9787 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:678f0c3666230661cc2eb686f542e0826e85e15dbd37cfad6ebe7389a5977430`  
		Last Modified: Sat, 09 Dec 2023 04:49:31 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d32f9aad6103cced4b35c96612442af944d128b943374e3c6ba82ce6cc4addc1`  
		Last Modified: Sat, 09 Dec 2023 04:49:31 GMT  
		Size: 171.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0c4d73da597d69c67f4dbd9b894b431fae91eda04e8ef111c827e78f2ea9e9ed`  
		Last Modified: Sat, 09 Dec 2023 04:49:32 GMT  
		Size: 4.8 KB (4786 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:15-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:40d7abb7ae5e5fa203854153171bc863ada612ceb86239f45506bba4815e0b4c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4948081 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e06d28534c8846fc41323ce1222569061098d997155ca1749fc48dc7079597b`

```dockerfile
```

-	Layers:
	-	`sha256:dc7bf7d3b52887b7373781598254abe50aaa2a8ef4dadb5a48a6fb3fc9c74c2b`  
		Last Modified: Sat, 09 Dec 2023 04:49:31 GMT  
		Size: 4.9 MB (4897436 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7ba46a8e5e2ef6d1cce6ee6bf994c7b25cbcdf89b7b2d65a0b9fc0dfb0ccf4a1`  
		Last Modified: Sat, 09 Dec 2023 04:49:30 GMT  
		Size: 50.6 KB (50645 bytes)  
		MIME: application/vnd.in-toto+json

### `postgres:15-bookworm` - linux; s390x

```console
$ docker pull postgres@sha256:5df48afaa80afcabe769bd42bd22a502ff33bf64e2f27b8d720ee4d9bdbcc845
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.5 MB (156547096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9af2827efa0bdcdeb8249ebc9f966c5369835e0b054d49f5308340b6d9407895`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:35 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Tue, 21 Nov 2023 05:04:41 GMT
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
ENV PG_VERSION=15.5-1.pgdg120+1
# Thu, 07 Dec 2023 22:39:53 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version # buildkit
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
	-	`sha256:fbb75167d761f2f5cd3eda298ae7213b097f3939d9f064e76e43755a32a78e5b`  
		Last Modified: Sat, 09 Dec 2023 01:59:18 GMT  
		Size: 8.1 MB (8122273 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:40a818c801adb9fe2619494f02d44d6bfd8553ce331001dbda8e792ce893c841`  
		Last Modified: Sat, 09 Dec 2023 01:59:18 GMT  
		Size: 1.1 MB (1095731 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:08942158f77ced9b1b87c5d52551306d38aca1c61950b8e882fcfb119ae163c7`  
		Last Modified: Sat, 09 Dec 2023 01:59:17 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fe5ccd328d41b41c2308349b20b876d2982ab878c7c1317a470f85fe0e36ad67`  
		Last Modified: Sat, 09 Dec 2023 01:59:17 GMT  
		Size: 3.1 KB (3141 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0aaa28aa651a8805aae149000e8cd12d682a71ad0146fe97500425a97b0ecbd9`  
		Last Modified: Sat, 09 Dec 2023 02:07:06 GMT  
		Size: 114.1 MB (114104272 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2b3eadb941afa893440523e962d1d0019bc75bba93c9f59e26de401e2c4c1828`  
		Last Modified: Sat, 09 Dec 2023 02:07:05 GMT  
		Size: 9.8 KB (9786 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:68db31d12f95c7401f01af46ba2768f67eb67a95c81d85b68a585fe7ba40f3ba`  
		Last Modified: Sat, 09 Dec 2023 02:07:05 GMT  
		Size: 128.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:56c95349df5164269200daff02d2caf5240d1df19a2a42e23007172c30c36acb`  
		Last Modified: Sat, 09 Dec 2023 02:07:04 GMT  
		Size: 172.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7ab5e2f5600137afe95bf47977986df4ddf2eb4cabfd129501e66283d42c308`  
		Last Modified: Sat, 09 Dec 2023 02:07:06 GMT  
		Size: 4.8 KB (4785 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `postgres:15-bookworm` - unknown; unknown

```console
$ docker pull postgres@sha256:452ca1b6f6e6d3483d09f507d59d3fa7adcb45cc2ceafe7e6b88909e0d8728bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4939975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fa9ad140a9c3c2f3367f22d6f670a05cfcc0cefffa1664b539ae60d24dfabce`

```dockerfile
```

-	Layers:
	-	`sha256:e9348e0d6385bdb6db0b0f2f55652c64526468231f31fe08028377dbf26db6e3`  
		Last Modified: Sat, 09 Dec 2023 02:07:04 GMT  
		Size: 4.9 MB (4889389 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4cbad10c09a851772c10bb6f4da87ea48a7efce05815e4ea7fb2f8095e864b18`  
		Last Modified: Sat, 09 Dec 2023 02:07:04 GMT  
		Size: 50.6 KB (50586 bytes)  
		MIME: application/vnd.in-toto+json
