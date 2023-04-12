## `postgres:latest`

```console
$ docker pull postgres@sha256:20fc8081acb0ea2f18e78772a7703054ea1cafb843f0ab447c8794112bc29597
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

### `postgres:latest` - linux; amd64

```console
$ docker pull postgres@sha256:f1f635486b8673d041e2b180a029b712a37ac42ca5479ea13029b53988ed164c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.9 MB (138856207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80c558ffdc314a930fe201d69d9cd58a0fc0f6a833e3f5014268a02d36438c65`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 11:05:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 11:05:32 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 23 Mar 2023 11:05:32 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 11:05:40 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 11:05:47 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 23 Mar 2023 11:05:47 GMT
ENV LANG=en_US.utf8
# Thu, 23 Mar 2023 11:05:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 11:05:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Mar 2023 11:05:52 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 11:05:52 GMT
ENV PG_MAJOR=15
# Thu, 23 Mar 2023 11:05:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Thu, 23 Mar 2023 11:05:52 GMT
ENV PG_VERSION=15.2-1.pgdg110+1
# Thu, 23 Mar 2023 11:06:13 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 23 Mar 2023 11:06:14 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 23 Mar 2023 11:06:14 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Mar 2023 11:06:14 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Mar 2023 11:06:15 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Mar 2023 11:06:15 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 27 Mar 2023 22:29:58 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Mon, 27 Mar 2023 22:29:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Mar 2023 22:29:58 GMT
STOPSIGNAL SIGINT
# Mon, 27 Mar 2023 22:29:58 GMT
EXPOSE 5432
# Mon, 27 Mar 2023 22:29:58 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c04f8741265c9cb018d6e0dc852fa48d9ca605cc4a8b910701149c268b46c4c`  
		Last Modified: Thu, 23 Mar 2023 11:08:27 GMT  
		Size: 4.4 MB (4414969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffc353b86ebafc024e489eb30725dec939794c5c853d8c40e8a228061ef618d`  
		Last Modified: Thu, 23 Mar 2023 11:08:25 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c4a9e6c414bdb0cea88de7b9d555fb825bbbd7b3ceff82ac6de73109460c58`  
		Last Modified: Thu, 23 Mar 2023 11:08:26 GMT  
		Size: 1.5 MB (1471387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f47e7b385280253a608f12b70c590d831395a3efe2908bc3f1eb9f18ba06b6`  
		Last Modified: Thu, 23 Mar 2023 11:08:25 GMT  
		Size: 8.0 MB (8045374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e26c947960d4da4154c7610b237230df37598a1cc6fbcaf57e6aa25b10e7a9d`  
		Last Modified: Thu, 23 Mar 2023 11:08:24 GMT  
		Size: 1.3 MB (1261165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c3dc85e8c3b85d3f412d47e5e3091453f92a0ca1de2154fee0efd915202eb4`  
		Last Modified: Thu, 23 Mar 2023 11:08:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17df73636f012eaeb40d794735572017fd87f992aa4338ac562491cfcd3b8a6c`  
		Last Modified: Thu, 23 Mar 2023 11:08:23 GMT  
		Size: 3.2 KB (3201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713535cdf17c2aadcd4b2680b3b338d8b28af1f96b25dc717b35ba3f52b4874b`  
		Last Modified: Thu, 23 Mar 2023 11:08:34 GMT  
		Size: 92.2 MB (92231868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52278a39eea280d0e88483c4370e80c9214d07a91ae96d746f54116451bd6f93`  
		Last Modified: Thu, 23 Mar 2023 11:08:22 GMT  
		Size: 9.8 KB (9780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ded87da67f6c1ac0d991ec6b5a9cf9f47b2708f81a24287f151481f03ee4765`  
		Last Modified: Thu, 23 Mar 2023 11:08:22 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05fae4678312afe8df03c1daecbc999b7ea692a1622f685949bfaf6590eeb48b`  
		Last Modified: Thu, 23 Mar 2023 11:08:22 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b4f4aeea2d061747cd2cbc3ad388ded2b1b4720b12fdd7ebbe5facdc0f978c`  
		Last Modified: Mon, 27 Mar 2023 22:30:47 GMT  
		Size: 4.8 KB (4782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; arm variant v5

```console
$ docker pull postgres@sha256:fad7667de840d58a8121a8c47869dfa1b91f52e78bc351ce17623af25ed8e0ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.1 MB (132134979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55f523d5707dc7563818adb00d83b7bae525a974a9d3e69a6f09d05ba7a3ca45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 23 Mar 2023 00:48:44 GMT
ADD file:7595c7bfa6b3741f57a3ec7790e3108bb526244e52bb4a54548b8b5541e66616 in / 
# Thu, 23 Mar 2023 00:48:44 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 05:41:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 05:41:44 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 23 Mar 2023 05:41:44 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 05:41:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 05:42:01 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 23 Mar 2023 05:42:01 GMT
ENV LANG=en_US.utf8
# Thu, 23 Mar 2023 05:42:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 05:42:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Mar 2023 05:42:09 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 05:42:09 GMT
ENV PG_MAJOR=15
# Thu, 23 Mar 2023 05:42:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Thu, 23 Mar 2023 05:42:09 GMT
ENV PG_VERSION=15.2-1.pgdg110+1
# Thu, 23 Mar 2023 05:56:22 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 23 Mar 2023 05:56:23 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 23 Mar 2023 05:56:24 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Mar 2023 05:56:24 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Mar 2023 05:56:24 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Mar 2023 05:56:24 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 28 Mar 2023 00:10:05 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Tue, 28 Mar 2023 00:10:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Mar 2023 00:10:06 GMT
STOPSIGNAL SIGINT
# Tue, 28 Mar 2023 00:10:06 GMT
EXPOSE 5432
# Tue, 28 Mar 2023 00:10:06 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:b83d345710cdef1626d1940689dd3160e5ce3e4f63b3154cf612c52b704baa66`  
		Last Modified: Thu, 23 Mar 2023 02:22:00 GMT  
		Size: 28.9 MB (28915852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b596a08513f5f10750e2615df1971bd90af28e28fac7ee07c14b2aeb3b7999d`  
		Last Modified: Sat, 25 Mar 2023 01:17:25 GMT  
		Size: 4.1 MB (4096504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648d61fe59a2d792ab82557840572e0e5f0109175839fdcd8c45456ae9a3285b`  
		Last Modified: Sat, 25 Mar 2023 01:17:24 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b13ffb35c1d1c6e3b0a43baa49961dc6b971b250f0fe9a4d63f558a59f30aa`  
		Last Modified: Sat, 25 Mar 2023 01:17:24 GMT  
		Size: 1.4 MB (1448662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0ab220b1e90dd4d594cd7c7ae5d8a7a7a455aa0b59dc50476e0ab77096991f`  
		Last Modified: Sat, 25 Mar 2023 01:17:24 GMT  
		Size: 8.0 MB (8045131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b781cef1e55785ae4f8dbdb8013b906a28cd5033f97d7c32d5bcb209b619588`  
		Last Modified: Sat, 25 Mar 2023 01:17:22 GMT  
		Size: 1.3 MB (1257266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0281e259b86d066ef1338563cdb0b418144d33fb5fd95b6de5424db6e694ae0`  
		Last Modified: Sat, 25 Mar 2023 01:17:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3b3c0d5ba475db73b0763716a29edcd77c0235c582caf9155089e0ff48bee1`  
		Last Modified: Sat, 25 Mar 2023 01:17:21 GMT  
		Size: 3.2 KB (3194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4adeb918952b54f420cfb5de76377d29c0c0b89a6f280f806408ae495007cd7c`  
		Last Modified: Sat, 25 Mar 2023 01:17:34 GMT  
		Size: 88.4 MB (88351538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2a48c81a77669feef16004e83d8d726c53cf37928b228bc8ad0982f204b8bb`  
		Last Modified: Sat, 25 Mar 2023 01:17:20 GMT  
		Size: 9.8 KB (9784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b0947810ec5000dce52a0680a7fdf161094b8cd8878acebf799da8a9275732`  
		Last Modified: Sat, 25 Mar 2023 01:17:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3747422d192b0a0fc9c9d44aa58230c252b8cc0a4f0b01da7c02bfb1f36dd6e`  
		Last Modified: Sat, 25 Mar 2023 01:17:20 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2a2187cfe6ea612c2aa2fd5f035057a625c09aba7d3f06d0fca7b0fbffd556`  
		Last Modified: Tue, 28 Mar 2023 00:17:39 GMT  
		Size: 4.8 KB (4782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; arm variant v7

```console
$ docker pull postgres@sha256:412c81d6b8a278d15fdedf1418d79ec4e091e6a0f9bfb1ea3f6160f9451c339d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.8 MB (126772583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb39c5c1381ef626bb5e8d83a85c70b87e7cbae081cfca9975d74c2bbcddb0bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 10:58:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 10:58:17 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 23 Mar 2023 10:58:17 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 10:58:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 10:58:32 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 23 Mar 2023 10:58:32 GMT
ENV LANG=en_US.utf8
# Thu, 23 Mar 2023 10:58:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 10:58:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Mar 2023 10:58:38 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 10:58:38 GMT
ENV PG_MAJOR=15
# Thu, 23 Mar 2023 10:58:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Thu, 23 Mar 2023 10:58:38 GMT
ENV PG_VERSION=15.2-1.pgdg110+1
# Thu, 23 Mar 2023 11:11:36 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 23 Mar 2023 11:11:37 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 23 Mar 2023 11:11:37 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Mar 2023 11:11:38 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Mar 2023 11:11:38 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Mar 2023 11:11:38 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 27 Mar 2023 23:53:05 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Mon, 27 Mar 2023 23:53:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Mar 2023 23:53:05 GMT
STOPSIGNAL SIGINT
# Mon, 27 Mar 2023 23:53:05 GMT
EXPOSE 5432
# Mon, 27 Mar 2023 23:53:05 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3a8667968a2db1a4d8fdfe4de326db3f475b097b6bb67fd8c96aaf5aa1a1fa7`  
		Last Modified: Thu, 23 Mar 2023 11:59:17 GMT  
		Size: 3.7 MB (3717300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6bbc02bbbd7873d21e453b297a9054998edc6166c926089caa9bfee5a74f67`  
		Last Modified: Thu, 23 Mar 2023 11:59:16 GMT  
		Size: 1.8 KB (1791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe548cbd05be1647b4c58950c26d4ebc0b8d6715e97c8772b7eb1c803e8f6935`  
		Last Modified: Thu, 23 Mar 2023 11:59:16 GMT  
		Size: 1.4 MB (1438727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f5bdef234eb976f6da02f71c24a8ea2d93d64ce81699e9b92062a0c6efdd9c`  
		Last Modified: Thu, 23 Mar 2023 11:59:15 GMT  
		Size: 8.0 MB (8045293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517a1d4afc5c67eb89563508719ce343a997056a6aa3aeaf398487b6fac2881d`  
		Last Modified: Thu, 23 Mar 2023 11:59:14 GMT  
		Size: 1.1 MB (1131177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8069c9944fe98f6bd9941fc370d6728cc9e16e9c10739ad1cd2508adaf65a760`  
		Last Modified: Thu, 23 Mar 2023 11:59:14 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54b099283053085aa8d8acbd3366ee31e047486e58af6b8f02860f032e89adb`  
		Last Modified: Thu, 23 Mar 2023 11:59:14 GMT  
		Size: 3.2 KB (3200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c974b5aafebcf4715515eb1cf3b6cfa08016958b6bfd4cb3a3d819178ed14d1`  
		Last Modified: Thu, 23 Mar 2023 11:59:25 GMT  
		Size: 85.8 MB (85842717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df859666740f9334fb2987a586d51ea634f540928ec028d5aa218e82ede4494f`  
		Last Modified: Thu, 23 Mar 2023 11:59:12 GMT  
		Size: 9.8 KB (9789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d422aa31043c22d8c9f53c35f48fd8ee1f3f22826f15a1e64744faffaa2ab0ae`  
		Last Modified: Thu, 23 Mar 2023 11:59:12 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5957d71cb6695c469da6a3a48969b9a5563363e8bbb9d315c347fe7db6bfe528`  
		Last Modified: Thu, 23 Mar 2023 11:59:12 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ec50803b37cef92b2c342ca4e873984dfe9f4afdf225d24f478ff3390d82e5`  
		Last Modified: Tue, 28 Mar 2023 00:03:17 GMT  
		Size: 4.8 KB (4782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:6c684cf8da87bbb8cacea3c700289138487eff08da2200c6a68a2de7b3e7795a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133921991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45ca3dd3a1887736bb5f367c0d7e3ed07aceea2bf05ea14ab9a19d087f36500f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:28:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 13:28:19 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 23 Mar 2023 13:28:19 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 13:28:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 13:28:33 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 23 Mar 2023 13:28:33 GMT
ENV LANG=en_US.utf8
# Thu, 23 Mar 2023 13:28:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:28:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Mar 2023 13:28:38 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 13:28:38 GMT
ENV PG_MAJOR=15
# Thu, 23 Mar 2023 13:28:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Thu, 23 Mar 2023 13:28:38 GMT
ENV PG_VERSION=15.2-1.pgdg110+1
# Thu, 23 Mar 2023 13:28:56 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 23 Mar 2023 13:28:58 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 23 Mar 2023 13:28:58 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Mar 2023 13:28:58 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Mar 2023 13:28:59 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Mar 2023 13:28:59 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 28 Mar 2023 01:20:19 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Tue, 28 Mar 2023 01:20:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Mar 2023 01:20:20 GMT
STOPSIGNAL SIGINT
# Tue, 28 Mar 2023 01:20:20 GMT
EXPOSE 5432
# Tue, 28 Mar 2023 01:20:20 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4de29c30b99b39aed5a35ff544bb397a90bd47de48bcbd6555014b8a6f0b60c`  
		Last Modified: Thu, 23 Mar 2023 13:31:03 GMT  
		Size: 4.4 MB (4416207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e28158506a33fe300a3fabc8eeb43bb6afa873ac85c93eb56ea47b9c5f4b97f`  
		Last Modified: Thu, 23 Mar 2023 13:31:05 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53514e250b72009b86f4fb727db037d7bd0a3b2f9a5f1591e15fc13d4c0f7d8c`  
		Last Modified: Thu, 23 Mar 2023 13:31:02 GMT  
		Size: 1.4 MB (1403222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c081701961bb12cf06f601dfcdfa3f1ee1e2d1b009549600c0be0a51318323`  
		Last Modified: Thu, 23 Mar 2023 13:31:02 GMT  
		Size: 8.0 MB (8045308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33cfeaf50096d9814b4481c61121dfaf3e755f772974f3652841ce4eaaac768a`  
		Last Modified: Thu, 23 Mar 2023 13:31:00 GMT  
		Size: 1.2 MB (1249198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0a34468e21b167f0644c1d2af2e24967064548ded0d9bf90a29c7c3bb7dd82d`  
		Last Modified: Thu, 23 Mar 2023 13:31:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9edf60e692b4f0262a6a66c6d6a4e1bb9c4a4606b59d65377ce3e9775c781c4a`  
		Last Modified: Thu, 23 Mar 2023 13:31:00 GMT  
		Size: 3.2 KB (3198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0c25c97dd604fa0eaa9e52e20863cf422a718dc1e8624b1555cfbc61972fcc4`  
		Last Modified: Thu, 23 Mar 2023 13:31:07 GMT  
		Size: 88.7 MB (88725312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a38583ca5be4fa2614d4e9e836669b0743faecca5cf8a4d042d24b09da6c848`  
		Last Modified: Thu, 23 Mar 2023 13:30:58 GMT  
		Size: 9.8 KB (9782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bccac71f89d3f58697f20f663db97d19babba324cb88f1769fcd7e297cd004e`  
		Last Modified: Thu, 23 Mar 2023 13:30:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962d017c84f9b4fb46e3d0efee236f4efebdd38797c89ac3bf8b60e69a88fbea`  
		Last Modified: Thu, 23 Mar 2023 13:30:58 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061240d550769b9d2796b1cb8feaff1ec6ce7e6e52ba78970eb37d04a737e4ed`  
		Last Modified: Tue, 28 Mar 2023 01:20:59 GMT  
		Size: 4.8 KB (4783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; 386

```console
$ docker pull postgres@sha256:dc8d20379d9f3c2c3e0ad7d2593a277ca079fd95a123e1e89201a681e198d54b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.9 MB (140939087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adee5c061202f717eaf26e9fcec8d8afbc25d4a8862cf91dacb15cca7d878ae1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 23 Mar 2023 00:39:18 GMT
ADD file:315d843eefd4a8bb2345366dcd6bab00a06fca4a7970e220ae8946123d07d7ed in / 
# Thu, 23 Mar 2023 00:39:19 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 10:59:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 10:59:15 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 23 Mar 2023 10:59:15 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 10:59:24 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 10:59:31 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 23 Mar 2023 10:59:31 GMT
ENV LANG=en_US.utf8
# Thu, 23 Mar 2023 10:59:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 10:59:37 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Mar 2023 10:59:38 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 10:59:38 GMT
ENV PG_MAJOR=15
# Thu, 23 Mar 2023 10:59:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Thu, 23 Mar 2023 10:59:38 GMT
ENV PG_VERSION=15.2-1.pgdg110+1
# Thu, 23 Mar 2023 11:14:21 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 23 Mar 2023 11:14:23 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 23 Mar 2023 11:14:24 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Mar 2023 11:14:24 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Mar 2023 11:14:24 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Mar 2023 11:14:24 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 28 Mar 2023 02:38:02 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Tue, 28 Mar 2023 02:38:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Mar 2023 02:38:03 GMT
STOPSIGNAL SIGINT
# Tue, 28 Mar 2023 02:38:03 GMT
EXPOSE 5432
# Tue, 28 Mar 2023 02:38:03 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:3e638a975ea99fe8646002726dcb1ccdccc49ad33967b30337b9b2413e0619b5`  
		Last Modified: Thu, 23 Mar 2023 00:43:09 GMT  
		Size: 32.4 MB (32396277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b5efc39d67da7b52ec54a8ad72b8103590c4e63ab903d7ec703ab719c24fd2`  
		Last Modified: Thu, 23 Mar 2023 12:07:49 GMT  
		Size: 4.8 MB (4813530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba67f18258ea767381c586bbed5a3c15e7a488bfc2caa3b99ce1771ab9b7ef7`  
		Last Modified: Thu, 23 Mar 2023 12:07:47 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446760225b0f099934406c4f375ec245a5de5e8f6811146647baf0486d19cdfb`  
		Last Modified: Thu, 23 Mar 2023 12:07:47 GMT  
		Size: 1.4 MB (1446938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e560907e97a51eb7ba2276bbfff20c1db32c60f627fa2a03776df53c08391e19`  
		Last Modified: Thu, 23 Mar 2023 12:07:48 GMT  
		Size: 8.0 MB (8045241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27814b26385849b51a7063a8114af61e7342658147f027c5fc6c84aee576911c`  
		Last Modified: Thu, 23 Mar 2023 12:07:45 GMT  
		Size: 1.3 MB (1251648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100a5ac21d53d61c336bfca6501fc393b2c84eb7219b48f1a3372920e47fa318`  
		Last Modified: Thu, 23 Mar 2023 12:07:45 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7eb509452c7ea72442acea397c433e531f0fab32051a290ef62b2e508915e42`  
		Last Modified: Thu, 23 Mar 2023 12:07:45 GMT  
		Size: 3.2 KB (3198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc14506e4164a865d4130a66ac71086b15b663bc16b4708bc0b830f93023886`  
		Last Modified: Thu, 23 Mar 2023 12:08:01 GMT  
		Size: 93.0 MB (92965414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be3697d189da3d30e3788815a86f87cc48e71e11fe2d7641a2185c0a6aa2472a`  
		Last Modified: Thu, 23 Mar 2023 12:07:43 GMT  
		Size: 9.8 KB (9783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69765bb0fd3a128e0b196eaa1baec469ce772f2761b5721536f78ea701ca9d95`  
		Last Modified: Thu, 23 Mar 2023 12:07:43 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7978e2a35693b2c534ef0f53b3d32d835b7a6c94cfbe6a3298e557aa169e0425`  
		Last Modified: Thu, 23 Mar 2023 12:07:43 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d828efa8853c0bdfb726c68130c58fdbdac61b761bb44e04a13de800761eca7`  
		Last Modified: Tue, 28 Mar 2023 02:38:44 GMT  
		Size: 4.8 KB (4792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; mips64le

```console
$ docker pull postgres@sha256:abdf9decaf59682122a32e6c7c90d9657a65bf12711e3f2b6ebea1ee9fe12fa8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.2 MB (133219556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d3b48787708498b9176f9f702ea56d3715ef4624f65267e0128959e5f278912`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 23 Mar 2023 05:17:57 GMT
ADD file:fd3a8eec4ae8f6058f522536ca9af1b391f3032504c085d8ddb6f4878ca478d5 in / 
# Thu, 23 Mar 2023 05:18:02 GMT
CMD ["bash"]
# Fri, 24 Mar 2023 00:01:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 24 Mar 2023 00:01:43 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 24 Mar 2023 00:01:45 GMT
ENV GOSU_VERSION=1.16
# Fri, 24 Mar 2023 00:02:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Mar 2023 00:02:45 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Fri, 24 Mar 2023 00:02:47 GMT
ENV LANG=en_US.utf8
# Fri, 24 Mar 2023 00:03:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Mar 2023 00:03:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Mar 2023 00:03:15 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 24 Mar 2023 00:03:18 GMT
ENV PG_MAJOR=15
# Fri, 24 Mar 2023 00:03:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Fri, 24 Mar 2023 00:03:23 GMT
ENV PG_VERSION=15.2-1.pgdg110+1
# Fri, 24 Mar 2023 01:04:11 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 24 Mar 2023 01:04:17 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 24 Mar 2023 01:04:23 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 24 Mar 2023 01:04:26 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 24 Mar 2023 01:04:32 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 24 Mar 2023 01:04:35 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 28 Mar 2023 01:10:19 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Tue, 28 Mar 2023 01:10:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Mar 2023 01:10:25 GMT
STOPSIGNAL SIGINT
# Tue, 28 Mar 2023 01:10:29 GMT
EXPOSE 5432
# Tue, 28 Mar 2023 01:10:32 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:735f9e60414e17ec59baef702f7013b7327899801df2ecf10123ce2727d8dea5`  
		Last Modified: Thu, 23 Mar 2023 05:25:53 GMT  
		Size: 29.6 MB (29634483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f99e1729f3fe396e54005c638a841adbc8d91d377d7477477beee661c93ab65`  
		Last Modified: Fri, 24 Mar 2023 04:54:15 GMT  
		Size: 4.2 MB (4196296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03cd6a7f7dbefc0d6edad4cac9d3305bb9b2e65e63694e81eb6ca68b8c2e0ecb`  
		Last Modified: Fri, 24 Mar 2023 04:54:11 GMT  
		Size: 1.7 KB (1655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09e8b2ec035b7d03a3d62bc303d0f4236caaeb19286e8ed719ba86c876bc99d`  
		Last Modified: Fri, 24 Mar 2023 04:54:12 GMT  
		Size: 1.4 MB (1358242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f194c2ef27189c68e61ca346b1dbbe915027f0043051c9328208db69b0d27f5`  
		Last Modified: Fri, 24 Mar 2023 04:54:15 GMT  
		Size: 8.0 MB (8043844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7f618231d553098705ab70a718b95b9fdcff585305e1bf045d247a0f4e39d1`  
		Last Modified: Fri, 24 Mar 2023 04:54:09 GMT  
		Size: 1.1 MB (1089515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f864e76dd744496c5e6df154192dcf1309ffd336f98a0359adbee0531586b236`  
		Last Modified: Fri, 24 Mar 2023 04:54:09 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d961bb093587b7196b7ba7d0fa06da37079b393d89ad7c544394d8ba070e4f22`  
		Last Modified: Fri, 24 Mar 2023 04:54:09 GMT  
		Size: 3.1 KB (3142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8da4d45c3edba715291e142732abee802b0feeb6b74263d0366e46ef1ee80d`  
		Last Modified: Fri, 24 Mar 2023 04:55:01 GMT  
		Size: 88.9 MB (88877386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662c09223eb1c6934a1422922224877d42a6309f980b9c78f7b5d4570018d0fb`  
		Last Modified: Fri, 24 Mar 2023 04:54:06 GMT  
		Size: 9.8 KB (9793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbaa41eacc26aac205eeb07a1bc596eda85ecd06c0a379aa8a2c9b3c58661edf`  
		Last Modified: Fri, 24 Mar 2023 04:54:06 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb05df66c195784291c8c8e8dbe0453103bf0a860daf0165c88e07309f54502`  
		Last Modified: Fri, 24 Mar 2023 04:54:06 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f168cc1852939584d770fded531298b53d99330ac18b3175aefb456b097cb605`  
		Last Modified: Tue, 28 Mar 2023 01:12:24 GMT  
		Size: 4.8 KB (4785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; ppc64le

```console
$ docker pull postgres@sha256:ba568d114db5b71427a4a9dde0077c47df5b0ca8c1d5a8f699dababa90ff5d8f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.9 MB (147943837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8fc6e758d000a81b9c82b7cf4723859d546f952feb3751cc89f3027a5262698`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 12 Apr 2023 00:08:20 GMT
ADD file:63eb52aaff02c15bceabb87a78eb1b36389066ff4774cf8a754160ca7d509816 in / 
# Wed, 12 Apr 2023 00:08:23 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 05:02:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 Apr 2023 05:02:55 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 12 Apr 2023 05:02:55 GMT
ENV GOSU_VERSION=1.16
# Wed, 12 Apr 2023 05:03:15 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 12 Apr 2023 05:03:30 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 12 Apr 2023 05:03:31 GMT
ENV LANG=en_US.utf8
# Wed, 12 Apr 2023 05:03:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 05:03:43 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 12 Apr 2023 05:03:45 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 12 Apr 2023 05:03:46 GMT
ENV PG_MAJOR=15
# Wed, 12 Apr 2023 05:03:46 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Wed, 12 Apr 2023 05:03:47 GMT
ENV PG_VERSION=15.2-1.pgdg110+1
# Wed, 12 Apr 2023 05:04:47 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 12 Apr 2023 05:04:53 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 12 Apr 2023 05:04:55 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 12 Apr 2023 05:04:55 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 12 Apr 2023 05:04:57 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 12 Apr 2023 05:04:58 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 12 Apr 2023 05:04:58 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Wed, 12 Apr 2023 05:04:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 Apr 2023 05:05:00 GMT
STOPSIGNAL SIGINT
# Wed, 12 Apr 2023 05:05:01 GMT
EXPOSE 5432
# Wed, 12 Apr 2023 05:05:02 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:5b41d5ec640939cf684959234ad3b80909268a32bfd520a31c6720a91521c2fa`  
		Last Modified: Wed, 12 Apr 2023 00:13:13 GMT  
		Size: 35.3 MB (35291995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccb1ca2e8082d7f2e908c0f65ecfca3cb5a0e476d3fd37e81690608c036d044`  
		Last Modified: Wed, 12 Apr 2023 05:10:57 GMT  
		Size: 5.2 MB (5222909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3ecbb301ff302aec5f49ff035102a2f07531dbe1c21358695d166ab7a15658`  
		Last Modified: Wed, 12 Apr 2023 05:10:55 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508555663cada6c60557882d6189b4d045a4aa289ccf31dac997bd59b6387a9c`  
		Last Modified: Wed, 12 Apr 2023 05:10:55 GMT  
		Size: 1.4 MB (1393372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78a033a897e17a1245626e4ccaf84c5060086835b2f66bba8812cb8221a4afc`  
		Last Modified: Wed, 12 Apr 2023 05:10:56 GMT  
		Size: 8.0 MB (8045553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1d7d764d1b4a1e87a59e66a9cf5965f688361d41570c2ab5b26e7e69ac6fe6`  
		Last Modified: Wed, 12 Apr 2023 05:10:53 GMT  
		Size: 1.4 MB (1420262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e66b07f0bb7da9ebb8303127eb0799e5f983297c86857bfbba37e0b2b2d4a9b1`  
		Last Modified: Wed, 12 Apr 2023 05:10:53 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3262e34438ad23be530486ecba19d8e44ade415898517f06476504621b12bae2`  
		Last Modified: Wed, 12 Apr 2023 05:10:53 GMT  
		Size: 3.2 KB (3198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24cd14786d2a220b12abfeb5b44e744c45e236cdf0821995e182efb2a600b7c7`  
		Last Modified: Wed, 12 Apr 2023 05:11:14 GMT  
		Size: 96.5 MB (96549699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aedc237dea5524f9754c3bb06675db602e7f18817143c101daacd473484339aa`  
		Last Modified: Wed, 12 Apr 2023 05:10:51 GMT  
		Size: 9.8 KB (9782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9680142609ae1513fbd31ad007908f09caf26b41109b3940e1cb67a25506bd`  
		Last Modified: Wed, 12 Apr 2023 05:10:51 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94715cd35bece7ce630d041b4d0b899ea1c1eb1e58123a576b3c851d3f617821`  
		Last Modified: Wed, 12 Apr 2023 05:10:51 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bee5f6af92ba5528d579d7a1eb7ca1568bd16f74782fd70e96f4f9ce58f8fd`  
		Last Modified: Wed, 12 Apr 2023 05:10:51 GMT  
		Size: 4.8 KB (4785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:latest` - linux; s390x

```console
$ docker pull postgres@sha256:f1624d2c7b19e781a62dfc104f9b0562986f52018a96c64030efca8fb8fb2023
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.7 MB (85687753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a07d5675bebf713e6bbd8af8b4b74d42d91f429b68a5ba2a701a470123e43a8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 23 Mar 2023 00:44:06 GMT
ADD file:8b6d3f57adaa8af2e0599a6468c50b713d281165b4e61150850bedf587f7ad4f in / 
# Thu, 23 Mar 2023 00:44:08 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 11:21:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Mar 2023 11:21:04 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 23 Mar 2023 11:21:04 GMT
ENV GOSU_VERSION=1.16
# Thu, 23 Mar 2023 11:21:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Mar 2023 11:21:16 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 23 Mar 2023 11:21:16 GMT
ENV LANG=en_US.utf8
# Thu, 23 Mar 2023 11:21:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 11:21:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 23 Mar 2023 11:21:21 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 23 Mar 2023 11:21:21 GMT
ENV PG_MAJOR=15
# Thu, 23 Mar 2023 11:21:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Thu, 23 Mar 2023 11:21:21 GMT
ENV PG_VERSION=15.2-1.pgdg110+1
# Thu, 23 Mar 2023 11:28:31 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 23 Mar 2023 11:28:34 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 23 Mar 2023 11:28:35 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 23 Mar 2023 11:28:35 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 23 Mar 2023 11:28:35 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 23 Mar 2023 11:28:35 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 28 Mar 2023 00:08:29 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Tue, 28 Mar 2023 00:08:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Mar 2023 00:08:29 GMT
STOPSIGNAL SIGINT
# Tue, 28 Mar 2023 00:08:29 GMT
EXPOSE 5432
# Tue, 28 Mar 2023 00:08:29 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:25d08e051bb75230bad82e3a7a054083beec6b4f6a46c8345c731582c297a408`  
		Last Modified: Thu, 23 Mar 2023 00:47:20 GMT  
		Size: 29.6 MB (29646820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e18e93532c47246c3e9d57ecb387990e7550eea2787dae7037142d19e01337a`  
		Last Modified: Thu, 23 Mar 2023 12:05:48 GMT  
		Size: 4.3 MB (4302258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73de5c12adebd6a7a0dc2589be59a06e4f17976c3866d76a38cf50445e545195`  
		Last Modified: Thu, 23 Mar 2023 12:05:47 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cfe3000adb28f647c1e4e0c03addef7c47e742a2afd401faabfc0e1e544f2d9`  
		Last Modified: Thu, 23 Mar 2023 12:05:47 GMT  
		Size: 1.4 MB (1436969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38bad433379bb95836e22787c14c0020c31aee2487d83ffd945b5830795ea25`  
		Last Modified: Thu, 23 Mar 2023 12:05:47 GMT  
		Size: 8.1 MB (8099253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a1552993a1e18aec49dbe9c1620df541b14ea8bae5854d1128d03a9b6a9804`  
		Last Modified: Thu, 23 Mar 2023 12:05:46 GMT  
		Size: 1.2 MB (1237928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4266bfab125be5fc09061853d0826b2efd8e64d56db2761f056141dfbcd572a`  
		Last Modified: Thu, 23 Mar 2023 12:05:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b05f15f4a85e9df955d88f52cdefc7820f61d84059d52cfe0a4aae9b90e94bc`  
		Last Modified: Thu, 23 Mar 2023 12:05:46 GMT  
		Size: 3.2 KB (3197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d643aeb8b7bf46cf55cf44ab3d54f376bb047953daa594d8b811fd37219a875`  
		Last Modified: Thu, 23 Mar 2023 12:05:51 GMT  
		Size: 40.9 MB (40944474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35afdde0f473d679629bc033e6e7be5bc5550ced4540cf0ba3f8a9ee3243daf6`  
		Last Modified: Thu, 23 Mar 2023 12:05:45 GMT  
		Size: 9.8 KB (9788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5924a10940f52e02b4ae26ce85f4231118af3004e0726377b93948a05c2ee4`  
		Last Modified: Thu, 23 Mar 2023 12:05:45 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78727626cea4ce9e90afd534bf064a384d5308c0e3e2f158a71de50dad74ed8`  
		Last Modified: Thu, 23 Mar 2023 12:05:45 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b8536b9c144c84b765fff2b633839cfef227d9035fac48dbe45fce8bcb993c`  
		Last Modified: Tue, 28 Mar 2023 00:09:47 GMT  
		Size: 4.8 KB (4783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
