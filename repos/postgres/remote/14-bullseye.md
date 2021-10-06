## `postgres:14-bullseye`

```console
$ docker pull postgres@sha256:c731979fd21f34562e32f56fc367d8ba92e43685376cc7203c5c39fc81584807
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

### `postgres:14-bullseye` - linux; amd64

```console
$ docker pull postgres@sha256:2b8a60d4ae4b3cf9dc5ae823700f699fdabdb0d03901dd480c9a410ca72c4571
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.9 MB (136944669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ce504119cc8171027b8b77f53b47ccf731ac286ff9661b7917d8999dfa74ebc`
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
# Tue, 28 Sep 2021 17:29:36 GMT
ENV PG_MAJOR=14
# Tue, 28 Sep 2021 17:29:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Fri, 01 Oct 2021 00:39:13 GMT
ENV PG_VERSION=14.0-1.pgdg110+1
# Fri, 01 Oct 2021 00:39:35 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 01 Oct 2021 00:39:36 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 01 Oct 2021 00:39:37 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 01 Oct 2021 00:39:37 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 01 Oct 2021 00:39:38 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 01 Oct 2021 00:39:38 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 01 Oct 2021 00:39:39 GMT
COPY file:39dd79c055f47ef80495def6993f3e85eb124d02824dc47db35d1043455e54bc in /usr/local/bin/ 
# Fri, 01 Oct 2021 00:39:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Oct 2021 00:39:39 GMT
STOPSIGNAL SIGINT
# Fri, 01 Oct 2021 00:39:39 GMT
EXPOSE 5432
# Fri, 01 Oct 2021 00:39:39 GMT
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
	-	`sha256:596c65fd344f25851596d0a45fce253d43ac478ab56cea31701f4f1c4858999d`  
		Last Modified: Fri, 01 Oct 2021 00:49:58 GMT  
		Size: 91.2 MB (91204573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad62c5f06a97ab3a11f6680400f89097c70bda14be7b076bc59075cb03e6b50`  
		Last Modified: Fri, 01 Oct 2021 00:49:44 GMT  
		Size: 9.5 KB (9525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf659d84c20b05b68198d0e75e58bc0e3f085198ef89d07389461a446c098dd5`  
		Last Modified: Fri, 01 Oct 2021 00:49:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42945cf6db151ccf068f69d4521cb9332c168cfb97f337ff1720ffa8b2366558`  
		Last Modified: Fri, 01 Oct 2021 00:49:44 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f7bf05d84e725a915d110d3e280fcac246cb725297322f2b5d94f908539e84`  
		Last Modified: Fri, 01 Oct 2021 00:49:43 GMT  
		Size: 4.6 KB (4556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-bullseye` - linux; arm variant v5

```console
$ docker pull postgres@sha256:f3f4b4a38d3a55a8d2aafc6e0d7f691961b7599265204ef28390a1017b1cb297
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.2 MB (130234311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:905fc13cbc075fe7d1379e61a5d0795f653911182b7c2329a75cd5ee48cf4f97`
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
# Tue, 28 Sep 2021 04:22:56 GMT
ENV PG_MAJOR=14
# Tue, 28 Sep 2021 04:22:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Fri, 01 Oct 2021 01:10:11 GMT
ENV PG_VERSION=14.0-1.pgdg110+1
# Fri, 01 Oct 2021 01:47:39 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 01 Oct 2021 01:47:41 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 01 Oct 2021 01:47:43 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 01 Oct 2021 01:47:43 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 01 Oct 2021 01:47:45 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 01 Oct 2021 01:47:45 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 01 Oct 2021 01:47:46 GMT
COPY file:39dd79c055f47ef80495def6993f3e85eb124d02824dc47db35d1043455e54bc in /usr/local/bin/ 
# Fri, 01 Oct 2021 01:47:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Oct 2021 01:47:47 GMT
STOPSIGNAL SIGINT
# Fri, 01 Oct 2021 01:47:47 GMT
EXPOSE 5432
# Fri, 01 Oct 2021 01:47:48 GMT
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
	-	`sha256:d2916215d1453c885a0d2caf9f63035d5b656a5c704f9974044c09a62779da26`  
		Last Modified: Fri, 01 Oct 2021 02:29:40 GMT  
		Size: 87.3 MB (87313022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6052abaca1fb4ad40f1c713649a01fd586e67279fd0ba84739eba53472fe3f9`  
		Last Modified: Fri, 01 Oct 2021 02:28:45 GMT  
		Size: 9.5 KB (9529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7fc9c756086b9f707dfa85647a851f9ac4fefe873a8b247028d04b112a5b3b`  
		Last Modified: Fri, 01 Oct 2021 02:28:45 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e2f2065dfa0ba7d8721a0116c86a49584a3b38165459f974de5786f4eed071`  
		Last Modified: Fri, 01 Oct 2021 02:28:45 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c25bd345bc8ec059596452255e80da8d57584dd34a8fc764c9235dbdc58c6a77`  
		Last Modified: Fri, 01 Oct 2021 02:28:45 GMT  
		Size: 4.6 KB (4560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-bullseye` - linux; arm variant v7

```console
$ docker pull postgres@sha256:054a0dfc211336545a5328a11f907662e7d3df83658435e06c05fc18f5ddf796
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.0 MB (125031338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9a58a62e119ec80babe7daed56ba19bdf444c132ec493120e75e90c7e5d9734`
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
# Thu, 30 Sep 2021 22:19:41 GMT
ENV PG_MAJOR=14
# Thu, 30 Sep 2021 22:19:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Thu, 30 Sep 2021 22:19:41 GMT
ENV PG_VERSION=14.0-1.pgdg110+1
# Thu, 30 Sep 2021 22:54:19 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 30 Sep 2021 22:54:22 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 30 Sep 2021 22:54:23 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Sep 2021 22:54:24 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Sep 2021 22:54:25 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Sep 2021 22:54:26 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Sep 2021 22:54:26 GMT
COPY file:39dd79c055f47ef80495def6993f3e85eb124d02824dc47db35d1043455e54bc in /usr/local/bin/ 
# Thu, 30 Sep 2021 22:54:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Sep 2021 22:54:27 GMT
STOPSIGNAL SIGINT
# Thu, 30 Sep 2021 22:54:28 GMT
EXPOSE 5432
# Thu, 30 Sep 2021 22:54:28 GMT
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
	-	`sha256:d85f73cd1d71a6f2b7df3a9638e7822ef799fe6a7ec96993b28a665ff1de54d5`  
		Last Modified: Fri, 01 Oct 2021 02:35:58 GMT  
		Size: 84.8 MB (84840798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b27a5a43bbf53319c6a3fbec3c64f3672e37b23b392c88612e032ac5c6e8b9`  
		Last Modified: Fri, 01 Oct 2021 02:35:07 GMT  
		Size: 9.5 KB (9536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb096d3a7d3f515d6affef36d55b6154f555728bf72efcc23e3a66cfd538317`  
		Last Modified: Fri, 01 Oct 2021 02:35:07 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa04beb8613cd891f22a8bfa23f8376439e135ef20f513704fddd3d7129a3c8`  
		Last Modified: Fri, 01 Oct 2021 02:35:07 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3f57e4aa545ce7fba1911963f38429e901962420f4293dffa67f8368bb0dc9`  
		Last Modified: Fri, 01 Oct 2021 02:35:07 GMT  
		Size: 4.6 KB (4561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-bullseye` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:e247c43d5966747ed724630d4ab2565098fb23f79688c94aaf250a6470259178
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.1 MB (132083044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef50259a66782b86ccfc3fa5ffb1e1c767e90ea0adb7f08d083ab925368be3c1`
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
# Tue, 28 Sep 2021 11:21:17 GMT
ENV PG_MAJOR=14
# Tue, 28 Sep 2021 11:21:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Fri, 01 Oct 2021 00:18:03 GMT
ENV PG_VERSION=14.0-1.pgdg110+1
# Fri, 01 Oct 2021 00:18:31 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 01 Oct 2021 00:18:32 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 01 Oct 2021 00:18:33 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 01 Oct 2021 00:18:33 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 01 Oct 2021 00:18:34 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 01 Oct 2021 00:18:34 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 01 Oct 2021 00:18:34 GMT
COPY file:39dd79c055f47ef80495def6993f3e85eb124d02824dc47db35d1043455e54bc in /usr/local/bin/ 
# Fri, 01 Oct 2021 00:18:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Oct 2021 00:18:35 GMT
STOPSIGNAL SIGINT
# Fri, 01 Oct 2021 00:18:35 GMT
EXPOSE 5432
# Fri, 01 Oct 2021 00:18:35 GMT
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
	-	`sha256:07f0553587383c55edadd78be147af5bdf08317de2e62ceb04abede4a4b3722b`  
		Last Modified: Fri, 01 Oct 2021 00:27:54 GMT  
		Size: 87.7 MB (87719096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63008bd65bdf67b483ca179fc209f3c64f382c4a8f7d734bae2f12eace55c0a7`  
		Last Modified: Fri, 01 Oct 2021 00:27:40 GMT  
		Size: 9.5 KB (9523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b16ef8c572b8a030a4d44446548db413c126f93b0f7c6725cf8c7d7d128736`  
		Last Modified: Fri, 01 Oct 2021 00:27:40 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bd67bed6bfbfcff2b6d79a204ecb399b24fd1cfa76ff558922bdef69235487`  
		Last Modified: Fri, 01 Oct 2021 00:27:41 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2edd840f24b773891b8e4a2ab156a4c2704c8d6b00b377751740c1715f0a96`  
		Last Modified: Fri, 01 Oct 2021 00:27:41 GMT  
		Size: 4.6 KB (4557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-bullseye` - linux; 386

```console
$ docker pull postgres@sha256:da98eb3d0ac42daede96c9cdf77ac57ef8e3c50614f48fcafe55e691b7d9a590
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.1 MB (139054640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dbae312d988b8cc84e74ea1586bdf85bf4b862ada5b86e20e7c43facf475278`
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
# Tue, 28 Sep 2021 17:15:05 GMT
ENV PG_MAJOR=14
# Tue, 28 Sep 2021 17:15:05 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Fri, 01 Oct 2021 00:57:02 GMT
ENV PG_VERSION=14.0-1.pgdg110+1
# Fri, 01 Oct 2021 01:13:02 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 01 Oct 2021 01:13:03 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 01 Oct 2021 01:13:04 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 01 Oct 2021 01:13:04 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 01 Oct 2021 01:13:05 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 01 Oct 2021 01:13:05 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 01 Oct 2021 01:13:05 GMT
COPY file:39dd79c055f47ef80495def6993f3e85eb124d02824dc47db35d1043455e54bc in /usr/local/bin/ 
# Fri, 01 Oct 2021 01:13:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Oct 2021 01:13:06 GMT
STOPSIGNAL SIGINT
# Fri, 01 Oct 2021 01:13:06 GMT
EXPOSE 5432
# Fri, 01 Oct 2021 01:13:06 GMT
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
	-	`sha256:b1a2c8139f5fe19f89e64fa5b809a596dfff7f57f9f512aa89ec5c95576e2600`  
		Last Modified: Fri, 01 Oct 2021 01:39:06 GMT  
		Size: 91.9 MB (91928479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30403c5b27f6928bc724620946cf1a5f7c9cd29bb56c6dd75dafda7267fa7002`  
		Last Modified: Fri, 01 Oct 2021 01:38:47 GMT  
		Size: 9.5 KB (9527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb47419286ccfbd7eb43284bdf0b8f6e6ddccfb434254657fc697c60d663eb0`  
		Last Modified: Fri, 01 Oct 2021 01:38:47 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11fc24868cde945b3495fd22a2be3b0faa64699916718920f916b0b03739a654`  
		Last Modified: Fri, 01 Oct 2021 01:38:47 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12355fafba00c5ba3a36df52b72fa6818d79fbb8d2e60293d99a9c7bf595af7`  
		Last Modified: Fri, 01 Oct 2021 01:38:47 GMT  
		Size: 4.6 KB (4566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-bullseye` - linux; mips64le

```console
$ docker pull postgres@sha256:fa5bcbae7db85113e9e0660a81b104acd746d9ab1c724b372138100b3ca0f917
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.8 MB (131760973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5466d1f22d78a9b9e9751368d92f91b76c44dd32394caaeb6a53f0d7d542d55a`
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
# Wed, 06 Oct 2021 01:08:27 GMT
ENV PG_MAJOR=14
# Wed, 06 Oct 2021 01:08:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Wed, 06 Oct 2021 01:08:27 GMT
ENV PG_VERSION=14.0-1.pgdg110+1
# Wed, 06 Oct 2021 02:04:19 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 06 Oct 2021 02:04:22 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 06 Oct 2021 02:04:24 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 06 Oct 2021 02:04:24 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 06 Oct 2021 02:04:26 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 06 Oct 2021 02:04:26 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 06 Oct 2021 02:04:27 GMT
COPY file:39dd79c055f47ef80495def6993f3e85eb124d02824dc47db35d1043455e54bc in /usr/local/bin/ 
# Wed, 06 Oct 2021 02:04:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 06 Oct 2021 02:04:27 GMT
STOPSIGNAL SIGINT
# Wed, 06 Oct 2021 02:04:28 GMT
EXPOSE 5432
# Wed, 06 Oct 2021 02:04:28 GMT
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
	-	`sha256:eadeefab3c9d0ee2cd21afffb0d88f8ff81d3bf8b397bebe86549e12acf49a9a`  
		Last Modified: Wed, 06 Oct 2021 05:50:26 GMT  
		Size: 87.9 MB (87888605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b18ff57fa75c7be8a22ca8ce792ff983a57721fbf453a709ed1bdceb276fc9`  
		Last Modified: Wed, 06 Oct 2021 05:49:24 GMT  
		Size: 9.5 KB (9535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510b9e01e40bbc3f62433c3d19cbe895cae822ddaca3def3e97f3ffdea64ba10`  
		Last Modified: Wed, 06 Oct 2021 05:49:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a452fad05ab40f5f3ad57eb84a4b879a4cf1c86e5a9b798093be033dad4ed242`  
		Last Modified: Wed, 06 Oct 2021 05:49:24 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a68a80baeae626afe2d8b808507b6f8aa14bfadd0ca75a9601efbae70f236842`  
		Last Modified: Wed, 06 Oct 2021 05:49:24 GMT  
		Size: 4.6 KB (4561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-bullseye` - linux; ppc64le

```console
$ docker pull postgres@sha256:c95ec2fc5cd577e6d58b7e93c9cd4ba1f93a584ffac266f546b66499153d1f84
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.9 MB (145868736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8d12a74bb9ea58eca1b9b053bf13a4e2fe8c786614eb165282acb99127ca729`
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
# Tue, 05 Oct 2021 07:56:14 GMT
ENV PG_MAJOR=14
# Tue, 05 Oct 2021 07:56:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Tue, 05 Oct 2021 07:56:20 GMT
ENV PG_VERSION=14.0-1.pgdg110+1
# Tue, 05 Oct 2021 07:57:33 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 05 Oct 2021 07:57:44 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 05 Oct 2021 07:57:51 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 05 Oct 2021 07:57:55 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 05 Oct 2021 07:58:02 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 05 Oct 2021 07:58:05 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 05 Oct 2021 07:58:07 GMT
COPY file:39dd79c055f47ef80495def6993f3e85eb124d02824dc47db35d1043455e54bc in /usr/local/bin/ 
# Tue, 05 Oct 2021 07:58:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Oct 2021 07:58:12 GMT
STOPSIGNAL SIGINT
# Tue, 05 Oct 2021 07:58:14 GMT
EXPOSE 5432
# Tue, 05 Oct 2021 07:58:18 GMT
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
	-	`sha256:d152ace5be9816b7ead5e341bacdc75d6f1f8e644e836a686e12416e83101b3b`  
		Last Modified: Tue, 05 Oct 2021 08:23:50 GMT  
		Size: 95.5 MB (95487341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19e02954cfc57aa2b05dc59199654b22cc3689583e403a9dab16d86b61e4d5e`  
		Last Modified: Tue, 05 Oct 2021 08:23:33 GMT  
		Size: 9.5 KB (9535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e4b623db0b9b3118a4984c14760aa70f440e5ea6f26630a800079f12adfdc0`  
		Last Modified: Tue, 05 Oct 2021 08:23:33 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:279af163397c84277588910797f6c0e42a420710bda51fda85d1fffeed557a80`  
		Last Modified: Tue, 05 Oct 2021 08:23:33 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4259b5c8c196c9a5995a0116e92d1fbc16f9d084a251493e98425504f6934833`  
		Last Modified: Tue, 05 Oct 2021 08:23:33 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-bullseye` - linux; s390x

```console
$ docker pull postgres@sha256:2f58c14c8416a26010787fe6688f0f000d4e695db49798029a081852ab13009f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.8 MB (140827837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5120d126c32835253a6812ea92024274fd87fbed60230ef43353b61fd4ca7bad`
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
# Tue, 28 Sep 2021 02:37:01 GMT
ENV PG_MAJOR=14
# Tue, 28 Sep 2021 02:37:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Thu, 30 Sep 2021 23:38:24 GMT
ENV PG_VERSION=14.0-1.pgdg110+1
# Thu, 30 Sep 2021 23:47:46 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 30 Sep 2021 23:47:51 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 30 Sep 2021 23:47:51 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 30 Sep 2021 23:47:51 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 30 Sep 2021 23:47:52 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 30 Sep 2021 23:47:52 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 30 Sep 2021 23:47:52 GMT
COPY file:39dd79c055f47ef80495def6993f3e85eb124d02824dc47db35d1043455e54bc in /usr/local/bin/ 
# Thu, 30 Sep 2021 23:47:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Sep 2021 23:47:52 GMT
STOPSIGNAL SIGINT
# Thu, 30 Sep 2021 23:47:52 GMT
EXPOSE 5432
# Thu, 30 Sep 2021 23:47:53 GMT
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
	-	`sha256:0f9a8af34d69ee33d0e476c4f44e46139a69c77fd62653f0ecf81349fda4c722`  
		Last Modified: Fri, 01 Oct 2021 00:03:19 GMT  
		Size: 96.9 MB (96880954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd4defacf89db0ac9060992510e442bd7763ba33001bf837e2f03e884d60eab`  
		Last Modified: Fri, 01 Oct 2021 00:03:07 GMT  
		Size: 9.5 KB (9532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af40b819c43346a58d33a918fef1bb7169828199186b6527bf17a95cbdecadc`  
		Last Modified: Fri, 01 Oct 2021 00:03:07 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ad8e714229744c13dc3906359aaf71d4f1c42cb6fbb910af5ee1e915f235e7`  
		Last Modified: Fri, 01 Oct 2021 00:03:07 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca2262d6a12b9d12b5b6e7ad24259a739c0044f7831773e6e239d05aac45b6e`  
		Last Modified: Fri, 01 Oct 2021 00:03:07 GMT  
		Size: 4.6 KB (4559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
