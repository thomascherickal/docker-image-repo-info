## `postgres:11-bullseye`

```console
$ docker pull postgres@sha256:717e89fa51e2382df2494067e8d849743f56143310e24699000714e18c14c084
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

### `postgres:11-bullseye` - linux; amd64

```console
$ docker pull postgres@sha256:8395d33c44b51a5e12c3aa128b3d3ee1c3c3c552dfb06df395e83672f71d16cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.4 MB (134357623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76c69d6c3b8dfdbd7dba575dccc654d3b4a6d41e21878b04685938203d0fd6a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:40 GMT
ADD file:3c520ad50b13b922356e0a5e4f7c12b202e09584acf332a65d5603dacd4a9380 in / 
# Tue, 28 Sep 2021 01:22:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 17:29:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 17:29:04 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 28 Sep 2021 17:29:04 GMT
ENV GOSU_VERSION=1.12
# Tue, 28 Sep 2021 17:29:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 28 Sep 2021 17:29:22 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 28 Sep 2021 17:29:23 GMT
ENV LANG=en_US.utf8
# Tue, 28 Sep 2021 17:29:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 17:29:27 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 28 Sep 2021 17:29:35 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 28 Sep 2021 17:30:32 GMT
ENV PG_MAJOR=11
# Tue, 28 Sep 2021 17:30:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Tue, 28 Sep 2021 17:30:33 GMT
ENV PG_VERSION=11.13-1.pgdg110+1
# Fri, 01 Oct 2021 00:47:10 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 01 Oct 2021 00:47:11 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 01 Oct 2021 00:47:12 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 01 Oct 2021 00:47:12 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 01 Oct 2021 00:47:13 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 01 Oct 2021 00:47:13 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 01 Oct 2021 00:47:14 GMT
COPY file:39dd79c055f47ef80495def6993f3e85eb124d02824dc47db35d1043455e54bc in /usr/local/bin/ 
# Fri, 01 Oct 2021 00:47:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Oct 2021 00:47:14 GMT
STOPSIGNAL SIGINT
# Fri, 01 Oct 2021 00:47:14 GMT
EXPOSE 5432
# Fri, 01 Oct 2021 00:47:14 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:bd897bb914af2ec64f1cff5856aefa1ae99b072e38db0b7d801f9679b04aad74`  
		Last Modified: Tue, 28 Sep 2021 01:29:00 GMT  
		Size: 31.4 MB (31368912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f145551e8b989c685bc04b1b9ee8572ead0d8ba0caa3ef64e9c9fe02027edcc`  
		Last Modified: Fri, 01 Oct 2021 00:49:50 GMT  
		Size: 4.4 MB (4414464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d21bf1caa4a5fd9cdf6cd6cb99400152b9810f13c44e635cab5d0a26a5e66243`  
		Last Modified: Fri, 01 Oct 2021 00:49:48 GMT  
		Size: 1.8 KB (1798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d593d17cf792006c9a690d7139f77b6fd32a9eaefccb6d84067c75b01606fcd`  
		Last Modified: Fri, 01 Oct 2021 00:49:48 GMT  
		Size: 1.5 MB (1450497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c468fd1ea1841060f3cd9b40c0df9c1d9096f45a744b679625fd96f96be78ab4`  
		Last Modified: Fri, 01 Oct 2021 00:49:48 GMT  
		Size: 8.0 MB (8045277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd96a2d4842d8a2b6e88ad42ddb7d1c2ac6f95e41b8862a3c40e207bb1b20d8e`  
		Last Modified: Fri, 01 Oct 2021 00:49:47 GMT  
		Size: 441.5 KB (441531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fbbf9d6306e2f791c2137e71e6fcb1598b6d222806ad52a9ddd41bb8837b35`  
		Last Modified: Fri, 01 Oct 2021 00:49:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e3d6202528fdcb63cf465fc799c3858d8fccbbffca792b34b5a4ad52d3a7b3`  
		Last Modified: Fri, 01 Oct 2021 00:49:46 GMT  
		Size: 3.1 KB (3055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d428b28120872a010bc99e9bb190616149450f6f143e7344f8373598646175fe`  
		Last Modified: Fri, 01 Oct 2021 00:52:33 GMT  
		Size: 88.6 MB (88618728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd630bc0b26b4e074407c6f9fc7b408909c4ca7f01afe01626731cadc88e2228`  
		Last Modified: Fri, 01 Oct 2021 00:52:21 GMT  
		Size: 8.3 KB (8325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4db63e3734fdb36a79c8a3185d50de7264129f5c040d92a07eedaef30042089`  
		Last Modified: Fri, 01 Oct 2021 00:52:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb75345d14b12e5764118d9b43545d878a4f71a5c246209ed9447784bdb8897`  
		Last Modified: Fri, 01 Oct 2021 00:52:20 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de744a5f89c9ca094e623d0d1a3b23384bba5262274df1a1d98d39f7c3325dcb`  
		Last Modified: Fri, 01 Oct 2021 00:52:20 GMT  
		Size: 4.6 KB (4557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-bullseye` - linux; arm variant v5

```console
$ docker pull postgres@sha256:c5eebf073878816b94494eaefd6f6237868163d21d54855f9e930819ca247242
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.6 MB (127573614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f81e8bc72f728658970ea9933246d84007670f565969d04757025d52bee78f6f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 28 Sep 2021 01:50:38 GMT
ADD file:da0067258fc1c6a50273e6b3b2673e88fad974a5a1fe4d5eecfeca2df1ff54b3 in / 
# Tue, 28 Sep 2021 01:50:39 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 04:21:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 04:21:51 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 28 Sep 2021 04:21:52 GMT
ENV GOSU_VERSION=1.12
# Tue, 28 Sep 2021 04:22:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 28 Sep 2021 04:22:38 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 28 Sep 2021 04:22:39 GMT
ENV LANG=en_US.utf8
# Tue, 28 Sep 2021 04:22:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 04:22:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 28 Sep 2021 04:22:55 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 28 Sep 2021 06:12:03 GMT
ENV PG_MAJOR=11
# Tue, 28 Sep 2021 06:12:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Tue, 28 Sep 2021 06:12:04 GMT
ENV PG_VERSION=11.13-1.pgdg110+1
# Tue, 28 Sep 2021 06:45:18 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 28 Sep 2021 06:45:21 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 28 Sep 2021 06:45:22 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 28 Sep 2021 06:45:23 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 28 Sep 2021 06:45:24 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 28 Sep 2021 06:45:24 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 01 Oct 2021 02:24:39 GMT
COPY file:39dd79c055f47ef80495def6993f3e85eb124d02824dc47db35d1043455e54bc in /usr/local/bin/ 
# Fri, 01 Oct 2021 02:24:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Oct 2021 02:24:40 GMT
STOPSIGNAL SIGINT
# Fri, 01 Oct 2021 02:24:40 GMT
EXPOSE 5432
# Fri, 01 Oct 2021 02:24:40 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:86f2b8be18fc44e8eb430e2c472979a79cda6eb6fa3add10cc8c5d8764eb90ac`  
		Last Modified: Tue, 28 Sep 2021 02:06:35 GMT  
		Size: 28.9 MB (28910670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d30eb8504c56819605185af701845341d8975e406423278405097f62af2306`  
		Last Modified: Tue, 28 Sep 2021 08:52:54 GMT  
		Size: 4.1 MB (4096354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a243eeeaa2c00737bdd6e98a1fa9a012a7867782cf48628d9ff8924d18b9f18`  
		Last Modified: Tue, 28 Sep 2021 08:52:52 GMT  
		Size: 1.8 KB (1791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11403c7ba143852cedde2cb5fc5d9667ab0334c046a7c9ebc8c7850e05fb9c83`  
		Last Modified: Tue, 28 Sep 2021 08:52:52 GMT  
		Size: 1.4 MB (1409777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f8edfacdf52bfedbf204f96cfb85a0e19c8565f7466afdffca94537cd94624`  
		Last Modified: Tue, 28 Sep 2021 08:52:57 GMT  
		Size: 8.0 MB (8045267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823170a97ccf0c83730d7cc699ed2b8cc784fa3a3a434fca8d95389d5a47dee3`  
		Last Modified: Tue, 28 Sep 2021 08:52:50 GMT  
		Size: 439.8 KB (439807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b92b828995d7ff6cb1b2a36baf84eadb6717f6070738cd8e1f2e79abdb34e6`  
		Last Modified: Tue, 28 Sep 2021 08:52:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a0b55cf0d04e78b149e19f243e52ab82558abba6430057c63594f69cc4f8b0`  
		Last Modified: Tue, 28 Sep 2021 08:52:50 GMT  
		Size: 3.1 KB (3054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e30541e4ce1abad740bc6a70de4d25e77e453e74ff40c94464558336b781d3`  
		Last Modified: Tue, 28 Sep 2021 08:57:28 GMT  
		Size: 84.7 MB (84653527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11619ffc93c99e9a5c71a2802f73f2dbebefcb0c37c868856d910eec90a67e60`  
		Last Modified: Tue, 28 Sep 2021 08:56:34 GMT  
		Size: 8.3 KB (8329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ad5823a326251d155c4fcb628b64702a22a67fc22ba61270d9e30a3e2e93b0`  
		Last Modified: Tue, 28 Sep 2021 08:56:34 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21fb8b86ec36d5f72354d9b556e9b1261c0ef8c3de204beeebe5da83ffa9d60b`  
		Last Modified: Tue, 28 Sep 2021 08:56:34 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f000499bbf8f410c5da44a0ec13b50e7c336f23eaa0a38f70022d6ac56e14e2`  
		Last Modified: Fri, 01 Oct 2021 02:31:46 GMT  
		Size: 4.6 KB (4558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-bullseye` - linux; arm variant v7

```console
$ docker pull postgres@sha256:1310e1e38b4524d128b6b820bda1d5650021388928a81ff0ef66214007404712
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.6 MB (122583814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:157b1b4d677b6445abaea15def416e93441588389b1ae7a1d13bb256c158d466`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 30 Sep 2021 18:03:01 GMT
ADD file:129e2106788d883a456b145d9aff00c3003ee3480901a30318933b46961d31f3 in / 
# Thu, 30 Sep 2021 18:03:02 GMT
CMD ["bash"]
# Thu, 30 Sep 2021 22:18:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 30 Sep 2021 22:18:46 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 30 Sep 2021 22:18:46 GMT
ENV GOSU_VERSION=1.12
# Thu, 30 Sep 2021 22:19:04 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 30 Sep 2021 22:19:25 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 30 Sep 2021 22:19:26 GMT
ENV LANG=en_US.utf8
# Thu, 30 Sep 2021 22:19:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 30 Sep 2021 22:19:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 30 Sep 2021 22:19:40 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Fri, 01 Oct 2021 00:05:42 GMT
ENV PG_MAJOR=11
# Fri, 01 Oct 2021 00:05:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Fri, 01 Oct 2021 00:05:43 GMT
ENV PG_VERSION=11.13-1.pgdg110+1
# Fri, 01 Oct 2021 00:36:10 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 01 Oct 2021 00:36:12 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 01 Oct 2021 00:36:14 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 01 Oct 2021 00:36:14 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 01 Oct 2021 00:36:16 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 01 Oct 2021 00:36:16 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 01 Oct 2021 00:36:17 GMT
COPY file:39dd79c055f47ef80495def6993f3e85eb124d02824dc47db35d1043455e54bc in /usr/local/bin/ 
# Fri, 01 Oct 2021 00:36:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Oct 2021 00:36:18 GMT
STOPSIGNAL SIGINT
# Fri, 01 Oct 2021 00:36:18 GMT
EXPOSE 5432
# Fri, 01 Oct 2021 00:36:18 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:aad43ac6bd46b2cab91485c8f1dac6a985df690af3e431e9e0b9fd57ad5ed423`  
		Last Modified: Thu, 30 Sep 2021 18:19:26 GMT  
		Size: 26.6 MB (26571924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:580c30d6212fc0c5e892b1da4593e8090bf2ecb6c11bb67204e1d91edba90a39`  
		Last Modified: Fri, 01 Oct 2021 02:35:13 GMT  
		Size: 3.7 MB (3717077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13bbf6baf12d4196c3344ddb309f9125e53b1c5519b7c02807638f4d1566cb35`  
		Last Modified: Fri, 01 Oct 2021 02:35:11 GMT  
		Size: 1.8 KB (1794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1cbe192408c0f71246f8a977f99e7be4f481ea1022978c9913c05b93ea22d27`  
		Last Modified: Fri, 01 Oct 2021 02:35:11 GMT  
		Size: 1.4 MB (1402357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a1f485a8c627ff66806f8ee4e773ddb8386c720e66d121774251b9f910d8a2`  
		Last Modified: Fri, 01 Oct 2021 02:35:15 GMT  
		Size: 8.0 MB (8045260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26fd04001559f62fa19628b46b41fe3f1e6ffb10ca949add4de4e51c5f4a5c3`  
		Last Modified: Fri, 01 Oct 2021 02:35:09 GMT  
		Size: 434.5 KB (434498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec64541f883f087718d008ba9e9ef66a9ba101930a756e7b384fd86ca818eadd`  
		Last Modified: Fri, 01 Oct 2021 02:35:09 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8404f1793575907eab013312ee0f7b699f70be4dd9b53aded7cfe598781f7b83`  
		Last Modified: Fri, 01 Oct 2021 02:35:09 GMT  
		Size: 3.1 KB (3054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027b49c068c03a55ccb678e429d77ff3f703888bf5a13d619fbdaf7c74ddd9c0`  
		Last Modified: Fri, 01 Oct 2021 02:41:33 GMT  
		Size: 82.4 MB (82394487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746c867421e9e0a2a0fee438cf88c920b76183e3fe3a65e5a8bb5d055b54a0b9`  
		Last Modified: Fri, 01 Oct 2021 02:40:42 GMT  
		Size: 8.3 KB (8329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5fd7240dfb80b2a062fe6f866af3093d3b5ce08046bbb538c2e543e7d4b96f`  
		Last Modified: Fri, 01 Oct 2021 02:40:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca6945d9f15e030561bd946ef74e1913d69d0e7e44178e06bd6ddfcbe55f8e3`  
		Last Modified: Fri, 01 Oct 2021 02:40:43 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a9e96520a022a11125e112525b8d30d84cfa248b1dbbec82d7d77d4e4c147f`  
		Last Modified: Fri, 01 Oct 2021 02:40:43 GMT  
		Size: 4.6 KB (4557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-bullseye` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:ea1f91d1824780623e78c7f3e5b44734a5c4922cb30ffb79d6ff360d3467c5b3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129485171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b04ff402b2faf9202b8f7aa0d165277e32b15469fe0ec44fff835dc1fa68e49`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:43 GMT
ADD file:6472ab63529e688735f77634402740e08fdbd5bfa788c150915027993df7e8ec in / 
# Tue, 28 Sep 2021 01:40:44 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 11:20:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 11:20:47 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 28 Sep 2021 11:20:47 GMT
ENV GOSU_VERSION=1.12
# Tue, 28 Sep 2021 11:20:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 28 Sep 2021 11:21:03 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 28 Sep 2021 11:21:03 GMT
ENV LANG=en_US.utf8
# Tue, 28 Sep 2021 11:21:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 11:21:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 28 Sep 2021 11:21:17 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 28 Sep 2021 11:23:07 GMT
ENV PG_MAJOR=11
# Tue, 28 Sep 2021 11:23:07 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Tue, 28 Sep 2021 11:23:07 GMT
ENV PG_VERSION=11.13-1.pgdg110+1
# Tue, 28 Sep 2021 11:23:23 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 28 Sep 2021 11:23:24 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 28 Sep 2021 11:23:24 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 28 Sep 2021 11:23:25 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 28 Sep 2021 11:23:25 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 28 Sep 2021 11:23:25 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 01 Oct 2021 00:24:16 GMT
COPY file:39dd79c055f47ef80495def6993f3e85eb124d02824dc47db35d1043455e54bc in /usr/local/bin/ 
# Fri, 01 Oct 2021 00:24:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Oct 2021 00:24:16 GMT
STOPSIGNAL SIGINT
# Fri, 01 Oct 2021 00:24:16 GMT
EXPOSE 5432
# Fri, 01 Oct 2021 00:24:17 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:2f8871a8654eb1158cb626f8dc69992dba7e4bd8796fae6aa7cf967f951f5fe9`  
		Last Modified: Tue, 28 Sep 2021 01:48:25 GMT  
		Size: 30.1 MB (30055408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35bafe1dc851fc9aefa3c150d0df88515dcf3afb315d604f502e1313c697eff`  
		Last Modified: Tue, 28 Sep 2021 11:56:14 GMT  
		Size: 4.4 MB (4415378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8feff4c760546b2e2560db40263f042ce1e57b338319954bca0c1cbcef2707d7`  
		Last Modified: Tue, 28 Sep 2021 11:56:13 GMT  
		Size: 1.8 KB (1801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f175da21aafede406ceb81e27cda155f042eaa7c1fea3c05829a1f136e723c`  
		Last Modified: Tue, 28 Sep 2021 11:56:14 GMT  
		Size: 1.4 MB (1386622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b3fad7d77eb59ed5fa57422307a2372ebc1a9f193950f8ff52378be6478a55`  
		Last Modified: Tue, 28 Sep 2021 11:56:13 GMT  
		Size: 8.0 MB (8045158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98de1af01d5a81bb7a1bafee7fc0d2e5b0afc9a30fc01ecd6256383dfa5aa2b2`  
		Last Modified: Tue, 28 Sep 2021 11:56:11 GMT  
		Size: 442.0 KB (441967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285b5ffb3d52a92ee4fbf5f8ce32ee6534d4ef30b4a9d37e4c331ed5ac8838b2`  
		Last Modified: Tue, 28 Sep 2021 11:56:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc74bee4254ef9704b713fcd2daadfd3a426387e3b26f4fa80800c46d9468c4`  
		Last Modified: Tue, 28 Sep 2021 11:56:11 GMT  
		Size: 3.1 KB (3054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9fd419ae02ef0c27b25260535be34a8876dbf68870cf21bee2cfa82c06a63b`  
		Last Modified: Tue, 28 Sep 2021 11:58:09 GMT  
		Size: 85.1 MB (85122421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a06c9fd4b908731a240702c6ad453dc1b57a0c9a8d1e0099a5bcae50b5a58e6b`  
		Last Modified: Tue, 28 Sep 2021 11:57:56 GMT  
		Size: 8.3 KB (8329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666fcb6433ade0ee863f7b304bac8166b8b0f425714623ccff80bc5ef8b4384d`  
		Last Modified: Tue, 28 Sep 2021 11:57:56 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac8ab5f57a5b5ed127748f1dbd915034e152a4ce3ad17f9fabd9ee008df4b4e`  
		Last Modified: Tue, 28 Sep 2021 11:57:56 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f373a72ac45617a2519862580529525ec23aefc823fd837eb6ac6461961e49`  
		Last Modified: Fri, 01 Oct 2021 00:30:22 GMT  
		Size: 4.6 KB (4557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-bullseye` - linux; 386

```console
$ docker pull postgres@sha256:e7c29ef717960e5bc07ce75b198efba5825a1d7ea3a96252f6f65614f2ec7f71
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.3 MB (136341766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a13c72098b829ff55dd101e4d968affe97205ac52939eb5c716c6d597609122`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:08 GMT
ADD file:8466bd8df052ea7fa26e49575ac95fd4934ddafdad54a9736ac2bd8e7fc6e735 in / 
# Tue, 28 Sep 2021 01:40:08 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 17:14:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 17:14:35 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 28 Sep 2021 17:14:35 GMT
ENV GOSU_VERSION=1.12
# Tue, 28 Sep 2021 17:14:47 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 28 Sep 2021 17:14:54 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 28 Sep 2021 17:14:54 GMT
ENV LANG=en_US.utf8
# Tue, 28 Sep 2021 17:14:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 17:14:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 28 Sep 2021 17:15:05 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 28 Sep 2021 18:00:12 GMT
ENV PG_MAJOR=11
# Tue, 28 Sep 2021 18:00:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Tue, 28 Sep 2021 18:00:13 GMT
ENV PG_VERSION=11.13-1.pgdg110+1
# Tue, 28 Sep 2021 18:14:25 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 28 Sep 2021 18:14:27 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 28 Sep 2021 18:14:28 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 28 Sep 2021 18:14:29 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 28 Sep 2021 18:14:30 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 28 Sep 2021 18:14:30 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 01 Oct 2021 01:34:59 GMT
COPY file:39dd79c055f47ef80495def6993f3e85eb124d02824dc47db35d1043455e54bc in /usr/local/bin/ 
# Fri, 01 Oct 2021 01:34:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Oct 2021 01:35:00 GMT
STOPSIGNAL SIGINT
# Fri, 01 Oct 2021 01:35:00 GMT
EXPOSE 5432
# Fri, 01 Oct 2021 01:35:00 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:e79fce1f6442094a82dc5f6b4d1aa352e04aae39bba821c9021f6da08b1cacaf`  
		Last Modified: Tue, 28 Sep 2021 01:49:07 GMT  
		Size: 32.4 MB (32380160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e1ab074ce3dd0eab68edc193efa5fd98ea3eec7dd073437db711a25cde909a`  
		Last Modified: Tue, 28 Sep 2021 18:43:38 GMT  
		Size: 4.8 MB (4812781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a14356ccb65950a1b3e70fe898d4019f400afb14a7e4687532ae9ebc7b1a32`  
		Last Modified: Tue, 28 Sep 2021 18:43:34 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bacd355e554709f268386f1aacbcdc511d5e4a0b536be582f7155e2392f3d120`  
		Last Modified: Tue, 28 Sep 2021 18:43:34 GMT  
		Size: 1.4 MB (1420865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ab11af800164f2414b9338520598835ca1fd0b36b7a265157038de15bdbe23`  
		Last Modified: Tue, 28 Sep 2021 18:43:38 GMT  
		Size: 8.0 MB (8045087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324260c4b80910870de54fb8041c61b9b3789fa5df5d1c3699ee6062f16e36ec`  
		Last Modified: Tue, 28 Sep 2021 18:43:32 GMT  
		Size: 447.9 KB (447854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1982aa9ef1665c9c6f25fe4a451bc06b594ff13a3e6339a34eab1d91a5d64bd6`  
		Last Modified: Tue, 28 Sep 2021 18:43:31 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f398ac1d73896e6163ea396677a41c48cba95c0c52b6dfe4039a111dedce906f`  
		Last Modified: Tue, 28 Sep 2021 18:43:31 GMT  
		Size: 3.1 KB (3052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3ca2047935e313f1a16c2ae728cae57072150162e0e2ea6b146f63a37b769a`  
		Last Modified: Tue, 28 Sep 2021 18:46:16 GMT  
		Size: 89.2 MB (89216811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbb91f0964e59e1f25230b21fc944429689dac75541f1dffa852cdee6645e68`  
		Last Modified: Tue, 28 Sep 2021 18:46:00 GMT  
		Size: 8.3 KB (8324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ded63badc3e0d9880052e7359fe73ccad7390c21f8edf474a684706238b4e6b`  
		Last Modified: Tue, 28 Sep 2021 18:45:57 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f2e97b3cab90645151ac1b00b1c5f5c65dd30fe3303d7d4601a8faabc8a196`  
		Last Modified: Tue, 28 Sep 2021 18:46:00 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b662f15edb0b951aabbb82f08b49ab1b47820a9d451a5c09f55a2cd669be31d`  
		Last Modified: Fri, 01 Oct 2021 01:41:56 GMT  
		Size: 4.6 KB (4563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-bullseye` - linux; mips64le

```console
$ docker pull postgres@sha256:8131394fd6dff10cea759daa63589b502d1b20827eff3723be996c8258676c7b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.2 MB (129167659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e55800c194ee6dc399c2d6c3420d9b3e78bb1c9b2bd30e61d0c51b6ab60ad82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 28 Sep 2021 02:10:40 GMT
ADD file:43593ef3d79c9b74a92e318d44aacb578f6f8d835dd72665e057bbfe73df1a93 in / 
# Tue, 28 Sep 2021 02:10:41 GMT
CMD ["bash"]
# Wed, 06 Oct 2021 01:07:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 06 Oct 2021 01:07:25 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 06 Oct 2021 01:07:25 GMT
ENV GOSU_VERSION=1.12
# Wed, 06 Oct 2021 01:07:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 06 Oct 2021 01:08:09 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 06 Oct 2021 01:08:10 GMT
ENV LANG=en_US.utf8
# Wed, 06 Oct 2021 01:08:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 06 Oct 2021 01:08:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 06 Oct 2021 01:08:27 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Wed, 06 Oct 2021 03:49:15 GMT
ENV PG_MAJOR=11
# Wed, 06 Oct 2021 03:49:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Wed, 06 Oct 2021 03:49:15 GMT
ENV PG_VERSION=11.13-1.pgdg110+1
# Wed, 06 Oct 2021 04:38:31 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 06 Oct 2021 04:38:33 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 06 Oct 2021 04:38:36 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 06 Oct 2021 04:38:36 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 06 Oct 2021 04:38:38 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 06 Oct 2021 04:38:38 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 06 Oct 2021 04:38:39 GMT
COPY file:39dd79c055f47ef80495def6993f3e85eb124d02824dc47db35d1043455e54bc in /usr/local/bin/ 
# Wed, 06 Oct 2021 04:38:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Oct 2021 04:38:39 GMT
STOPSIGNAL SIGINT
# Wed, 06 Oct 2021 04:38:40 GMT
EXPOSE 5432
# Wed, 06 Oct 2021 04:38:40 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:1f46ea49e27fccc580c8910db39ba7f51ae208a8d24d46a33140afa92ea3d955`  
		Last Modified: Tue, 28 Sep 2021 02:20:45 GMT  
		Size: 29.6 MB (29627871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06363e2276471f2588e3b07792bb620f65e3663f0d5654392e2faa610869e926`  
		Last Modified: Wed, 06 Oct 2021 05:49:33 GMT  
		Size: 4.4 MB (4402808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96daee93ea6f2e4be7d44a99e4512499ffc408a1e6103e8e7cee0402b7a32a50`  
		Last Modified: Wed, 06 Oct 2021 05:49:29 GMT  
		Size: 1.8 KB (1771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c859907b98bc1accdae3d2587f19041a649d9cffa92fbb61b37353dd04e042b0`  
		Last Modified: Wed, 06 Oct 2021 05:49:30 GMT  
		Size: 1.3 MB (1339323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bac0ffca8ad59c7d25840cb5a0a52110fbc60217c9c2defdb1970071f9833e`  
		Last Modified: Wed, 06 Oct 2021 05:49:34 GMT  
		Size: 8.0 MB (8043929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bdd3ee6acab6c2ce672c80a90f2ed8c923534e14942c9b3db1633cbacda3b09`  
		Last Modified: Wed, 06 Oct 2021 05:49:27 GMT  
		Size: 439.1 KB (439103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e29347902a2953400a73635544f2fef07dbdec1ec25ba7c4e1452db91d8217c`  
		Last Modified: Wed, 06 Oct 2021 05:49:27 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170ac2499b1b209ef7391e84ab318a9a3928496ffc037db3619d65f980a23696`  
		Last Modified: Wed, 06 Oct 2021 05:49:26 GMT  
		Size: 3.1 KB (3054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaba6f2041f3305e168edd2953e461ec63162d086e8d63523f58b25997aa925d`  
		Last Modified: Wed, 06 Oct 2021 05:54:27 GMT  
		Size: 85.3 MB (85296494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b88cb84b27ed69fe3f4e5e8840d4970b9908e295ebaa75025853ccea77fce1ae`  
		Last Modified: Wed, 06 Oct 2021 05:53:28 GMT  
		Size: 8.3 KB (8332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6af9f905b9004f37b1f2eb70463e3d669d80040ef653784cb71abd8b172386`  
		Last Modified: Wed, 06 Oct 2021 05:53:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f825ebdeeaf376f1c9b39e84a204076330640618346bbe7fd9f049ddf39fdff`  
		Last Modified: Wed, 06 Oct 2021 05:53:29 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c7338e877d92814a8cba3b48f0837552f133a2f9c4c9e62a5b3e26a3d4db3d7`  
		Last Modified: Wed, 06 Oct 2021 05:53:28 GMT  
		Size: 4.6 KB (4558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-bullseye` - linux; ppc64le

```console
$ docker pull postgres@sha256:41b660cbbe879f6667a4289b886250662f3bcb645f09954dd7eb53c0a09a2eaa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.1 MB (143111410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6612f4a320bf4bb99933ef45e0591a53024cd2b1c587d01d9b1e3cb415495054`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Mon, 04 Oct 2021 17:55:01 GMT
ADD file:f4b696a766a0d9a808c171a1d5db4f0877b0a784649d63bf461dfcf54b532239 in / 
# Mon, 04 Oct 2021 17:55:06 GMT
CMD ["bash"]
# Tue, 05 Oct 2021 07:54:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 05 Oct 2021 07:54:34 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 05 Oct 2021 07:54:37 GMT
ENV GOSU_VERSION=1.12
# Tue, 05 Oct 2021 07:55:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 05 Oct 2021 07:55:35 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 05 Oct 2021 07:55:38 GMT
ENV LANG=en_US.utf8
# Tue, 05 Oct 2021 07:55:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Oct 2021 07:55:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 05 Oct 2021 07:56:11 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 05 Oct 2021 08:11:44 GMT
ENV PG_MAJOR=11
# Tue, 05 Oct 2021 08:11:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Tue, 05 Oct 2021 08:11:51 GMT
ENV PG_VERSION=11.13-1.pgdg110+1
# Tue, 05 Oct 2021 08:12:57 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 05 Oct 2021 08:13:10 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 05 Oct 2021 08:13:21 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 05 Oct 2021 08:13:24 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 05 Oct 2021 08:13:34 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 05 Oct 2021 08:13:39 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 05 Oct 2021 08:13:40 GMT
COPY file:39dd79c055f47ef80495def6993f3e85eb124d02824dc47db35d1043455e54bc in /usr/local/bin/ 
# Tue, 05 Oct 2021 08:13:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Oct 2021 08:13:46 GMT
STOPSIGNAL SIGINT
# Tue, 05 Oct 2021 08:13:50 GMT
EXPOSE 5432
# Tue, 05 Oct 2021 08:13:54 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:c3b7af0ed242d09d9fee2dfc48d4553d58ad90c5fb862ab58fb89e2d04c5b922`  
		Last Modified: Mon, 04 Oct 2021 18:07:32 GMT  
		Size: 35.3 MB (35272408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1dfe8576fe80020094eca6a18a1f9824137e677472de220dd08a3a25abd925`  
		Last Modified: Tue, 05 Oct 2021 08:23:43 GMT  
		Size: 5.2 MB (5222842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20320ad4b2721c4785d600224feec4dd2c7872c57c9f2f85fb946648661cefe9`  
		Last Modified: Tue, 05 Oct 2021 08:23:40 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a319d4e6eb9b4b5959c4aeb383e920bdf1af22ea18df0e5f0b4a0075890ffa`  
		Last Modified: Tue, 05 Oct 2021 08:23:39 GMT  
		Size: 1.4 MB (1369874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d150b46cf8a7ef9937ac1b92e672324e678dd53846b61ff7a56b9eb635fa72ac`  
		Last Modified: Tue, 05 Oct 2021 08:23:39 GMT  
		Size: 8.0 MB (8045351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8382f9aa2593f76ac6e748522be16471183ddf642ce38d0d38a51b272e7e32ea`  
		Last Modified: Tue, 05 Oct 2021 08:23:38 GMT  
		Size: 451.5 KB (451490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e20df117a725abc5a24d144190dd6cbd599b4e19a0b5f0e4f90d248333b7ab`  
		Last Modified: Tue, 05 Oct 2021 08:23:37 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e2ab1d4b57fd22540582a33d508d428cedb009060666413073e9585ac98a3d`  
		Last Modified: Tue, 05 Oct 2021 08:23:36 GMT  
		Size: 3.1 KB (3053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e866863a3d61f713561b1b99b59cc83c2893bc9217084c99091adfb7862f94`  
		Last Modified: Tue, 05 Oct 2021 08:27:03 GMT  
		Size: 92.7 MB (92731217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac4100cd107a6980d0d9e76272a6c1a6a60efe55c07588a609ef4ae0fe32da2`  
		Last Modified: Tue, 05 Oct 2021 08:26:46 GMT  
		Size: 8.3 KB (8335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:075249a2b2e53de05ef75b85d9262c0e1e3f11dfba5a151d83746ee1eb4b6aad`  
		Last Modified: Tue, 05 Oct 2021 08:26:46 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44947ba57326245e4ba6d06f980cc4fa36836a9aa67859c3e3d8fe73b20a31f`  
		Last Modified: Tue, 05 Oct 2021 08:26:46 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2edae7bf41b5cd9f5a0aa5a2a19b643f05173a28abe207ca61b51604c1d5e05`  
		Last Modified: Tue, 05 Oct 2021 08:26:47 GMT  
		Size: 4.6 KB (4558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-bullseye` - linux; s390x

```console
$ docker pull postgres@sha256:58bbb2c56beb86e20bc9541956245671d5109fe799913ebde9b7dd65e9b73b85
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.1 MB (138097961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe45fc7bb95d7f0ed228929b78f64cc651a2daee518eed9637ef12f6fd16d760`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 28 Sep 2021 01:42:57 GMT
ADD file:2daa8824c30440336bc6ea1448af03234d491ad7c0d0cac917cae5eb54c315fc in / 
# Tue, 28 Sep 2021 01:42:59 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:36:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 02:36:39 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 28 Sep 2021 02:36:39 GMT
ENV GOSU_VERSION=1.12
# Tue, 28 Sep 2021 02:36:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 28 Sep 2021 02:36:51 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 28 Sep 2021 02:36:51 GMT
ENV LANG=en_US.utf8
# Tue, 28 Sep 2021 02:36:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:36:55 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 28 Sep 2021 02:37:01 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 28 Sep 2021 03:02:09 GMT
ENV PG_MAJOR=11
# Tue, 28 Sep 2021 03:02:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Tue, 28 Sep 2021 03:02:09 GMT
ENV PG_VERSION=11.13-1.pgdg110+1
# Tue, 28 Sep 2021 03:11:32 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 28 Sep 2021 03:11:45 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 28 Sep 2021 03:11:46 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 28 Sep 2021 03:11:47 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 28 Sep 2021 03:11:48 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 28 Sep 2021 03:11:48 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 01 Oct 2021 00:00:44 GMT
COPY file:39dd79c055f47ef80495def6993f3e85eb124d02824dc47db35d1043455e54bc in /usr/local/bin/ 
# Fri, 01 Oct 2021 00:00:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Oct 2021 00:00:44 GMT
STOPSIGNAL SIGINT
# Fri, 01 Oct 2021 00:00:44 GMT
EXPOSE 5432
# Fri, 01 Oct 2021 00:00:44 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:e8e2938f4df931c46d7575f0b7bad5bc357277fc3e132b720e704ac7a4d1c9ee`  
		Last Modified: Tue, 28 Sep 2021 01:49:01 GMT  
		Size: 29.7 MB (29650795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beec9abc08cf3416245d8969464ffc09bd7d906b53ccb79e8a871fa76ff53345`  
		Last Modified: Tue, 28 Sep 2021 03:27:46 GMT  
		Size: 4.3 MB (4302149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a76b20cabec1e9c13874c288a755ecb8be19bff7cde71239da194df4f8c4f8`  
		Last Modified: Tue, 28 Sep 2021 03:27:45 GMT  
		Size: 1.8 KB (1802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74df8fb2145140202ec944f2eec276009afed7dac0058e18627ab9092ec4b32b`  
		Last Modified: Tue, 28 Sep 2021 03:27:46 GMT  
		Size: 1.4 MB (1437294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165aa9ea8f851bf56a4b0a02d952d04b16d85fe90c215c95bee50946b3c3b371`  
		Last Modified: Tue, 28 Sep 2021 03:27:45 GMT  
		Size: 8.1 MB (8098989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7beb5a03c6f20aa530f94ace58ca4c26cab6b8a9c07ff8e60584b9bb75e55cf`  
		Last Modified: Tue, 28 Sep 2021 03:27:44 GMT  
		Size: 438.2 KB (438229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9ca31c5b54e8da36d434096006a112bfca32e5098d8af92803146e54f2cd83`  
		Last Modified: Tue, 28 Sep 2021 03:27:44 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc2177f334345af5c565c7ab75adf6a52e25583a1ddb3dea012692f4476b9c7`  
		Last Modified: Tue, 28 Sep 2021 03:27:44 GMT  
		Size: 3.1 KB (3056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61d836479dc14ef826c3a806160a8f07d7e7150840b433204bb2b037e151d44`  
		Last Modified: Tue, 28 Sep 2021 03:29:09 GMT  
		Size: 94.2 MB (94152282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99d3c61815329af4b69ef7eb932e8c407d81528aa564a84189eb45946e5ba85`  
		Last Modified: Tue, 28 Sep 2021 03:28:58 GMT  
		Size: 8.3 KB (8329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b91fdd999988c8e8c0c2d0ae2ae15db0da2fa3bc263342619ecd7c5d2ef614`  
		Last Modified: Tue, 28 Sep 2021 03:28:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9543043f376d257a35d719293a0ff1f26cc49b0005507487644d3f206833df3b`  
		Last Modified: Tue, 28 Sep 2021 03:28:58 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f49dd7cd5dfdfc94a5edb34d72d917f198541b7d128213b54f1131dccbd056`  
		Last Modified: Fri, 01 Oct 2021 00:05:09 GMT  
		Size: 4.6 KB (4558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
