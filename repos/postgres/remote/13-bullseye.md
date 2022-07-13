## `postgres:13-bullseye`

```console
$ docker pull postgres@sha256:50b92ee0e1639d6bf65283c482b306158c3d16e70b77f8af0ddf228630f4acc9
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
$ docker pull postgres@sha256:46311c13081272a362ccb44d914e815a506cd77548adf306af50d7fdd81c19f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136570623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13e6da1782a5ed454bc78f36b679ce3a98106e83a03db0046b517300cb57c757`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 09:54:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 09:54:14 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 12 Jul 2022 09:54:14 GMT
ENV GOSU_VERSION=1.14
# Tue, 12 Jul 2022 09:54:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Jul 2022 09:54:29 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 12 Jul 2022 09:54:30 GMT
ENV LANG=en_US.utf8
# Tue, 12 Jul 2022 09:54:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 09:54:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 12 Jul 2022 09:54:35 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 12 Jul 2022 09:55:32 GMT
ENV PG_MAJOR=13
# Tue, 12 Jul 2022 09:55:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 12 Jul 2022 09:55:33 GMT
ENV PG_VERSION=13.7-1.pgdg110+1
# Tue, 12 Jul 2022 09:55:51 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 12 Jul 2022 09:55:53 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 12 Jul 2022 09:55:53 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 12 Jul 2022 09:55:53 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 12 Jul 2022 09:55:54 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 12 Jul 2022 09:55:54 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 12 Jul 2022 09:55:54 GMT
COPY file:925d466681c8349f58385c00a8caa567c76b695158aa04bf4ad2ac92604e11c7 in /usr/local/bin/ 
# Tue, 12 Jul 2022 09:55:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 09:55:54 GMT
STOPSIGNAL SIGINT
# Tue, 12 Jul 2022 09:55:54 GMT
EXPOSE 5432
# Tue, 12 Jul 2022 09:55:55 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6943e62c5432f1fddd4b062713d5f400098bbff34365f5bb27bfabc25d4e2f`  
		Last Modified: Tue, 12 Jul 2022 09:58:08 GMT  
		Size: 4.4 MB (4414784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558c55f04e35e37b5fc62fae99a2a3d22db8849bb0e0749cbb87ca839c19ec97`  
		Last Modified: Tue, 12 Jul 2022 09:58:06 GMT  
		Size: 1.8 KB (1798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186be55594a7d6d67609c7b12dffed9456b34bd896bd37a04fa97b17a69af375`  
		Last Modified: Tue, 12 Jul 2022 09:58:07 GMT  
		Size: 1.4 MB (1418439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f382409811573b22f5e8bc8bf2a0914d10a9a833e8240cdc8c83250ad804fe93`  
		Last Modified: Tue, 12 Jul 2022 09:58:06 GMT  
		Size: 8.0 MB (8045418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0699dc58a927d7fd277588b8bf597f36656f1736c4d515fee9c4faa9ce80933`  
		Last Modified: Tue, 12 Jul 2022 09:58:05 GMT  
		Size: 1.3 MB (1261148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066f440c89a6a396ba84cc695715ae8725044a62b4da02b63e0b7daefec84ab7`  
		Last Modified: Tue, 12 Jul 2022 09:58:04 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce20e6e2a202387101b61cf08d53693f0363b0b90ce84f729b6266e0d8a9f8aa`  
		Last Modified: Tue, 12 Jul 2022 09:58:04 GMT  
		Size: 3.2 KB (3201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9945c466321df4a9c07fca7f8d059f7e42bb1be38a1e6dd7035c342195f21a0`  
		Last Modified: Tue, 12 Jul 2022 09:59:23 GMT  
		Size: 90.0 MB (90044693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8293214c54058e3750d2d9ef27370ea93a07d05eb87c6f0b2408f4fa03f4954e`  
		Last Modified: Tue, 12 Jul 2022 09:59:10 GMT  
		Size: 9.4 KB (9353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc4d9b2983adae2cc9f083699402eb0612330e1a22f0e884696cdf3e0224687`  
		Last Modified: Tue, 12 Jul 2022 09:59:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f88faff4eae4bfa8851e2bd4d2e814bb2d58a3a6156ad73df28ecba82ba494`  
		Last Modified: Tue, 12 Jul 2022 09:59:10 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1121f582683012bf500aff06bbdfc4bde46f2ba0c2aad8a2fde5c94c64c06a1`  
		Last Modified: Tue, 12 Jul 2022 09:59:10 GMT  
		Size: 4.7 KB (4700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; arm variant v5

```console
$ docker pull postgres@sha256:f2413072b61ab08b259547616d915e7315855c9be394b35768fa3f2917d39558
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.8 MB (129841596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be8148732c54eff5792c94085b040d691d68429c979717a9f7d5982626a63157`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 12 Jul 2022 00:50:38 GMT
ADD file:c11ce95201c98565eb5f40f837837d88c7b16d81d608b6dce953f51c90167b03 in / 
# Tue, 12 Jul 2022 00:50:39 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 22:02:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 22:02:57 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 12 Jul 2022 22:02:57 GMT
ENV GOSU_VERSION=1.14
# Tue, 12 Jul 2022 22:03:20 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Jul 2022 22:03:43 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 12 Jul 2022 22:03:43 GMT
ENV LANG=en_US.utf8
# Tue, 12 Jul 2022 22:03:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 22:03:56 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 12 Jul 2022 22:03:58 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 12 Jul 2022 23:22:52 GMT
ENV PG_MAJOR=13
# Tue, 12 Jul 2022 23:22:53 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 12 Jul 2022 23:22:53 GMT
ENV PG_VERSION=13.7-1.pgdg110+1
# Tue, 12 Jul 2022 23:59:18 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 12 Jul 2022 23:59:21 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 12 Jul 2022 23:59:22 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 12 Jul 2022 23:59:23 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 12 Jul 2022 23:59:24 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 12 Jul 2022 23:59:25 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 12 Jul 2022 23:59:25 GMT
COPY file:925d466681c8349f58385c00a8caa567c76b695158aa04bf4ad2ac92604e11c7 in /usr/local/bin/ 
# Tue, 12 Jul 2022 23:59:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 23:59:26 GMT
STOPSIGNAL SIGINT
# Tue, 12 Jul 2022 23:59:27 GMT
EXPOSE 5432
# Tue, 12 Jul 2022 23:59:27 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f9371f3d7174b9da7d72bb3a49a5a3c5e96d5b106ef3113b25c27d30bb020de9`  
		Last Modified: Tue, 12 Jul 2022 01:03:01 GMT  
		Size: 28.9 MB (28905415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303acbd7d12eff24909ea84de32e3a3e047c2d338309a57f7b2db1333994e624`  
		Last Modified: Wed, 13 Jul 2022 01:35:30 GMT  
		Size: 4.1 MB (4096507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06c71baba1b279bc50bfc65939318dead2b185539c8805111bc9afbd894b2a49`  
		Last Modified: Wed, 13 Jul 2022 01:35:27 GMT  
		Size: 1.8 KB (1791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea634a8cca7deef60da8dc0a61932c6976f69c0dcd18d0a99889020a998de27`  
		Last Modified: Wed, 13 Jul 2022 01:35:27 GMT  
		Size: 1.4 MB (1382635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6139eedb336c3fd6df4d0510d7614e4c175e7ff1764279b902f1107f491f91e3`  
		Last Modified: Wed, 13 Jul 2022 01:35:30 GMT  
		Size: 8.0 MB (8045367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab585889f4c1329f6bc956e6a3c66dccd57a9c3030d2100b226b3712adf3b0b6`  
		Last Modified: Wed, 13 Jul 2022 01:35:26 GMT  
		Size: 1.3 MB (1257281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777b38adc96420d99b18aa4d1367427b9275a6a40a1826e8fc80a0021a405386`  
		Last Modified: Wed, 13 Jul 2022 01:35:25 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6284190bd92a199006d5b64022dd91f1a8f72f68d2323886e25e9800db1a93b5`  
		Last Modified: Wed, 13 Jul 2022 01:35:24 GMT  
		Size: 3.2 KB (3193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfef6b7c59b1568cceea75ef2cfb1f41836830145427b91137a4c9ad65478c07`  
		Last Modified: Wed, 13 Jul 2022 01:38:53 GMT  
		Size: 86.1 MB (86134875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba9391f6f129151b36ad76a583dc2034b7a6bab012e38019418dbba32734b9f`  
		Last Modified: Wed, 13 Jul 2022 01:37:58 GMT  
		Size: 9.4 KB (9353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f52a9615a86b023ead337c19f822520b21f39a2df58c9a8b8013d6603952ec0`  
		Last Modified: Wed, 13 Jul 2022 01:37:58 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abde0e550d37ef534ed24e47d1693c61f5309b9df8619ec894cd884934c1c0cf`  
		Last Modified: Wed, 13 Jul 2022 01:37:58 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:158a1e31a4ac530a797fd2506d66bbc0d1f778707427bbda3e7cfe5dc4169889`  
		Last Modified: Wed, 13 Jul 2022 01:37:58 GMT  
		Size: 4.7 KB (4702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; arm variant v7

```console
$ docker pull postgres@sha256:7b5df55b86abe6490a67bfb27b1d8d7713c9bd51971d9895e1434a8f494ef21d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.6 MB (124566029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:674dc2e3dd475b7523f5afc147542649e3af0eaf269a0e6c254675da1d09803e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:54 GMT
ADD file:ae890621b36ff6e27364bb7316b5bd4319a820ddf7e65565c6201eb11d70fde9 in / 
# Tue, 12 Jul 2022 00:59:55 GMT
CMD ["bash"]
# Wed, 13 Jul 2022 03:31:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Jul 2022 03:31:21 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 13 Jul 2022 03:31:21 GMT
ENV GOSU_VERSION=1.14
# Wed, 13 Jul 2022 03:31:42 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 13 Jul 2022 03:32:02 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 13 Jul 2022 03:32:03 GMT
ENV LANG=en_US.utf8
# Wed, 13 Jul 2022 03:32:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Jul 2022 03:32:13 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 13 Jul 2022 03:32:15 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Wed, 13 Jul 2022 04:44:05 GMT
ENV PG_MAJOR=13
# Wed, 13 Jul 2022 04:44:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Wed, 13 Jul 2022 04:44:07 GMT
ENV PG_VERSION=13.7-1.pgdg110+1
# Wed, 13 Jul 2022 05:17:14 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 13 Jul 2022 05:17:16 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 13 Jul 2022 05:17:18 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 13 Jul 2022 05:17:18 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 13 Jul 2022 05:17:20 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 13 Jul 2022 05:17:20 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 13 Jul 2022 05:17:21 GMT
COPY file:925d466681c8349f58385c00a8caa567c76b695158aa04bf4ad2ac92604e11c7 in /usr/local/bin/ 
# Wed, 13 Jul 2022 05:17:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 05:17:22 GMT
STOPSIGNAL SIGINT
# Wed, 13 Jul 2022 05:17:22 GMT
EXPOSE 5432
# Wed, 13 Jul 2022 05:17:23 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:314cda9d0ef2282082d2bd0efd7659e0d9edb3ceae8e7919d990bcf95cbb3d2b`  
		Last Modified: Tue, 12 Jul 2022 01:12:37 GMT  
		Size: 26.6 MB (26560559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4fa3e19062d6b83e3bc5692c5c2edcaf08075b83500a0542347c807fa34d01`  
		Last Modified: Wed, 13 Jul 2022 06:18:14 GMT  
		Size: 3.7 MB (3717146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040f645a4c35522950453c3024997228884acad8dc37c5552fbff7a8e439e4d2`  
		Last Modified: Wed, 13 Jul 2022 06:18:12 GMT  
		Size: 1.8 KB (1791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5bd0eb26ff40a4493692e166f7f618f907a5bf72117ada2f6a07cf4efa08d5`  
		Last Modified: Wed, 13 Jul 2022 06:18:13 GMT  
		Size: 1.4 MB (1375295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:117ae6e9521f41fbea7d12e55cc11a1c0433718ba29165076ad4aa65aaee776c`  
		Last Modified: Wed, 13 Jul 2022 06:18:16 GMT  
		Size: 8.0 MB (8045393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db053fb5e6f2476a038ffb0ade71f7d9ae420c23d519db36d0c9dda5d8e1d59`  
		Last Modified: Wed, 13 Jul 2022 06:18:11 GMT  
		Size: 1.1 MB (1131201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7245b8a4f54c3fb9689e54d6be9e1753b6b44f926be3f7175743cd5dfb337b`  
		Last Modified: Wed, 13 Jul 2022 06:18:10 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5875ee71e6aa8c5e69fed568ef965e0f377a29a11d3e2df4ccfb291dbb8c2e48`  
		Last Modified: Wed, 13 Jul 2022 06:18:10 GMT  
		Size: 3.2 KB (3198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47899480dda70e4a4813d77b0454771e4fc5df8dc5207ca0038a69de4e0ba932`  
		Last Modified: Wed, 13 Jul 2022 06:21:29 GMT  
		Size: 83.7 MB (83716901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac5edfad79a1af5f43aa797a44565f5942529b4eedcdc596d3a8372545dd9b5`  
		Last Modified: Wed, 13 Jul 2022 06:20:38 GMT  
		Size: 9.4 KB (9364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee690d92fdc39dbe24cd84ab6ed02b784d26b4dcba7e11dedb06c93d7465084c`  
		Last Modified: Wed, 13 Jul 2022 06:20:38 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31cf8bf0853b40430738fd11981ffaa9df2558283365f8542976b7b7ea079273`  
		Last Modified: Wed, 13 Jul 2022 06:20:38 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a040a0d4cff7fe66564aaca6c857c74f94d0cefb34f2a9259b7775136b527739`  
		Last Modified: Wed, 13 Jul 2022 06:20:38 GMT  
		Size: 4.7 KB (4703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:81d31d6b26d1c227d47ede3c1187a5e6066f4df839a00b6b449c3f5a0284b3fb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.2 MB (131235734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ade537adc1bc617a95266300bdf3edee64e9c08d99ea03c4b01eda9538ccb1be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 14:36:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 14:36:01 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 12 Jul 2022 14:36:02 GMT
ENV GOSU_VERSION=1.14
# Tue, 12 Jul 2022 14:36:11 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Jul 2022 14:36:18 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 12 Jul 2022 14:36:18 GMT
ENV LANG=en_US.utf8
# Tue, 12 Jul 2022 14:36:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 14:36:23 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 12 Jul 2022 14:36:25 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 12 Jul 2022 14:37:57 GMT
ENV PG_MAJOR=13
# Tue, 12 Jul 2022 14:37:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 12 Jul 2022 14:37:59 GMT
ENV PG_VERSION=13.7-1.pgdg110+1
# Tue, 12 Jul 2022 14:38:17 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 12 Jul 2022 14:38:18 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 12 Jul 2022 14:38:18 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 12 Jul 2022 14:38:19 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 12 Jul 2022 14:38:20 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 12 Jul 2022 14:38:21 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 12 Jul 2022 14:38:23 GMT
COPY file:925d466681c8349f58385c00a8caa567c76b695158aa04bf4ad2ac92604e11c7 in /usr/local/bin/ 
# Tue, 12 Jul 2022 14:38:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 14:38:24 GMT
STOPSIGNAL SIGINT
# Tue, 12 Jul 2022 14:38:25 GMT
EXPOSE 5432
# Tue, 12 Jul 2022 14:38:26 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fad7962cc38b78b27b6eebfc7a57f9a5e1de8729d4af07005fc934614f4732`  
		Last Modified: Tue, 12 Jul 2022 14:42:17 GMT  
		Size: 4.2 MB (4209348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac096a3cfeb6feba14c27eeb59eae906a26dfa5607563f9535407cd420e57e6a`  
		Last Modified: Tue, 12 Jul 2022 14:42:16 GMT  
		Size: 1.6 KB (1650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6505ea08ff74e5bbe0a291f6024343fef91f688dcdc55bdff3238cb784e7126e`  
		Last Modified: Tue, 12 Jul 2022 14:42:16 GMT  
		Size: 1.3 MB (1346177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273081b4002f3f50d8d7d4e130136e623b24bbc8872edca1aa5d44c2d686173c`  
		Last Modified: Tue, 12 Jul 2022 14:42:15 GMT  
		Size: 8.0 MB (8043669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1b3627e1624264a16e3fd6f9d094ab16b365ac4bf92c8a208c6542b3137e1a`  
		Last Modified: Tue, 12 Jul 2022 14:42:13 GMT  
		Size: 1.0 MB (1025886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56b0e9d7500c4e398ae2062f74634ed38558ed6972d51dce6e30eb478a466a7`  
		Last Modified: Tue, 12 Jul 2022 14:42:13 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db829696ec4587ad45fcc3fb03310870d70cb4971939fc31766adb42b0d0d86`  
		Last Modified: Tue, 12 Jul 2022 14:42:13 GMT  
		Size: 3.1 KB (3139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76fc0860395abc43254ef325d382bddf368b16dad1bb4797b255c40607e97b7b`  
		Last Modified: Tue, 12 Jul 2022 14:43:30 GMT  
		Size: 86.5 MB (86537168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa1f005da1560e45b2ec44f19a56a550087cbb13f552827cff2b132e0c012a8`  
		Last Modified: Tue, 12 Jul 2022 14:43:18 GMT  
		Size: 9.4 KB (9357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395abeb1620b11d8c411725d79147737ac1da80615c7b6de82295e22b77e9c6d`  
		Last Modified: Tue, 12 Jul 2022 14:43:18 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e158d569f1153374020efe5b345fd95ff1f557751d1f08d1efc352c20fccffaa`  
		Last Modified: Tue, 12 Jul 2022 14:43:18 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9efe9795f4180489fead9450951917ffc64dc41eb08e23b58ac81991f8a708e7`  
		Last Modified: Tue, 12 Jul 2022 14:43:18 GMT  
		Size: 4.7 KB (4700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; 386

```console
$ docker pull postgres@sha256:b325b9a7fd782c9c15941e0e88ab8f16cb073165c585649381b50771c88f8ac6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.2 MB (138207357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df7f2be72d10c3bd0021ed65e88753a9cc86254c4cad8a44cddc3538d7e7a0de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 12 Jul 2022 00:39:27 GMT
ADD file:7f2bf44013d7848f051407d854b68c0d415a5328a3f5d241fca3150ce23bde65 in / 
# Tue, 12 Jul 2022 00:39:27 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 08:51:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 08:51:34 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 12 Jul 2022 08:51:35 GMT
ENV GOSU_VERSION=1.14
# Tue, 12 Jul 2022 08:51:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Jul 2022 08:51:52 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 12 Jul 2022 08:51:52 GMT
ENV LANG=en_US.utf8
# Tue, 12 Jul 2022 08:51:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 08:51:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 12 Jul 2022 08:52:00 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 12 Jul 2022 09:19:53 GMT
ENV PG_MAJOR=13
# Tue, 12 Jul 2022 09:19:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 12 Jul 2022 09:19:55 GMT
ENV PG_VERSION=13.7-1.pgdg110+1
# Tue, 12 Jul 2022 09:32:21 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 12 Jul 2022 09:32:22 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 12 Jul 2022 09:32:23 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 12 Jul 2022 09:32:24 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 12 Jul 2022 09:32:25 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 12 Jul 2022 09:32:26 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 12 Jul 2022 09:32:28 GMT
COPY file:925d466681c8349f58385c00a8caa567c76b695158aa04bf4ad2ac92604e11c7 in /usr/local/bin/ 
# Tue, 12 Jul 2022 09:32:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 09:32:29 GMT
STOPSIGNAL SIGINT
# Tue, 12 Jul 2022 09:32:30 GMT
EXPOSE 5432
# Tue, 12 Jul 2022 09:32:31 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:1c0050b86a85a326857dbfa0456b3321f92df7e98ca468c048ee3e60dd14c923`  
		Last Modified: Tue, 12 Jul 2022 00:45:18 GMT  
		Size: 32.4 MB (32373949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99306d3f43cc08589c29edb9393be11902948a33d05cb262f943f8f5149babd9`  
		Last Modified: Tue, 12 Jul 2022 10:07:53 GMT  
		Size: 4.6 MB (4607252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a10fe24459a77ea0e46e11e5bb11876a49dc0ff86a269d24c5309538c6100b4c`  
		Last Modified: Tue, 12 Jul 2022 10:07:51 GMT  
		Size: 1.6 KB (1640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b21f13f56adff3d5b9ff40b37379ecdde2033eb563545a8e159c38dc3619091`  
		Last Modified: Tue, 12 Jul 2022 10:07:52 GMT  
		Size: 1.4 MB (1385103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ebfb8865e8a5691a2a9fbaf00969e6ccd5d2dc9a4a05873751de763b287f27`  
		Last Modified: Tue, 12 Jul 2022 10:07:51 GMT  
		Size: 8.0 MB (8043598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654726c07f09f38b39dbb1f53f125f5f9b754ccf9ae63898dcefc9122e4df025`  
		Last Modified: Tue, 12 Jul 2022 10:07:49 GMT  
		Size: 1.0 MB (1027918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac512b35d7fe6806ee227cb2f29f11af2c5e6e15d0cfbdc89c0e20139075e69`  
		Last Modified: Tue, 12 Jul 2022 10:07:49 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d31a88d66016ccd87d1071e63814586e128de31c72fd96f6150444a7f7cbc79`  
		Last Modified: Tue, 12 Jul 2022 10:07:49 GMT  
		Size: 3.1 KB (3140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55ecfaeed54d04a7738008fd1cea43502e3e29b34f51f0e2eb49d361135d4f30`  
		Last Modified: Tue, 12 Jul 2022 10:09:13 GMT  
		Size: 90.8 MB (90750278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ca2ca1a07dde77afcf0d49464921099550938aa6370de1ab3a0bd105b372bf`  
		Last Modified: Tue, 12 Jul 2022 10:09:01 GMT  
		Size: 9.4 KB (9361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01818e6bb59ca3ac3b80eb2ab1982c95413ec2f86aa04d4e5a796f4700d127d`  
		Last Modified: Tue, 12 Jul 2022 10:09:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e557f5e67de81fe53f793659f282efc484defc132143b8f98207ab5fb92d3321`  
		Last Modified: Tue, 12 Jul 2022 10:09:01 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8be8f839bb008ccc7d3a1d897ece943a1c46d72641b15c340b0286bee04e2b8`  
		Last Modified: Tue, 12 Jul 2022 10:09:01 GMT  
		Size: 4.7 KB (4704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; mips64le

```console
$ docker pull postgres@sha256:638e7c3c40c9a449443004ebe3134224016c5fa929d72d23b5cf8c67e44ba071
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.0 MB (131022238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59c257e4a5982b796b2354bc4fcd585973c704c2e09b10b31c3adcb604bb36df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 23 Jun 2022 01:10:25 GMT
ADD file:fd1174cc47ac636f0cab382578a899d69ed489e4dee53ec838955e36066f526a in / 
# Thu, 23 Jun 2022 01:10:29 GMT
CMD ["bash"]
# Fri, 24 Jun 2022 19:08:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 24 Jun 2022 19:09:04 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 24 Jun 2022 19:09:07 GMT
ENV GOSU_VERSION=1.14
# Fri, 24 Jun 2022 19:09:39 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Jun 2022 19:10:11 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Fri, 24 Jun 2022 19:10:14 GMT
ENV LANG=en_US.utf8
# Fri, 24 Jun 2022 19:10:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2022 19:10:39 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 24 Jun 2022 19:10:46 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 24 Jun 2022 21:15:08 GMT
ENV PG_MAJOR=13
# Fri, 24 Jun 2022 21:15:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Fri, 24 Jun 2022 21:15:14 GMT
ENV PG_VERSION=13.7-1.pgdg110+1
# Fri, 24 Jun 2022 22:12:40 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 24 Jun 2022 22:12:47 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 24 Jun 2022 22:12:54 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 24 Jun 2022 22:12:57 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 24 Jun 2022 22:13:04 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 24 Jun 2022 22:13:07 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 24 Jun 2022 22:13:11 GMT
COPY file:925d466681c8349f58385c00a8caa567c76b695158aa04bf4ad2ac92604e11c7 in /usr/local/bin/ 
# Fri, 24 Jun 2022 22:13:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Jun 2022 22:13:18 GMT
STOPSIGNAL SIGINT
# Fri, 24 Jun 2022 22:13:21 GMT
EXPOSE 5432
# Fri, 24 Jun 2022 22:13:25 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:9d199cb5e183b38c9edcc527cbaaa79bb56da73bd09ed449223842775ef4a244`  
		Last Modified: Thu, 23 Jun 2022 01:20:19 GMT  
		Size: 29.6 MB (29641027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7648df165c72f296de832007d97f5fed3103723bba2ec19e91a081d123ee09e7`  
		Last Modified: Sat, 25 Jun 2022 00:45:36 GMT  
		Size: 4.2 MB (4196313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f5094daceac1c9ea62422703d283d7ca3356004152b456f74be3d055af0e89`  
		Last Modified: Sat, 25 Jun 2022 00:45:31 GMT  
		Size: 1.7 KB (1655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8028c8241c5cfdc7d26f2f98828ac6ca21697fc61939c206f438ea938469343e`  
		Last Modified: Sat, 25 Jun 2022 00:45:32 GMT  
		Size: 1.3 MB (1298125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4da59c25c5c741ecf4a7e069b8f2fddd3de1fa0325f2337b9306fa4929a401d2`  
		Last Modified: Sat, 25 Jun 2022 00:45:37 GMT  
		Size: 8.0 MB (8044020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f4695602a43632b8ab413c75f11b6c8f5a4eca6f3a131c8df10a9bbb97e499`  
		Last Modified: Sat, 25 Jun 2022 00:45:29 GMT  
		Size: 1.1 MB (1089523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265c9fc5fd743333be08a366a9788cfcaf43f1f7f34d40e268052237a0aa5c48`  
		Last Modified: Sat, 25 Jun 2022 00:45:28 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa126eaa1168050f95cc77afc8925815476991faf31d837286c0e2e62e63340`  
		Last Modified: Sat, 25 Jun 2022 00:45:28 GMT  
		Size: 3.1 KB (3144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c0d8ce1e872c4b937bcf18ee09997120a68604515a648448be8c9c3b34260d`  
		Last Modified: Sat, 25 Jun 2022 00:48:53 GMT  
		Size: 86.7 MB (86733942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7263ea1c0da8d535091c45c3a53168a61a503e359efb04b38e5abf65ec2e30d9`  
		Last Modified: Sat, 25 Jun 2022 00:47:58 GMT  
		Size: 9.4 KB (9368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c04460618116c8ccc13f56fd1833f8f6fc35d1ac7a073572d7206528350670`  
		Last Modified: Sat, 25 Jun 2022 00:47:58 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e7c0fc2ecd1416c15c4b7c6df07151c943f5eb6c9599c035bf47ed12a09d54`  
		Last Modified: Sat, 25 Jun 2022 00:47:58 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece2a41e8923f0f5893783d61be8f33e107122ab6fd87e697a09e066a91259e0`  
		Last Modified: Sat, 25 Jun 2022 00:47:58 GMT  
		Size: 4.7 KB (4705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; ppc64le

```console
$ docker pull postgres@sha256:72e937cdca034aaec651b934267e009dbafc3d82f477dae4fbd8c2e865f53226
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.5 MB (145549177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15d537f9d0699d183e223099d45d5ff37553c70535bf7e24ddb488c307b91496`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 12 Jul 2022 01:25:28 GMT
ADD file:9e1afe48f40d94f879aefb12a7e68da2f0772d701e95b8219bd1f79a83e1933a in / 
# Tue, 12 Jul 2022 01:25:32 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 10:48:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 10:48:17 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 12 Jul 2022 10:48:24 GMT
ENV GOSU_VERSION=1.14
# Tue, 12 Jul 2022 10:49:31 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Jul 2022 10:50:12 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 12 Jul 2022 10:50:15 GMT
ENV LANG=en_US.utf8
# Tue, 12 Jul 2022 10:50:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 10:50:45 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 12 Jul 2022 10:50:59 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 12 Jul 2022 10:58:01 GMT
ENV PG_MAJOR=13
# Tue, 12 Jul 2022 10:58:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 12 Jul 2022 10:58:14 GMT
ENV PG_VERSION=13.7-1.pgdg110+1
# Tue, 12 Jul 2022 11:00:18 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 12 Jul 2022 11:00:40 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 12 Jul 2022 11:00:51 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 12 Jul 2022 11:00:58 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 12 Jul 2022 11:01:24 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 12 Jul 2022 11:01:28 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 12 Jul 2022 11:01:31 GMT
COPY file:925d466681c8349f58385c00a8caa567c76b695158aa04bf4ad2ac92604e11c7 in /usr/local/bin/ 
# Tue, 12 Jul 2022 11:01:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 11:01:41 GMT
STOPSIGNAL SIGINT
# Tue, 12 Jul 2022 11:01:44 GMT
EXPOSE 5432
# Tue, 12 Jul 2022 11:01:52 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:bd3d68d1ce583727f6378a16916795b955cc0ad39e0ebe754a26007ef54744fa`  
		Last Modified: Tue, 12 Jul 2022 01:36:03 GMT  
		Size: 35.3 MB (35272500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23cc31dfc1945301a2dbacd3a88a1e4b7a63f60f5e8ada822152d12d63c749d`  
		Last Modified: Tue, 12 Jul 2022 11:15:08 GMT  
		Size: 5.2 MB (5222939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fcf6cec36bf0efe83531e55d6cb9e568c015e1d05b4d3a37d89c57dc7cce983`  
		Last Modified: Tue, 12 Jul 2022 11:15:07 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb8e6da024bd6b488abbaea614cd1389339a37bc1a0c341c0199a2fa17f93123`  
		Last Modified: Tue, 12 Jul 2022 11:15:06 GMT  
		Size: 1.3 MB (1317666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d4756d654e5ca648fafdfe4c70e0c4c0ee3d31a86ad6a2432c2c15fb8c1fe6`  
		Last Modified: Tue, 12 Jul 2022 11:15:05 GMT  
		Size: 8.0 MB (8045613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdf429696abc3727d1df61bd070a27f143687141941048a42d3ea8f4e5176e3`  
		Last Modified: Tue, 12 Jul 2022 11:15:03 GMT  
		Size: 1.4 MB (1420311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cb5984f8629ebe78169a779004f16f35b0fa8aa0586734bf3b4c1698fd6b3d`  
		Last Modified: Tue, 12 Jul 2022 11:15:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af42b06acd74d24966a20432ca1c1ff84246d779e95f0655deb625dd1e55250e`  
		Last Modified: Tue, 12 Jul 2022 11:15:03 GMT  
		Size: 3.2 KB (3200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc48013db32919ce469c5fcad4c5bd5127d6d96f9c0dfa6b891e9f8390d705b`  
		Last Modified: Tue, 12 Jul 2022 11:16:47 GMT  
		Size: 94.3 MB (94250603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e63743c5ff94c2e95fae78deaf15fd40fc513f57b16f78d09861c71f022cf01`  
		Last Modified: Tue, 12 Jul 2022 11:16:31 GMT  
		Size: 9.4 KB (9361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6040f6ff3c2672efb5238024f623e102a3974cb73193cc82930ebc0e39ee6a7d`  
		Last Modified: Tue, 12 Jul 2022 11:16:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a461683b8d24b9d8eaba7e9ed37385c0dc82f1e77ff68606de785e1f9f32e705`  
		Last Modified: Tue, 12 Jul 2022 11:16:31 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1f4f91a4fec0c8d696fd4d38ec0167ea6fe75b1ab32c79d3f0733c30680b3b`  
		Last Modified: Tue, 12 Jul 2022 11:16:31 GMT  
		Size: 4.7 KB (4702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:13-bullseye` - linux; s390x

```console
$ docker pull postgres@sha256:55466792d5e1ef97252a8a6ed6700d49d5b71fa9d895d98069ff7f94488913bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.3 MB (140275082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:114cf51b2ce2e762b62d4d8faab5d699356a3ef8739d1806044e9dd5f2d41a7e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 12 Jul 2022 00:43:45 GMT
ADD file:70135711d42f7b2b32586e31afb57a0590019326efa82abf1402dc7a8f02a3f2 in / 
# Tue, 12 Jul 2022 00:43:49 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 10:05:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jul 2022 10:05:40 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 12 Jul 2022 10:05:40 GMT
ENV GOSU_VERSION=1.14
# Tue, 12 Jul 2022 10:06:21 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Jul 2022 10:06:36 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 12 Jul 2022 10:06:38 GMT
ENV LANG=en_US.utf8
# Tue, 12 Jul 2022 10:06:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 10:06:47 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 12 Jul 2022 10:06:50 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 12 Jul 2022 10:38:28 GMT
ENV PG_MAJOR=13
# Tue, 12 Jul 2022 10:38:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/13/bin
# Tue, 12 Jul 2022 10:38:30 GMT
ENV PG_VERSION=13.7-1.pgdg110+1
# Tue, 12 Jul 2022 10:53:49 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			DEBIAN_FRONTEND=noninteractive 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 12 Jul 2022 10:54:07 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 12 Jul 2022 10:54:09 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 12 Jul 2022 10:54:09 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 12 Jul 2022 10:54:11 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 12 Jul 2022 10:54:12 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 12 Jul 2022 10:54:12 GMT
COPY file:925d466681c8349f58385c00a8caa567c76b695158aa04bf4ad2ac92604e11c7 in /usr/local/bin/ 
# Tue, 12 Jul 2022 10:54:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 10:54:13 GMT
STOPSIGNAL SIGINT
# Tue, 12 Jul 2022 10:54:13 GMT
EXPOSE 5432
# Tue, 12 Jul 2022 10:54:14 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:447abc12b0c6da6e339b4fa17a2a7dd672d6f0631d30ee44c28b8b06e78884bd`  
		Last Modified: Tue, 12 Jul 2022 00:53:41 GMT  
		Size: 29.6 MB (29640209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7b26d4950b94e4688deadca00cb0009b94b72053e16f3577b9eb53c25a093a`  
		Last Modified: Tue, 12 Jul 2022 11:39:23 GMT  
		Size: 4.3 MB (4302311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9442592ec81a6f758da53abb01b49b3d717eef442785058fadbb914d0b9ab90`  
		Last Modified: Tue, 12 Jul 2022 11:39:21 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebb0037a974440a3899900eb8b1cb9e71616923bdf361c000263bcb05881742`  
		Last Modified: Tue, 12 Jul 2022 11:39:22 GMT  
		Size: 1.4 MB (1381608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e57982a35204b8cb0a413ed5fad4c568101e4a56eff1a1281aceb751bbc2df1`  
		Last Modified: Tue, 12 Jul 2022 11:39:21 GMT  
		Size: 8.1 MB (8099254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b3153d253d1a6195d829c0eed58397c1720cde84cad9ae4d82748d7f5eff4e`  
		Last Modified: Tue, 12 Jul 2022 11:39:19 GMT  
		Size: 1.2 MB (1238009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5d7f04c24324e7b4b7b07c9fb9aa89ef64437da6eab2007f23f93c793c7cd4`  
		Last Modified: Tue, 12 Jul 2022 11:39:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e1128f0e0c3968222b5a2c5f79a67dccfadc9e5c42ba2407648c158047e317`  
		Last Modified: Tue, 12 Jul 2022 11:39:19 GMT  
		Size: 3.2 KB (3193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6181f333ebf7b818075873f914f8ebda927dcec7be4b36aa89185ee5b373f472`  
		Last Modified: Tue, 12 Jul 2022 11:40:21 GMT  
		Size: 95.6 MB (95594145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac198c35f410fef5ef5006fe114291a4e2dc7c7eba94d4660b3096616a43be46`  
		Last Modified: Tue, 12 Jul 2022 11:40:08 GMT  
		Size: 9.4 KB (9366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbefd1db2766573cba5717c04331b280b379546c055b82b4ce0555e5c2e9cd5`  
		Last Modified: Tue, 12 Jul 2022 11:40:08 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acdc175dfa654ba84aacc440a535e905117273e8a431bbdfc30b2391d1a39f32`  
		Last Modified: Tue, 12 Jul 2022 11:40:08 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8254bdb9897924a296563b5b3a250b476745118afcc81f0a3070f1671e0e0d77`  
		Last Modified: Tue, 12 Jul 2022 11:40:08 GMT  
		Size: 4.7 KB (4703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
