## `postgres:13-bullseye`

```console
$ docker pull postgres@sha256:916627b75381ce9e0a0433731a622ca2d47d6f123f1294f9430a7810346bd0e8
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

### `postgres:13-bullseye` - linux; amd64

```console
$ docker pull postgres@sha256:0cc8a57338859ab207f331a03a0876a04547d07531a90eb0d784a5552bf2c97d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.7 MB (135715043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0896a8e0282d1f1be779b0b154d6bf4ffcb61414d9fd93e9c18593447e72c6c9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 23:31:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 23:31:33 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 21 Dec 2021 23:31:34 GMT
ENV GOSU_VERSION=1.14
# Tue, 21 Dec 2021 23:31:57 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 21 Dec 2021 23:32:11 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 21 Dec 2021 23:32:11 GMT
ENV LANG=en_US.utf8
# Tue, 21 Dec 2021 23:32:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:32:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 21 Dec 2021 23:32:29 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 21 Dec 2021 23:33:14 GMT
ENV PG_MAJOR=13
# Tue, 21 Dec 2021 23:33:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 21 Dec 2021 23:33:15 GMT
ENV PG_VERSION=13.5-1.pgdg110+1
# Tue, 21 Dec 2021 23:33:38 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 21 Dec 2021 23:33:39 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 21 Dec 2021 23:33:40 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 21 Dec 2021 23:33:40 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 21 Dec 2021 23:33:41 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 21 Dec 2021 23:33:41 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 04 Jan 2022 01:20:06 GMT
COPY file:b2fac085615145a2bee98d4185ef0748655fa7c086ca21daef1ca6cac272bf59 in /usr/local/bin/ 
# Tue, 04 Jan 2022 01:20:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jan 2022 01:20:06 GMT
STOPSIGNAL SIGINT
# Tue, 04 Jan 2022 01:20:06 GMT
EXPOSE 5432
# Tue, 04 Jan 2022 01:20:07 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1769f49f9101e08b259481961baceea032c026337b960a2737ba58d84c08d5f`  
		Last Modified: Tue, 21 Dec 2021 23:39:01 GMT  
		Size: 4.4 MB (4414603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a59cfee47cee21e9a3725fc141ad856917e95a1817f3719d5e7bae0c4e9515`  
		Last Modified: Tue, 21 Dec 2021 23:38:59 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461b2090c345e5af01940b13f92bcdbd47ef70bd372fd0a565af08f53c0f1601`  
		Last Modified: Tue, 21 Dec 2021 23:39:00 GMT  
		Size: 1.4 MB (1418382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed8ab6290ac04d65ebec4245056773a6679334d17b77a9a6bf1b7f1e26ad08a`  
		Last Modified: Tue, 21 Dec 2021 23:38:59 GMT  
		Size: 8.0 MB (8045343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495e42c822a03224fc27a04cf05716b82a5f1c4c9252cc7457673be355ab12f2`  
		Last Modified: Tue, 21 Dec 2021 23:38:57 GMT  
		Size: 441.7 KB (441681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e858c71c58fe45a750a830bfab4fe11bbd4618ace209d0ad397e4647d648d2`  
		Last Modified: Tue, 21 Dec 2021 23:38:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594792c80d5fa95924c9f7abe6acec205e5db07fc6bd04c299e3cd48174d1fab`  
		Last Modified: Tue, 21 Dec 2021 23:38:57 GMT  
		Size: 3.1 KB (3057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce2d192c3200dd5b83642cca1fa0a5b5d77e71fef7d6c991e5bc05f1b568a2f`  
		Last Modified: Tue, 21 Dec 2021 23:39:47 GMT  
		Size: 90.0 MB (90017988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00cfe308d7935f7c3ac2df885a30b5084191503df4c12a149e1bc57f31003d11`  
		Last Modified: Tue, 21 Dec 2021 23:39:34 GMT  
		Size: 9.4 KB (9365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4a326c1cb32b4118679fde76520eac4fe2df27b9dad7ffe6eeeb6c01f4507f`  
		Last Modified: Tue, 21 Dec 2021 23:39:34 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f2a6fdb326c3fad113bfecf632c4f177df2fdc8f86063c8cd3a9437f32f4d6`  
		Last Modified: Tue, 21 Dec 2021 23:39:34 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1f873a68ce55566074486fedc0843e988fce135492403577a7db108b65221e`  
		Last Modified: Tue, 04 Jan 2022 01:22:45 GMT  
		Size: 4.7 KB (4716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; arm variant v5

```console
$ docker pull postgres@sha256:2638208a765a412ce5fbaca96ddac7e641b35f48a45b39e3b9d0eb2ab056de3e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.0 MB (128984635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d52749519e7aecfb2d147e0bf0d96bb1db5c98d02618626da70930e7ba27b40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Dec 2021 01:50:31 GMT
ADD file:a3023f71bd93966e7db1419adda3ccde4fcc5e2e8cf58e7b13c51036ed5ff796 in / 
# Tue, 21 Dec 2021 01:50:32 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:30:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 07:30:43 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 21 Dec 2021 07:30:44 GMT
ENV GOSU_VERSION=1.14
# Tue, 21 Dec 2021 07:31:07 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 21 Dec 2021 07:31:30 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 21 Dec 2021 07:31:31 GMT
ENV LANG=en_US.utf8
# Tue, 21 Dec 2021 07:31:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:31:43 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 21 Dec 2021 07:31:46 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 21 Dec 2021 08:10:24 GMT
ENV PG_MAJOR=13
# Tue, 21 Dec 2021 08:10:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 21 Dec 2021 08:10:25 GMT
ENV PG_VERSION=13.5-1.pgdg110+1
# Tue, 21 Dec 2021 08:46:31 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 21 Dec 2021 08:46:33 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 21 Dec 2021 08:46:35 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 21 Dec 2021 08:46:35 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 21 Dec 2021 08:46:37 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 21 Dec 2021 08:46:37 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 04 Jan 2022 01:49:07 GMT
COPY file:b2fac085615145a2bee98d4185ef0748655fa7c086ca21daef1ca6cac272bf59 in /usr/local/bin/ 
# Tue, 04 Jan 2022 01:49:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jan 2022 01:49:08 GMT
STOPSIGNAL SIGINT
# Tue, 04 Jan 2022 01:49:08 GMT
EXPOSE 5432
# Tue, 04 Jan 2022 01:49:09 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:054429d0cf4038fef39a3b5eb6ce52f600f9a2cbb71a4fb3e95ecf9b2da62581`  
		Last Modified: Tue, 21 Dec 2021 02:05:52 GMT  
		Size: 28.9 MB (28900253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11c3b8663b33872a4cd51280b3b6213125ffb664af3544f78a8c00861d96529`  
		Last Modified: Tue, 21 Dec 2021 12:06:36 GMT  
		Size: 4.1 MB (4096469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7885af84e3728315efcdad4126b9cf21704918c9bd5b532975c20b15618b6d83`  
		Last Modified: Tue, 21 Dec 2021 12:06:31 GMT  
		Size: 1.8 KB (1798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6966bd647e990282b34e4b0ccdcee10086f054b44ed0b3f0133f098b9967b23b`  
		Last Modified: Tue, 21 Dec 2021 12:06:31 GMT  
		Size: 1.4 MB (1382552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a4a1fd7b75dec70f07b372ad523c88e90a1d337f5a2488b84a134db9bbfe15`  
		Last Modified: Tue, 21 Dec 2021 12:06:35 GMT  
		Size: 8.0 MB (8045155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d0038c65b0aafcf1ea56729903d012a7a37126d4900f4861ca4a16d7573fa8`  
		Last Modified: Tue, 21 Dec 2021 12:06:30 GMT  
		Size: 439.8 KB (439838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359b44a703071420b378dcf42f848c5aa8fdf777498ebfb37c8cbe52f38c64b9`  
		Last Modified: Tue, 21 Dec 2021 12:06:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af723b478cfbdf181802077d97fe3ff370c9c0d1505f26ad33f479f19545e442`  
		Last Modified: Tue, 21 Dec 2021 12:06:29 GMT  
		Size: 3.1 KB (3056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eecd32b2bd75aa1ca723da72182b8fd79435b7fede8efbb50e81e56503633cc`  
		Last Modified: Tue, 21 Dec 2021 12:08:47 GMT  
		Size: 86.1 MB (86100957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf35ca57be6478c790ab24c72a64ee9c75d6bff49949405ddabff14a3d926943`  
		Last Modified: Tue, 21 Dec 2021 12:07:53 GMT  
		Size: 9.4 KB (9363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcb5906c38ab2dd996e0d32fa9b0a01ec74c2c62c978e25225fd57b19a00461`  
		Last Modified: Tue, 21 Dec 2021 12:07:53 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0517994343662fcc3d5eb316ea992db766cbc5a9fd22a5bd68607eed53f51f`  
		Last Modified: Tue, 21 Dec 2021 12:07:53 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65553428c0496cfddeac4a2ac545aacff244ad6f2d9af2b4977914977208394`  
		Last Modified: Tue, 04 Jan 2022 01:54:14 GMT  
		Size: 4.7 KB (4716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; arm variant v7

```console
$ docker pull postgres@sha256:5c59e693ad2fc00c65913556582aef2e39a834d73d2b192d9c9095a4738528e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.8 MB (123835300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fe9408b62edd21e82a0a9a4cfa6a31190416911ba8c4f84e325b8e882fdfcd2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Dec 2021 01:59:48 GMT
ADD file:6a5555c3e40db91fae5bb112464a4c405a976de17ff64c98f25d3033a6a608d8 in / 
# Tue, 21 Dec 2021 01:59:48 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 13:34:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 13:34:52 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 21 Dec 2021 13:34:53 GMT
ENV GOSU_VERSION=1.14
# Tue, 21 Dec 2021 13:35:15 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 21 Dec 2021 13:35:35 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 21 Dec 2021 13:35:36 GMT
ENV LANG=en_US.utf8
# Tue, 21 Dec 2021 13:35:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 13:35:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 21 Dec 2021 13:35:51 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 21 Dec 2021 14:11:02 GMT
ENV PG_MAJOR=13
# Tue, 21 Dec 2021 14:11:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 21 Dec 2021 14:11:03 GMT
ENV PG_VERSION=13.5-1.pgdg110+1
# Tue, 21 Dec 2021 14:43:50 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 21 Dec 2021 14:43:53 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 21 Dec 2021 14:43:54 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 21 Dec 2021 14:43:55 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 21 Dec 2021 14:43:56 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 21 Dec 2021 14:43:57 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 04 Jan 2022 00:58:41 GMT
COPY file:b2fac085615145a2bee98d4185ef0748655fa7c086ca21daef1ca6cac272bf59 in /usr/local/bin/ 
# Tue, 04 Jan 2022 00:58:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jan 2022 00:58:42 GMT
STOPSIGNAL SIGINT
# Tue, 04 Jan 2022 00:58:43 GMT
EXPOSE 5432
# Tue, 04 Jan 2022 00:58:43 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:d0061d6703dc4975804c3419e00c85efbe3f1b79c86d87e048fa14a683e88e31`  
		Last Modified: Tue, 21 Dec 2021 02:15:26 GMT  
		Size: 26.6 MB (26560815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63faa60732a43e018f66952afb7f45d04d6d4758ee3d81183a163f9b6f804d2a`  
		Last Modified: Tue, 21 Dec 2021 17:48:01 GMT  
		Size: 3.7 MB (3717142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0323b5281fb94b32757850d02213a35a5f22c233d2c30a49504f89067f72f573`  
		Last Modified: Tue, 21 Dec 2021 17:47:59 GMT  
		Size: 1.8 KB (1794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22b25778e1eb533d3a049204db0bd7f35e725b44748eb5b53d7dbcfb5b3adf6`  
		Last Modified: Tue, 21 Dec 2021 17:48:00 GMT  
		Size: 1.4 MB (1375223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89817e68a18fa0bdfc9458a9b332f5b365056be1f503efa9c21faad188af3e92`  
		Last Modified: Tue, 21 Dec 2021 17:48:03 GMT  
		Size: 8.0 MB (8045328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1d4b88549ac5042ce416127fca3eb9ad03134d3f87810ea59ea4234237cfb5`  
		Last Modified: Tue, 21 Dec 2021 17:47:57 GMT  
		Size: 434.5 KB (434535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7fd84c8b77f1bed6ce41ca44ab4fb3dcd41ff89c2536a428f8652b8ddd33a5`  
		Last Modified: Tue, 21 Dec 2021 17:47:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0160dd882bce5ce444f89bf8732ff499fc30f3469341d635ea8d721d047c0505`  
		Last Modified: Tue, 21 Dec 2021 17:47:57 GMT  
		Size: 3.1 KB (3058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0f8c67ef1740738aadb117309321dea6b8c86f1c4787d7a7287222aa91edb9`  
		Last Modified: Tue, 21 Dec 2021 17:50:14 GMT  
		Size: 83.7 MB (83682852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10359ab73d21e656db89eaf95c5df0a27b76f7d12737cfa239907cbb097d31b0`  
		Last Modified: Tue, 21 Dec 2021 17:49:24 GMT  
		Size: 9.4 KB (9361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3536186da3757f016be3e6dec671ff32ddd8d0d8b27e710387ce0f9cfa3096`  
		Last Modified: Tue, 21 Dec 2021 17:49:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edae4e3bbca5861cfaba0f00df9358181a0004d91e79db05d7b0c43e8f3f8ac8`  
		Last Modified: Tue, 21 Dec 2021 17:49:24 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf3fc327c7d6bf9f033a53523859146b595bc4afd9ce8e9db37a9a915fe2bee8`  
		Last Modified: Tue, 04 Jan 2022 01:07:55 GMT  
		Size: 4.7 KB (4714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:54330c5cb9a56ec189534da90a25df85689bd154b0c2c76e81f883ae0a1e32a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130403358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cfb877dbde5450cf54870817adc54175b8ca4f3c3a4b850bdc68d2188907918`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 06:32:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 06:32:16 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 26 Jan 2022 06:32:17 GMT
ENV GOSU_VERSION=1.14
# Wed, 26 Jan 2022 06:32:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 26 Jan 2022 06:32:33 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 26 Jan 2022 06:32:33 GMT
ENV LANG=en_US.utf8
# Wed, 26 Jan 2022 06:32:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 06:32:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 26 Jan 2022 06:33:11 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Wed, 26 Jan 2022 06:34:12 GMT
ENV PG_MAJOR=13
# Wed, 26 Jan 2022 06:34:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Wed, 26 Jan 2022 06:34:14 GMT
ENV PG_VERSION=13.5-1.pgdg110+1
# Wed, 26 Jan 2022 06:34:34 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 26 Jan 2022 06:34:35 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 26 Jan 2022 06:34:36 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 26 Jan 2022 06:34:37 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 26 Jan 2022 06:34:38 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 26 Jan 2022 06:34:39 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 26 Jan 2022 06:34:41 GMT
COPY file:b2fac085615145a2bee98d4185ef0748655fa7c086ca21daef1ca6cac272bf59 in /usr/local/bin/ 
# Wed, 26 Jan 2022 06:34:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 06:34:42 GMT
STOPSIGNAL SIGINT
# Wed, 26 Jan 2022 06:34:43 GMT
EXPOSE 5432
# Wed, 26 Jan 2022 06:34:44 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c57ecc00197f74ecfe5cb4695ff8e4c31d88315d3c8f6b13e57f32b9fb6f2a2`  
		Last Modified: Wed, 26 Jan 2022 07:07:50 GMT  
		Size: 4.2 MB (4208911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1aaa551482e30d108cc7d900e1c329efc065835004868fe1a2f3f19f0a95fb`  
		Last Modified: Wed, 26 Jan 2022 07:07:49 GMT  
		Size: 1.6 KB (1649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409382316c269c57d22fdaa5f25f0738d8914b50707c8983a175dad92d7b4d0d`  
		Last Modified: Wed, 26 Jan 2022 07:07:49 GMT  
		Size: 1.3 MB (1345987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2a428af099e0f069419eb87af03d305891b574838113f91ba44539a05deb4b`  
		Last Modified: Wed, 26 Jan 2022 07:07:48 GMT  
		Size: 8.0 MB (8043388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44b8e834aba8ae7109dbcdff531b91c5939db21d3c6bbffd871e7252c32641a`  
		Last Modified: Wed, 26 Jan 2022 07:07:47 GMT  
		Size: 218.6 KB (218594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1372eb84c820add30aceea443ba9e01d2344f670f92c272837b72f1ad299a0ad`  
		Last Modified: Wed, 26 Jan 2022 07:07:46 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39188dbce14f3aee4c4502bb5b5ccaf9e2ca0ee598f44e6a187a21ab891edfe4`  
		Last Modified: Wed, 26 Jan 2022 07:07:47 GMT  
		Size: 3.0 KB (3032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b529154f0cbca0b0413b143da5bdda3bd988a6776126f60dd460a065bbcba3`  
		Last Modified: Wed, 26 Jan 2022 07:08:40 GMT  
		Size: 86.5 MB (86510530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fba4d3bc7d8e310c46613c1e1b064da931d369224cbe9050d1cb48a406d688`  
		Last Modified: Wed, 26 Jan 2022 07:08:25 GMT  
		Size: 9.4 KB (9362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47f8ba4cca4277d4a51aab313a2b683f0db12f0f1fc3b4e95fc73840d0e228d9`  
		Last Modified: Wed, 26 Jan 2022 07:08:25 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb7763a26e44bd29a1bbecf723b71516bff3be905939b66817c5b7e0992834d`  
		Last Modified: Wed, 26 Jan 2022 07:08:25 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be72a49431d0a86626af1d153ae419522f870a2142b0af814a7fe089a8b30eeb`  
		Last Modified: Wed, 26 Jan 2022 07:08:25 GMT  
		Size: 4.7 KB (4715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; 386

```console
$ docker pull postgres@sha256:6a897df6926c6ee528dcee1af0f29638e06ea07dcf630761cce918d339ccde9a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137809903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3211bdf3d6a68d1713fbaf61f6c58523b53ac33a8bb98e0cb2a17cf367a6e8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 17:32:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 17:32:31 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 21 Dec 2021 17:32:31 GMT
ENV GOSU_VERSION=1.14
# Tue, 21 Dec 2021 17:32:42 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 21 Dec 2021 17:32:50 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 21 Dec 2021 17:32:51 GMT
ENV LANG=en_US.utf8
# Tue, 21 Dec 2021 17:32:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 17:32:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 21 Dec 2021 17:33:04 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 21 Dec 2021 17:56:13 GMT
ENV PG_MAJOR=13
# Tue, 21 Dec 2021 17:56:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 21 Dec 2021 17:56:14 GMT
ENV PG_VERSION=13.5-1.pgdg110+1
# Tue, 21 Dec 2021 18:14:05 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 21 Dec 2021 18:14:07 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 21 Dec 2021 18:14:08 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 21 Dec 2021 18:14:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 21 Dec 2021 18:14:09 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 21 Dec 2021 18:14:09 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 04 Jan 2022 01:39:09 GMT
COPY file:b2fac085615145a2bee98d4185ef0748655fa7c086ca21daef1ca6cac272bf59 in /usr/local/bin/ 
# Tue, 04 Jan 2022 01:39:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jan 2022 01:39:09 GMT
STOPSIGNAL SIGINT
# Tue, 04 Jan 2022 01:39:10 GMT
EXPOSE 5432
# Tue, 04 Jan 2022 01:39:10 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e1cde80251c811d2a11419dd7d755ffd8bb6ee6c48d6c26f4963af66231091`  
		Last Modified: Tue, 21 Dec 2021 19:09:13 GMT  
		Size: 4.8 MB (4812928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e5319205e69940a9e1c4aa2eb8b128ceb099b3b1ff04f95e9b807a57bee635`  
		Last Modified: Tue, 21 Dec 2021 19:09:11 GMT  
		Size: 1.8 KB (1791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:986b5046b42a04043dea030af38801a4786894d4282a6c18ca760a3a7dc08a91`  
		Last Modified: Tue, 21 Dec 2021 19:09:11 GMT  
		Size: 1.4 MB (1385420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69e50d5aff566bb6bc43ae83d6f252488788b3297a5932cd665a9c9df4816a8`  
		Last Modified: Tue, 21 Dec 2021 19:09:12 GMT  
		Size: 8.0 MB (8045063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d4116276636907e25c3224b8a72e1c62e1b6040aae2a429a921513da0d0e4a`  
		Last Modified: Tue, 21 Dec 2021 19:09:09 GMT  
		Size: 448.0 KB (447958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e3213019f61cd51f01af4a70a4182fc67bdd71b82ea07c074f6796d4ff00f6`  
		Last Modified: Tue, 21 Dec 2021 19:09:09 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05967f41fcb3ecba7545ee6ced7b3f5419d14bc5e1fec038363f5e01c268e986`  
		Last Modified: Tue, 21 Dec 2021 19:09:08 GMT  
		Size: 3.1 KB (3053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2819137140ca776d23e56caf936a6d47467730062badb91f49576bf255d7ab2d`  
		Last Modified: Tue, 21 Dec 2021 19:10:16 GMT  
		Size: 90.7 MB (90728278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22fffe80554b5f2178d17adc4f5c867d0bf161d200feea5fac92c27992c7c07f`  
		Last Modified: Tue, 21 Dec 2021 19:09:57 GMT  
		Size: 9.4 KB (9359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6ccc078969bdaf9ed9997f113fbd2f636a037175e37b05426915a54b586b73`  
		Last Modified: Tue, 21 Dec 2021 19:09:57 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1200bf9b13abce32c70e8aac5d43bf23b5c02ca9c100571531cae76382f7278`  
		Last Modified: Tue, 21 Dec 2021 19:09:57 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126031fafa8ee422f7f2a2566cf00281a290c403a2b37e24da3135860b7de8f8`  
		Last Modified: Tue, 04 Jan 2022 01:43:48 GMT  
		Size: 4.7 KB (4726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; mips64le

```console
$ docker pull postgres@sha256:a0cea229a99bbfc96c81b8f25bcadea2451caf9a017e93bc0763ac46d0420305
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.5 MB (130531140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de9f74cf7b0d005338f2030f424c6f42c6b6af469b3ede1b243738fe70a103e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Dec 2021 02:09:07 GMT
ADD file:9e5931d5ed32a23b2e93bd8846258c647613637c581b6813bbc7d7e6b86bbdf5 in / 
# Tue, 21 Dec 2021 02:09:08 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 19:46:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 19:46:42 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 21 Dec 2021 19:46:42 GMT
ENV GOSU_VERSION=1.14
# Tue, 21 Dec 2021 19:47:03 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 21 Dec 2021 19:47:27 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 21 Dec 2021 19:47:27 GMT
ENV LANG=en_US.utf8
# Tue, 21 Dec 2021 19:47:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 19:47:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 21 Dec 2021 19:47:45 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 21 Dec 2021 20:43:54 GMT
ENV PG_MAJOR=13
# Tue, 21 Dec 2021 20:43:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 21 Dec 2021 20:43:55 GMT
ENV PG_VERSION=13.5-1.pgdg110+1
# Tue, 21 Dec 2021 21:36:45 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 21 Dec 2021 21:36:48 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 21 Dec 2021 21:36:50 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 21 Dec 2021 21:36:50 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 21 Dec 2021 21:36:52 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 21 Dec 2021 21:36:53 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 04 Jan 2022 01:07:38 GMT
COPY file:b2fac085615145a2bee98d4185ef0748655fa7c086ca21daef1ca6cac272bf59 in /usr/local/bin/ 
# Tue, 04 Jan 2022 01:07:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jan 2022 01:07:39 GMT
STOPSIGNAL SIGINT
# Tue, 04 Jan 2022 01:07:39 GMT
EXPOSE 5432
# Tue, 04 Jan 2022 01:07:39 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:6a6edb95e2485a5b9b3c44b27b7ebad16384c0e08a3d61b7e48c65d7278763cf`  
		Last Modified: Tue, 21 Dec 2021 02:18:14 GMT  
		Size: 29.6 MB (29619177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653335db2e28f4bfd481492903832070d7b54f24e6dbe67b45fbffb8f93f5f20`  
		Last Modified: Wed, 22 Dec 2021 00:29:22 GMT  
		Size: 4.4 MB (4402849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:383e4074bda5fb21527af7a93e33f31c633e43a90f4e44b18a33310b19b408fb`  
		Last Modified: Wed, 22 Dec 2021 00:29:17 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f76b983b76977ca3c9f7673149aeb74d2c70667cdaa2fd417ad3230f650169`  
		Last Modified: Wed, 22 Dec 2021 00:29:19 GMT  
		Size: 1.3 MB (1298144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7171701033e64ea4d7fa9ccf50c04e53f4dc6c699892fd7e860ea1a5a8909e`  
		Last Modified: Wed, 22 Dec 2021 00:29:23 GMT  
		Size: 8.0 MB (8043972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116ca8f780ee3685a34795364c930ee965bfb719b63da395abf7ffd84fd9b0cd`  
		Last Modified: Wed, 22 Dec 2021 00:29:15 GMT  
		Size: 439.2 KB (439173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87675c81c5f9c9c33f33cb6639eb0d676b031d16b7d33da01e300cb5ac98845c`  
		Last Modified: Wed, 22 Dec 2021 00:29:15 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc52613f4cea3e4b18408762b08e16750865b57c281ec9e1e567fe182a169ea`  
		Last Modified: Wed, 22 Dec 2021 00:29:15 GMT  
		Size: 3.1 KB (3058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939906b0b35c8777b623eb5adef3e2b8699a2ea88b177c2ff2200c8a2e8a8aef`  
		Last Modified: Wed, 22 Dec 2021 00:31:45 GMT  
		Size: 86.7 MB (86708508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5d5a9680f0589c5a6b1d3d423afcb6ae869effcb8c0dae8809ada38c9e7bbc`  
		Last Modified: Wed, 22 Dec 2021 00:30:44 GMT  
		Size: 9.4 KB (9365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2ecd004d56bd4ec22b8e38e688ddef82eafebf43ddea959b9a49c46894390a`  
		Last Modified: Wed, 22 Dec 2021 00:30:44 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a66f65c28615e1e4262e795ee5ba5a512edd071168b28aa52dbe38fb4a1da5d`  
		Last Modified: Wed, 22 Dec 2021 00:30:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0733f1ec4ae2efbbcd650badbfc855770814d1623cfce1667196fcf52b4da06d`  
		Last Modified: Tue, 04 Jan 2022 01:08:56 GMT  
		Size: 4.7 KB (4711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; ppc64le

```console
$ docker pull postgres@sha256:8897c1b12ff9674d67e555c9b8b2d46ef3981b419954a418e7fabd087dd75cb3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.5 MB (144532091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9aecf504b9aa1d53ee9ad0c6e3ee189d1061554e6fb9a217d643edc9f399a719`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Dec 2021 02:20:24 GMT
ADD file:078a17bf7e519cb7a60fbbf743ba7e5897554201cb44957154ab518d6991a033 in / 
# Tue, 21 Dec 2021 02:20:28 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 19:32:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 19:32:29 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 21 Dec 2021 19:32:32 GMT
ENV GOSU_VERSION=1.14
# Tue, 21 Dec 2021 19:33:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 21 Dec 2021 19:33:41 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 21 Dec 2021 19:33:45 GMT
ENV LANG=en_US.utf8
# Tue, 21 Dec 2021 19:34:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 19:34:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 21 Dec 2021 19:34:32 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 21 Dec 2021 19:37:09 GMT
ENV PG_MAJOR=13
# Tue, 21 Dec 2021 19:37:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 21 Dec 2021 19:37:13 GMT
ENV PG_VERSION=13.5-1.pgdg110+1
# Tue, 21 Dec 2021 19:39:22 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 21 Dec 2021 19:39:38 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 21 Dec 2021 19:39:46 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 21 Dec 2021 19:39:51 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 21 Dec 2021 19:39:56 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 21 Dec 2021 19:39:59 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 04 Jan 2022 01:17:49 GMT
COPY file:b2fac085615145a2bee98d4185ef0748655fa7c086ca21daef1ca6cac272bf59 in /usr/local/bin/ 
# Tue, 04 Jan 2022 01:17:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jan 2022 01:17:54 GMT
STOPSIGNAL SIGINT
# Tue, 04 Jan 2022 01:17:56 GMT
EXPOSE 5432
# Tue, 04 Jan 2022 01:17:58 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:3345479fea0cdce1382b927b0908af4f239b288b30efa203c50edf7ac0cb055e`  
		Last Modified: Tue, 21 Dec 2021 02:29:20 GMT  
		Size: 35.3 MB (35258992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08fad619d5e9b9134c50ee46d26ef57809bfd04852d94a70061b465fedc2585`  
		Last Modified: Tue, 21 Dec 2021 19:55:57 GMT  
		Size: 5.2 MB (5222905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7102b847099d38448e8497d5c9b44e7f49361334982bf01fda2a73889b9878`  
		Last Modified: Tue, 21 Dec 2021 19:55:53 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0c6341861b7e8f732f3cedf24bf499bd159fbeef06cc0fd930903f828d113b`  
		Last Modified: Tue, 21 Dec 2021 19:55:53 GMT  
		Size: 1.3 MB (1317578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371ec02786458e7b7790fdf8d336a55bed62bc6eedbd144764af964a5181ae0e`  
		Last Modified: Tue, 21 Dec 2021 19:55:54 GMT  
		Size: 8.0 MB (8045507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4be2382fa6b141791fb24b126e80a5bee7e0217eee2a2a84108bcf8e3552a59`  
		Last Modified: Tue, 21 Dec 2021 19:55:52 GMT  
		Size: 451.7 KB (451666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89eecb4fbb66e4fea8d2b8dea47313c87717e686ccd4171ca1596bf1105b5558`  
		Last Modified: Tue, 21 Dec 2021 19:55:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5242e0f07598b8e0622a3525e3dfeca963999a00291b9d74c727d0c15314f8fe`  
		Last Modified: Tue, 21 Dec 2021 19:55:49 GMT  
		Size: 3.1 KB (3058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40128690f3a8431c4f1a31fbe6242080516659e939e3fc3e9c501b56828a545d`  
		Last Modified: Tue, 21 Dec 2021 19:56:53 GMT  
		Size: 94.2 MB (94216017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9f85ee7be767c9d6167805599538422f29035c24e969f7e454df0e39388a38`  
		Last Modified: Tue, 21 Dec 2021 19:56:35 GMT  
		Size: 9.4 KB (9366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c4cf19d4d0c1809c82d0bb920d7443b0ae0f2e0c1a9796b5115b54e75924191`  
		Last Modified: Tue, 21 Dec 2021 19:56:35 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6d03bcd820e77679011af1338c2a7b7614ec606b6543982fe3669670d67d1f`  
		Last Modified: Tue, 21 Dec 2021 19:56:35 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9033873014b2d7c05f2b1a22adc64c70378b5b7bcd434337a47171a6a043a9d7`  
		Last Modified: Tue, 04 Jan 2022 01:23:34 GMT  
		Size: 4.7 KB (4715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; s390x

```console
$ docker pull postgres@sha256:0a325a9585ccc0fc5eed5e7f7ac7553992f513929b6444b620cf7d58e69247e7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.4 MB (139448044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de4518a8e979d36f6a890d036e4d2755c15fc07632e389c11ad602f01ca4540d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:13 GMT
ADD file:03b224b82f458b08d3b5071e42b67915a3db309332c0fc9229db7cf1148bc1b5 in / 
# Wed, 26 Jan 2022 01:41:15 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 07:32:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 07:32:30 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 26 Jan 2022 07:32:30 GMT
ENV GOSU_VERSION=1.14
# Wed, 26 Jan 2022 07:32:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 26 Jan 2022 07:32:43 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 26 Jan 2022 07:32:44 GMT
ENV LANG=en_US.utf8
# Wed, 26 Jan 2022 07:32:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 07:32:48 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 26 Jan 2022 07:33:20 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Wed, 26 Jan 2022 07:43:01 GMT
ENV PG_MAJOR=13
# Wed, 26 Jan 2022 07:43:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Wed, 26 Jan 2022 07:43:01 GMT
ENV PG_VERSION=13.5-1.pgdg110+1
# Wed, 26 Jan 2022 07:51:44 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 26 Jan 2022 07:51:50 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 26 Jan 2022 07:51:50 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 26 Jan 2022 07:51:50 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 26 Jan 2022 07:51:51 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 26 Jan 2022 07:51:51 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 26 Jan 2022 07:51:51 GMT
COPY file:b2fac085615145a2bee98d4185ef0748655fa7c086ca21daef1ca6cac272bf59 in /usr/local/bin/ 
# Wed, 26 Jan 2022 07:51:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 07:51:52 GMT
STOPSIGNAL SIGINT
# Wed, 26 Jan 2022 07:51:52 GMT
EXPOSE 5432
# Wed, 26 Jan 2022 07:51:52 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:70bed29526f8483937e4d2540d19256d30786007c7c321e717e00d2e74700380`  
		Last Modified: Wed, 26 Jan 2022 01:46:57 GMT  
		Size: 29.6 MB (29647071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adab0b82ec25a88edeaf5e951f0f97b4b3f541b0a9f855ad9bdbab5ec3b82258`  
		Last Modified: Wed, 26 Jan 2022 08:21:41 GMT  
		Size: 4.3 MB (4302200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32845bcd9646d96ac1ebedc163e8b332b93ec5e381b7adb28b4e048446a479c`  
		Last Modified: Wed, 26 Jan 2022 08:21:40 GMT  
		Size: 1.8 KB (1800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db75c1a18cfc37dc49d94fcdf1fe55bf7a3958cd66472580b982daf1dcd60559`  
		Last Modified: Wed, 26 Jan 2022 08:21:40 GMT  
		Size: 1.4 MB (1381382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f042f08b8d2c3c370464daac9b5ca277fd2a7a01d201191427aa3d54d62dcd`  
		Last Modified: Wed, 26 Jan 2022 08:21:40 GMT  
		Size: 8.1 MB (8098986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb531aa668e0f5cb99281939a526713946c9f8b6e071f14fb2a9d9dccdc9fb3`  
		Last Modified: Wed, 26 Jan 2022 08:21:38 GMT  
		Size: 438.3 KB (438285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d904e25ceb71481a5b408ee7254f7e4c6744d23294351859f7ff73ddfeb9f2`  
		Last Modified: Wed, 26 Jan 2022 08:21:39 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce09051744ed10c4ffd4e9537e54551dd68775dcfc11b633dfa6765c67e258c`  
		Last Modified: Wed, 26 Jan 2022 08:21:39 GMT  
		Size: 3.1 KB (3058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae783c62633b83572f548ba9e937d0c62b5e0c46f95e57aa6d385e9f9294f99`  
		Last Modified: Wed, 26 Jan 2022 08:22:29 GMT  
		Size: 95.6 MB (95560701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a0ab72b9601066bc0799b453f1a963042b0a2a8828a99856e0157a1e8ebae9`  
		Last Modified: Wed, 26 Jan 2022 08:22:17 GMT  
		Size: 9.4 KB (9364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8188b3d754b5dfb0dcd62d3e104f99db88b7002c2b3547bc78cedc2a943d74c`  
		Last Modified: Wed, 26 Jan 2022 08:22:16 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356d9d352675eeea657e0142d474660141773f359b4f4a08662b878149104bcf`  
		Last Modified: Wed, 26 Jan 2022 08:22:16 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de478b1892bbc2197439277f9a0aa52e96cfd3757e57b6307a35c79f622cb8e6`  
		Last Modified: Wed, 26 Jan 2022 08:22:16 GMT  
		Size: 4.7 KB (4718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
