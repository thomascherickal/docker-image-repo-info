## `postgres:15-bullseye`

```console
$ docker pull postgres@sha256:e1293d29c5cc633fca2b599c37304d3d426e71fa28bd9604acf67187bb37ff01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `postgres:15-bullseye` - linux; amd64

```console
$ docker pull postgres@sha256:296844abdfffb6ca374b13f2ce95fbe0c63b579593b8e379d34ac0520e002365
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.1 MB (139059492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9942bf3ae3eaf441ed1ed0e1fc57bccd043763a288e14f8ab68d6796e3a0259`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 20 Sep 2023 04:56:03 GMT
ADD file:7eb149bcaba1d7dcab06b3f9a0615ca459e9cb28459a0864f92b0037f270ba66 in / 
# Wed, 20 Sep 2023 04:56:03 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:36:41 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 20 Sep 2023 09:36:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:36:46 GMT
ENV GOSU_VERSION=1.16
# Wed, 20 Sep 2023 09:36:54 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 20 Sep 2023 09:37:00 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 20 Sep 2023 09:37:00 GMT
ENV LANG=en_US.utf8
# Wed, 20 Sep 2023 09:37:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:37:04 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 20 Sep 2023 09:37:06 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 20 Sep 2023 09:38:08 GMT
ENV PG_MAJOR=15
# Wed, 20 Sep 2023 09:38:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Wed, 20 Sep 2023 09:38:08 GMT
ENV PG_VERSION=15.4-2.pgdg110+1
# Wed, 20 Sep 2023 09:38:28 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 20 Sep 2023 09:38:29 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 20 Sep 2023 09:38:29 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 20 Sep 2023 09:38:29 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 20 Sep 2023 09:38:30 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 20 Sep 2023 09:38:30 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 20 Sep 2023 09:38:30 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Wed, 20 Sep 2023 09:38:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Sep 2023 09:38:30 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 09:38:30 GMT
EXPOSE 5432
# Wed, 20 Sep 2023 09:38:30 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:7dbc1adf280e1aa588c033eaa746aa6db327ee16be705740f81741f5e6945c86`  
		Last Modified: Wed, 20 Sep 2023 05:01:05 GMT  
		Size: 31.4 MB (31417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2de80609985cc7ec5fd98269e356515b4c21e7a4b96315b98dd97ccf845a9fa`  
		Last Modified: Wed, 20 Sep 2023 09:43:36 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd8e4a5f92cfb5e83b917aa87a5f7bb3c0bd9aa022a66452526b8a3c7285f04`  
		Last Modified: Wed, 20 Sep 2023 09:43:36 GMT  
		Size: 4.4 MB (4415030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4aee9e01982609cbbbe239bd093171b8bb53324baf444c5c167b12858ed49a`  
		Last Modified: Wed, 20 Sep 2023 09:43:35 GMT  
		Size: 1.5 MB (1471546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:304b18d1b3a93fa0b97533c0103c9196117572fe71b044c8f2bed1889788daf7`  
		Last Modified: Wed, 20 Sep 2023 09:43:34 GMT  
		Size: 8.0 MB (8045658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273cf38fe976a57247f61a8569c04c29642f3a05f1c82898ef2224cb6839a198`  
		Last Modified: Wed, 20 Sep 2023 09:43:33 GMT  
		Size: 1.3 MB (1261290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e3982beb4fb303a36f43c2f5d0639c1e10124499de77f61ebfc04d67394b3bb`  
		Last Modified: Wed, 20 Sep 2023 09:43:33 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038acb10572e5fb5578fa96c8e432a2bb7279566159fce9fe47554ea806dd2ae`  
		Last Modified: Wed, 20 Sep 2023 09:43:33 GMT  
		Size: 3.2 KB (3195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb59979f0a023aabf809413a0d9a5ae9510d9b461d40d1d83fc01a995dda7b5f`  
		Last Modified: Wed, 20 Sep 2023 09:44:37 GMT  
		Size: 92.4 MB (92428222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3b06a7160f57de461c2290b79f0df2f4bfa45c8ed4063ba4cb0a60b8a65f28`  
		Last Modified: Wed, 20 Sep 2023 09:44:25 GMT  
		Size: 9.8 KB (9783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6bc4e0b3b676a6effce37fcaacbb2f6f38ce140fcf3821e6984517db681439`  
		Last Modified: Wed, 20 Sep 2023 09:44:25 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31996949d31f92f1ca3092fac8570566f03ad4124141a887c7f92fdcf61a65f4`  
		Last Modified: Wed, 20 Sep 2023 09:44:25 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9aa62166bc3694ee612c51c7b513ecf4385e0352053d44ac7a3d1af28e6745`  
		Last Modified: Wed, 20 Sep 2023 09:44:25 GMT  
		Size: 4.8 KB (4784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15-bullseye` - linux; arm variant v5

```console
$ docker pull postgres@sha256:625dc0eb079652ba35c5d783d20d936b4f84d94dd9097e7d08109bbf869c5f88
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.3 MB (132292307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dca15b76157c1eafd9fc81ab3bffa26fad2a778c61b20f096a212f71f6afff64`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 20 Sep 2023 00:50:22 GMT
ADD file:3fafe6196c5a5c30a92e0a7cca16de98eecf20e6e40a25a36034e3512e0fceb7 in / 
# Wed, 20 Sep 2023 00:50:23 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 10:32:08 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 20 Sep 2023 10:32:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 10:32:16 GMT
ENV GOSU_VERSION=1.16
# Wed, 20 Sep 2023 10:32:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 20 Sep 2023 10:32:33 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 20 Sep 2023 10:32:33 GMT
ENV LANG=en_US.utf8
# Wed, 20 Sep 2023 10:32:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 10:32:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 20 Sep 2023 10:32:41 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 20 Sep 2023 11:02:55 GMT
ENV PG_MAJOR=15
# Wed, 20 Sep 2023 11:02:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Wed, 20 Sep 2023 11:02:56 GMT
ENV PG_VERSION=15.4-2.pgdg110+1
# Wed, 20 Sep 2023 11:17:14 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 20 Sep 2023 11:17:16 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 20 Sep 2023 11:17:17 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 20 Sep 2023 11:17:17 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 20 Sep 2023 11:17:18 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 20 Sep 2023 11:17:19 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 20 Sep 2023 11:17:19 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Wed, 20 Sep 2023 11:17:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Sep 2023 11:17:19 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 11:17:20 GMT
EXPOSE 5432
# Wed, 20 Sep 2023 11:17:20 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:028bb77b977c8effa899ef4c01139f4f5f8d4c94b82f792204b8bca21961fceb`  
		Last Modified: Wed, 20 Sep 2023 00:55:38 GMT  
		Size: 28.9 MB (28919128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e99b956524e51cafee3d8d215eda8ea9c16edf9c5e6e97facfb64d7e9a2713a`  
		Last Modified: Wed, 20 Sep 2023 13:07:20 GMT  
		Size: 1.8 KB (1793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c425f32665411f1c736f922216b3867281a10272f4789caa6cfa44e394356fb3`  
		Last Modified: Wed, 20 Sep 2023 13:07:21 GMT  
		Size: 4.1 MB (4096584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356487af2c64153d88579291788772a4a71a95200bd08423ab7d7cde92063625`  
		Last Modified: Wed, 20 Sep 2023 13:07:20 GMT  
		Size: 1.4 MB (1448835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177744c808e7c884ea12ed23c2867db81beca39a40c0b9df250c7d1cd3be1918`  
		Last Modified: Wed, 20 Sep 2023 13:07:21 GMT  
		Size: 8.0 MB (8045533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77dbfbb03c1c019ef792516ce09eef92c52dca52bf1f7ecfbc453ac7a1dbf9d`  
		Last Modified: Wed, 20 Sep 2023 13:07:18 GMT  
		Size: 1.3 MB (1257339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f03bb84ef4aa7099ea8b25a5011c83c295d185f08bbdd6a621e71f51a72cad`  
		Last Modified: Wed, 20 Sep 2023 13:07:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1d231fb4b90f91954a817a048009a3111f1496dd02a279595e5f134e70d73f`  
		Last Modified: Wed, 20 Sep 2023 13:07:18 GMT  
		Size: 3.2 KB (3193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f6b564b57bb57a4ba601c7fa16952a0ab01089152054dc032ed54bbae92692`  
		Last Modified: Wed, 20 Sep 2023 13:08:31 GMT  
		Size: 88.5 MB (88504845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465e53e35fd7a96baf0cb726fb1ac00b10e520c9d00870bb51884b41aa0b0b98`  
		Last Modified: Wed, 20 Sep 2023 13:08:15 GMT  
		Size: 9.8 KB (9790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001cecc40aa4181654e02ebf1678592025d351e367ca53b87adbfce24031c644`  
		Last Modified: Wed, 20 Sep 2023 13:08:15 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a75cc834fe6f1d6ac99576c4cb4d26344ecae3bef62ad02bb8c31857475857`  
		Last Modified: Wed, 20 Sep 2023 13:08:15 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30932104e4e28b08c7dce630bebfe8ac3b23ca192ba49d32161cd657ed1fc7e`  
		Last Modified: Wed, 20 Sep 2023 13:08:15 GMT  
		Size: 4.8 KB (4787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15-bullseye` - linux; arm variant v7

```console
$ docker pull postgres@sha256:35b71d51516d0399d25ec56b25b65076d1dbfe7e380a1247de11a80ebd392769
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.9 MB (126925149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4619278a52ba25156a7f6587a8d7234c8ecc3fce87111af003b3c7f1ce0fff7f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 07 Sep 2023 00:58:09 GMT
ADD file:d714939aacc810de397a02461ce4b9dd85e92783aff066bd3da685e3d2d97439 in / 
# Thu, 07 Sep 2023 00:58:10 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 04:27:11 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 07 Sep 2023 04:27:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 04:27:17 GMT
ENV GOSU_VERSION=1.16
# Thu, 07 Sep 2023 04:27:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 07 Sep 2023 04:27:33 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 07 Sep 2023 04:27:33 GMT
ENV LANG=en_US.utf8
# Thu, 07 Sep 2023 04:27:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 04:27:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 07 Sep 2023 04:27:40 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 07 Sep 2023 04:56:30 GMT
ENV PG_MAJOR=15
# Thu, 07 Sep 2023 04:56:30 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Fri, 15 Sep 2023 23:12:48 GMT
ENV PG_VERSION=15.4-2.pgdg110+1
# Fri, 15 Sep 2023 23:25:42 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 15 Sep 2023 23:25:44 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 15 Sep 2023 23:25:45 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 15 Sep 2023 23:25:45 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 15 Sep 2023 23:25:45 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 15 Sep 2023 23:25:46 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 15 Sep 2023 23:25:46 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Fri, 15 Sep 2023 23:25:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 Sep 2023 23:25:46 GMT
STOPSIGNAL SIGINT
# Fri, 15 Sep 2023 23:25:46 GMT
EXPOSE 5432
# Fri, 15 Sep 2023 23:25:46 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:323242406c24248128abc25e113055d272350b4ac4ecd985dbabfb7061c48d49`  
		Last Modified: Thu, 07 Sep 2023 01:03:12 GMT  
		Size: 26.6 MB (26578710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e8aab239bb85fd9d8959959a6618c6c567479d60c2676490d93667213cc58d`  
		Last Modified: Thu, 07 Sep 2023 06:56:07 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a16c2e61abc85a7be526ce4f71bec9e2061bb5d13c74f7f6e592479868cc0b`  
		Last Modified: Thu, 07 Sep 2023 06:56:07 GMT  
		Size: 3.7 MB (3717412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3e75d90e94b39bab44f1b37075dd18e64c34e4002a782d274078e8ec88a8bf`  
		Last Modified: Thu, 07 Sep 2023 06:56:06 GMT  
		Size: 1.4 MB (1438891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30731fa08c3b4d5af5bb23206acb944498d8e00b0eea4a9e44d91a084ae2b821`  
		Last Modified: Thu, 07 Sep 2023 06:56:06 GMT  
		Size: 8.0 MB (8045533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e49f21508789c22832cb0d1c5b3b0a844754fa25edb54b0c3f7a85c00b6a3b`  
		Last Modified: Thu, 07 Sep 2023 06:56:05 GMT  
		Size: 1.1 MB (1131259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9312e1b297f389d835004304afd0753a3c28aea63272f2715935e583fc370bd`  
		Last Modified: Thu, 07 Sep 2023 06:56:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d2068b512c24d8edd70cfccc9c1288a051378c4a9b02c0ea578f94c20e9cea`  
		Last Modified: Thu, 07 Sep 2023 06:56:04 GMT  
		Size: 3.2 KB (3192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4bd53ed42e7ce6626732e5a0d6d9819df98d7f3e78ae91e7002e8e4df138640`  
		Last Modified: Fri, 15 Sep 2023 23:29:45 GMT  
		Size: 86.0 MB (85993311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0062b9b51153acfbbf26687cfbf5a9145ff9eb3e8607fa1994eeb5e8117c280`  
		Last Modified: Fri, 15 Sep 2023 23:29:32 GMT  
		Size: 9.8 KB (9786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1127c2220864ce7ccc253dd4a7dbd262216e75492867c2c5f8608753d98b01`  
		Last Modified: Fri, 15 Sep 2023 23:29:32 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b870c0facc3e65f67310c487d3789e6e576e7f5664d5b795f6fac4cc6f9c4e9`  
		Last Modified: Fri, 15 Sep 2023 23:29:32 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802049cb3aa542ed50b80cb5bd14a7349c5a9619445b8b3e8bf99e9ca6de190a`  
		Last Modified: Fri, 15 Sep 2023 23:29:32 GMT  
		Size: 4.8 KB (4788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15-bullseye` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:7d0716f5e7cf687b45868fc2fffa47989916ec3ed37b68f5b9c5577f49c98bba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.1 MB (134137306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:088bd723ce90b5311a7585e031779a5140936f7fc5208b41f82849f518de14f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:28 GMT
ADD file:024479be439b4ecb37c939e68673adc72955f3345ca0e809bd13e897709e59e4 in / 
# Wed, 20 Sep 2023 02:44:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 12:15:11 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 20 Sep 2023 12:15:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 12:15:15 GMT
ENV GOSU_VERSION=1.16
# Wed, 20 Sep 2023 12:15:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 20 Sep 2023 12:15:28 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 20 Sep 2023 12:15:28 GMT
ENV LANG=en_US.utf8
# Wed, 20 Sep 2023 12:15:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 12:15:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 20 Sep 2023 12:15:32 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 20 Sep 2023 12:16:25 GMT
ENV PG_MAJOR=15
# Wed, 20 Sep 2023 12:16:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Wed, 20 Sep 2023 12:16:25 GMT
ENV PG_VERSION=15.4-2.pgdg110+1
# Wed, 20 Sep 2023 12:16:40 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 20 Sep 2023 12:16:41 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 20 Sep 2023 12:16:42 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 20 Sep 2023 12:16:42 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 20 Sep 2023 12:16:42 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 20 Sep 2023 12:16:42 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 20 Sep 2023 12:16:42 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Wed, 20 Sep 2023 12:16:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Sep 2023 12:16:42 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 12:16:42 GMT
EXPOSE 5432
# Wed, 20 Sep 2023 12:16:43 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:fc521c5b98350f6fd8c72ace1e48558bb7b53cb3db201a2a3b42095401cd02f1`  
		Last Modified: Wed, 20 Sep 2023 02:48:13 GMT  
		Size: 30.1 MB (30062869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6028bab77a5110687362f198eac3941cf64904dcf8deff1e61c683ab6035360d`  
		Last Modified: Wed, 20 Sep 2023 12:21:23 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c9f422128daf39a7a9a998a5d8dad3cabc2c2fdea4b02bde5300da18440ef5`  
		Last Modified: Wed, 20 Sep 2023 12:21:23 GMT  
		Size: 4.4 MB (4416342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2458da00c6aec029eeb7fe4794904394ce4c227dffc013c4f5142a76ce2344`  
		Last Modified: Wed, 20 Sep 2023 12:21:23 GMT  
		Size: 1.4 MB (1403330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2ee6a6c2a6cb84e90e37fa440a5c12fd506c05ffb1a44b36c00cb7182664fe`  
		Last Modified: Wed, 20 Sep 2023 12:21:22 GMT  
		Size: 8.0 MB (8045566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53127996f90ea36ed6a48a5c9427d319521e6c8a8a63c4670a72f75e42f8b133`  
		Last Modified: Wed, 20 Sep 2023 12:21:21 GMT  
		Size: 1.2 MB (1249330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7090b8ac3e3d429d27126dcc496b171295df59fb5d67f51f937351907ce677e1`  
		Last Modified: Wed, 20 Sep 2023 12:21:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f6c05cd417ba92efa4bfb2673241edc78c26771171e4b5773f0bc51199cc82`  
		Last Modified: Wed, 20 Sep 2023 12:21:21 GMT  
		Size: 3.2 KB (3197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab5f9a37668e6b685b332c2bb4ad63b82659376b63b05c60fd9ad118c365d40`  
		Last Modified: Wed, 20 Sep 2023 12:22:16 GMT  
		Size: 88.9 MB (88939818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b031d5cb18b793b47bef5f678eecfa6623c7a8fe4c0737e51801ef83d7ee00`  
		Last Modified: Wed, 20 Sep 2023 12:22:07 GMT  
		Size: 9.8 KB (9785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43925662385d267a367dba33b992529c3dc221a1ca8b0028d2ff2de45992995`  
		Last Modified: Wed, 20 Sep 2023 12:22:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562cfeeeb2ddd592074a743d0877fdd9ce7ac2cec637306569d4b6904cdae096`  
		Last Modified: Wed, 20 Sep 2023 12:22:07 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7880f022679578dd371cd8944bd737bf2d101a2f2f39c806982e0cc80f6f86`  
		Last Modified: Wed, 20 Sep 2023 12:22:07 GMT  
		Size: 4.8 KB (4786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15-bullseye` - linux; 386

```console
$ docker pull postgres@sha256:eb8adb77df4b0a43d80f2c5ed15095fd3e0bd6e0b2ef77fd223b61ce43f93a5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.1 MB (141099692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cca4e3f844e25c8e7f5f7234f2d8bc9f0594e6cfcc767b6edcd71f69d7256a6a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:23 GMT
ADD file:7da3a32fda5f1208b9e4a0151bc02b156c151608c0a2c17b70ca382b4446d87f in / 
# Thu, 07 Sep 2023 00:39:24 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:29:27 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 07 Sep 2023 01:29:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:29:34 GMT
ENV GOSU_VERSION=1.16
# Thu, 07 Sep 2023 01:29:44 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 07 Sep 2023 01:29:52 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 07 Sep 2023 01:29:52 GMT
ENV LANG=en_US.utf8
# Thu, 07 Sep 2023 01:29:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:29:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 07 Sep 2023 01:29:59 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 07 Sep 2023 02:07:32 GMT
ENV PG_MAJOR=15
# Thu, 07 Sep 2023 02:07:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Fri, 15 Sep 2023 23:35:08 GMT
ENV PG_VERSION=15.4-2.pgdg110+1
# Fri, 15 Sep 2023 23:53:10 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 15 Sep 2023 23:53:11 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 15 Sep 2023 23:53:12 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 15 Sep 2023 23:53:12 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 15 Sep 2023 23:53:13 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 15 Sep 2023 23:53:13 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 15 Sep 2023 23:53:13 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Fri, 15 Sep 2023 23:53:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 Sep 2023 23:53:13 GMT
STOPSIGNAL SIGINT
# Fri, 15 Sep 2023 23:53:13 GMT
EXPOSE 5432
# Fri, 15 Sep 2023 23:53:13 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:2508d8884943a2a8ff1cc6a8264b3085b7d7637e9de43269faf016019de5c311`  
		Last Modified: Thu, 07 Sep 2023 00:44:37 GMT  
		Size: 32.4 MB (32397335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74655300548258d7d25a328c0bffde08bed08c717de98f207d242c77bf5d14b2`  
		Last Modified: Thu, 07 Sep 2023 04:40:36 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149f9e39276753b35626d23a8eddc070887e3ac5589ed5e7b5d5880a6de76294`  
		Last Modified: Thu, 07 Sep 2023 04:40:37 GMT  
		Size: 4.8 MB (4813656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7907ad5c40789baddd839d2c311dab67e2cb2f0a9d6fa34a75c2fec78fc13f8c`  
		Last Modified: Thu, 07 Sep 2023 04:40:36 GMT  
		Size: 1.4 MB (1447125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6200fa51c3a49e06e95994515ae4ba82449632ef84569828f5a25fee8b9936`  
		Last Modified: Thu, 07 Sep 2023 04:40:36 GMT  
		Size: 8.0 MB (8045465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95726e25d4a4ae499c2adfa9a5b2f9269c200653b1e6efb566504c7003e260f`  
		Last Modified: Thu, 07 Sep 2023 04:40:34 GMT  
		Size: 1.3 MB (1251714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3301c04d87c5b94008e871f7874cc33ccfe5fc3a7a889e6fb75f4986cacdd2`  
		Last Modified: Thu, 07 Sep 2023 04:40:33 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98e073cab7e407921a11a8c0077a8650f69f363a19a92cf06772a24e4b2151a`  
		Last Modified: Thu, 07 Sep 2023 04:40:33 GMT  
		Size: 3.2 KB (3201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b936471d581e709b1928881321f7c7dc56cb6cdda3fb6ed34a5cc139735cb3aa`  
		Last Modified: Fri, 15 Sep 2023 23:57:48 GMT  
		Size: 93.1 MB (93124356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dfb5d6e876dd1f2bc12a1a1a9fe450df04009919d7177a64e8636e6cb1be089`  
		Last Modified: Fri, 15 Sep 2023 23:57:29 GMT  
		Size: 9.8 KB (9782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fbed00746a74839a4b1c84cef2138290800330481e8c9dbdf66a6a264a2785e`  
		Last Modified: Fri, 15 Sep 2023 23:57:29 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0ca1c80f1d786abc454371ee5e8dfe7c0c26388f85346dd457e64a0c979fbf`  
		Last Modified: Fri, 15 Sep 2023 23:57:29 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94bd7b56e7831d9bffe005249082b85553425aee5c3350c23783b4d6a8870b34`  
		Last Modified: Fri, 15 Sep 2023 23:57:29 GMT  
		Size: 4.8 KB (4794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15-bullseye` - linux; mips64le

```console
$ docker pull postgres@sha256:c5ebf066d313a6e6051b08cacff1b368905b7eabc9e2f51aec215d83d89b0261
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.4 MB (133370038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a34833289b7154f4e8ef311bae70a50b199deb88f79940117a004789cbc4093`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 07 Sep 2023 01:10:26 GMT
ADD file:d38d449a8bdd452a8b7527e92adb18283eee35701f577c61deb4ab93f1b88721 in / 
# Thu, 07 Sep 2023 01:10:31 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 20:52:48 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 07 Sep 2023 20:53:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 20:53:22 GMT
ENV GOSU_VERSION=1.16
# Thu, 07 Sep 2023 20:53:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 07 Sep 2023 20:54:21 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 07 Sep 2023 20:54:24 GMT
ENV LANG=en_US.utf8
# Thu, 07 Sep 2023 20:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 20:54:47 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 07 Sep 2023 20:54:52 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 07 Sep 2023 23:01:56 GMT
ENV PG_MAJOR=15
# Thu, 07 Sep 2023 23:01:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Sat, 16 Sep 2023 01:29:00 GMT
ENV PG_VERSION=15.4-2.pgdg110+1
# Sat, 16 Sep 2023 02:29:33 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Sat, 16 Sep 2023 02:29:40 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 16 Sep 2023 02:29:45 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 16 Sep 2023 02:29:49 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 16 Sep 2023 02:29:54 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 16 Sep 2023 02:29:57 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 16 Sep 2023 02:30:00 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Sat, 16 Sep 2023 02:30:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Sep 2023 02:30:07 GMT
STOPSIGNAL SIGINT
# Sat, 16 Sep 2023 02:30:11 GMT
EXPOSE 5432
# Sat, 16 Sep 2023 02:30:14 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:daedb7bf89cfe84a87bcfe1ba162d42f6ff21c2cb822f6199737968dee1ec769`  
		Last Modified: Thu, 07 Sep 2023 01:21:41 GMT  
		Size: 29.6 MB (29634539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24db17c5a45628d02b906593fd4c6e8bcda2fdf86793522f9e96c8584afb6f74`  
		Last Modified: Fri, 08 Sep 2023 07:47:40 GMT  
		Size: 1.6 KB (1644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95687259bb0d5acfd39d6d7ff72b815606e1b6bb9ac96c47a3176a4d397161f7`  
		Last Modified: Fri, 08 Sep 2023 07:47:42 GMT  
		Size: 4.2 MB (4196306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2cb141e46d8d59ecb8fbf1ce4a746880cec4d0e6804a72028057b1c9789b5b`  
		Last Modified: Fri, 08 Sep 2023 07:47:40 GMT  
		Size: 1.4 MB (1358357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9859c88d53a0c022792d55095baf99e1d4d784ac05b989de675a3c02eab681d`  
		Last Modified: Fri, 08 Sep 2023 07:47:44 GMT  
		Size: 8.0 MB (8044133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472497b2a64d442c3c8a9b1129c464aabaa9e1610c55eba4d6df846a1382104d`  
		Last Modified: Fri, 08 Sep 2023 07:47:37 GMT  
		Size: 1.1 MB (1089514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7028d39043f5fb123fd08fa8798f2c2f475cb68deb10221f09bedffb753e4b95`  
		Last Modified: Fri, 08 Sep 2023 07:47:36 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d253ad0ed17e54cf4ec6e1797578e678b8755c5c39b186a17d1c4fdf8c495a`  
		Last Modified: Fri, 08 Sep 2023 07:47:36 GMT  
		Size: 3.1 KB (3140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c515b06ad8ec752230c04922c4c511c8fe2d30ec098efd8f4deb9e93637f9de`  
		Last Modified: Sat, 16 Sep 2023 02:36:24 GMT  
		Size: 89.0 MB (89027415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b00df6c04374605ef0ceb117b3e760c061cf063eba11e353e1dcc6cd9a676d`  
		Last Modified: Sat, 16 Sep 2023 02:35:29 GMT  
		Size: 9.8 KB (9787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c0121b69da2eaee6dee39a61a9d8889390c21c30394114302eac07887697a4`  
		Last Modified: Sat, 16 Sep 2023 02:35:29 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c42c39f09e96a139ec69c4a9959953293c986acbf45c732ab774538ef5d579`  
		Last Modified: Sat, 16 Sep 2023 02:35:29 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d06f61642eb8243fe826b2c33fd1bf3390dd28a2b79d770d6307bd5ad0a4247`  
		Last Modified: Sat, 16 Sep 2023 02:35:29 GMT  
		Size: 4.8 KB (4790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15-bullseye` - linux; ppc64le

```console
$ docker pull postgres@sha256:f38f30da531550e344a3ddd43ff1c1a029842aae2bcd288c228c62da73fa5199
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.1 MB (148144466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:285cfd88b24571a7224dcc6649597df755eb52c454130429b8dd1328daefd844`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 07 Sep 2023 00:18:05 GMT
ADD file:bf50998bef8a71b4723f6c17cc5c3e929d9c3b7a71b56060fea91ea0cd3502c4 in / 
# Thu, 07 Sep 2023 00:18:08 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 16:27:39 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 07 Sep 2023 16:27:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 16:27:56 GMT
ENV GOSU_VERSION=1.16
# Thu, 07 Sep 2023 16:28:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 07 Sep 2023 16:28:30 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 07 Sep 2023 16:28:31 GMT
ENV LANG=en_US.utf8
# Thu, 07 Sep 2023 16:28:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 16:28:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 07 Sep 2023 16:28:46 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 07 Sep 2023 16:31:02 GMT
ENV PG_MAJOR=15
# Thu, 07 Sep 2023 16:31:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Fri, 15 Sep 2023 23:07:54 GMT
ENV PG_VERSION=15.4-2.pgdg110+1
# Fri, 15 Sep 2023 23:09:00 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 15 Sep 2023 23:09:07 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 15 Sep 2023 23:09:11 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 15 Sep 2023 23:09:12 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 15 Sep 2023 23:09:15 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 15 Sep 2023 23:09:16 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 15 Sep 2023 23:09:17 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Fri, 15 Sep 2023 23:09:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 Sep 2023 23:09:26 GMT
STOPSIGNAL SIGINT
# Fri, 15 Sep 2023 23:09:30 GMT
EXPOSE 5432
# Fri, 15 Sep 2023 23:09:32 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:2365f3cb8bc5e18258159454852d941d92577738f79c1b5594afaec8481b47f3`  
		Last Modified: Thu, 07 Sep 2023 00:24:24 GMT  
		Size: 35.3 MB (35291070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c09abbdb9a4c91ed611264b43af95860c64c6e8ddc2c837fe5014b97b452d0`  
		Last Modified: Thu, 07 Sep 2023 16:42:47 GMT  
		Size: 1.8 KB (1798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a99e6868ef28298f7180867a76c70a8d344204691f661dbb43eabb5591b282`  
		Last Modified: Thu, 07 Sep 2023 16:42:47 GMT  
		Size: 5.2 MB (5222924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a4e1a341ee4e6298d6f91e520f9004b397136fa55ec240cdf8334901ffb96e`  
		Last Modified: Thu, 07 Sep 2023 16:42:46 GMT  
		Size: 1.4 MB (1393372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5666274ad2e84c5c187905c411cf5320b04145f2a5e14a4259018d165ef34926`  
		Last Modified: Thu, 07 Sep 2023 16:42:47 GMT  
		Size: 8.0 MB (8045628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13eb1d789503af1457aae3e5f82e0501c6e2ae2b952c1d281dd2ad3e3d389fb`  
		Last Modified: Thu, 07 Sep 2023 16:42:44 GMT  
		Size: 1.4 MB (1420253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e26a7a977522e0d153f0d357a4dadc1b97dd24956fb7ad0a2a8c7411c9a0e4`  
		Last Modified: Thu, 07 Sep 2023 16:42:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ced060017cbf614a43fa5077d2ce9e2988ae44d9582bc890c372111a46cb4d9`  
		Last Modified: Thu, 07 Sep 2023 16:42:43 GMT  
		Size: 3.2 KB (3201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce56590dbc56b8257d942a32706511004aeae410c76d382d808980f8b685b23`  
		Last Modified: Fri, 15 Sep 2023 23:15:03 GMT  
		Size: 96.8 MB (96751169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57cd9537815a4d269dc8baa9ff0cde879789576d3889c6bc71c03297a8bf983f`  
		Last Modified: Fri, 15 Sep 2023 23:14:41 GMT  
		Size: 9.8 KB (9784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679941ddd265ca74380eb848182dfdf9c7fd0405b5451f70366031f372609e27`  
		Last Modified: Fri, 15 Sep 2023 23:14:40 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c8c287f2988e6fea857f1eaff3b3aa04d936348c7bd350610758b10013c3bf`  
		Last Modified: Fri, 15 Sep 2023 23:14:41 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b376ea26795c22493f4a9aaf746ff67f94514aee92f045930f6cf08157e4d06b`  
		Last Modified: Fri, 15 Sep 2023 23:14:41 GMT  
		Size: 4.8 KB (4788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15-bullseye` - linux; s390x

```console
$ docker pull postgres@sha256:b10492b70a4e87660d9a14d1e057ec0bd3d3343b0acf7b508fee08b1b07c068f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.7 MB (142667063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b09199d9c6274477d1f0b0a0e07a4be017b76d3d43033007f2c7c5da1abe9ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 20 Sep 2023 02:54:54 GMT
ADD file:02a97e0d5f41f84ac0284849646284fa41b5e324d24f4d95bb1e2419899da811 in / 
# Wed, 20 Sep 2023 02:54:57 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 10:07:13 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 20 Sep 2023 10:07:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 10:07:19 GMT
ENV GOSU_VERSION=1.16
# Wed, 20 Sep 2023 10:07:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 20 Sep 2023 10:07:33 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 20 Sep 2023 10:07:34 GMT
ENV LANG=en_US.utf8
# Wed, 20 Sep 2023 10:07:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 10:07:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 20 Sep 2023 10:07:39 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 20 Sep 2023 10:09:32 GMT
ENV PG_MAJOR=15
# Wed, 20 Sep 2023 10:09:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Wed, 20 Sep 2023 10:09:32 GMT
ENV PG_VERSION=15.4-2.pgdg110+1
# Wed, 20 Sep 2023 10:09:51 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 20 Sep 2023 10:09:57 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 20 Sep 2023 10:09:58 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 20 Sep 2023 10:09:58 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 20 Sep 2023 10:09:59 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 20 Sep 2023 10:09:59 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 20 Sep 2023 10:09:59 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Wed, 20 Sep 2023 10:09:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Sep 2023 10:09:59 GMT
STOPSIGNAL SIGINT
# Wed, 20 Sep 2023 10:09:59 GMT
EXPOSE 5432
# Wed, 20 Sep 2023 10:09:59 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:d2d51167e651784cce0bd658d0c2caa328adef8ccf264d8c09860a95bc2a2fc6`  
		Last Modified: Wed, 20 Sep 2023 03:00:22 GMT  
		Size: 29.7 MB (29653129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa183c449b5c9ea178d10cf825ae17da30ccd1df4865e0cdc6af587487139897`  
		Last Modified: Wed, 20 Sep 2023 10:17:21 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416afad9503f77597514f50b9dbed41db184f6ba25e2b1a3c4a6217403bf2763`  
		Last Modified: Wed, 20 Sep 2023 10:17:21 GMT  
		Size: 4.3 MB (4302353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0809d552a589cff056ebe0544797d2a6bb7f514f29a105cf02822d594fe1c03e`  
		Last Modified: Wed, 20 Sep 2023 10:17:21 GMT  
		Size: 1.4 MB (1437205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493ef821e411e2ec4d271e3067bde00b9b681c247707441a131ec0e07b8ff4f9`  
		Last Modified: Wed, 20 Sep 2023 10:17:21 GMT  
		Size: 8.1 MB (8099344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5e9f140034667ea63c2bd6f25b21cd713318cda32483e74d25aeb0d4162752`  
		Last Modified: Wed, 20 Sep 2023 10:17:20 GMT  
		Size: 1.2 MB (1238084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef553e67e198d924dad74b574113c21380f2ba944b85339c1d7994315350468e`  
		Last Modified: Wed, 20 Sep 2023 10:17:20 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1787e8182ee1afb6b7a2b2d8b35185d3fa921581ca40274f9d2cf20567744cf`  
		Last Modified: Wed, 20 Sep 2023 10:17:20 GMT  
		Size: 3.2 KB (3198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef1257ebd2f1910a5ec6778c46c85cdd53eceb5d457e461ded70d363f4ffdd5`  
		Last Modified: Wed, 20 Sep 2023 10:18:22 GMT  
		Size: 97.9 MB (97916901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62fd4b2d8cc0e76b46e724196719db33b306a4a822aef5526a4a42aec926c1f7`  
		Last Modified: Wed, 20 Sep 2023 10:18:10 GMT  
		Size: 9.8 KB (9783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1d82b693fa7073cdf3cc34a48a618ca3357138b442b8979250d3def30c6158`  
		Last Modified: Wed, 20 Sep 2023 10:18:10 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1b832b076f09ce9498ba953b3532827c5cb0afdb3e8db50b2086bf502f1363`  
		Last Modified: Wed, 20 Sep 2023 10:18:10 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:878237ec23a62eb7effd10c14bbc65ecef3bc9254bb7fe20f03bfddbf502af14`  
		Last Modified: Wed, 20 Sep 2023 10:18:10 GMT  
		Size: 4.8 KB (4784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
