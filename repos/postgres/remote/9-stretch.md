## `postgres:9-stretch`

```console
$ docker pull postgres@sha256:2edb55745c61b24b5239d2f52ddcf316ee945f17571dc9dbf2e6b3c5f670492d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `postgres:9-stretch` - linux; amd64

```console
$ docker pull postgres@sha256:2bd06eb6958fc4fd8144ddfd1377df0eb580680d97d7161b9a9b86c3e58360ca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73583608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1a34867d7732a3b420533192c9db1cae20c620025a39ade99e0732139d312f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 28 Sep 2021 01:25:30 GMT
ADD file:c7a3b8a1e87bedfb6605855ad703321050112d02c9925ece42f4111d7a42cdd0 in / 
# Tue, 28 Sep 2021 01:25:30 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 17:30:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 17:30:56 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 28 Sep 2021 17:30:56 GMT
ENV GOSU_VERSION=1.12
# Tue, 28 Sep 2021 17:31:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 28 Sep 2021 17:31:15 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 28 Sep 2021 17:31:16 GMT
ENV LANG=en_US.utf8
# Tue, 28 Sep 2021 17:31:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 17:31:21 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 28 Sep 2021 17:31:28 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 28 Sep 2021 17:33:14 GMT
ENV PG_MAJOR=9.6
# Tue, 28 Sep 2021 17:33:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Tue, 28 Sep 2021 17:33:15 GMT
ENV PG_VERSION=9.6.23-1.pgdg90+1
# Tue, 28 Sep 2021 17:33:32 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 28 Sep 2021 17:33:33 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 28 Sep 2021 17:33:34 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 28 Sep 2021 17:33:34 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 28 Sep 2021 17:33:35 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 28 Sep 2021 17:33:35 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 28 Sep 2021 17:33:35 GMT
COPY file:b14ac9ddf7e0a36b021a2f5ce366f60c1befa4d9e96285f4c5a38ce8c3886b3e in /usr/local/bin/ 
# Tue, 28 Sep 2021 17:33:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 28 Sep 2021 17:33:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 17:33:36 GMT
STOPSIGNAL SIGINT
# Tue, 28 Sep 2021 17:33:37 GMT
EXPOSE 5432
# Tue, 28 Sep 2021 17:33:37 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:36d925ed8e305498a951c3b56d100d153ae3babf046b88e2d00899105fe81c31`  
		Last Modified: Tue, 28 Sep 2021 01:32:51 GMT  
		Size: 22.5 MB (22527699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b0099cd1a09b0b2194a09eade24217dcb33a323b2a9c9fa0b1e9675baef91b`  
		Last Modified: Tue, 28 Sep 2021 17:34:37 GMT  
		Size: 4.5 MB (4503770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf2a548fff24ee8a6e8600d9a56374234c0680c30fa06acac089c9ef8bb098b`  
		Last Modified: Tue, 28 Sep 2021 17:34:36 GMT  
		Size: 1.8 KB (1810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e6fa05828bd66b1400946230cb0abe47efae886d300472fa79807765aca6f4`  
		Last Modified: Tue, 28 Sep 2021 17:34:36 GMT  
		Size: 1.4 MB (1412200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000ab621c9681911a41670d9e0b8bb0c51a2b35e65521176e331978e6f6d8b4e`  
		Last Modified: Tue, 28 Sep 2021 17:34:35 GMT  
		Size: 6.2 MB (6185581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6855b4b63497ce5eb706ca2d1c07ee4b92780cfb0f81d00277b9196365ed334b`  
		Last Modified: Tue, 28 Sep 2021 17:34:34 GMT  
		Size: 385.0 KB (384996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9201c39bd81382aed94e5f314936bc4ce379b446ffce65b0ae820577eca6157c`  
		Last Modified: Tue, 28 Sep 2021 17:34:33 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de19e180543b563772c95d696cefc28f3750fa4b9570da276edc631f2078e0a4`  
		Last Modified: Tue, 28 Sep 2021 17:34:33 GMT  
		Size: 5.3 KB (5337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2dc5d4c4017e0a36e4fc97b873172f7e04e0f36ff6af027db255e6329e4e30a`  
		Last Modified: Tue, 28 Sep 2021 17:35:37 GMT  
		Size: 38.5 MB (38549347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af105717b899961918591dcbd9ca626801902d4cd626d2b19306b06628b10636`  
		Last Modified: Tue, 28 Sep 2021 17:35:28 GMT  
		Size: 7.9 KB (7863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c34181d8de310666d9e939d4c33c2686037980368365f2eaaca06cb91238b9b`  
		Last Modified: Tue, 28 Sep 2021 17:35:28 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9a17dced7f4203311a4144be65f424524e53be9b9a94619364402e6a15dbd5`  
		Last Modified: Tue, 28 Sep 2021 17:35:28 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7cc7ee175c3faeecf982eedab1c40d5835a07b4a995c6044d9436bb5a370c2`  
		Last Modified: Tue, 28 Sep 2021 17:35:28 GMT  
		Size: 4.4 KB (4407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a837e2587522ef88cb0cfec0ced723626872950c3ec0939fe224f88c45b976c`  
		Last Modified: Tue, 28 Sep 2021 17:35:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-stretch` - linux; arm variant v5

```console
$ docker pull postgres@sha256:f15cbf157f410581faf0bb777b1d31a5ad0a75bbfb7e1d5fd75edfb9622090fb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.5 MB (70516227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fbe2f18f42e96fa10e5d88a7db9d6acf444f05976228fddae867fe80db3279d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 28 Sep 2021 01:56:40 GMT
ADD file:c0e9a99ba405945353742a7ca9ee5f4807d9626de940828c7e91ea7613fbce6b in / 
# Tue, 28 Sep 2021 01:56:41 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 06:46:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 06:46:02 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 28 Sep 2021 06:46:03 GMT
ENV GOSU_VERSION=1.12
# Tue, 28 Sep 2021 06:46:36 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 28 Sep 2021 06:46:54 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 28 Sep 2021 06:46:55 GMT
ENV LANG=en_US.utf8
# Tue, 28 Sep 2021 06:47:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 06:47:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 28 Sep 2021 06:47:20 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 28 Sep 2021 08:24:50 GMT
ENV PG_MAJOR=9.6
# Tue, 28 Sep 2021 08:24:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Tue, 28 Sep 2021 08:24:51 GMT
ENV PG_VERSION=9.6.23-1.pgdg90+1
# Tue, 28 Sep 2021 08:49:52 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 28 Sep 2021 08:49:54 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 28 Sep 2021 08:49:56 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 28 Sep 2021 08:49:57 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 28 Sep 2021 08:49:58 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 28 Sep 2021 08:49:59 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 28 Sep 2021 08:49:59 GMT
COPY file:b14ac9ddf7e0a36b021a2f5ce366f60c1befa4d9e96285f4c5a38ce8c3886b3e in /usr/local/bin/ 
# Tue, 28 Sep 2021 08:50:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 28 Sep 2021 08:50:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 08:50:02 GMT
STOPSIGNAL SIGINT
# Tue, 28 Sep 2021 08:50:02 GMT
EXPOSE 5432
# Tue, 28 Sep 2021 08:50:03 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:bb8e5fcfd7de8c6ce0f02070264ebe0df51ac6b9717272bead263dd7cca70d0b`  
		Last Modified: Tue, 28 Sep 2021 02:14:29 GMT  
		Size: 21.2 MB (21204242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73644ff9757bcb8fb39d6a3b1f344813adfa61e0a5d9c8cdaa2658d0676d6f6c`  
		Last Modified: Tue, 28 Sep 2021 08:57:47 GMT  
		Size: 4.2 MB (4239296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9581d5c8bb5b918c595eb3b441df16f0486030075effd635f73303bf1e93c9`  
		Last Modified: Tue, 28 Sep 2021 08:57:44 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f69dc224794f632860a105721f6276d38a558bcec13ed570c55a9729c87c4e`  
		Last Modified: Tue, 28 Sep 2021 08:57:45 GMT  
		Size: 1.4 MB (1371454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fd2b370b6cd657f3c85a759ccf13677ef00b7105f3045ba9f10de236ee68ae`  
		Last Modified: Tue, 28 Sep 2021 08:57:47 GMT  
		Size: 6.2 MB (6185662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d625d40558540b118f49566d2c79a33e33b747256c90f5c676fd1a5b8b3db9a`  
		Last Modified: Tue, 28 Sep 2021 08:57:43 GMT  
		Size: 385.1 KB (385051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be0df4e8a7ddf013a43ab3fed0e023abd64860a2f84de78b531eefd31959823`  
		Last Modified: Tue, 28 Sep 2021 08:57:42 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104d0a12b4a41de11f1ff8d9235398510ca444d8ab81cf1448f27a86d982b020`  
		Last Modified: Tue, 28 Sep 2021 08:57:42 GMT  
		Size: 5.3 KB (5342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9fa11f5a54c4e8e1743f369584fb77c9227d99be699cadce81ae5df85ef4b4`  
		Last Modified: Tue, 28 Sep 2021 09:01:09 GMT  
		Size: 37.1 MB (37110492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2245f9f53d7c8807cb6e7251616082cd4326c64a2de4eb405963d1ef491f6e22`  
		Last Modified: Tue, 28 Sep 2021 09:00:41 GMT  
		Size: 7.9 KB (7872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4340cb7b58b40b76aa9f4b8e3610c4125bacb00c14c5529494de961469b1399`  
		Last Modified: Tue, 28 Sep 2021 09:00:41 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9d886fc833c4a0aebb8ff430c7c68154641e34fa85f23905faa08ed148cb63`  
		Last Modified: Tue, 28 Sep 2021 09:00:42 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e136c2827e6f4ddfe393117799865dff40e13748b0a9fcb6ed69f1691e5e7b04`  
		Last Modified: Tue, 28 Sep 2021 09:00:41 GMT  
		Size: 4.4 KB (4410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d10d68e0034d2e61bf128da2c68f2e12e69278c24191c58d43bae8318f976b`  
		Last Modified: Tue, 28 Sep 2021 09:00:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-stretch` - linux; arm variant v7

```console
$ docker pull postgres@sha256:7b9c0c8791c8d7625aef7f8d5d1167ae149645da93ad2f01c26ef14c620b4ccb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67199435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b3f8b650b4596b65ffdfff533a058f1a81d7ab86d5fad64b868482b00530ad6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 03 Sep 2021 01:05:16 GMT
ADD file:425f8ae3b1354b9858904edb027190b58b65692a710cb50a4d463ac554f853a6 in / 
# Fri, 03 Sep 2021 01:05:17 GMT
CMD ["bash"]
# Sat, 04 Sep 2021 02:11:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Sep 2021 02:11:04 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 04 Sep 2021 02:11:05 GMT
ENV GOSU_VERSION=1.12
# Sat, 04 Sep 2021 02:11:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 04 Sep 2021 02:11:50 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 04 Sep 2021 02:11:50 GMT
ENV LANG=en_US.utf8
# Sat, 04 Sep 2021 02:11:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 02:12:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 04 Sep 2021 02:12:13 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Sat, 04 Sep 2021 03:43:01 GMT
ENV PG_MAJOR=9.6
# Sat, 04 Sep 2021 03:43:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Sat, 04 Sep 2021 03:43:02 GMT
ENV PG_VERSION=9.6.23-1.pgdg90+1
# Sat, 04 Sep 2021 04:05:22 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Sat, 04 Sep 2021 04:05:24 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 04 Sep 2021 04:05:25 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 04 Sep 2021 04:05:26 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 04 Sep 2021 04:05:27 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 04 Sep 2021 04:05:28 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 04 Sep 2021 04:05:28 GMT
COPY file:b14ac9ddf7e0a36b021a2f5ce366f60c1befa4d9e96285f4c5a38ce8c3886b3e in /usr/local/bin/ 
# Sat, 04 Sep 2021 04:05:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 04 Sep 2021 04:05:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Sep 2021 04:05:31 GMT
STOPSIGNAL SIGINT
# Sat, 04 Sep 2021 04:05:31 GMT
EXPOSE 5432
# Sat, 04 Sep 2021 04:05:32 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:0c15a1a8c9dffe5dfe059b37d14b92f1eb4ea47f16ae7bf66bf62f34a7510dd6`  
		Last Modified: Fri, 03 Sep 2021 01:22:37 GMT  
		Size: 19.3 MB (19316099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642403b1e08021dae4d804216e6501bd8b4a3b34cec478bd4594d6fb139dd9a6`  
		Last Modified: Sat, 04 Sep 2021 04:14:28 GMT  
		Size: 3.9 MB (3875029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa64f67793a8ed73b6ff1146fb4db81a78e28d52ff9ab133ecd2bafc6c88a90e`  
		Last Modified: Sat, 04 Sep 2021 04:14:25 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbcd3ceed3a694d009ad496642ebb964a00f9d7e7760b8cb0c0dc782d374a84`  
		Last Modified: Sat, 04 Sep 2021 04:14:26 GMT  
		Size: 1.4 MB (1363892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f36abad1d80c59106f577f71dd6fb25594c68ee1d5a5a0c4b6dc431276bb93`  
		Last Modified: Sat, 04 Sep 2021 04:14:28 GMT  
		Size: 6.2 MB (6185677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe2d438af800bceae74d2bb8c1a7715359edfd08c59d16e2efb6673d08d75f2`  
		Last Modified: Sat, 04 Sep 2021 04:14:24 GMT  
		Size: 379.2 KB (379190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef580edaacbebee4a7089addfbc28818dc888de118bdafc377b80d4d976be0d8`  
		Last Modified: Sat, 04 Sep 2021 04:14:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9bd7a8b9c74171813bf055eb26cea24384c3ea40c7a5f122243dba962c80460`  
		Last Modified: Sat, 04 Sep 2021 04:14:23 GMT  
		Size: 5.3 KB (5342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f098fef3b3bef69cd1045047b5e9d1bafcc5bdb2e73f35bd7f9737eaf5a029`  
		Last Modified: Sat, 04 Sep 2021 04:18:00 GMT  
		Size: 36.1 MB (36059531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1852a25565df1ed29303ebe0d371552ca6bb6168049232c11a66b564dfea44f`  
		Last Modified: Sat, 04 Sep 2021 04:17:34 GMT  
		Size: 7.9 KB (7869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822612bd5ec1ed9b178d9ca3a9eb22467bd93a5103231457e7a5fa628ce83287`  
		Last Modified: Sat, 04 Sep 2021 04:17:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae90d20f9e2b6618d7ebdfbb16ec815032672e5bd0653ebcdb45b6e79892dcf`  
		Last Modified: Sat, 04 Sep 2021 04:17:34 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9229f079d62904252cdff97ea5e41a03c4b4c6505fa86caad37f942826ac55b`  
		Last Modified: Sat, 04 Sep 2021 04:17:34 GMT  
		Size: 4.4 KB (4411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49623c4d62e50a64be54c14561956fdfcf92a2d1caf479d4e44790a6be103809`  
		Last Modified: Sat, 04 Sep 2021 04:17:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-stretch` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:175dbfefa3bbb42891aa7fa89fd389eb9bc77a9a63474a8bf11a80128f8e9f1b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69797121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db2d6c22d6bae97a7cd171caea0767cc0ac8dac4e6de543c1e57c50696169c2a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 28 Sep 2021 01:43:26 GMT
ADD file:be175324382a4d494cf1f644f77b27f17829f187478f9eed602be03b358ffbdc in / 
# Tue, 28 Sep 2021 01:43:27 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 11:23:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 11:23:40 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 28 Sep 2021 11:23:40 GMT
ENV GOSU_VERSION=1.12
# Tue, 28 Sep 2021 11:23:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 28 Sep 2021 11:23:59 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 28 Sep 2021 11:23:59 GMT
ENV LANG=en_US.utf8
# Tue, 28 Sep 2021 11:24:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 11:24:04 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 28 Sep 2021 11:24:15 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 28 Sep 2021 11:44:32 GMT
ENV PG_MAJOR=9.6
# Tue, 28 Sep 2021 11:44:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Tue, 28 Sep 2021 11:44:32 GMT
ENV PG_VERSION=9.6.23-1.pgdg90+1
# Tue, 28 Sep 2021 11:53:46 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 28 Sep 2021 11:53:47 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 28 Sep 2021 11:53:48 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 28 Sep 2021 11:53:48 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 28 Sep 2021 11:53:48 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 28 Sep 2021 11:53:49 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 28 Sep 2021 11:53:49 GMT
COPY file:b14ac9ddf7e0a36b021a2f5ce366f60c1befa4d9e96285f4c5a38ce8c3886b3e in /usr/local/bin/ 
# Tue, 28 Sep 2021 11:53:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 28 Sep 2021 11:53:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 11:53:50 GMT
STOPSIGNAL SIGINT
# Tue, 28 Sep 2021 11:53:50 GMT
EXPOSE 5432
# Tue, 28 Sep 2021 11:53:50 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:754614322eeee5db75df451bbdaf75a2049b3ffb0bbcc404a80770f454125583`  
		Last Modified: Tue, 28 Sep 2021 01:52:52 GMT  
		Size: 20.4 MB (20389432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c66dc0f0439952f17ff81d475fd9f303fd7a160a7b1a37f068bc3e3d1d0b02`  
		Last Modified: Tue, 28 Sep 2021 11:58:26 GMT  
		Size: 4.1 MB (4078920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:110c52665f42bfc240a88897e37a28a669c3876d39e55fce27d64139aafd2770`  
		Last Modified: Tue, 28 Sep 2021 11:58:25 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b224527b40165c66a822c2b7cb119e61d9e719b23bf8a9cbba1c481cad2cc77e`  
		Last Modified: Tue, 28 Sep 2021 11:58:25 GMT  
		Size: 1.3 MB (1347007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd958bf215af4549f6f9f997f01e7a994e7a84afd160a9fc368cba5ca09f027b`  
		Last Modified: Tue, 28 Sep 2021 11:58:23 GMT  
		Size: 6.2 MB (6185143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5dc95d3093c4b910c3d8aaaa6974f2a832161e5cccb60cce75c19b4c52d3407`  
		Last Modified: Tue, 28 Sep 2021 11:58:23 GMT  
		Size: 377.9 KB (377852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc73d8c3095228b0f0825a32dda1b173c25a2b78d086cf3d672436ffe5f5c5cd`  
		Last Modified: Tue, 28 Sep 2021 11:58:22 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a20fc9638f39345ff08af30613d61a26fe26efd0ebec0801c19ef15c6fcb91`  
		Last Modified: Tue, 28 Sep 2021 11:58:22 GMT  
		Size: 5.3 KB (5339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46894fd9e9ad722b827840e12979a3b389d94a13e16fba8fe204f0ee6195f1ed`  
		Last Modified: Tue, 28 Sep 2021 12:00:14 GMT  
		Size: 37.4 MB (37398735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e35410551d489164d0697eddb85c21803dc3301ac16401f029630452161e0d`  
		Last Modified: Tue, 28 Sep 2021 12:00:05 GMT  
		Size: 7.9 KB (7870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eefb5e9d14387284938d67b13aa6abdc161d1c71f3482230969edd0b75fd1c2`  
		Last Modified: Tue, 28 Sep 2021 12:00:05 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872dbca735aa4444974d8d8fdad6e2a1e786d2bc1ebaa9c467e5a08006615535`  
		Last Modified: Tue, 28 Sep 2021 12:00:05 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5e4e52948ed6da51249518d068dfb9e481ccbff95a521be76d48c3f97befe4`  
		Last Modified: Tue, 28 Sep 2021 12:00:06 GMT  
		Size: 4.4 KB (4411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:549ad6e23dcce2a9d0063bf1974dcdcb171e98165c81c8a438bfa47cae90302d`  
		Last Modified: Tue, 28 Sep 2021 12:00:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-stretch` - linux; 386

```console
$ docker pull postgres@sha256:31d58f2965720924991b7130aa5bf45d739802b0abfcbf1e0de212843b106182
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74724255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df9a56359820f2bf2bb25be53199eec7d8640cf647b5f516592fdf3e47d3db66`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Fri, 03 Sep 2021 00:42:46 GMT
ADD file:6c8a44184bf1d38b16f52d58ecb80d627ab86fce72a78b094170535fe1f76ad0 in / 
# Fri, 03 Sep 2021 00:42:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 16:04:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 03 Sep 2021 16:04:13 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 03 Sep 2021 16:04:13 GMT
ENV GOSU_VERSION=1.12
# Fri, 03 Sep 2021 16:04:36 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 03 Sep 2021 16:04:49 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Fri, 03 Sep 2021 16:04:50 GMT
ENV LANG=en_US.utf8
# Fri, 03 Sep 2021 16:04:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 16:05:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 03 Sep 2021 16:05:08 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Fri, 03 Sep 2021 16:07:46 GMT
ENV PG_MAJOR=9.6
# Fri, 03 Sep 2021 16:07:46 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Fri, 03 Sep 2021 16:07:47 GMT
ENV PG_VERSION=9.6.23-1.pgdg90+1
# Fri, 03 Sep 2021 16:08:17 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 03 Sep 2021 16:08:19 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 03 Sep 2021 16:08:21 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 03 Sep 2021 16:08:22 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 03 Sep 2021 16:08:24 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 03 Sep 2021 16:08:24 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 03 Sep 2021 16:08:24 GMT
COPY file:b14ac9ddf7e0a36b021a2f5ce366f60c1befa4d9e96285f4c5a38ce8c3886b3e in /usr/local/bin/ 
# Fri, 03 Sep 2021 16:08:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 03 Sep 2021 16:08:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Sep 2021 16:08:26 GMT
STOPSIGNAL SIGINT
# Fri, 03 Sep 2021 16:08:27 GMT
EXPOSE 5432
# Fri, 03 Sep 2021 16:08:27 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:0b43614231856f083f6dc06bd012a7ac7ff26410a945ea25d4c887e8218a878c`  
		Last Modified: Fri, 03 Sep 2021 00:53:23 GMT  
		Size: 23.2 MB (23156443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abea021c5bc89b9f765dd715203d1385b53a29ccfa57f89bcd984005cf69c726`  
		Last Modified: Fri, 03 Sep 2021 16:14:45 GMT  
		Size: 4.8 MB (4811150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a98f6a5975361064b7aeb87d1b9d605c8de7dbe54b5cd6fc8a79a05b3dfd0f8`  
		Last Modified: Fri, 03 Sep 2021 16:14:42 GMT  
		Size: 1.8 KB (1800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838d0a09d7215471a71ef652e21e61fdb937b1ed8bec98d0ab985e8231bad43a`  
		Last Modified: Fri, 03 Sep 2021 16:14:43 GMT  
		Size: 1.4 MB (1382508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ee70d258a0c0b0a9b70578eea4506ef1e0d9c2957b6d53c71d3da95adfde2f`  
		Last Modified: Fri, 03 Sep 2021 16:14:43 GMT  
		Size: 6.2 MB (6185570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fd2706bb58d86695a5979067348a92b7efa5d06c3fa2d270f514e79881239d`  
		Last Modified: Fri, 03 Sep 2021 16:14:40 GMT  
		Size: 393.3 KB (393335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c646f28e6bd0662e1b06bbc1a601e2f95e19182e9645749540f1a8e7092a49`  
		Last Modified: Fri, 03 Sep 2021 16:14:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff53030bfd0020aeb52e4e9f505cb48941c20105c32895230eb4985ebb7c8e8`  
		Last Modified: Fri, 03 Sep 2021 16:14:39 GMT  
		Size: 5.3 KB (5343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc1f27adef8c04213c66b6c012170f907b7cd77b7fbd0e0d29aa2aa9edb8d689`  
		Last Modified: Fri, 03 Sep 2021 16:17:36 GMT  
		Size: 38.8 MB (38775236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44253c0528c8e6067ccf5ffe7b3533cfce614dde988a41593a1d0a4c4d3c35a`  
		Last Modified: Fri, 03 Sep 2021 16:17:20 GMT  
		Size: 7.9 KB (7865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4e755f648f1172bec7d413708e45e62e0761000a23510d8decf8a8dadc84be`  
		Last Modified: Fri, 03 Sep 2021 16:17:20 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb940d1b1b68c776780f462325bb1bb985cf4f6918bd3a6251cfb440a306e550`  
		Last Modified: Fri, 03 Sep 2021 16:17:20 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b5e81c55fc68346a7831f2948d8f67f4516c5fd92730872ea2f5d64ad7c6e6`  
		Last Modified: Fri, 03 Sep 2021 16:17:20 GMT  
		Size: 4.4 KB (4406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4c0a7fb4ab81bfb293977721f97cf49bbf15fe8fc89483cce4686420691927`  
		Last Modified: Fri, 03 Sep 2021 16:17:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
