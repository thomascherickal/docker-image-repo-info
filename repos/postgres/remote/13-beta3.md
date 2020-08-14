## `postgres:13-beta3`

```console
$ docker pull postgres@sha256:2c94dcf7b43527d7daaafdaee8cf53bebd7ee986f97aaa5dcfff08912468b1c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `postgres:13-beta3` - linux; amd64

```console
$ docker pull postgres@sha256:4b05d2fd12fe09848025a39b9b3adf137045e884d82b9ce4ef2c71489a4669b0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.3 MB (115299327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2e0ea262c7cc00b4ef42e5e3f974ed9c56861f48cd1cb2809e38807f4a8ad55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 04 Aug 2020 15:42:51 GMT
ADD file:3af3091e7d2bb40bc1e6550eb5ea290badc6bbf3339105626f245a963cc11450 in / 
# Tue, 04 Aug 2020 15:42:51 GMT
CMD ["bash"]
# Wed, 05 Aug 2020 06:21:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Aug 2020 06:21:35 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 05 Aug 2020 06:21:35 GMT
ENV GOSU_VERSION=1.12
# Wed, 05 Aug 2020 06:21:44 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 05 Aug 2020 06:21:51 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 05 Aug 2020 06:21:51 GMT
ENV LANG=en_US.utf8
# Wed, 05 Aug 2020 06:21:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Aug 2020 06:21:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 05 Aug 2020 06:21:58 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Wed, 05 Aug 2020 06:21:58 GMT
ENV PG_MAJOR=13
# Fri, 14 Aug 2020 17:20:27 GMT
ENV PG_VERSION=13~beta3-1.pgdg100+1
# Fri, 14 Aug 2020 17:20:47 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Fri, 14 Aug 2020 17:20:48 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 14 Aug 2020 17:20:49 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 Aug 2020 17:20:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Fri, 14 Aug 2020 17:20:49 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 Aug 2020 17:20:50 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 Aug 2020 17:20:50 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 Aug 2020 17:20:51 GMT
COPY file:bf774aaf2659f8308202ce0332f960783bfecabcf593dd9b2d25e19fe5c4b946 in /usr/local/bin/ 
# Fri, 14 Aug 2020 17:20:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 14 Aug 2020 17:20:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 Aug 2020 17:20:52 GMT
EXPOSE 5432
# Fri, 14 Aug 2020 17:20:52 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:bf59529304463f62efa7179fa1a32718a611528cc4ce9f30c0d1bbc6724ec3fb`  
		Last Modified: Tue, 04 Aug 2020 15:49:09 GMT  
		Size: 27.1 MB (27092121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9577476abb009895d51d2c1b4d09a1fb4e1cc8d6225577becfd2e7d1f08ff069`  
		Last Modified: Wed, 05 Aug 2020 06:25:58 GMT  
		Size: 4.2 MB (4178087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd105512d5c231f824d94ee3a2eb3514978a2e05a91a4e2dd44a149c2360dd2`  
		Last Modified: Wed, 05 Aug 2020 06:25:57 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1cd21c26e81085f46a3fbfbbd54874414ecc7e47419c4ed8cd38b6673574cf1`  
		Last Modified: Wed, 05 Aug 2020 06:25:57 GMT  
		Size: 1.4 MB (1419217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a7c86cf8fc3cf0e051b8fd51cba57aa5fa74c73ad8dd5f70fa68ec97641e0b`  
		Last Modified: Wed, 05 Aug 2020 06:25:58 GMT  
		Size: 8.0 MB (7964543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274e7b0c38d57518d48e3c69e20760154794f81242f7dc627e2d9bafe9f04570`  
		Last Modified: Wed, 05 Aug 2020 06:25:56 GMT  
		Size: 391.0 KB (391042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e831b350d37dd5123f3112bb1a7030bbbdc38faff24759ad442666d268f8c9c`  
		Last Modified: Wed, 05 Aug 2020 06:25:55 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38fa0d49653474db61ab3cd7ec7db8753c2f545fe4f85c14ff0ded85c648b2f8`  
		Last Modified: Wed, 05 Aug 2020 06:25:55 GMT  
		Size: 3.0 KB (3050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a58d279d4a1307fae954aafd0ac37aef06df7389c57ac6817edcfc9d8977e39`  
		Last Modified: Fri, 14 Aug 2020 17:55:42 GMT  
		Size: 74.2 MB (74235434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:831b15d31edb7fb62fa6244cdaca23b033f62e30d42bbba39c2c295a03ef5297`  
		Last Modified: Fri, 14 Aug 2020 17:55:22 GMT  
		Size: 9.3 KB (9268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c13552c01ed319d7b795c32c18a83a546653badb3e3a5df66306c2a22061e1b`  
		Last Modified: Fri, 14 Aug 2020 17:55:22 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd5fa174bfcc97ac6c2767dc0a42247a0c2cb19aba65301b9b95b6e9be72a62`  
		Last Modified: Fri, 14 Aug 2020 17:55:22 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce6bb121910624ef10ce33313e1704e1f13009cdfa048c8ac92805139e3cad8`  
		Last Modified: Fri, 14 Aug 2020 17:55:22 GMT  
		Size: 4.3 KB (4259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e708ef81668d86319bf33dca74e37c08cc3fc88c265bb1a700ad45bd223686c9`  
		Last Modified: Fri, 14 Aug 2020 17:55:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-beta3` - linux; 386

```console
$ docker pull postgres@sha256:7329da935d1454cfe6876b840affa866db2bde15e410d6b1b5a88be434e2b75f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.0 MB (115970745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35b492727b0b236b09865f455a203ec982ec16a2f5ac1d3cb89aec9e85b5b2de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:35 GMT
ADD file:cc791c21e6022a12dd1445a35f4cca9392ad8edfe34ea5852f3e87862c943628 in / 
# Tue, 04 Aug 2020 03:37:35 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 15:05:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 15:05:43 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 04 Aug 2020 15:05:43 GMT
ENV GOSU_VERSION=1.12
# Tue, 04 Aug 2020 15:05:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Aug 2020 15:06:02 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 04 Aug 2020 15:06:02 GMT
ENV LANG=en_US.utf8
# Tue, 04 Aug 2020 15:06:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 15:06:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Aug 2020 15:06:09 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 04 Aug 2020 15:06:09 GMT
ENV PG_MAJOR=13
# Fri, 14 Aug 2020 17:38:39 GMT
ENV PG_VERSION=13~beta3-1.pgdg100+1
# Fri, 14 Aug 2020 17:39:03 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Fri, 14 Aug 2020 17:39:04 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 14 Aug 2020 17:39:05 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 Aug 2020 17:39:05 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Fri, 14 Aug 2020 17:39:05 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 Aug 2020 17:39:06 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 Aug 2020 17:39:06 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 Aug 2020 17:39:07 GMT
COPY file:bf774aaf2659f8308202ce0332f960783bfecabcf593dd9b2d25e19fe5c4b946 in /usr/local/bin/ 
# Fri, 14 Aug 2020 17:39:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 14 Aug 2020 17:39:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 Aug 2020 17:39:08 GMT
EXPOSE 5432
# Fri, 14 Aug 2020 17:39:08 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:23ad22c16ab9d635a179d5d341096c34912941507b0c77ac97083b9795d8516f`  
		Last Modified: Tue, 04 Aug 2020 03:42:33 GMT  
		Size: 27.8 MB (27750435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ea487ca63570cafb329ea9e344f5a5b99ea59fbd6c57e4141bb5275bfafe76`  
		Last Modified: Tue, 04 Aug 2020 15:10:48 GMT  
		Size: 4.5 MB (4542268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0154231add66b7111be1d1107702b72243ec1f4cc21ec7928ca1afe9960de0fc`  
		Last Modified: Tue, 04 Aug 2020 15:10:46 GMT  
		Size: 1.8 KB (1764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4fbfa021e0fe03ebfe9552701093878bb7f90520d681dd9515adc362835c74`  
		Last Modified: Tue, 04 Aug 2020 15:10:47 GMT  
		Size: 1.4 MB (1389500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc5482d80e98b8869017e91e8cd32c3ca9e15be344cc22aa5bec30703311f70`  
		Last Modified: Tue, 04 Aug 2020 15:10:50 GMT  
		Size: 8.0 MB (7964435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53a5ef67b75391c1cebc5c18f23ebe80cb45a8c58f1061169e8e59824aa505d`  
		Last Modified: Tue, 04 Aug 2020 15:10:45 GMT  
		Size: 398.2 KB (398234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2127fe0de98007eed9b7dc66e8eb44d5912c24bec73c27760eb05cd19adf2502`  
		Last Modified: Tue, 04 Aug 2020 15:10:45 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f4cee315191742201e24bfab8b7d55d5b84811f7cc9dd55104a8af8912b2f69`  
		Last Modified: Tue, 04 Aug 2020 15:10:45 GMT  
		Size: 3.1 KB (3051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59c1675bef4463291c273ad9674b0a5fa1bf798d63c34bd9e2bf9d650b8b596`  
		Last Modified: Fri, 14 Aug 2020 18:21:31 GMT  
		Size: 73.9 MB (73907001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2f9541f747d802042ea130e7a05667329746578517fdd7865c8df3f3bbf497`  
		Last Modified: Fri, 14 Aug 2020 18:21:13 GMT  
		Size: 9.3 KB (9263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87464cb1fd11c4bd67280168095a2b15dded7903710b8ff81466f411833bb218`  
		Last Modified: Fri, 14 Aug 2020 18:21:13 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7fb92daad8c665556e04984b335898df775b5a39b32566225f99b1ad48e691f`  
		Last Modified: Fri, 14 Aug 2020 18:21:13 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7f0ebd6773a5c74d324f348b4378e8fbb6b62d889257f841a7cb7d2736c4a9`  
		Last Modified: Fri, 14 Aug 2020 18:21:13 GMT  
		Size: 4.3 KB (4259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afd982b58a2f2db4c5fa57f53cd0017ce14dbb517662738b5040bbe0528e5739`  
		Last Modified: Fri, 14 Aug 2020 18:21:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-beta3` - linux; mips64le

```console
$ docker pull postgres@sha256:c42fd18de1a5bbc3a7609a8f37014fe73ae89701184a049367874063a105fcf8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.9 MB (110858349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aedcead3b6ee0040502ca99b45cb9ef8c14e5dd43a231374a171cdfc9c620143`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 04 Aug 2020 06:42:23 GMT
ADD file:4164c71b841ba2c1f213c9fdc073ec3d4c7d79dadfcd9d771768750a3085d616 in / 
# Tue, 04 Aug 2020 06:42:24 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 15:54:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 15:54:22 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 04 Aug 2020 15:54:22 GMT
ENV GOSU_VERSION=1.12
# Tue, 04 Aug 2020 15:54:44 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Aug 2020 15:55:08 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 04 Aug 2020 15:55:08 GMT
ENV LANG=en_US.utf8
# Tue, 04 Aug 2020 15:55:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 15:55:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Aug 2020 15:55:25 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 04 Aug 2020 15:55:25 GMT
ENV PG_MAJOR=13
# Fri, 14 Aug 2020 17:07:28 GMT
ENV PG_VERSION=13~beta3-1.pgdg100+1
# Fri, 14 Aug 2020 17:59:33 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Fri, 14 Aug 2020 17:59:35 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 14 Aug 2020 17:59:36 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 Aug 2020 17:59:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Fri, 14 Aug 2020 17:59:36 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 Aug 2020 17:59:38 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 Aug 2020 17:59:39 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 Aug 2020 17:59:39 GMT
COPY file:bf774aaf2659f8308202ce0332f960783bfecabcf593dd9b2d25e19fe5c4b946 in /usr/local/bin/ 
# Fri, 14 Aug 2020 17:59:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 14 Aug 2020 17:59:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 Aug 2020 17:59:42 GMT
EXPOSE 5432
# Fri, 14 Aug 2020 17:59:42 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:1333f76e75c0136aa2eb56b14271ef57d1f975f40fe2a56536d99b7c86c3aa29`  
		Last Modified: Tue, 04 Aug 2020 06:48:41 GMT  
		Size: 25.8 MB (25762724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9485ae4cb9c692241b4d24159c9a6b6f8a60feaf5a546fe3902f0a38f6717d1d`  
		Last Modified: Tue, 04 Aug 2020 17:38:32 GMT  
		Size: 4.2 MB (4182342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9507bb79051508f20607e04eeffbf239ed1a88c7a26b6fba389ae6d5926056e`  
		Last Modified: Tue, 04 Aug 2020 17:38:27 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7585abae33e6d55642da8b45d055f24e519219eccb4dd214cabd5d4ed4b692b2`  
		Last Modified: Tue, 04 Aug 2020 17:38:29 GMT  
		Size: 1.3 MB (1307249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c418d58584984f6ba6f6cebd2e1a0a8ec1867d3005140740a75beea7964263f6`  
		Last Modified: Tue, 04 Aug 2020 17:38:34 GMT  
		Size: 8.0 MB (7964577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01d23344be3ef84bad8d4c7bd25c0a922c47563dcd84b352238e97b34a42ab8`  
		Last Modified: Tue, 04 Aug 2020 17:38:25 GMT  
		Size: 389.2 KB (389239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dff147213ec90c0790c6d808587b3f3d1f044c7a687cb88e1a00def1593ed9a`  
		Last Modified: Tue, 04 Aug 2020 17:38:24 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3136b66ab1e267cfba7830052a44c69b7fcb1d2306107749c43fd75e485d785`  
		Last Modified: Tue, 04 Aug 2020 17:38:24 GMT  
		Size: 3.1 KB (3057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12362dcb0782ad40db960f21489c86b16def01102bfdfbe414b5ef173f72e167`  
		Last Modified: Fri, 14 Aug 2020 18:50:52 GMT  
		Size: 71.2 MB (71233324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d41348fc55ab5ae6407f95340074b6d53aac0ca951f77d2f24db9a05746477a`  
		Last Modified: Fri, 14 Aug 2020 18:50:01 GMT  
		Size: 9.3 KB (9273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32fed259c35dcd28ff5e8213af299c8430cc231930ff02c0fc397844ccf6e57d`  
		Last Modified: Fri, 14 Aug 2020 18:50:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ac11a2001e9e1da3e8f0b2d59d10ab3f2258c0fd3736ba3911cdbf1284d733b`  
		Last Modified: Fri, 14 Aug 2020 18:50:01 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5f856b806dc4f0176aff333032c647818a3a8c9132dcf906649df988bc42be`  
		Last Modified: Fri, 14 Aug 2020 18:50:01 GMT  
		Size: 4.3 KB (4261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1f4b6b035935cd5134af9221ecbcea05082ac236f27dece77f071aeed58805`  
		Last Modified: Fri, 14 Aug 2020 18:50:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-beta3` - linux; ppc64le

```console
$ docker pull postgres@sha256:b668ee4781a21d4ce24cecc3977c92e336be4a3fe54054f498663df5659d8638
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.6 MB (122582306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b88527bdd06f0a2d8f4c4443e6611eb2318ce05af3546e929dab73610d2ce2b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 04 Aug 2020 04:45:34 GMT
ADD file:3bab6d2b62fe6a548ee28480d9eebf3251e942c4bb66362b87396b73af7aa586 in / 
# Tue, 04 Aug 2020 04:45:40 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 15:39:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 15:40:28 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 04 Aug 2020 15:40:38 GMT
ENV GOSU_VERSION=1.12
# Tue, 04 Aug 2020 15:41:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Aug 2020 15:42:08 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 04 Aug 2020 15:42:13 GMT
ENV LANG=en_US.utf8
# Tue, 04 Aug 2020 15:42:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 15:42:49 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Aug 2020 15:43:02 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 04 Aug 2020 15:43:06 GMT
ENV PG_MAJOR=13
# Fri, 14 Aug 2020 17:17:34 GMT
ENV PG_VERSION=13~beta3-1.pgdg100+1
# Fri, 14 Aug 2020 17:20:55 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Fri, 14 Aug 2020 17:21:18 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 14 Aug 2020 17:21:36 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 Aug 2020 17:21:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Fri, 14 Aug 2020 17:21:48 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 Aug 2020 17:22:00 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 Aug 2020 17:22:05 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 Aug 2020 17:22:07 GMT
COPY file:bf774aaf2659f8308202ce0332f960783bfecabcf593dd9b2d25e19fe5c4b946 in /usr/local/bin/ 
# Fri, 14 Aug 2020 17:22:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 14 Aug 2020 17:22:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 Aug 2020 17:22:40 GMT
EXPOSE 5432
# Fri, 14 Aug 2020 17:22:44 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:0827434caf9c0b71f95b3bcbe29d60f4f887199db59b3994d9315c478def41c3`  
		Last Modified: Tue, 04 Aug 2020 04:53:24 GMT  
		Size: 30.5 MB (30517844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c8f6e5ffd40357e5073edd4deef4909425501c6b2f1ad7ccb030d63efcaad4`  
		Last Modified: Tue, 04 Aug 2020 15:51:17 GMT  
		Size: 5.0 MB (4967262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb1a0f3f77d552a566cc2ac0b9dd44c1de83a5ed226dd3c17b948369ff3de16`  
		Last Modified: Tue, 04 Aug 2020 15:51:15 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95966569a37ea8a9bdbb58cebb98ef4ed8b838a138bc3a78f826bfaab720ea1a`  
		Last Modified: Tue, 04 Aug 2020 15:51:18 GMT  
		Size: 1.3 MB (1337985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18416276fcedb414eccc6cafe9637eb93c37eef560bcff2a7defd1d465753190`  
		Last Modified: Tue, 04 Aug 2020 15:51:12 GMT  
		Size: 8.0 MB (7965495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3112b926e74ac1fac07ed8c4060917bd13ed8f5c610512217c8d59655f2d93b0`  
		Last Modified: Tue, 04 Aug 2020 15:51:10 GMT  
		Size: 397.1 KB (397067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f67e95ec50b45d3acccfe0fc989844956feff07998fc43317ba19d3de413f7`  
		Last Modified: Tue, 04 Aug 2020 15:51:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9dfd211babd19dce43e64c71a5e41e3900e0efb7af7bd99a4aa17881ad96b9`  
		Last Modified: Tue, 04 Aug 2020 15:51:10 GMT  
		Size: 3.1 KB (3060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7066060f1477d1758856441bd73e109497eb89aacd7cfd651d1abd9e6039548`  
		Last Modified: Fri, 14 Aug 2020 18:10:45 GMT  
		Size: 77.4 MB (77377628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac01510812c6e1dd77679758bd2052a758265a392cefd760941dbdc07d5da993`  
		Last Modified: Fri, 14 Aug 2020 18:10:24 GMT  
		Size: 9.3 KB (9276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f2932ab1112cd4c8ba84b7b4ce9ee46a4711d4d70825c724723f78206290d6`  
		Last Modified: Fri, 14 Aug 2020 18:10:23 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffd5a165aa29781a61edead2d0117556439d399893cb0e2184af486fd77d802`  
		Last Modified: Fri, 14 Aug 2020 18:10:23 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9240716328ef851f855cfeb1aeffd1e14d795651764dc7e184c48cf3910879e0`  
		Last Modified: Fri, 14 Aug 2020 18:10:23 GMT  
		Size: 4.3 KB (4262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ddfa8847a3bb22b2611824c581646bc3fb7735a85931910b968d9685c0eb315`  
		Last Modified: Fri, 14 Aug 2020 18:10:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-beta3` - linux; s390x

```console
$ docker pull postgres@sha256:9b5962f92ccec557d7ccd163da8d82558c5330c10a4ea7191cf64b7c1fe647bd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.6 MB (113605827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0754b16d418ceca6db92b2d1ab799d3307e26ab1338ec417188ca07759eaeda1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 04 Aug 2020 01:17:16 GMT
ADD file:2ffa27c57800f9370adbaecca870158ec38c3d25a58b8803e2447c5e9320c5bb in / 
# Tue, 04 Aug 2020 01:17:17 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 03:00:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 03:00:13 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 04 Aug 2020 03:00:13 GMT
ENV GOSU_VERSION=1.12
# Tue, 04 Aug 2020 03:00:20 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Aug 2020 03:00:25 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 04 Aug 2020 03:00:26 GMT
ENV LANG=en_US.utf8
# Tue, 04 Aug 2020 03:00:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 03:00:30 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Aug 2020 03:00:31 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 04 Aug 2020 03:00:31 GMT
ENV PG_MAJOR=13
# Fri, 14 Aug 2020 17:41:53 GMT
ENV PG_VERSION=13~beta3-1.pgdg100+1
# Fri, 14 Aug 2020 17:50:45 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ buster-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						case "$PG_MAJOR" in 				9.* | 10 ) ;; 				*) 					echo 'deb http://deb.debian.org/debian buster-backports main' >> /etc/apt/sources.list.d/pgdg.list; 					;; 			esac; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +
# Fri, 14 Aug 2020 17:50:49 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 14 Aug 2020 17:50:50 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 14 Aug 2020 17:50:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Fri, 14 Aug 2020 17:50:50 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 14 Aug 2020 17:50:51 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 14 Aug 2020 17:50:51 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 14 Aug 2020 17:50:51 GMT
COPY file:bf774aaf2659f8308202ce0332f960783bfecabcf593dd9b2d25e19fe5c4b946 in /usr/local/bin/ 
# Fri, 14 Aug 2020 17:50:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 14 Aug 2020 17:50:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 Aug 2020 17:50:52 GMT
EXPOSE 5432
# Fri, 14 Aug 2020 17:50:52 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:0c46adfa2de4a7b7eb1fe2f0cb928f9e15a4cc94b7b975f13392f397cbfb0f2c`  
		Last Modified: Tue, 04 Aug 2020 01:20:03 GMT  
		Size: 25.7 MB (25707641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb124f8f03c4667968c848dcca60d2aac298629753144f5b27e101e411324dff`  
		Last Modified: Tue, 04 Aug 2020 03:16:57 GMT  
		Size: 4.1 MB (4059808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8ce248da649f400762d7d4e1b696a8aea73fc7a1e9e15fcfe631edbfb9bc05`  
		Last Modified: Tue, 04 Aug 2020 03:16:55 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ee98c3423e3dd74f3ca70a321403c333466ab2565bb6381af785ee3a1e1681`  
		Last Modified: Tue, 04 Aug 2020 03:16:55 GMT  
		Size: 1.4 MB (1406013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a284cf2aa172702b274192c6bec18d3730658b5d062c2c17229176990f0dc57f`  
		Last Modified: Tue, 04 Aug 2020 03:16:56 GMT  
		Size: 8.0 MB (8019360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34a2733eb76f9823ffb8656c16c558be8b38edec2cd63d3de68fde74a40dd7a`  
		Last Modified: Tue, 04 Aug 2020 03:16:54 GMT  
		Size: 388.3 KB (388299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdcdb7e623f62be72213a378d6a612157b6821853984bcd6561f1600b50923bd`  
		Last Modified: Tue, 04 Aug 2020 03:16:53 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5714e5559acb56e54cc2c15c0d00b7549a488e65dc2c14a7b34a68bb76908943`  
		Last Modified: Tue, 04 Aug 2020 03:16:53 GMT  
		Size: 3.0 KB (3049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0171993366a0797f9fb6fdcfa914ec975a9033b25bf999a2ea89eefe89870bed`  
		Last Modified: Fri, 14 Aug 2020 18:20:04 GMT  
		Size: 74.0 MB (74005724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc94d66b1af30e589ad7997d7291902fb3c671d7d2e60f67e263a4048066a878`  
		Last Modified: Fri, 14 Aug 2020 18:19:52 GMT  
		Size: 9.3 KB (9268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810885c1bbfedfde4d8baab6aa9e050e523a7aa762e25e7221d741a828acfa8c`  
		Last Modified: Fri, 14 Aug 2020 18:19:52 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2502d2487ec85b24967873e835acb630f506d2ee4efa4bdc2a0ce711f0e40fc2`  
		Last Modified: Fri, 14 Aug 2020 18:19:52 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70266212858b53d1b5acdafa3d06d28ce92e63eedf8ea0317a1323de674c4da`  
		Last Modified: Fri, 14 Aug 2020 18:19:52 GMT  
		Size: 4.3 KB (4258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffaa28e81e847939391c0378ac29464c8700a2d82af03e45ef3fe3546b1d2b78`  
		Last Modified: Fri, 14 Aug 2020 18:19:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
