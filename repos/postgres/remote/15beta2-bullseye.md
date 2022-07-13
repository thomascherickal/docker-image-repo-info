## `postgres:15beta2-bullseye`

```console
$ docker pull postgres@sha256:e942c0eef67e58c9da60f249194604799715f30cdf6d0b7dfb43d851905b1013
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

### `postgres:15beta2-bullseye` - linux; amd64

```console
$ docker pull postgres@sha256:833dd8777c27d7d611531e06a9cc901f8fdaa03f442a6db3745f23c904a4c86d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.8 MB (139791270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:541d40755842c99974b6f81144fc87f2aea183df6c1bc0b1a26deeae0811198e`
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
# Tue, 12 Jul 2022 09:54:35 GMT
ENV PG_MAJOR=15
# Tue, 12 Jul 2022 09:54:35 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Tue, 12 Jul 2022 09:54:36 GMT
ENV PG_VERSION=15~beta2-1.pgdg110+1
# Tue, 12 Jul 2022 09:54:56 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 12 Jul 2022 09:54:57 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 12 Jul 2022 09:54:58 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 12 Jul 2022 09:54:58 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 12 Jul 2022 09:54:58 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 12 Jul 2022 09:54:58 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 12 Jul 2022 09:54:59 GMT
COPY file:925d466681c8349f58385c00a8caa567c76b695158aa04bf4ad2ac92604e11c7 in /usr/local/bin/ 
# Tue, 12 Jul 2022 09:54:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 09:54:59 GMT
STOPSIGNAL SIGINT
# Tue, 12 Jul 2022 09:54:59 GMT
EXPOSE 5432
# Tue, 12 Jul 2022 09:54:59 GMT
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
	-	`sha256:bec4b01568c1fb6bead04777e2dccbf0cd5379f0a25ce6da7f7eb24632752b50`  
		Last Modified: Tue, 12 Jul 2022 09:58:15 GMT  
		Size: 93.3 MB (93264901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a052c26ad499a095fda0d0c50903730e2f5fd70048fca193ac372a2cab7ee608`  
		Last Modified: Tue, 12 Jul 2022 09:58:01 GMT  
		Size: 9.8 KB (9790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c6b64906df2391385129dd492819f60b37f175cb60bc355c9c582ffe32e4b14`  
		Last Modified: Tue, 12 Jul 2022 09:58:01 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5309af75d1de06ea8a10116fb008a9f3c6b648f96ad2045a2f108bf3c2bfb75`  
		Last Modified: Tue, 12 Jul 2022 09:58:01 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452483e1d6d8103d68aba907d3ce435b45df5f96119599bbe10379c7838950d1`  
		Last Modified: Tue, 12 Jul 2022 09:58:02 GMT  
		Size: 4.7 KB (4702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta2-bullseye` - linux; arm variant v5

```console
$ docker pull postgres@sha256:0064bb3e721998961cd5f9a83f9b09bcc0902542b84c7071ef323c702b10474f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.1 MB (133082430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31157849d7fbec002902634301dac5953962402e69c3204dca3a7fca8b1de4e0`
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
# Tue, 12 Jul 2022 22:03:58 GMT
ENV PG_MAJOR=15
# Tue, 12 Jul 2022 22:03:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Tue, 12 Jul 2022 22:03:59 GMT
ENV PG_VERSION=15~beta2-1.pgdg110+1
# Tue, 12 Jul 2022 22:43:54 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 12 Jul 2022 22:43:56 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 12 Jul 2022 22:43:57 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 12 Jul 2022 22:43:58 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 12 Jul 2022 22:43:59 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 12 Jul 2022 22:44:00 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 12 Jul 2022 22:44:00 GMT
COPY file:925d466681c8349f58385c00a8caa567c76b695158aa04bf4ad2ac92604e11c7 in /usr/local/bin/ 
# Tue, 12 Jul 2022 22:44:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 22:44:01 GMT
STOPSIGNAL SIGINT
# Tue, 12 Jul 2022 22:44:01 GMT
EXPOSE 5432
# Tue, 12 Jul 2022 22:44:02 GMT
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
	-	`sha256:b7fce093d87f48363d4875049714a4c63a0cff439efba525bd7dc1005293926c`  
		Last Modified: Wed, 13 Jul 2022 01:36:20 GMT  
		Size: 89.4 MB (89375271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdcee96f62cf4902c0706365274f0bc922ef3154d1f10b70fc2de90618891d9b`  
		Last Modified: Wed, 13 Jul 2022 01:35:23 GMT  
		Size: 9.8 KB (9794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7878cb1a14d576b4a10b3118e6f3ae4ab22d3500e5b9442672ab859b5a87e9eb`  
		Last Modified: Wed, 13 Jul 2022 01:35:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf201a376394d83933683360a004e7b4160a673ab3b24e7a28a5cb5adb1b69b8`  
		Last Modified: Wed, 13 Jul 2022 01:35:23 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1f7235032dc98b615007fa3b83d35df7e27185127f2a45b21a6ab84266a7a4`  
		Last Modified: Wed, 13 Jul 2022 01:35:23 GMT  
		Size: 4.7 KB (4699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta2-bullseye` - linux; arm variant v7

```console
$ docker pull postgres@sha256:5de51b883535b03f36f46549cb10d00142e85f41daf50a8c850f7be0051e0c0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.7 MB (127708208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55d11b5e89b31ff0c4b53d5c57340bd7edcd71c0bcee72fb9810ed2d1cd5ae28`
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
# Wed, 13 Jul 2022 03:32:16 GMT
ENV PG_MAJOR=15
# Wed, 13 Jul 2022 03:32:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Wed, 13 Jul 2022 03:32:17 GMT
ENV PG_VERSION=15~beta2-1.pgdg110+1
# Wed, 13 Jul 2022 04:07:58 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 13 Jul 2022 04:08:01 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 13 Jul 2022 04:08:02 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 13 Jul 2022 04:08:03 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 13 Jul 2022 04:08:04 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 13 Jul 2022 04:08:04 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 13 Jul 2022 04:08:05 GMT
COPY file:925d466681c8349f58385c00a8caa567c76b695158aa04bf4ad2ac92604e11c7 in /usr/local/bin/ 
# Wed, 13 Jul 2022 04:08:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 04:08:06 GMT
STOPSIGNAL SIGINT
# Wed, 13 Jul 2022 04:08:06 GMT
EXPOSE 5432
# Wed, 13 Jul 2022 04:08:07 GMT
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
	-	`sha256:35dc1ee66ac5e51dd2c1ad7f1380c80c77915001271d9dd5e349e9db0698d815`  
		Last Modified: Wed, 13 Jul 2022 06:19:00 GMT  
		Size: 86.9 MB (86858655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e885bf12442a101d0068d9ab198cdf3f3510a2548354ecdd224171d2e2cdbc2c`  
		Last Modified: Wed, 13 Jul 2022 06:18:08 GMT  
		Size: 9.8 KB (9792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d2744cafe73eb504a91eef4331bc3b52083ecf2be0488252c9b4004f79392c`  
		Last Modified: Wed, 13 Jul 2022 06:18:08 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1bf7c5f8979d6109eb8c532ca665aa4049288cce574d8d771c34652172abc6e`  
		Last Modified: Wed, 13 Jul 2022 06:18:08 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268a5c79eba405622b58d409910d21acd8e1f49a71cd5287ab4d8557461b4709`  
		Last Modified: Wed, 13 Jul 2022 06:18:08 GMT  
		Size: 4.7 KB (4699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta2-bullseye` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:4a1c210231d602497e1df52053b999c7574b1fe8acf4dbeeb55c8717fa4f2771
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.4 MB (134449285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c049e67935245269d7e63e2b7183f29d04697c013f4adb62aa344a92d6332a8`
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
# Tue, 12 Jul 2022 14:36:26 GMT
ENV PG_MAJOR=15
# Tue, 12 Jul 2022 14:36:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Tue, 12 Jul 2022 14:36:28 GMT
ENV PG_VERSION=15~beta2-1.pgdg110+1
# Tue, 12 Jul 2022 14:36:47 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 12 Jul 2022 14:36:48 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 12 Jul 2022 14:36:49 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 12 Jul 2022 14:36:50 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 12 Jul 2022 14:36:51 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 12 Jul 2022 14:36:52 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 12 Jul 2022 14:36:54 GMT
COPY file:925d466681c8349f58385c00a8caa567c76b695158aa04bf4ad2ac92604e11c7 in /usr/local/bin/ 
# Tue, 12 Jul 2022 14:36:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 14:36:55 GMT
STOPSIGNAL SIGINT
# Tue, 12 Jul 2022 14:36:56 GMT
EXPOSE 5432
# Tue, 12 Jul 2022 14:36:57 GMT
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
	-	`sha256:dc75e7874a91e4bccd2119d6fc9198dc3bf9374d0014ab36b198b3bafd08086d`  
		Last Modified: Tue, 12 Jul 2022 14:42:23 GMT  
		Size: 89.8 MB (89750288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e3a2df14b21fd1a2dc74fe873b7c47eceb49d02e9df44c031b85a14f5206714`  
		Last Modified: Tue, 12 Jul 2022 14:42:11 GMT  
		Size: 9.8 KB (9791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bccbb6c35eec6bce84a88e5ab75b2313833d6bd16b49098e3e2db7d687597b6`  
		Last Modified: Tue, 12 Jul 2022 14:42:11 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1aeec274fb72e9c6ece8691020af6b97a79c20f232f507146f059a88ca6fd43`  
		Last Modified: Tue, 12 Jul 2022 14:42:11 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c698958d71f44bbb776c378f1b09b4b5299087995ee03f34a94f658b69bbb56a`  
		Last Modified: Tue, 12 Jul 2022 14:42:11 GMT  
		Size: 4.7 KB (4696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta2-bullseye` - linux; 386

```console
$ docker pull postgres@sha256:f103aa69445410410417f19078b99a8a7bae1d3955772a9e7b5cf7cf766cd745
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.5 MB (141471799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af90db7b072ef1a2b84fc867bafc5893bcf9f29dbd962de14a564b8d5379b18b`
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
# Tue, 12 Jul 2022 08:52:00 GMT
ENV PG_MAJOR=15
# Tue, 12 Jul 2022 08:52:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Tue, 12 Jul 2022 08:52:02 GMT
ENV PG_VERSION=15~beta2-1.pgdg110+1
# Tue, 12 Jul 2022 09:05:52 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 12 Jul 2022 09:05:53 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 12 Jul 2022 09:05:54 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 12 Jul 2022 09:05:55 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 12 Jul 2022 09:05:56 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 12 Jul 2022 09:05:57 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 12 Jul 2022 09:05:59 GMT
COPY file:925d466681c8349f58385c00a8caa567c76b695158aa04bf4ad2ac92604e11c7 in /usr/local/bin/ 
# Tue, 12 Jul 2022 09:05:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 09:06:00 GMT
STOPSIGNAL SIGINT
# Tue, 12 Jul 2022 09:06:01 GMT
EXPOSE 5432
# Tue, 12 Jul 2022 09:06:02 GMT
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
	-	`sha256:5f5de384580dcf993b9bc45ad7175fb8f507f6ad3579963f8d81de1cb2684698`  
		Last Modified: Tue, 12 Jul 2022 10:08:05 GMT  
		Size: 94.0 MB (94014283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf78d787c7c59ae91813d1916b71bf590500be1dec316c49e44b14f49eecfff`  
		Last Modified: Tue, 12 Jul 2022 10:07:47 GMT  
		Size: 9.8 KB (9794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f345440a6776644cb73b25f455ea39551043bfb42251a2e5e3a2ad27da82cabb`  
		Last Modified: Tue, 12 Jul 2022 10:07:47 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb171dd91180151ecd30e6ee5453a1e44aba7d19bcc80cee51593d3e20fdb57`  
		Last Modified: Tue, 12 Jul 2022 10:07:47 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662c7aba104cf744d1288a37611350ae75f4761b917be5506c168998c76efc29`  
		Last Modified: Tue, 12 Jul 2022 10:07:47 GMT  
		Size: 4.7 KB (4707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta2-bullseye` - linux; mips64le

```console
$ docker pull postgres@sha256:17495de7e21632815a9397ddc7b85ea1bf81e0c814f06a4215522040b36ddf21
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.5 MB (135467663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:735ee14413ac99422f2d4330549a445b2f7dd0f544bbbbf11893ade2323f3a69`
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
# Fri, 24 Jun 2022 19:10:49 GMT
ENV PG_MAJOR=15
# Fri, 24 Jun 2022 19:10:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Fri, 01 Jul 2022 03:52:26 GMT
ENV PG_VERSION=15~beta2-1.pgdg110+1
# Fri, 01 Jul 2022 04:53:11 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 01 Jul 2022 04:53:18 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 01 Jul 2022 04:53:24 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 01 Jul 2022 04:53:28 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 01 Jul 2022 04:53:34 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 01 Jul 2022 04:53:37 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 01 Jul 2022 04:53:40 GMT
COPY file:925d466681c8349f58385c00a8caa567c76b695158aa04bf4ad2ac92604e11c7 in /usr/local/bin/ 
# Fri, 01 Jul 2022 04:53:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 01 Jul 2022 04:53:47 GMT
STOPSIGNAL SIGINT
# Fri, 01 Jul 2022 04:53:50 GMT
EXPOSE 5432
# Fri, 01 Jul 2022 04:53:54 GMT
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
	-	`sha256:dcbe5d98ffb45a33ec102e8a5908f5634cbe0ffa007c1499f0c0357c3d1d63dc`  
		Last Modified: Fri, 01 Jul 2022 04:55:29 GMT  
		Size: 91.2 MB (91178941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edc632fc8b061ce00d61d05292d45a4eedc5426ba6746c5835cd8ff77abe2e5`  
		Last Modified: Fri, 01 Jul 2022 04:54:31 GMT  
		Size: 9.8 KB (9795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db2898f0a17b85c191b79b1dffdcdcaad59a20ed3028872f4e386edce49a08e`  
		Last Modified: Fri, 01 Jul 2022 04:54:31 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59476fbf372aa65a4505d24809ff41a77737898b8107b3ab786c8e7c4f33967a`  
		Last Modified: Fri, 01 Jul 2022 04:54:31 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a78afafd9b52a0451cb0566b2a3d351326e7c930caf36cf5320168449a7e3da`  
		Last Modified: Fri, 01 Jul 2022 04:54:31 GMT  
		Size: 4.7 KB (4705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta2-bullseye` - linux; ppc64le

```console
$ docker pull postgres@sha256:b9e3598b2c8259a33597044958bb442f634377046262ce1470ebc96d75f81919
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.9 MB (148888933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:472a3e755cd3313f62b8c8bce947304d86b246876e69eeba8a4aa9c99b29d0ba`
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
# Tue, 12 Jul 2022 10:51:04 GMT
ENV PG_MAJOR=15
# Tue, 12 Jul 2022 10:51:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Tue, 12 Jul 2022 10:51:14 GMT
ENV PG_VERSION=15~beta2-1.pgdg110+1
# Tue, 12 Jul 2022 10:52:53 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 12 Jul 2022 10:53:07 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 12 Jul 2022 10:53:19 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 12 Jul 2022 10:53:25 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 12 Jul 2022 10:53:34 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 12 Jul 2022 10:53:39 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 12 Jul 2022 10:53:40 GMT
COPY file:925d466681c8349f58385c00a8caa567c76b695158aa04bf4ad2ac92604e11c7 in /usr/local/bin/ 
# Tue, 12 Jul 2022 10:53:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 10:53:48 GMT
STOPSIGNAL SIGINT
# Tue, 12 Jul 2022 10:53:50 GMT
EXPOSE 5432
# Tue, 12 Jul 2022 10:53:55 GMT
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
	-	`sha256:be0221619ec1393e4bcc3f9a1e5966acc2d64dbb12a64d01187e53e9dc3d3cec`  
		Last Modified: Tue, 12 Jul 2022 11:15:17 GMT  
		Size: 97.6 MB (97589932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdff6edc4b697af5f0ff441085c06c9bc5b499e34c1142752efb58c2eab32441`  
		Last Modified: Tue, 12 Jul 2022 11:15:00 GMT  
		Size: 9.8 KB (9791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d265853c16591afd991c96d5cf614fb6c423b0730a277aaba8670e348b4117f`  
		Last Modified: Tue, 12 Jul 2022 11:15:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12005b1446ef2a114fd630aa2b764b9e7995d0d5287cebcec6f424f044a7697`  
		Last Modified: Tue, 12 Jul 2022 11:15:00 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa4a50c61d5053d154208ade5c77aa5d82344344635f8ac37ccb5e88ff656cb`  
		Last Modified: Tue, 12 Jul 2022 11:15:00 GMT  
		Size: 4.7 KB (4699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:15beta2-bullseye` - linux; s390x

```console
$ docker pull postgres@sha256:5a8f943427d66a6c877ee7c667b4c53b68ecab257c93095b43635386cd5872eb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.5 MB (86537352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1a8e979f4786e2b6ec654ff9f72d2c07580ee8145118d122fa8b8214b729f86`
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
# Tue, 12 Jul 2022 10:06:50 GMT
ENV PG_MAJOR=15
# Tue, 12 Jul 2022 10:06:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Tue, 12 Jul 2022 10:06:52 GMT
ENV PG_VERSION=15~beta2-1.pgdg110+1
# Tue, 12 Jul 2022 10:22:25 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 12 Jul 2022 10:22:37 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 12 Jul 2022 10:22:39 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 12 Jul 2022 10:22:40 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 12 Jul 2022 10:22:42 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 12 Jul 2022 10:22:42 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 12 Jul 2022 10:22:43 GMT
COPY file:925d466681c8349f58385c00a8caa567c76b695158aa04bf4ad2ac92604e11c7 in /usr/local/bin/ 
# Tue, 12 Jul 2022 10:22:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Jul 2022 10:22:44 GMT
STOPSIGNAL SIGINT
# Tue, 12 Jul 2022 10:22:45 GMT
EXPOSE 5432
# Tue, 12 Jul 2022 10:22:45 GMT
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
	-	`sha256:4103987b61bb89ae77353146b9db50bcdaf118d82600ea6e72774ccfaf7dc814`  
		Last Modified: Tue, 12 Jul 2022 11:39:25 GMT  
		Size: 41.9 MB (41855990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83bf32a4637cf73112110265a8c664228d574c1f3154e058d05b4028a9d4c9ca`  
		Last Modified: Tue, 12 Jul 2022 11:39:18 GMT  
		Size: 9.8 KB (9793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab00c841a636cfd3628d496347c52b21ee7fca39840cabba1632b4546a6a566`  
		Last Modified: Tue, 12 Jul 2022 11:39:18 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436f4fa1a6578f5859bdc1fe369087835f73fa6f736d8db4f786af9a3e190e7b`  
		Last Modified: Tue, 12 Jul 2022 11:39:18 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d27043ad649a1f61e0adae6942d153e655ae724836c56c39dc755c15e66b45`  
		Last Modified: Tue, 12 Jul 2022 11:39:18 GMT  
		Size: 4.7 KB (4701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
