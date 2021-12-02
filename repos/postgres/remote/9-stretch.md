## `postgres:9-stretch`

```console
$ docker pull postgres@sha256:1c619c2b1ff8fee6ca29930e032bf853ece75aeb5e549bfc74a994a0e863a488
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
$ docker pull postgres@sha256:44128e2a3492fc644bb3e672797640a124aca6f27975d1b326e8a8bac69d2b62
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73550076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f068f0e4efc337156a22bcb55b54b072d5d65c87873f9c8f60ac3b637a49159`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 17 Nov 2021 02:22:38 GMT
ADD file:2868c3af63afe6b8aadac07b8776e5468a3ed135fd84ad22df15e48f0610c7ba in / 
# Wed, 17 Nov 2021 02:22:38 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 21:57:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 21:57:36 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 30 Nov 2021 05:25:58 GMT
ENV GOSU_VERSION=1.14
# Tue, 30 Nov 2021 05:26:20 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 30 Nov 2021 05:26:26 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 30 Nov 2021 05:26:26 GMT
ENV LANG=en_US.utf8
# Tue, 30 Nov 2021 05:26:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Nov 2021 05:26:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 30 Nov 2021 05:26:43 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 30 Nov 2021 05:39:45 GMT
ENV PG_MAJOR=9.6
# Tue, 30 Nov 2021 05:39:46 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Tue, 30 Nov 2021 05:39:46 GMT
ENV PG_VERSION=9.6.24-1.pgdg90+1
# Tue, 30 Nov 2021 05:40:11 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 30 Nov 2021 05:40:13 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 30 Nov 2021 05:40:14 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 30 Nov 2021 05:40:14 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 30 Nov 2021 05:40:16 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 30 Nov 2021 05:40:16 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 30 Nov 2021 05:40:16 GMT
COPY file:73785d4a64e88cd001941f2d0fb17c583e6d98ffda704b27106f5ef128737e5b in /usr/local/bin/ 
# Tue, 30 Nov 2021 05:40:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 30 Nov 2021 05:40:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 Nov 2021 05:40:19 GMT
STOPSIGNAL SIGINT
# Tue, 30 Nov 2021 05:40:19 GMT
EXPOSE 5432
# Tue, 30 Nov 2021 05:40:20 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:89166b5eeae47d8c878cb88f20cc67eda2a550a697f4be317c7b7abea566b76f`  
		Last Modified: Wed, 17 Nov 2021 02:29:32 GMT  
		Size: 22.5 MB (22527686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ee3d94b0b2d5764212e2d7e629e9c3de7128ae21f9676d21cf8a4345241960`  
		Last Modified: Wed, 17 Nov 2021 22:03:44 GMT  
		Size: 4.5 MB (4503831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11070db47648b9388a78654fa06b64818270d1fffd11f47b2d0724a2d2b5743`  
		Last Modified: Wed, 17 Nov 2021 22:03:43 GMT  
		Size: 1.8 KB (1811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e48ec3c101d1c9eb35ea72bf8bf7ea213f177f7b5ce712eccdb7d8981a543f9`  
		Last Modified: Tue, 30 Nov 2021 05:52:07 GMT  
		Size: 1.4 MB (1379405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a551d86500bc639cb60426e69632857adc622b692459f43201f680d8a75f2d7`  
		Last Modified: Tue, 30 Nov 2021 05:52:05 GMT  
		Size: 6.2 MB (6185285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21d1b96372a4d706f9a80b3973b4714d19fc5dfa05b2d4463d53f373ab5a3d5`  
		Last Modified: Tue, 30 Nov 2021 05:52:05 GMT  
		Size: 385.0 KB (385043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b707b86b0a88e71222795426118e56a17b9200c7548b14876c2436ed6cef80d0`  
		Last Modified: Tue, 30 Nov 2021 05:52:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51dbb0367cc1887e834da274499f2b7fcb2e594f60d20a2511cecf2931e33cf1`  
		Last Modified: Tue, 30 Nov 2021 05:52:04 GMT  
		Size: 5.3 KB (5342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeecd10a1ea135ab5a6446baa8a6ef9c4ff2c5bf6e9351e41f8cd6604187c760`  
		Last Modified: Tue, 30 Nov 2021 05:54:45 GMT  
		Size: 38.5 MB (38548474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f40406fc636f473e05359b0dd6944ffd4782e278c169a5e2ab274edf8f50bf`  
		Last Modified: Tue, 30 Nov 2021 05:54:35 GMT  
		Size: 7.9 KB (7873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11a895b2b56573cc891c2801f7ffe97a2e6e76e9e947d83800f3e0fc27de28e`  
		Last Modified: Tue, 30 Nov 2021 05:54:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24b80c81d33fb70d28d47b8ef8a811041426a6ef7b5326d799a9922df4b1c00`  
		Last Modified: Tue, 30 Nov 2021 05:54:35 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be8ca79649d8c00a8e2d60bbfb7db3401119fdc7ab94372cef62a476d839260`  
		Last Modified: Tue, 30 Nov 2021 05:54:35 GMT  
		Size: 4.7 KB (4726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7597519b7005a4f76d659e4546b9f3aa374071707fa5dfbff832f9bd6a1684d9`  
		Last Modified: Tue, 30 Nov 2021 05:54:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-stretch` - linux; arm variant v5

```console
$ docker pull postgres@sha256:05ae84ad8575529461c5afad78012a5ac1e93c9d1fc7f8211608eb6fcd121d96
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70576503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:033820e4fc19b38cd29b5101ed871f55904e09d959c39a5ef13b1c5a1299bd72`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 02 Dec 2021 02:57:55 GMT
ADD file:a1e328a7ceac3e567d9b78728b38c24f0199a7765deee05ba8115785a892b58f in / 
# Thu, 02 Dec 2021 02:57:56 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 08:26:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 08:26:55 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 02 Dec 2021 08:26:56 GMT
ENV GOSU_VERSION=1.14
# Thu, 02 Dec 2021 08:27:30 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 02 Dec 2021 08:27:49 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 02 Dec 2021 08:27:50 GMT
ENV LANG=en_US.utf8
# Thu, 02 Dec 2021 08:28:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 08:28:04 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 02 Dec 2021 08:28:14 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Thu, 02 Dec 2021 09:45:23 GMT
ENV PG_MAJOR=9.6
# Thu, 02 Dec 2021 09:45:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Thu, 02 Dec 2021 09:45:24 GMT
ENV PG_VERSION=9.6.24-1.pgdg90+1
# Thu, 02 Dec 2021 10:10:51 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 02 Dec 2021 10:10:53 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 02 Dec 2021 10:10:55 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 02 Dec 2021 10:10:55 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 02 Dec 2021 10:10:57 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 02 Dec 2021 10:10:57 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 02 Dec 2021 10:10:58 GMT
COPY file:73785d4a64e88cd001941f2d0fb17c583e6d98ffda704b27106f5ef128737e5b in /usr/local/bin/ 
# Thu, 02 Dec 2021 10:10:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 02 Dec 2021 10:11:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Dec 2021 10:11:00 GMT
STOPSIGNAL SIGINT
# Thu, 02 Dec 2021 10:11:01 GMT
EXPOSE 5432
# Thu, 02 Dec 2021 10:11:01 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:6213aa8d791a7975f08a10bcacb7d9ef2d07474b772a2fe57ff37c4b0d47b28a`  
		Last Modified: Thu, 02 Dec 2021 03:15:59 GMT  
		Size: 21.2 MB (21203460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913f1c876703293ef5eae9131b972093f1c34712ea17fbbe31dda31f5c3e9c0f`  
		Last Modified: Thu, 02 Dec 2021 10:19:41 GMT  
		Size: 4.2 MB (4239302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f10f1250dd99b3e36d245ab86fa2725737a96806e76525d81c1b3041a847d0b1`  
		Last Modified: Thu, 02 Dec 2021 10:19:38 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b10ebdde8c7786ff94f89a7c60484f69fef18f3725f301999097dfce3cf3b4`  
		Last Modified: Thu, 02 Dec 2021 10:19:38 GMT  
		Size: 1.3 MB (1344273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f398500633ceb3cf3841b9dc3fa07c4c1a7464be5a5a624619161844c67d55`  
		Last Modified: Thu, 02 Dec 2021 10:19:40 GMT  
		Size: 6.2 MB (6185675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e92443232f77b9ecda0a2c04dbc961034c17fecdfb0c2e00f4b546f980c80e3`  
		Last Modified: Thu, 02 Dec 2021 10:19:36 GMT  
		Size: 385.1 KB (385071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16588a6aa38d1c629c69c175cc7a99904c813960ff4a8ed3bfc7663595c623c`  
		Last Modified: Thu, 02 Dec 2021 10:19:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b9c1e6b3b638ad02886239e2d41b70d7192613762a4444115331b0538f3e95`  
		Last Modified: Thu, 02 Dec 2021 10:19:35 GMT  
		Size: 5.3 KB (5345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978d6e0a66f4abee78562f7da609206fc2b691334d4a63b049cc5ea27259cbcc`  
		Last Modified: Thu, 02 Dec 2021 10:22:18 GMT  
		Size: 37.2 MB (37198378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5b63dc4942b2c725150f58b29598f4c385f6c378e25af981b02ecf69f46e42`  
		Last Modified: Thu, 02 Dec 2021 10:21:51 GMT  
		Size: 7.9 KB (7871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:accaf4617f3a15df1fd71e1bef0743039e0047627cbb184378a00bf2cae9fcfd`  
		Last Modified: Thu, 02 Dec 2021 10:21:51 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf892a53871da9e33b293c147b9420896f7340943940e073d53adbe11313e10`  
		Last Modified: Thu, 02 Dec 2021 10:21:50 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546236e4128d5314e101dbdd56a7c85985c5257fdaa59209e0300a5a80138284`  
		Last Modified: Thu, 02 Dec 2021 10:21:51 GMT  
		Size: 4.7 KB (4730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d8a62f9fd72d13c74b7f12b51c7f11dbb66aaaa65e0aa34229aee7836cd32a`  
		Last Modified: Thu, 02 Dec 2021 10:21:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-stretch` - linux; arm variant v7

```console
$ docker pull postgres@sha256:fe2349a4b47cd0d13505987a0c0018a3a0f329a269d97d75135e4cce6a41c5a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67246299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d20c3e75c6c2a3da6dcd72f5ad17720058a9ba276b72001a9129fcc20ce26b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 17 Nov 2021 02:05:31 GMT
ADD file:f28546ff6a3759d3a957c25d4310c3065e1367dff4ae304caae1cf1dc64d061d in / 
# Wed, 17 Nov 2021 02:05:32 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 20:15:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 20:15:48 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 30 Nov 2021 09:36:26 GMT
ENV GOSU_VERSION=1.14
# Tue, 30 Nov 2021 09:36:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 30 Nov 2021 09:37:13 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 30 Nov 2021 09:37:14 GMT
ENV LANG=en_US.utf8
# Tue, 30 Nov 2021 09:37:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Nov 2021 09:37:24 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 30 Nov 2021 09:37:36 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 30 Nov 2021 11:35:34 GMT
ENV PG_MAJOR=9.6
# Tue, 30 Nov 2021 11:35:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Tue, 30 Nov 2021 11:35:35 GMT
ENV PG_VERSION=9.6.24-1.pgdg90+1
# Tue, 30 Nov 2021 11:58:03 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 30 Nov 2021 11:58:06 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 30 Nov 2021 11:58:07 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 30 Nov 2021 11:58:07 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 30 Nov 2021 11:58:09 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 30 Nov 2021 11:58:09 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 30 Nov 2021 11:58:10 GMT
COPY file:73785d4a64e88cd001941f2d0fb17c583e6d98ffda704b27106f5ef128737e5b in /usr/local/bin/ 
# Tue, 30 Nov 2021 11:58:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 30 Nov 2021 11:58:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 Nov 2021 11:58:12 GMT
STOPSIGNAL SIGINT
# Tue, 30 Nov 2021 11:58:13 GMT
EXPOSE 5432
# Tue, 30 Nov 2021 11:58:13 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:614e23553da11f1294dc969bcab416c9f981794bdbaee5641335a222730c63b2`  
		Last Modified: Wed, 17 Nov 2021 02:22:41 GMT  
		Size: 19.3 MB (19316397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2effe6a5f16302abc8031470eb48915a81617487a7cd06cf52b124ab1002c8fb`  
		Last Modified: Wed, 17 Nov 2021 22:20:28 GMT  
		Size: 3.9 MB (3875425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670859d248795266b6fcb5b5607b9fcbc56b555701abde40671010685985c17f`  
		Last Modified: Wed, 17 Nov 2021 22:20:25 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5cef825a5bdb6d9d0b514ff71911ebbc21ff0d7e8fa41f4adc5a7703649d1d`  
		Last Modified: Tue, 30 Nov 2021 12:17:07 GMT  
		Size: 1.3 MB (1335890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9deff4a6a0f4977c3df43dacb8403dba26757e1eafbfc2118f9aa6cb13fdb94`  
		Last Modified: Tue, 30 Nov 2021 12:17:09 GMT  
		Size: 6.2 MB (6185633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb78a400d60c6dd6f3663e8f5791a763c44a63f04cc2ae284c859da6e1bbd99b`  
		Last Modified: Tue, 30 Nov 2021 12:17:05 GMT  
		Size: 379.2 KB (379188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03780188e28825795488afc3dbdb645d03dbbe7b143bae4784460d96b7b0b314`  
		Last Modified: Tue, 30 Nov 2021 12:17:05 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27d85d8b3265729e4bef90d9b10463f843f9e84cab936f0d42c14795e81b30c`  
		Last Modified: Tue, 30 Nov 2021 12:17:05 GMT  
		Size: 5.3 KB (5346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6649e22c48f80bcc10a09b16fe2efb525a24b11a18ce3c3519e0e2f30c6b3bf9`  
		Last Modified: Tue, 30 Nov 2021 12:22:00 GMT  
		Size: 36.1 MB (36133410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f73678d4d40594a2aecf3bdde8d9e31a2ba76c312739901f6b4f6f776d752b`  
		Last Modified: Tue, 30 Nov 2021 12:21:35 GMT  
		Size: 7.9 KB (7878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e619e0d64666c4c02fb9bbab7f41c60607657f67cbc0308c3c0509ce4ac1c3d`  
		Last Modified: Tue, 30 Nov 2021 12:21:35 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d805483aed0c7642c39d2e114ac68cac0f90098e0fc42ee72dc644f55450aa`  
		Last Modified: Tue, 30 Nov 2021 12:21:35 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8183d5186ec69f402918efe47eddc39b47c2770baf2106ecd2826aaa522aed98`  
		Last Modified: Tue, 30 Nov 2021 12:21:35 GMT  
		Size: 4.7 KB (4731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116c7a6248b66578c3af402d98f595839c5368b98539351ea06fb452918d8ea3`  
		Last Modified: Tue, 30 Nov 2021 12:21:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-stretch` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:b533e30f1e08498e60014865c61a2b3280897f76f06106d007f5161cf9328703
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69449673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:068f7f0320020769fc24bfeb779d0910797eb03546880ef95e0ed6724fb61f24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 02 Dec 2021 08:10:23 GMT
ADD file:d9d01d3468e590cea0e2803b24fa9d34ca1d3eb31b517a5a0edf081f85e7dcc1 in / 
# Thu, 02 Dec 2021 08:10:23 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 14:24:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Dec 2021 14:24:52 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 02 Dec 2021 14:24:53 GMT
ENV GOSU_VERSION=1.14
# Thu, 02 Dec 2021 14:25:06 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 02 Dec 2021 14:25:12 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 02 Dec 2021 14:25:13 GMT
ENV LANG=en_US.utf8
# Thu, 02 Dec 2021 14:25:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 14:25:18 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 02 Dec 2021 14:25:27 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Thu, 02 Dec 2021 14:45:25 GMT
ENV PG_MAJOR=9.6
# Thu, 02 Dec 2021 14:45:26 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Thu, 02 Dec 2021 14:45:27 GMT
ENV PG_VERSION=9.6.24-1.pgdg90+1
# Thu, 02 Dec 2021 14:53:55 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 02 Dec 2021 14:53:56 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 02 Dec 2021 14:53:57 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 02 Dec 2021 14:53:58 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 02 Dec 2021 14:53:59 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 02 Dec 2021 14:54:00 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 02 Dec 2021 14:54:02 GMT
COPY file:73785d4a64e88cd001941f2d0fb17c583e6d98ffda704b27106f5ef128737e5b in /usr/local/bin/ 
# Thu, 02 Dec 2021 14:54:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 02 Dec 2021 14:54:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Dec 2021 14:54:04 GMT
STOPSIGNAL SIGINT
# Thu, 02 Dec 2021 14:54:05 GMT
EXPOSE 5432
# Thu, 02 Dec 2021 14:54:06 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:99dcd33b7a52fa23a15c1dc3456487807f7ad0f48f3df675dc13490656cc96f9`  
		Last Modified: Thu, 02 Dec 2021 08:44:55 GMT  
		Size: 20.4 MB (20389365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13f4e0a897ff7d8dfcbe3ebe4a891caa5e91281627586e8d4e0ba65fca20064`  
		Last Modified: Thu, 02 Dec 2021 14:58:38 GMT  
		Size: 3.9 MB (3890683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e4006bd82ee6a2e27a6d841e437077daa7202a8847fbca466f9f6561dc5322`  
		Last Modified: Thu, 02 Dec 2021 14:58:36 GMT  
		Size: 1.7 KB (1663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef5686a034a22c158862ab36d94a9e9352929f2824c0974089da35ab58e2fca`  
		Last Modified: Thu, 02 Dec 2021 14:58:36 GMT  
		Size: 1.3 MB (1307689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b36de2354f710c3cb7df0985cfe76bb9345dc93530826ffdb57279eb18a831`  
		Last Modified: Thu, 02 Dec 2021 14:58:36 GMT  
		Size: 6.2 MB (6182382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6aa3a5a53efc3ef238a0f8ebd180ca406afe7c11f2dbd4dc4ae449f36ebb1d9`  
		Last Modified: Thu, 02 Dec 2021 14:58:34 GMT  
		Size: 173.4 KB (173393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df4a4b5f9f5e989af72c0c52e177a4673f3a011cd4f626d62c59dbecfa702381`  
		Last Modified: Thu, 02 Dec 2021 14:58:34 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60555f757ad0ac1d25a58699559c20e5bb454774cf10a3fa887107d5fa344615`  
		Last Modified: Thu, 02 Dec 2021 14:58:34 GMT  
		Size: 5.3 KB (5316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f848e849b02bc9530e7adc75eb8cf64d31d5c66f3199e5e4a8a6af0e524081`  
		Last Modified: Thu, 02 Dec 2021 15:00:21 GMT  
		Size: 37.5 MB (37486042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5184cab493456f5b311b67aff1cf6eb3af8cc724dfea21ba937aa52d94c77a02`  
		Last Modified: Thu, 02 Dec 2021 15:00:10 GMT  
		Size: 7.9 KB (7878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956c2539b05102d65e0f6dda364e1712186675dd59fb8b5b94072367a8bdbd2b`  
		Last Modified: Thu, 02 Dec 2021 15:00:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34159ccae07791c491fa98a75c711e4057ba2ff2cd39ff5802c87decfad07022`  
		Last Modified: Thu, 02 Dec 2021 15:00:10 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61333c4cb334d39c3122c5316e176daee9746b42d95d97b6df2adc886096b06`  
		Last Modified: Thu, 02 Dec 2021 15:00:10 GMT  
		Size: 4.7 KB (4730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:435dde6f1790e049e1e369c1d48d9e1536a09c54ffd37dd39e4a5b5d111c5f88`  
		Last Modified: Thu, 02 Dec 2021 15:00:10 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-stretch` - linux; 386

```console
$ docker pull postgres@sha256:f02a35866eda4431f0af9713d1397d6e5224167e81490bce50625fd89a497c7f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74678841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d06a3f3934cc25cca3a098813f6a352cb6c3b4d07f6756a161680fc28010d3ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:36 GMT
ADD file:3c9c1d0f88db0341cbe43b594cf6d2d865e39d9518b8e2b124cb9736bebe18f3 in / 
# Wed, 17 Nov 2021 02:42:37 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 14:53:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 14:54:00 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 30 Nov 2021 03:57:13 GMT
ENV GOSU_VERSION=1.14
# Tue, 30 Nov 2021 03:57:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 30 Nov 2021 03:57:36 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 30 Nov 2021 03:57:36 GMT
ENV LANG=en_US.utf8
# Tue, 30 Nov 2021 03:57:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Nov 2021 03:57:41 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 30 Nov 2021 03:57:51 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 30 Nov 2021 04:34:14 GMT
ENV PG_MAJOR=9.6
# Tue, 30 Nov 2021 04:34:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Tue, 30 Nov 2021 04:34:15 GMT
ENV PG_VERSION=9.6.24-1.pgdg90+1
# Tue, 30 Nov 2021 04:34:35 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 30 Nov 2021 04:34:37 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 30 Nov 2021 04:34:38 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 30 Nov 2021 04:34:38 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 30 Nov 2021 04:34:39 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 30 Nov 2021 04:34:39 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 30 Nov 2021 04:34:39 GMT
COPY file:73785d4a64e88cd001941f2d0fb17c583e6d98ffda704b27106f5ef128737e5b in /usr/local/bin/ 
# Tue, 30 Nov 2021 04:34:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Tue, 30 Nov 2021 04:34:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 Nov 2021 04:34:41 GMT
STOPSIGNAL SIGINT
# Tue, 30 Nov 2021 04:34:41 GMT
EXPOSE 5432
# Tue, 30 Nov 2021 04:34:41 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:d213b39bd355350279fd232f3eedd77a11f7fb2a3d5a0017357dd45fa88342d1`  
		Last Modified: Wed, 17 Nov 2021 02:52:49 GMT  
		Size: 23.2 MB (23156564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc08762ac2638fdc5d798ba8a717a91d7fbcd7421f6ec0f557c6d1eb6f03c0d`  
		Last Modified: Wed, 17 Nov 2021 15:24:32 GMT  
		Size: 4.8 MB (4811942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358db85f042b097401ff43f08eea1438a5b1bc968738ae1cfa437a21d436f9be`  
		Last Modified: Wed, 17 Nov 2021 15:24:31 GMT  
		Size: 1.8 KB (1801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b86c0ee4273eb6b713c1debc299c7d302bb29e45f1a192ee6aabcebb4635050`  
		Last Modified: Tue, 30 Nov 2021 04:47:41 GMT  
		Size: 1.3 MB (1347275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd466c9fb1a48aca5f4a766f5caade3755ca75146d6bda121e30c5fc52f39c3`  
		Last Modified: Tue, 30 Nov 2021 04:47:41 GMT  
		Size: 6.2 MB (6185183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a368c593985ff88b2b23c18669f855caa928d32aba48b4e3bfd6e1e78a9d8b09`  
		Last Modified: Tue, 30 Nov 2021 04:47:39 GMT  
		Size: 393.3 KB (393334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a139a1de4c617e9683f6035bf8ab5e0ced6501dd7e4a15c8cc88b41b8b86b2eb`  
		Last Modified: Tue, 30 Nov 2021 04:47:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5751839c1edb4176c7478a91082aa9af772d520186d77b724011fce1f8c9848`  
		Last Modified: Tue, 30 Nov 2021 04:47:39 GMT  
		Size: 5.3 KB (5345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a669624a181772a1bec075d063c5474f8b9ddaee54b864add4d2f3540bba189`  
		Last Modified: Tue, 30 Nov 2021 04:50:53 GMT  
		Size: 38.8 MB (38764195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d660fb1acc91c6e982738d1ce91e50c85299b2600bb3191499962e9273da13e7`  
		Last Modified: Tue, 30 Nov 2021 04:50:43 GMT  
		Size: 7.9 KB (7872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39c78e234f210b21bf3ed6ed3627bbe90e22b4005c9a5d44641a94dbc82d318`  
		Last Modified: Tue, 30 Nov 2021 04:50:43 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc3185017fc2da731d1d0a2ea79b8fc5c42ce3ef9e9c405f70d1e8ada5c0fbf5`  
		Last Modified: Tue, 30 Nov 2021 04:50:43 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5da3d24ed53791480061b15f8cc2b3cd99349fa32b213c3b1c49aba875f0cef`  
		Last Modified: Tue, 30 Nov 2021 04:50:43 GMT  
		Size: 4.7 KB (4730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bd7988038636e62b2d80fff8c07d9b3ac8732f2345ade633aecb5d5736d7869`  
		Last Modified: Tue, 30 Nov 2021 04:50:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
