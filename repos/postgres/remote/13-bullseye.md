## `postgres:13-bullseye`

```console
$ docker pull postgres@sha256:155651966455c71ba73eb61db66068cbc2cb69c6f8bf2e9ee7f05211914b0a38
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
$ docker pull postgres@sha256:63917f87713702de5f92797e869dfb94865220fbc5f479868c6dadaa9ad058bc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.7 MB (135727369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d351c95a98509183288e37d6f3b7fd58e2baf4b7ceb3f15c3b4e0e566276b68`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:41 GMT
ADD file:a2405ebb9892d98be2eb585f6121864d12b3fd983ebf15e5f0b7486e106a79c6 in / 
# Wed, 17 Nov 2021 02:20:42 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 21:54:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 21:54:51 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 30 Nov 2021 04:58:24 GMT
ENV GOSU_VERSION=1.14
# Tue, 30 Nov 2021 04:58:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 30 Nov 2021 04:58:41 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 30 Nov 2021 04:58:41 GMT
ENV LANG=en_US.utf8
# Tue, 30 Nov 2021 04:58:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Nov 2021 04:58:47 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 30 Nov 2021 04:58:51 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 30 Nov 2021 05:08:26 GMT
ENV PG_MAJOR=13
# Tue, 30 Nov 2021 05:08:26 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 30 Nov 2021 05:08:27 GMT
ENV PG_VERSION=13.5-1.pgdg110+1
# Tue, 30 Nov 2021 05:08:46 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 30 Nov 2021 05:08:48 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 30 Nov 2021 05:08:49 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 30 Nov 2021 05:08:49 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 30 Nov 2021 05:08:50 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 30 Nov 2021 05:08:50 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 30 Nov 2021 05:08:50 GMT
COPY file:6e4de9271291e4bdd4a40b73fffe4d6d1aeff033460f5b14d74e948686daa095 in /usr/local/bin/ 
# Tue, 30 Nov 2021 05:08:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 Nov 2021 05:08:51 GMT
STOPSIGNAL SIGINT
# Tue, 30 Nov 2021 05:08:51 GMT
EXPOSE 5432
# Tue, 30 Nov 2021 05:08:51 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:eff15d958d664f0874d16aee393cc44387031ee0a68ef8542d0056c747f378e8`  
		Last Modified: Wed, 17 Nov 2021 02:25:45 GMT  
		Size: 31.4 MB (31370267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2b4ab3ade5ac7d8afea5bd7c2ba3747bcbeedcffa046a29b403f0fb358691c`  
		Last Modified: Wed, 17 Nov 2021 22:01:37 GMT  
		Size: 4.4 MB (4414468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108afa831d95d33af5adc9360a1bf1e5635459bb3ec8e3d9bd2ceb1c82b2632c`  
		Last Modified: Wed, 17 Nov 2021 22:01:36 GMT  
		Size: 1.8 KB (1794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f36a620c9a0d4789b1cc287e7cbc0fdb05a9de195131783608c7e5768b845e`  
		Last Modified: Tue, 30 Nov 2021 05:48:14 GMT  
		Size: 1.4 MB (1418386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c78220cdd7f632a539dc45b5f88e431dc0504bdd21f7c20b37985d747abc379`  
		Last Modified: Tue, 30 Nov 2021 05:48:14 GMT  
		Size: 8.0 MB (8045287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7fc8d555476ac466ce5474480981d09392b67fee009c0faebf7548ab5b4bb02`  
		Last Modified: Tue, 30 Nov 2021 05:48:12 GMT  
		Size: 441.6 KB (441629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf6f19a1e0f722a85c250ed5f0c54bbe44cd12e9ff87dee3fb8580c21402116`  
		Last Modified: Tue, 30 Nov 2021 05:48:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5367c24392415d54d11bea3e29d555f55dd363f7fb49cf9bd08a7793f575b6c7`  
		Last Modified: Tue, 30 Nov 2021 05:48:11 GMT  
		Size: 3.1 KB (3057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64bc7d70f1cca20fcc250cc03d5dea3b55a48cda52f32daed9ad1147c0da472`  
		Last Modified: Tue, 30 Nov 2021 05:49:45 GMT  
		Size: 90.0 MB (90017937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef4f481a727ef413e0ace0a87f89dfe90cc15412a27dcf5e755b921c73813ab`  
		Last Modified: Tue, 30 Nov 2021 05:49:28 GMT  
		Size: 9.4 KB (9353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965b11f6bf7bee080201d73c9bcec70f94a35b0679960508765a91e8621016bf`  
		Last Modified: Tue, 30 Nov 2021 05:49:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8076d08e9bcfb305bcd682e40e4d24ef01a1727cee279083346845b6b256d219`  
		Last Modified: Tue, 30 Nov 2021 05:49:28 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2340e84c9fe19975415993b4caa138a0365249b68eda621e3e7afd07e0df2d10`  
		Last Modified: Tue, 30 Nov 2021 05:49:28 GMT  
		Size: 4.7 KB (4713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; arm variant v5

```console
$ docker pull postgres@sha256:18e8e0f2588a293dd3104b76ff517aa0d45eb10a77e845a102ab22c8751017c2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.0 MB (128993688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a15fc086b5f34bc142c8d47b5197d4deec08c649209558739c96a4a8bbefa9b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:37 GMT
ADD file:7debbdb237139cb08189976f79cfa64cfd71f5cc98dfb2f560b558acb5f7cec9 in / 
# Thu, 02 Dec 2021 02:50:38 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 05:52:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 05:52:34 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 02 Dec 2021 05:52:35 GMT
ENV GOSU_VERSION=1.14
# Thu, 02 Dec 2021 05:53:18 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 02 Dec 2021 05:53:50 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 02 Dec 2021 05:53:51 GMT
ENV LANG=en_US.utf8
# Thu, 02 Dec 2021 05:54:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 05:54:13 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 02 Dec 2021 05:54:20 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Thu, 02 Dec 2021 06:39:25 GMT
ENV PG_MAJOR=13
# Thu, 02 Dec 2021 06:39:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Thu, 02 Dec 2021 06:39:27 GMT
ENV PG_VERSION=13.5-1.pgdg110+1
# Thu, 02 Dec 2021 07:15:58 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 02 Dec 2021 07:16:00 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 02 Dec 2021 07:16:02 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 02 Dec 2021 07:16:02 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 02 Dec 2021 07:16:04 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 02 Dec 2021 07:16:04 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 02 Dec 2021 07:16:05 GMT
COPY file:6e4de9271291e4bdd4a40b73fffe4d6d1aeff033460f5b14d74e948686daa095 in /usr/local/bin/ 
# Thu, 02 Dec 2021 07:16:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Dec 2021 07:16:06 GMT
STOPSIGNAL SIGINT
# Thu, 02 Dec 2021 07:16:06 GMT
EXPOSE 5432
# Thu, 02 Dec 2021 07:16:07 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:c5e429166894878430c39748965935f89ffa957667340c3c8bd872418dbce663`  
		Last Modified: Thu, 02 Dec 2021 03:09:28 GMT  
		Size: 28.9 MB (28910824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f60a47a77ecd85f55cb86a1bbd52e1d71e4b1cc64729485f013666cbf3b7754`  
		Last Modified: Thu, 02 Dec 2021 10:13:56 GMT  
		Size: 4.1 MB (4096455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d7ac3caf6c6d6382e415a80e002059b10cd2d2ac29790efe3c378e5653b758`  
		Last Modified: Thu, 02 Dec 2021 10:13:52 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f7551cebf281f85d430c3d41bdf156cdc5bcf70441e014c33382352e6c57df`  
		Last Modified: Thu, 02 Dec 2021 10:13:52 GMT  
		Size: 1.4 MB (1382572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022b63548e5c214f3e84a6208f5ca268fe38569c1786cf238e0cb1898623701e`  
		Last Modified: Thu, 02 Dec 2021 10:13:56 GMT  
		Size: 8.0 MB (8045250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3def92217ba508b5ee7bbd9f26186535f0efb51932e23fe6ab7c0d33536ac73d`  
		Last Modified: Thu, 02 Dec 2021 10:13:50 GMT  
		Size: 439.9 KB (439870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485106e7312a474e6737309cf50ebf57a38496b15ff49d0730d26a678fe085f2`  
		Last Modified: Thu, 02 Dec 2021 10:13:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a834947911a91355cf5d0732cf9dbf976de0da7755a860daf52f776677cbfd2`  
		Last Modified: Thu, 02 Dec 2021 10:13:50 GMT  
		Size: 3.1 KB (3057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e04dc599ea1a6ab8b5d4b3c277e468cb60ce7d0ce9adf926cbe3a31aea63a2c1`  
		Last Modified: Thu, 02 Dec 2021 10:16:23 GMT  
		Size: 86.1 MB (86099310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbae8d1973868c3847bcedeb34ba09cb7538ba5a55bceb45607584b519d18df`  
		Last Modified: Thu, 02 Dec 2021 10:15:28 GMT  
		Size: 9.4 KB (9356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3865d0e003d811afe151976710f6aa3e4319e3780f3d2db744b092816e545e8a`  
		Last Modified: Thu, 02 Dec 2021 10:15:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d977807120fa3cedee243ad6060c1bd9c8f1b3b468d3c6f953e50b75aa0a64`  
		Last Modified: Thu, 02 Dec 2021 10:15:28 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da679c90f099c2ea816f434d02006332b0a1e8ce73b8e25fe50eef199d10e4b`  
		Last Modified: Thu, 02 Dec 2021 10:15:28 GMT  
		Size: 4.7 KB (4719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; arm variant v7

```console
$ docker pull postgres@sha256:27b2136cefe59ea8f9d758ad9a4619c760de45df3841e9df19924af9926aaa82
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.8 MB (123847029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f168e3600828adba816fe3e5e69a1261e56bac87d29ba30b8110d892a8371f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 17 Nov 2021 01:59:43 GMT
ADD file:cd2ac52107a2ea6657f23850a4b29366309eb39fa177321e0a9fd6d58562ae80 in / 
# Wed, 17 Nov 2021 01:59:44 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 18:03:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 18:03:08 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 30 Nov 2021 07:09:33 GMT
ENV GOSU_VERSION=1.14
# Tue, 30 Nov 2021 07:09:54 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 30 Nov 2021 07:10:14 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 30 Nov 2021 07:10:14 GMT
ENV LANG=en_US.utf8
# Tue, 30 Nov 2021 07:10:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Nov 2021 07:10:26 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 30 Nov 2021 07:10:34 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 30 Nov 2021 07:50:27 GMT
ENV PG_MAJOR=13
# Tue, 30 Nov 2021 07:50:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 30 Nov 2021 07:50:28 GMT
ENV PG_VERSION=13.5-1.pgdg110+1
# Tue, 30 Nov 2021 08:23:01 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 30 Nov 2021 08:23:03 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 30 Nov 2021 08:23:05 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 30 Nov 2021 08:23:05 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 30 Nov 2021 08:23:07 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 30 Nov 2021 08:23:08 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 30 Nov 2021 08:23:09 GMT
COPY file:6e4de9271291e4bdd4a40b73fffe4d6d1aeff033460f5b14d74e948686daa095 in /usr/local/bin/ 
# Tue, 30 Nov 2021 08:23:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 Nov 2021 08:23:10 GMT
STOPSIGNAL SIGINT
# Tue, 30 Nov 2021 08:23:10 GMT
EXPOSE 5432
# Tue, 30 Nov 2021 08:23:11 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:b6e5ca4da96841e58eb27c88695a059e5105fad5a066de803f4b94ae4002ba66`  
		Last Modified: Wed, 17 Nov 2021 02:15:13 GMT  
		Size: 26.6 MB (26573160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ef876aa8c0afe0078ed4f8132182e2d6c94a884d4dce472cea77744820bc9fb`  
		Last Modified: Wed, 17 Nov 2021 22:13:45 GMT  
		Size: 3.7 MB (3717163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74a37ede70c9a36c8032109fff79b082ee9060ea110a45d59ead46d5f42159b`  
		Last Modified: Wed, 17 Nov 2021 22:13:43 GMT  
		Size: 1.8 KB (1794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512368ab2ae9393a1e8075b4e097142f06e628816f2f39508ac881ccb2be4c7f`  
		Last Modified: Tue, 30 Nov 2021 12:09:12 GMT  
		Size: 1.4 MB (1375247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b31c45adf2ad134826a5a0dfa1eed1c98beee40539b5e0a75e8582e1e9bb60e`  
		Last Modified: Tue, 30 Nov 2021 12:09:16 GMT  
		Size: 8.0 MB (8045279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece0a24dac3eb00428c4a625a308107d197324bf5f1977d6e7ac1c7b09d5b5f8`  
		Last Modified: Tue, 30 Nov 2021 12:09:10 GMT  
		Size: 434.5 KB (434534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6bf5ab83150f790dc4534ead8017e642c451f6390529446400764a8f9c77e4`  
		Last Modified: Tue, 30 Nov 2021 12:09:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c0456a3f47ec242d9e2cb85fff00e29aeec8a3ac1326d3a3bcc7c2d42e55664`  
		Last Modified: Tue, 30 Nov 2021 12:09:10 GMT  
		Size: 3.1 KB (3057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbd99403fd6373adb5b8b9995f74ad7bc4d6d3556ec7d6ed4a355a376c0e00a`  
		Last Modified: Tue, 30 Nov 2021 12:12:27 GMT  
		Size: 83.7 MB (83682234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a968e751e3198cff71d7b5f0ab670473164d6fa23f478b3fad03e2fd91c0cf6`  
		Last Modified: Tue, 30 Nov 2021 12:11:37 GMT  
		Size: 9.4 KB (9364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4842a35ceabdfd338c298543c7c193cb845eb28257cea1ac2f424c76230dab4`  
		Last Modified: Tue, 30 Nov 2021 12:11:37 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7226cd8c8390b45b9478cb8b7f03f6fdf7b44f2499304fa4bbf134057e6420b6`  
		Last Modified: Tue, 30 Nov 2021 12:11:37 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48f8f16adb6fd69b7391d5af18284fe10ed79c806e59628147c21d862057734`  
		Last Modified: Tue, 30 Nov 2021 12:11:37 GMT  
		Size: 4.7 KB (4716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:4b2e99c8bddc9c3d35ee774063bc097fedba5df95377fdffb2ddcb8d48894403
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130402487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a05c0a9d5714cd4f5b87d3289491f1902dbc5c78a747b644032c8138389a4d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:09 GMT
ADD file:002f2f7c6dc806b24b6c365882acd59d2b3d3fcec46d8fd99130b07a4575c88c in / 
# Thu, 02 Dec 2021 08:08:10 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:21:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 14:21:11 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 02 Dec 2021 14:21:12 GMT
ENV GOSU_VERSION=1.14
# Thu, 02 Dec 2021 14:21:20 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 02 Dec 2021 14:21:27 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 02 Dec 2021 14:21:28 GMT
ENV LANG=en_US.utf8
# Thu, 02 Dec 2021 14:21:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 14:21:33 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 02 Dec 2021 14:21:43 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Thu, 02 Dec 2021 14:22:39 GMT
ENV PG_MAJOR=13
# Thu, 02 Dec 2021 14:22:40 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Thu, 02 Dec 2021 14:22:41 GMT
ENV PG_VERSION=13.5-1.pgdg110+1
# Thu, 02 Dec 2021 14:23:02 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 02 Dec 2021 14:23:03 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 02 Dec 2021 14:23:04 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 02 Dec 2021 14:23:05 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 02 Dec 2021 14:23:06 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 02 Dec 2021 14:23:07 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 02 Dec 2021 14:23:09 GMT
COPY file:6e4de9271291e4bdd4a40b73fffe4d6d1aeff033460f5b14d74e948686daa095 in /usr/local/bin/ 
# Thu, 02 Dec 2021 14:23:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Dec 2021 14:23:10 GMT
STOPSIGNAL SIGINT
# Thu, 02 Dec 2021 14:23:11 GMT
EXPOSE 5432
# Thu, 02 Dec 2021 14:23:12 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:968621624b326084ed82349252b333e649eaab39f71866edb2b9a4f847283680`  
		Last Modified: Thu, 02 Dec 2021 08:40:45 GMT  
		Size: 30.1 MB (30056536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef9c0761899cb5b74e8aedb2644173870ecb40e685469fc36fa719afddd0ef3`  
		Last Modified: Thu, 02 Dec 2021 14:56:27 GMT  
		Size: 4.2 MB (4208852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:effb6e89256d9346ccf3f3b96274206d1593283743a31f956990b4ee75ef57fb`  
		Last Modified: Thu, 02 Dec 2021 14:56:26 GMT  
		Size: 1.7 KB (1652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19a7fe239e090b9d966d00268c043597a5a8007f845524f679f806b1347aea8`  
		Last Modified: Thu, 02 Dec 2021 14:56:27 GMT  
		Size: 1.3 MB (1346022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f97626b93ace1f49117c0c2d0997c9febb77d3050e3d479fdc62a7acf675c3a`  
		Last Modified: Thu, 02 Dec 2021 14:56:25 GMT  
		Size: 8.0 MB (8043389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc35a9a2c7cfcd76c65584eba5ee71257b34fc95a824abf6664bb9a87b57122`  
		Last Modified: Thu, 02 Dec 2021 14:56:24 GMT  
		Size: 218.6 KB (218587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b749e660435b374a3db49f2f0d3ede5b76c20ae067155b1173b6726ad539e1fa`  
		Last Modified: Thu, 02 Dec 2021 14:56:23 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457ea4f6253aef008eb78d932559c730b87d735aac0db0413b29be59f5ea7d63`  
		Last Modified: Thu, 02 Dec 2021 14:56:23 GMT  
		Size: 3.0 KB (3031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722af21d2ec3d34b4305a32f2500bbbb7cbc3db32eefadfe7396886083f23cd1`  
		Last Modified: Thu, 02 Dec 2021 14:57:15 GMT  
		Size: 86.5 MB (86509933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899eee526623bc2b253bb1f97fbf2d94ff068d3818fe2a143ef2ad9528ec34de`  
		Last Modified: Thu, 02 Dec 2021 14:57:03 GMT  
		Size: 9.4 KB (9354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746f304547aa619e947b1d0ba9d96fa220458408ed917e166effaefcd0f9ff83`  
		Last Modified: Thu, 02 Dec 2021 14:57:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4dfc6819e660b4521c5e8f88cce73ad7bce4d0428e4378dcc98830971ca293`  
		Last Modified: Thu, 02 Dec 2021 14:57:02 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99864ddd548ff50884e27018f57dc88001003b77a1a75db4d9dee1a55ea5d65`  
		Last Modified: Thu, 02 Dec 2021 14:57:03 GMT  
		Size: 4.7 KB (4717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; 386

```console
$ docker pull postgres@sha256:7aab658cd42f65f1349638bbee8a8cf6982c1b4f545b80dc6b39d7bb4fd71733
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137819323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:631b3aa44dbc0a72a4fd857c7e42cb602e724590891c3c04e0636969c3b82d83`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:53 GMT
ADD file:ff018048717c0f5aa1730480d0bfea1c2bf94d6e2dae2d7cef46d05ffb0d93e1 in / 
# Wed, 17 Nov 2021 02:39:53 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:42:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:42:31 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 30 Nov 2021 02:22:34 GMT
ENV GOSU_VERSION=1.14
# Tue, 30 Nov 2021 02:23:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 30 Nov 2021 02:23:16 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 30 Nov 2021 02:23:17 GMT
ENV LANG=en_US.utf8
# Tue, 30 Nov 2021 02:23:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Nov 2021 02:23:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 30 Nov 2021 02:23:25 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 30 Nov 2021 02:50:08 GMT
ENV PG_MAJOR=13
# Tue, 30 Nov 2021 02:50:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 30 Nov 2021 02:50:08 GMT
ENV PG_VERSION=13.5-1.pgdg110+1
# Tue, 30 Nov 2021 03:06:04 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 30 Nov 2021 03:06:07 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 30 Nov 2021 03:06:08 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 30 Nov 2021 03:06:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 30 Nov 2021 03:06:09 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 30 Nov 2021 03:06:09 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 30 Nov 2021 03:06:10 GMT
COPY file:6e4de9271291e4bdd4a40b73fffe4d6d1aeff033460f5b14d74e948686daa095 in /usr/local/bin/ 
# Tue, 30 Nov 2021 03:06:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 Nov 2021 03:06:10 GMT
STOPSIGNAL SIGINT
# Tue, 30 Nov 2021 03:06:10 GMT
EXPOSE 5432
# Tue, 30 Nov 2021 03:06:11 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:0bae0e1d4cb1d56ffeb9d05de7a097d3157267eef07b6d8131344d99bd97c431`  
		Last Modified: Wed, 17 Nov 2021 02:47:49 GMT  
		Size: 32.4 MB (32380683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47dc0c82cbdb8d80bc1e74add189651c4ffd82853181cb884190c0781a720bb`  
		Last Modified: Wed, 17 Nov 2021 15:21:35 GMT  
		Size: 4.8 MB (4812958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a5817009e5bad1ebe7c8bdaeb9bf7528a1dbf5f160bb79da932163b814a887`  
		Last Modified: Wed, 17 Nov 2021 15:21:33 GMT  
		Size: 1.8 KB (1791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9224d92437c5d642dc59456a1db1b95f8a3b56a04f34f3caaf91e85ad55ee1b7`  
		Last Modified: Tue, 30 Nov 2021 04:42:56 GMT  
		Size: 1.4 MB (1385584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b188aabed17ad4819a6802ce244fe2ae1ad0abc44cc8b45d61a0745a50fa86`  
		Last Modified: Tue, 30 Nov 2021 04:42:56 GMT  
		Size: 8.0 MB (8045186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ffbc79a6052c96f094712da112483d243d8fc9f67b1933bca51bd977c020fc`  
		Last Modified: Tue, 30 Nov 2021 04:42:53 GMT  
		Size: 448.1 KB (448065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e49a8f355f9a7ad2b204f215d77c352a4a2d00004dbd9bb5cb142564f545a9`  
		Last Modified: Tue, 30 Nov 2021 04:42:53 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1b3e8bea3acd7a497b47480f01ccde1bdafbcb01ff320a37a4e56a79d3c453`  
		Last Modified: Tue, 30 Nov 2021 04:42:53 GMT  
		Size: 3.1 KB (3054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ce39595a50b78af7b5579e9b5b42fd0a985a19a32f54f52c2d69499893b3ea`  
		Last Modified: Tue, 30 Nov 2021 04:44:45 GMT  
		Size: 90.7 MB (90727441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655e02481a3f70574b8a8e71c545f9ced944e32c883302c99976986ca5e96576`  
		Last Modified: Tue, 30 Nov 2021 04:44:23 GMT  
		Size: 9.4 KB (9357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cbeed3eda7e3b09cfe52f8e0474cfbe87ef90149041509c54594ab62ba50278`  
		Last Modified: Tue, 30 Nov 2021 04:44:23 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f799df37d04d0e6ba3e2af4ce515d3075367f8eeaf540241500ed2c06a46ca94`  
		Last Modified: Tue, 30 Nov 2021 04:44:23 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5982c8081167113fede7ed7a20129ae2b7ccb15ca65f2a5a3e55c3c2305320`  
		Last Modified: Tue, 30 Nov 2021 04:44:23 GMT  
		Size: 4.7 KB (4723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; mips64le

```console
$ docker pull postgres@sha256:0f5e1619e550be0d98252a3855f259c49e149c79bbcf4d6aad506fe58fa4454c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.5 MB (130544885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:199805fb1048ac2f0e8cd0e3d2f30cee93f3f27d8f860b2671f7140de72f0880`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 17 Nov 2021 02:10:13 GMT
ADD file:10bc783d286d0a800f59d5009e87ecb4651659c82cae1325132756c7c8b1dec0 in / 
# Wed, 17 Nov 2021 02:10:13 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:38:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:38:48 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 30 Nov 2021 03:51:38 GMT
ENV GOSU_VERSION=1.14
# Tue, 30 Nov 2021 03:51:59 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 30 Nov 2021 03:52:23 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 30 Nov 2021 03:52:24 GMT
ENV LANG=en_US.utf8
# Tue, 30 Nov 2021 03:52:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Nov 2021 03:52:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 30 Nov 2021 03:52:41 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 30 Nov 2021 04:48:48 GMT
ENV PG_MAJOR=13
# Tue, 30 Nov 2021 04:48:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 30 Nov 2021 04:48:49 GMT
ENV PG_VERSION=13.5-1.pgdg110+1
# Tue, 30 Nov 2021 05:41:37 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 30 Nov 2021 05:41:40 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 30 Nov 2021 05:41:42 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 30 Nov 2021 05:41:43 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 30 Nov 2021 05:41:45 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 30 Nov 2021 05:41:45 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 30 Nov 2021 05:41:45 GMT
COPY file:6e4de9271291e4bdd4a40b73fffe4d6d1aeff033460f5b14d74e948686daa095 in /usr/local/bin/ 
# Tue, 30 Nov 2021 05:41:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 Nov 2021 05:41:46 GMT
STOPSIGNAL SIGINT
# Tue, 30 Nov 2021 05:41:46 GMT
EXPOSE 5432
# Tue, 30 Nov 2021 05:41:47 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:08bca22fbffb4e58224e9e4f6a56f1ca5099c002b1aeb6181df63af308a3da58`  
		Last Modified: Wed, 17 Nov 2021 02:19:09 GMT  
		Size: 29.6 MB (29630388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173240a7e67fd44ecc0ad5edd818557628d50f00c5d2a5f3d580e0a2ac091610`  
		Last Modified: Wed, 17 Nov 2021 08:20:21 GMT  
		Size: 4.4 MB (4402817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5442a27e75e2c0fbbf3bcf39b1c33f75d31863490f96ba2f0f1921ef6da25caf`  
		Last Modified: Wed, 17 Nov 2021 08:20:17 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2054e4460d2a19717dd4a336b47653df9571eda928f0f361edc1ab86244ddcc2`  
		Last Modified: Tue, 30 Nov 2021 08:33:27 GMT  
		Size: 1.3 MB (1298194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7d76eb66b099fba3c2444676a5f23198b89f04ca562d92fe3cbad93e17ed6f`  
		Last Modified: Tue, 30 Nov 2021 08:33:31 GMT  
		Size: 8.0 MB (8043954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde934ccf5b463f3cc67c5e044fdb538461feed010e478a8adb22f25017f220b`  
		Last Modified: Tue, 30 Nov 2021 08:33:24 GMT  
		Size: 439.2 KB (439195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0517cbc7ba02213b80d94a9809694781806502aef56896f981df723099874173`  
		Last Modified: Tue, 30 Nov 2021 08:33:23 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ff4ee65102820557350a5542a9ce98ad5efe0fcb3cf0a382b9ef99f9850a99`  
		Last Modified: Tue, 30 Nov 2021 08:33:23 GMT  
		Size: 3.1 KB (3052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44ee210e0e98afe9468574891e854b1d424b87923108bb695c444c3f5329ca8`  
		Last Modified: Tue, 30 Nov 2021 08:35:52 GMT  
		Size: 86.7 MB (86711020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0d4a1893e5a23501124c21d741cfb196c6a9a34650e44ef076bba7b2809a27`  
		Last Modified: Tue, 30 Nov 2021 08:34:52 GMT  
		Size: 9.4 KB (9364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd544c4c49b8b8da1e32306b5e13b6abbb26b39796028293ab8971624dd45d5`  
		Last Modified: Tue, 30 Nov 2021 08:34:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14918a9c5e77d2201142f8f42f2709897ebcb4e441467632d4181aa37398587`  
		Last Modified: Tue, 30 Nov 2021 08:34:52 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da75bc19eaee2a5ff0e66fc4d9556e384adbaea95ad67610815baecd4c309d8`  
		Last Modified: Tue, 30 Nov 2021 08:34:52 GMT  
		Size: 4.7 KB (4720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; ppc64le

```console
$ docker pull postgres@sha256:cd77b177c8ef04c0b6cad21922fec38ceac7cc8ced772435ed27f39b3c236e80
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.5 MB (144544078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce0bbd2d1a1379e39aab64f6eb5450c166b460e733a5e69d920254f982fb0558`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 17 Nov 2021 03:28:22 GMT
ADD file:5ed330f0fe1328f694fcaefb961cf4da4d8a4ff03100b21af718b69316168706 in / 
# Wed, 17 Nov 2021 03:28:38 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 12:35:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 12:35:29 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 30 Nov 2021 04:22:31 GMT
ENV GOSU_VERSION=1.14
# Tue, 30 Nov 2021 04:23:03 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 30 Nov 2021 04:23:22 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 30 Nov 2021 04:23:25 GMT
ENV LANG=en_US.utf8
# Tue, 30 Nov 2021 04:23:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Nov 2021 04:23:52 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 30 Nov 2021 04:24:02 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 30 Nov 2021 04:33:09 GMT
ENV PG_MAJOR=13
# Tue, 30 Nov 2021 04:33:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 30 Nov 2021 04:33:12 GMT
ENV PG_VERSION=13.5-1.pgdg110+1
# Tue, 30 Nov 2021 04:34:16 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 30 Nov 2021 04:34:28 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 30 Nov 2021 04:34:38 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 30 Nov 2021 04:34:42 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 30 Nov 2021 04:34:50 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 30 Nov 2021 04:34:56 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 30 Nov 2021 04:34:59 GMT
COPY file:6e4de9271291e4bdd4a40b73fffe4d6d1aeff033460f5b14d74e948686daa095 in /usr/local/bin/ 
# Tue, 30 Nov 2021 04:35:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 Nov 2021 04:35:07 GMT
STOPSIGNAL SIGINT
# Tue, 30 Nov 2021 04:35:12 GMT
EXPOSE 5432
# Tue, 30 Nov 2021 04:35:16 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:258ff2a13858db8f51b65662e02137c0abcfd2528ca73e92b7a40061d938fb1e`  
		Last Modified: Wed, 17 Nov 2021 03:54:34 GMT  
		Size: 35.3 MB (35271382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b509e11eadbd1f0594371e0c0328a97ea632aee62bcb4d80035bf0eb4e27d9`  
		Last Modified: Wed, 17 Nov 2021 12:54:55 GMT  
		Size: 5.2 MB (5222878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7098bb2fd895d09bedc6646b1f22374ade668fedde3c9f80a50c9c2608420a5b`  
		Last Modified: Wed, 17 Nov 2021 12:54:52 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35b2a8dfe6aeea228d81c43283e5a62e5953809f4a37c66206ba07e6b1f8627`  
		Last Modified: Tue, 30 Nov 2021 05:09:39 GMT  
		Size: 1.3 MB (1317537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c1943e77464726e531ba0fa41402bf8b74e45d88b2f66a3ac4d88c8e91445d`  
		Last Modified: Tue, 30 Nov 2021 05:09:41 GMT  
		Size: 8.0 MB (8045492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43663cab90f09a0a9f91d3d042e111627e277fe2a8787747840d43232f316b3`  
		Last Modified: Tue, 30 Nov 2021 05:09:35 GMT  
		Size: 451.6 KB (451618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f804f299ce3f30a2131f474586ce820567662cf36273a04aff65c57497ee55fb`  
		Last Modified: Tue, 30 Nov 2021 05:09:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f36786db7d917c78021991cf37d395dd46c97e91ea5290fbb7f25d7bcbd318`  
		Last Modified: Tue, 30 Nov 2021 05:09:35 GMT  
		Size: 3.1 KB (3053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a05f1c9c5ba595edd404b8c252127304e5c32942660bd4434440fe00cc049938`  
		Last Modified: Tue, 30 Nov 2021 05:12:05 GMT  
		Size: 94.2 MB (94215752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b8b6f4b6a287d26d266a883e85bfda00c8442f55c78016292d30b30a63b2f18`  
		Last Modified: Tue, 30 Nov 2021 05:11:47 GMT  
		Size: 9.4 KB (9362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b824eb392c818165bd848536634e77621ea804f6e92098c4cca8cd6704d835`  
		Last Modified: Tue, 30 Nov 2021 05:11:47 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b11c776e398378c49f502b56451cdd8f52349bdf707972faa17df096d8ce23e`  
		Last Modified: Tue, 30 Nov 2021 05:11:47 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae40d03191ff62a3263d3e6a502f9e168245d9d708bed34ae19afda5d2c5883`  
		Last Modified: Tue, 30 Nov 2021 05:11:47 GMT  
		Size: 4.7 KB (4719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; s390x

```console
$ docker pull postgres@sha256:625074b198b968d959cb3394b5361ba2724cc7c3c4783512948b8f3b7f362ad6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139451693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf755b0415366c93cb13263d6598046d5df2cf5ffd9ea652ddd696ef2ec90e4b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 02 Dec 2021 07:19:07 GMT
ADD file:9303def035f391c14bdca007751c5061f36fe929d5b3f4d725ce376e25f7dd36 in / 
# Thu, 02 Dec 2021 07:19:09 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 08:57:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 08:57:56 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 02 Dec 2021 08:57:56 GMT
ENV GOSU_VERSION=1.14
# Thu, 02 Dec 2021 08:58:03 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 02 Dec 2021 08:58:09 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 02 Dec 2021 08:58:10 GMT
ENV LANG=en_US.utf8
# Thu, 02 Dec 2021 08:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 08:58:14 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 02 Dec 2021 08:58:15 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Thu, 02 Dec 2021 09:08:01 GMT
ENV PG_MAJOR=13
# Thu, 02 Dec 2021 09:08:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Thu, 02 Dec 2021 09:08:01 GMT
ENV PG_VERSION=13.5-1.pgdg110+1
# Thu, 02 Dec 2021 09:16:55 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 02 Dec 2021 09:16:59 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 02 Dec 2021 09:17:00 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 02 Dec 2021 09:17:00 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 02 Dec 2021 09:17:01 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 02 Dec 2021 09:17:01 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 02 Dec 2021 09:17:01 GMT
COPY file:6e4de9271291e4bdd4a40b73fffe4d6d1aeff033460f5b14d74e948686daa095 in /usr/local/bin/ 
# Thu, 02 Dec 2021 09:17:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Dec 2021 09:17:01 GMT
STOPSIGNAL SIGINT
# Thu, 02 Dec 2021 09:17:01 GMT
EXPOSE 5432
# Thu, 02 Dec 2021 09:17:01 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:bf2c280d82ca10801fb58bfc3f73029eef17592cbe00e94875cb189bdbac0c5f`  
		Last Modified: Thu, 02 Dec 2021 07:25:12 GMT  
		Size: 29.7 MB (29650954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cccf30ae203d70ff46090992cba2bdda1d7198fed71dbdacf93e0d69700eafd9`  
		Last Modified: Thu, 02 Dec 2021 09:47:23 GMT  
		Size: 4.3 MB (4302200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cccd5e99d29ae4eb714eff1cf02fc570b5396de13fb1c50cd07c2110e4483cc`  
		Last Modified: Thu, 02 Dec 2021 09:47:23 GMT  
		Size: 1.8 KB (1802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba86e48bb27139f7cbe5f48a224b9d87d2e855bd501ec444e8337ff4119a02e9`  
		Last Modified: Thu, 02 Dec 2021 09:47:22 GMT  
		Size: 1.4 MB (1381396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33dd99eeee7f25f79f9e21b0355e151667040bb0cf59e204f67e42b30c44426`  
		Last Modified: Thu, 02 Dec 2021 09:47:23 GMT  
		Size: 8.1 MB (8098988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4277ccbf4309b8500af6ae401c3711ff15c5eac7274dc9ffea124650dcd9f3`  
		Last Modified: Thu, 02 Dec 2021 09:47:21 GMT  
		Size: 438.3 KB (438327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3630e45db84209fe7903f54afeda1c207d11719ee41a3b7baffd3dc522293ca1`  
		Last Modified: Thu, 02 Dec 2021 09:47:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e496bc81a671dce19d1788be26b16945b10563b7fb7c0eeb3f21a4f134c86b5`  
		Last Modified: Thu, 02 Dec 2021 09:47:21 GMT  
		Size: 3.0 KB (3049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaacbeda22adcd3babf396db0c0c00ffecc5a1e0a4871edd80b0c426b9a8324a`  
		Last Modified: Thu, 02 Dec 2021 09:48:04 GMT  
		Size: 95.6 MB (95560424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16138cb3787d687f038981bc3155c63ff1ec0acac602c2af680a0edd0e7faa3`  
		Last Modified: Thu, 02 Dec 2021 09:47:52 GMT  
		Size: 9.4 KB (9361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b9646d38810245145233b030a091af5a039c8202da9c00acda270542bf3ab6`  
		Last Modified: Thu, 02 Dec 2021 09:47:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b376f9b22b40fa6a0aed35ac16df912ac5c1e5193e58550ef3eafb18d920c0`  
		Last Modified: Thu, 02 Dec 2021 09:47:52 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76654cc41ac28a54dffbaa62382ab9535f2ffa0619b6ee0b1367ca83fd07c739`  
		Last Modified: Thu, 02 Dec 2021 09:47:52 GMT  
		Size: 4.7 KB (4715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
