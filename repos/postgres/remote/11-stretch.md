## `postgres:11-stretch`

```console
$ docker pull postgres@sha256:bba187f7bbc8e99f7410621e983bce53825882e172cbcde2886f4b05ed6dca0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `postgres:11-stretch` - linux; amd64

```console
$ docker pull postgres@sha256:3efdf63f9010cea0136e73459a5d36583716dbfb21f4729752d122ac7840aab8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.5 MB (106547875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c136798ef3a3c3f24c1d1101befcf17b621cb8dbdb6071c483f3c40b7b581abf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 23 Jun 2021 00:22:13 GMT
ADD file:a63c6cc73701d6cb7195338c446b9e92ef6b7a0f9321f6cc1bf8738e3da57c66 in / 
# Wed, 23 Jun 2021 00:22:14 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 14:11:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 14:11:34 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 23 Jun 2021 14:11:34 GMT
ENV GOSU_VERSION=1.12
# Wed, 23 Jun 2021 14:11:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Jun 2021 14:11:51 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 23 Jun 2021 14:11:52 GMT
ENV LANG=en_US.utf8
# Wed, 23 Jun 2021 14:11:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 14:11:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 12 Jul 2021 22:23:14 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Mon, 12 Jul 2021 22:23:14 GMT
ENV PG_MAJOR=11
# Mon, 12 Jul 2021 22:23:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Mon, 12 Jul 2021 22:23:15 GMT
ENV PG_VERSION=11.12-1.pgdg90+1
# Mon, 12 Jul 2021 22:23:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Mon, 12 Jul 2021 22:23:56 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Mon, 12 Jul 2021 22:23:57 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 12 Jul 2021 22:23:57 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 12 Jul 2021 22:23:58 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 12 Jul 2021 22:23:58 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 12 Jul 2021 22:23:58 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Mon, 12 Jul 2021 22:23:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Jul 2021 22:23:59 GMT
STOPSIGNAL SIGINT
# Mon, 12 Jul 2021 22:23:59 GMT
EXPOSE 5432
# Mon, 12 Jul 2021 22:23:59 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:aed007321795cdc03a0ba9b238567ffa299459e9b0322a3d835a04d06afc2500`  
		Last Modified: Wed, 23 Jun 2021 00:28:29 GMT  
		Size: 22.5 MB (22528174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702c74af4354e452cb97a28a54832ac35ca997d6be881f91f6e3f123a471b642`  
		Last Modified: Wed, 23 Jun 2021 14:21:59 GMT  
		Size: 4.5 MB (4503261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef123e2ab09b3aa72b5b862f865f4732ff25525b5d05fd3d84f5bf480e63c7a3`  
		Last Modified: Wed, 23 Jun 2021 14:21:58 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84418d8530c106b495f17053fc19243acfe25a4e60eba743c08ab7917c4a1e5`  
		Last Modified: Wed, 23 Jun 2021 14:21:58 GMT  
		Size: 1.4 MB (1412246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b579800618becf4ae06f4d41000179ed592dee28a472e631d0da72e8c16bd848`  
		Last Modified: Wed, 23 Jun 2021 14:21:58 GMT  
		Size: 6.2 MB (6185452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6562ab9a134a4a0bbef0579a3c9302c45b605bab6782a333218807901fec5907`  
		Last Modified: Wed, 23 Jun 2021 14:21:55 GMT  
		Size: 385.0 KB (385038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9daa412a3b735592274e3e73e87f5a5b03fce5a267aed2d4d1a533e2984954`  
		Last Modified: Wed, 23 Jun 2021 14:21:55 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef585939c14054d75eae30f8d53510cc8d1c5059143cb98a5f13fad82164405e`  
		Last Modified: Mon, 12 Jul 2021 22:33:56 GMT  
		Size: 5.3 KB (5346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441afbb7b4bbed24296ef7a33b470abedc4bc8e76dd19a48da26cbb7057871f0`  
		Last Modified: Mon, 12 Jul 2021 22:34:04 GMT  
		Size: 71.5 MB (71513330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7aa402b2495a8774f290ca6a3c068fd83d01e2fe40db728fb24d97a3f4272c7`  
		Last Modified: Mon, 12 Jul 2021 22:33:54 GMT  
		Size: 8.3 KB (8326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3890ec9ba5d6b1a1eb8984d36561b82cb61469b5165c90f763a39d9a7b6a508a`  
		Last Modified: Mon, 12 Jul 2021 22:33:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a4fce211dfc53a7fc40ccf56bf83b3e87413848dde5ea5dd3dbf8b98b25a681`  
		Last Modified: Mon, 12 Jul 2021 22:33:54 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380c4b145ef63117de7cb5a6e4f66a614fde77e9f325d21d762497f445d72fe0`  
		Last Modified: Mon, 12 Jul 2021 22:33:54 GMT  
		Size: 4.4 KB (4411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-stretch` - linux; arm variant v5

```console
$ docker pull postgres@sha256:358a44fe6cf34bce50ef86a0dce4d4dfbaac3f28c023010d30ca0c7abc28add7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70635362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:742b9c86526589af9314a9f3a75e44d4857c89ca247a6cecfe7b718a7c7f0942`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 22 Jun 2021 23:53:17 GMT
ADD file:7ee5405955512bd1994a73279a3c014c01a8bf7144a11285a5277b3ad475670c in / 
# Tue, 22 Jun 2021 23:53:18 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 10:42:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 10:42:55 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 23 Jun 2021 10:42:55 GMT
ENV GOSU_VERSION=1.12
# Wed, 23 Jun 2021 10:43:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Jun 2021 10:43:47 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 23 Jun 2021 10:43:47 GMT
ENV LANG=en_US.utf8
# Wed, 23 Jun 2021 10:43:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 10:44:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Jun 2021 10:44:05 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Wed, 23 Jun 2021 10:44:05 GMT
ENV PG_MAJOR=11
# Wed, 23 Jun 2021 10:44:05 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Wed, 23 Jun 2021 10:44:06 GMT
ENV PG_VERSION=11.12-1.pgdg90+1
# Wed, 23 Jun 2021 11:10:10 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 23 Jun 2021 11:10:12 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 23 Jun 2021 11:10:13 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Jun 2021 11:10:14 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Jun 2021 11:10:15 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Jun 2021 11:10:16 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Jun 2021 11:10:16 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Wed, 23 Jun 2021 11:10:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 11:10:17 GMT
STOPSIGNAL SIGINT
# Wed, 23 Jun 2021 11:10:17 GMT
EXPOSE 5432
# Wed, 23 Jun 2021 11:10:18 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:9a9398bce1f19f52bcaa095c4f81de7eb887aab902d40b5307f32642fc13e129`  
		Last Modified: Wed, 23 Jun 2021 00:07:04 GMT  
		Size: 21.2 MB (21204003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a6074d73924bc4d6a842660f2ef9c9979b3336cbc8c17b913531026452fc38`  
		Last Modified: Wed, 23 Jun 2021 12:57:30 GMT  
		Size: 4.2 MB (4238933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf7cf30d5f9e4fdd6bf6580efab094b783204a2d13d8d43366ec09f4b523783`  
		Last Modified: Wed, 23 Jun 2021 12:57:27 GMT  
		Size: 1.8 KB (1801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88caaf682fb34956ee8bac83dfcd0f1e5a2250aa5fe0ae7afcf5e896e4a70d71`  
		Last Modified: Wed, 23 Jun 2021 12:57:28 GMT  
		Size: 1.4 MB (1371507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff520021d9f766366f412350218f9e0870ccea30eed7f897059b744059dff3a`  
		Last Modified: Wed, 23 Jun 2021 12:57:29 GMT  
		Size: 6.2 MB (6185836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03951f4af81e876dc9f79f01be0d652eafa9da077d881c3657ccf7fbe03e57c0`  
		Last Modified: Wed, 23 Jun 2021 12:57:26 GMT  
		Size: 385.1 KB (385101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5288ba522879781ca7a31290e55ce8258b545fa8bd89c846e44258156c9d023`  
		Last Modified: Wed, 23 Jun 2021 12:57:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0b0dd43a1772d2d87a5b895abe6f8e56dd6a05368d679fc0378cbac9bbbc94`  
		Last Modified: Wed, 23 Jun 2021 12:57:25 GMT  
		Size: 5.3 KB (5342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8abe482a0814d8db21b224e2683ba60f0ccda33d4470df832747b22aa18b43`  
		Last Modified: Wed, 23 Jun 2021 12:57:41 GMT  
		Size: 37.2 MB (37229621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39f212ede081b6f4f614fa1003f265c3bd2bc72790b1aefc0ca9612b6f1ecd1`  
		Last Modified: Wed, 23 Jun 2021 12:57:23 GMT  
		Size: 8.3 KB (8327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e942f1fef9a0627abb86f671e59826bff0d0848b4585f98c4a3d9e3b23762e80`  
		Last Modified: Wed, 23 Jun 2021 12:57:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc20fd2d1cfc81a994cb8c31a8b1b9dec911424ca0a89f59e67752c3ee1e168e`  
		Last Modified: Wed, 23 Jun 2021 12:57:23 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e1f62794fbe4c012ddb31b9eed75ce66a6d6f604482f6c5b121a90abf34502`  
		Last Modified: Wed, 23 Jun 2021 12:57:23 GMT  
		Size: 4.4 KB (4413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-stretch` - linux; arm variant v7

```console
$ docker pull postgres@sha256:cbea570628610aa05a3a8047418e336588be77649bc878ab268f02ebcf2e7633
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.3 MB (67299470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:781b531e711df6006d016d5dd677c677de42d5fd04d2367481f1ea5cf0832215`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 23 Jun 2021 00:23:36 GMT
ADD file:ffc5b643ebc5e4f3704b189af88d436975d60fe871dda953a3baa7bddc561512 in / 
# Wed, 23 Jun 2021 00:23:37 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 20:41:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 20:41:40 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 23 Jun 2021 20:41:40 GMT
ENV GOSU_VERSION=1.12
# Wed, 23 Jun 2021 20:42:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Jun 2021 20:42:25 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 23 Jun 2021 20:42:25 GMT
ENV LANG=en_US.utf8
# Wed, 23 Jun 2021 20:42:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 20:42:35 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 23 Jun 2021 20:42:40 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Wed, 23 Jun 2021 20:42:41 GMT
ENV PG_MAJOR=11
# Wed, 23 Jun 2021 20:42:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Wed, 23 Jun 2021 20:42:41 GMT
ENV PG_VERSION=11.12-1.pgdg90+1
# Wed, 23 Jun 2021 21:05:32 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 23 Jun 2021 21:05:34 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 23 Jun 2021 21:05:36 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 23 Jun 2021 21:05:36 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 23 Jun 2021 21:05:38 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 23 Jun 2021 21:05:39 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 23 Jun 2021 21:05:39 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Wed, 23 Jun 2021 21:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 21:05:40 GMT
STOPSIGNAL SIGINT
# Wed, 23 Jun 2021 21:05:41 GMT
EXPOSE 5432
# Wed, 23 Jun 2021 21:05:41 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:e53ed7a03b01895e35731de5c93cd7a3e826dc1ea9e08b7f35824394302d5c8c`  
		Last Modified: Wed, 23 Jun 2021 00:36:49 GMT  
		Size: 19.3 MB (19316486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:859343aaf0cf062fc2c3917986520c99ecb18adcea4767ded053a08d2f61907f`  
		Last Modified: Wed, 23 Jun 2021 22:52:31 GMT  
		Size: 3.9 MB (3875079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3841061d30a4d9c5e960d3f142f8766ead01f591a252a8278bdd8787757c65f5`  
		Last Modified: Wed, 23 Jun 2021 22:52:28 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46fdde00e79a9ebe490939e8ae3efb9e234413b5b3603818561144c34c222acc`  
		Last Modified: Wed, 23 Jun 2021 22:52:29 GMT  
		Size: 1.4 MB (1363930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6960a7adfe74e851d953c72e0961fe51c3074e0ce18353a19dc71611a50bf98c`  
		Last Modified: Wed, 23 Jun 2021 22:52:31 GMT  
		Size: 6.2 MB (6185701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4caa1d78bceb0bc79de0f44a33a69c5c395dc7d462c7d56c7edd5b04e0139f`  
		Last Modified: Wed, 23 Jun 2021 22:52:26 GMT  
		Size: 379.2 KB (379183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c3b7ea16bc4701221d527c5bd129a34a31b3038a3b34969728ddc959611264`  
		Last Modified: Wed, 23 Jun 2021 22:52:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e55da4113f1f0918e6750d47c24c2be4904f053bede51d8f463622511e61f01`  
		Last Modified: Wed, 23 Jun 2021 22:52:26 GMT  
		Size: 4.8 KB (4795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989cd9d73abe45294bba0246210c9e01d34d0b3a446d2ec396f81a6730559d24`  
		Last Modified: Wed, 23 Jun 2021 22:52:49 GMT  
		Size: 36.2 MB (36159274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35161e963b8178acc451704ab3532911a4509219a2fcbbc173b778a1ca6de125`  
		Last Modified: Wed, 23 Jun 2021 22:52:24 GMT  
		Size: 8.3 KB (8326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e5bac7b6a628b1da604ebd2e0a2f7578bbb75a94cedc3aad2977a0e564da51`  
		Last Modified: Wed, 23 Jun 2021 22:52:24 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d0ca1307c27dfaf4e073fc1e72301bc426a9922008488f31f40e09a36aff5c`  
		Last Modified: Wed, 23 Jun 2021 22:52:24 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a3dfa38d085520cf09ee40d6121a99ba571ce104ee2eb5df40fd27a8136131`  
		Last Modified: Wed, 23 Jun 2021 22:52:24 GMT  
		Size: 4.4 KB (4415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-stretch` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:c64cc4f745dea4d72e587bdeeffc41fb4fd5ba4d020075f4ca85e02c0737a929
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.9 MB (69902649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec5d6382ba4c6bf7406800369c6b162ba648f4dedeb2ed2bf79c63023620b57e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 22 Jun 2021 23:51:10 GMT
ADD file:0124cb1e13f08e2df3878b9faa69d962ba2b9c7d5afdf72fff8b1e22201ce065 in / 
# Tue, 22 Jun 2021 23:51:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 08:07:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 08:07:35 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 23 Jun 2021 08:07:35 GMT
ENV GOSU_VERSION=1.12
# Wed, 23 Jun 2021 08:07:47 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Jun 2021 08:07:53 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 23 Jun 2021 08:07:53 GMT
ENV LANG=en_US.utf8
# Wed, 23 Jun 2021 08:07:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 08:07:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 12 Jul 2021 22:44:09 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Mon, 12 Jul 2021 22:44:09 GMT
ENV PG_MAJOR=11
# Mon, 12 Jul 2021 22:44:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Mon, 12 Jul 2021 22:44:09 GMT
ENV PG_VERSION=11.12-1.pgdg90+1
# Mon, 12 Jul 2021 22:53:25 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Mon, 12 Jul 2021 22:53:26 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Mon, 12 Jul 2021 22:53:27 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 12 Jul 2021 22:53:27 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 12 Jul 2021 22:53:28 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 12 Jul 2021 22:53:28 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 12 Jul 2021 22:53:28 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Mon, 12 Jul 2021 22:53:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Jul 2021 22:53:29 GMT
STOPSIGNAL SIGINT
# Mon, 12 Jul 2021 22:53:29 GMT
EXPOSE 5432
# Mon, 12 Jul 2021 22:53:29 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:3ac59e1f301a0b03211a0a7f10a84730165b09211c4a8ef9636673101bf1220f`  
		Last Modified: Tue, 22 Jun 2021 23:58:21 GMT  
		Size: 20.4 MB (20389316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f8547797f662b08b509ae4eb02e73d048dd0c927231212bffe8735c0c1e460`  
		Last Modified: Wed, 23 Jun 2021 08:45:25 GMT  
		Size: 4.1 MB (4078553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b48c9e359cf172e3a99287aef455c5569379839f36bb10bf7ce657cb757181`  
		Last Modified: Wed, 23 Jun 2021 08:45:24 GMT  
		Size: 1.8 KB (1810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a56f7f512a64c85b46725b2165669b3c005979f7341338db312415433aa854`  
		Last Modified: Wed, 23 Jun 2021 08:45:24 GMT  
		Size: 1.3 MB (1347016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0cae3f38facb088c2f3b69f7701ac026e914fcc7c6d3b3a3032ff31a02280d8`  
		Last Modified: Wed, 23 Jun 2021 08:45:25 GMT  
		Size: 6.2 MB (6185484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ff3e1a276f71211cba39e7a5fa1707a6b52e241bd096f2c00b4c64ff39563b3`  
		Last Modified: Wed, 23 Jun 2021 08:45:21 GMT  
		Size: 377.9 KB (377860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686e132b118df44e9b93bb835b8b705435cbf96fc8ce86bd5405d73bd74efabc`  
		Last Modified: Wed, 23 Jun 2021 08:45:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccf8c02869383e9ba2ab017dfbc52e7b202ceb7f7f50345e2bd5e6344e564ac`  
		Last Modified: Mon, 12 Jul 2021 23:23:06 GMT  
		Size: 5.3 KB (5342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f590c58535d404963a31edd0579b7548aede4773e6eb86567529709a1248caa0`  
		Last Modified: Mon, 12 Jul 2021 23:23:11 GMT  
		Size: 37.5 MB (37504052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1371cba680b00f05b5c8f7e456e0f72278bedeeac365a5faaec45393780d8e7`  
		Last Modified: Mon, 12 Jul 2021 23:23:04 GMT  
		Size: 8.3 KB (8326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2bfcce5ebf3645829acad727989863f99ad4ccfd3aeb47f0ed5a45e6db3ad59`  
		Last Modified: Mon, 12 Jul 2021 23:23:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7598984f6caaef75d38cfbc3c953dcda70126cbe6c0ac3cf669e3855946455`  
		Last Modified: Mon, 12 Jul 2021 23:23:04 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5dfaae7c174d2db81ba31a3c60b0e7266504812525a0446f9759e0b1fe6392`  
		Last Modified: Mon, 12 Jul 2021 23:23:04 GMT  
		Size: 4.4 KB (4412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-stretch` - linux; 386

```console
$ docker pull postgres@sha256:3a105c46d59bf8403d6e90ef6325f40361dff3aed046aa04d8b8ab1583f3da60
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (109994186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:801a836d75ee8f6d77fe0f65a2e972d4f7821a9cbeb89a7a74a5161a30f1a7aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 22 Jun 2021 23:41:26 GMT
ADD file:f8625bcae5378e2f791822c618e8c826ad9340effb236866d52e61ffc603feae in / 
# Tue, 22 Jun 2021 23:41:26 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 12:49:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 12:49:42 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 23 Jun 2021 12:49:42 GMT
ENV GOSU_VERSION=1.12
# Wed, 23 Jun 2021 12:49:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Jun 2021 12:50:04 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 23 Jun 2021 12:50:04 GMT
ENV LANG=en_US.utf8
# Wed, 23 Jun 2021 12:50:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 12:50:09 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Mon, 12 Jul 2021 22:42:51 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Mon, 12 Jul 2021 22:42:51 GMT
ENV PG_MAJOR=11
# Mon, 12 Jul 2021 22:42:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Mon, 12 Jul 2021 22:42:52 GMT
ENV PG_VERSION=11.12-1.pgdg90+1
# Mon, 12 Jul 2021 22:43:15 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Mon, 12 Jul 2021 22:43:17 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Mon, 12 Jul 2021 22:43:18 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Mon, 12 Jul 2021 22:43:18 GMT
ENV PGDATA=/var/lib/postgresql/data
# Mon, 12 Jul 2021 22:43:19 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Mon, 12 Jul 2021 22:43:19 GMT
VOLUME [/var/lib/postgresql/data]
# Mon, 12 Jul 2021 22:43:19 GMT
COPY file:e9c9c5e19c7b014c81f4ef8bcc5c1f247c4d9b165d34d35e9a28ca5adb5e0ab3 in /usr/local/bin/ 
# Mon, 12 Jul 2021 22:43:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Jul 2021 22:43:19 GMT
STOPSIGNAL SIGINT
# Mon, 12 Jul 2021 22:43:20 GMT
EXPOSE 5432
# Mon, 12 Jul 2021 22:43:20 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:18847bdd326b9eee5c5cd45fa0b632d342e39ffbf31b13627bbbe8824c90466b`  
		Last Modified: Tue, 22 Jun 2021 23:49:53 GMT  
		Size: 23.2 MB (23157219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8eb346cb708bc94579a3d536fa1086e8ac1e8dd270d3d8ce0be0a2d3ca1f478`  
		Last Modified: Wed, 23 Jun 2021 13:04:16 GMT  
		Size: 4.8 MB (4811146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c756d8fd7ad198b4477af4bf63ee400c5ee5d096281d8010c71cec4af755f6ed`  
		Last Modified: Wed, 23 Jun 2021 13:04:14 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f230c4a0936cab5e7391ffd581074562b49fd56ef44c6d6059e61e996505b6`  
		Last Modified: Wed, 23 Jun 2021 13:04:15 GMT  
		Size: 1.4 MB (1382541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc0f82a05d48135e71d69806f943025914e9709231c33486a8e7ecbacfce741`  
		Last Modified: Wed, 23 Jun 2021 13:04:14 GMT  
		Size: 6.2 MB (6185597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1119047a071ed37ffc81aab5b96c2e0d4d17a149a390a1aea34202f3e1cc4f`  
		Last Modified: Wed, 23 Jun 2021 13:04:12 GMT  
		Size: 393.4 KB (393358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e408cd574fbfdd94822129a83d1818928e7a30bd0823654212a81a1adc0fadf3`  
		Last Modified: Wed, 23 Jun 2021 13:04:12 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615568d4ac44650682b08cd381be299cfcc63346936523343e78b70e27666962`  
		Last Modified: Mon, 12 Jul 2021 22:56:04 GMT  
		Size: 5.3 KB (5345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3550f99d82868603dbcdfdf61b1a6d7ad302a5c89eb3f8f4892dd56159312d6b`  
		Last Modified: Mon, 12 Jul 2021 22:56:15 GMT  
		Size: 74.0 MB (74043956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635d84181a7f28e992ff77cc0cbd0877eb843f048a4af514106e9b4688da3832`  
		Last Modified: Mon, 12 Jul 2021 22:56:02 GMT  
		Size: 8.3 KB (8326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9a507e9ea8a75019bffcfd03701c201a3ab758d50bb5253df8317301bd5017`  
		Last Modified: Mon, 12 Jul 2021 22:56:01 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f4e2934a728a6397197dfb64b7cffa800be6cfe77151f384fe9a68340c44f4`  
		Last Modified: Mon, 12 Jul 2021 22:56:02 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e704b8a2751bc608ee96addccb7be0513593f010c92c633e7ec26194cd979ccf`  
		Last Modified: Mon, 12 Jul 2021 22:56:02 GMT  
		Size: 4.4 KB (4410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
