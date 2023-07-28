## `postgres:14-bookworm`

```console
$ docker pull postgres@sha256:b89109ace3f5934a6d5f2f9bf7802ac02acd6b14ed49aa9e5e27939a97079ae2
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

### `postgres:14-bookworm` - linux; amd64

```console
$ docker pull postgres@sha256:55247e19106a3998b54d8f06d0c5070285a7f47b20f34a56c23ed9a75573d0e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.9 MB (147943400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8209c0eb96e53e0d28d9f32b432b8a49e080deff352427a1833e49177386291e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:44 GMT
ADD file:209589a8bdb5a3788ee42ecdbccbbb561835dab96b0d8286bb5a2229d2f41be7 in / 
# Thu, 27 Jul 2023 23:24:45 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 10:45:38 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 28 Jul 2023 10:45:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 10:45:45 GMT
ENV GOSU_VERSION=1.16
# Fri, 28 Jul 2023 10:45:54 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 28 Jul 2023 10:46:00 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Fri, 28 Jul 2023 10:46:00 GMT
ENV LANG=en_US.utf8
# Fri, 28 Jul 2023 10:46:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 10:46:04 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 28 Jul 2023 10:46:06 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 28 Jul 2023 10:48:37 GMT
ENV PG_MAJOR=14
# Fri, 28 Jul 2023 10:48:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Fri, 28 Jul 2023 10:48:37 GMT
ENV PG_VERSION=14.8-1.pgdg120+1
# Fri, 28 Jul 2023 10:48:55 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 28 Jul 2023 10:48:56 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 28 Jul 2023 10:48:57 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 28 Jul 2023 10:48:57 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 28 Jul 2023 10:48:57 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 28 Jul 2023 10:48:57 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 28 Jul 2023 10:48:57 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Fri, 28 Jul 2023 10:48:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 10:48:58 GMT
STOPSIGNAL SIGINT
# Fri, 28 Jul 2023 10:48:58 GMT
EXPOSE 5432
# Fri, 28 Jul 2023 10:48:58 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:648e0aadf75ac2ef63c5390adc6dc14fde37a5ad88c2870ea604df0a9c0eb4e5`  
		Last Modified: Thu, 27 Jul 2023 23:29:26 GMT  
		Size: 29.1 MB (29124532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f715c8c55756faa0bec5b1ce8aa2bb0432a7cd55c6e86f34d05bfe9c5ba9c005`  
		Last Modified: Fri, 28 Jul 2023 10:52:48 GMT  
		Size: 1.2 KB (1214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11a1dc32c8c291374285b4cd4e5f48cd5e4c958edddf9056a74f177970d9c73`  
		Last Modified: Fri, 28 Jul 2023 10:52:49 GMT  
		Size: 4.6 MB (4618719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e8ba9d17cfa147141648b72ff8ab49a86234dfe1194f6220690939f1daa3c`  
		Last Modified: Fri, 28 Jul 2023 10:52:48 GMT  
		Size: 1.4 MB (1444793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78af88a8afb04f31eae4b90dffac0fbb975596ef328a0d70e9a184401866bd56`  
		Last Modified: Fri, 28 Jul 2023 10:52:47 GMT  
		Size: 8.1 MB (8065048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74279c188d99e2dbb5ead108ad72c4f7221404333671d2a046446086d57703b`  
		Last Modified: Fri, 28 Jul 2023 10:52:46 GMT  
		Size: 1.4 MB (1405683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e3e5bf64fd22db1cf2de5cbb55932e2fb2445d18fe0d9d36356f96fd5262cbe`  
		Last Modified: Fri, 28 Jul 2023 10:52:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62a2c2d2ce5d3525282c6f7413a4857734214371c44afea48678cfb3df844e9`  
		Last Modified: Fri, 28 Jul 2023 10:52:46 GMT  
		Size: 3.2 KB (3196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765629a1b92ddd20465d26c1a8716255e0965b59b1108b0653cc9ef7bbf0a133`  
		Last Modified: Fri, 28 Jul 2023 10:54:35 GMT  
		Size: 103.3 MB (103265415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365d9a2458821e97dc8eeeda7817f7d69a9db34c74f832ca160207d1154f2a76`  
		Last Modified: Fri, 28 Jul 2023 10:54:22 GMT  
		Size: 9.5 KB (9531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb308034f5ef2d446db04d2ad8c65df6466fb379b28f00f162227bc6b1c6e70`  
		Last Modified: Fri, 28 Jul 2023 10:54:22 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddb205754449881497eb013787fce990d25e83e51749522cb325b02824d6cf4d`  
		Last Modified: Fri, 28 Jul 2023 10:54:22 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d403994c183315001dda26644a93c67c62577837c7957565297bcf3d51fcceb1`  
		Last Modified: Fri, 28 Jul 2023 10:54:22 GMT  
		Size: 4.8 KB (4788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-bookworm` - linux; arm variant v5

```console
$ docker pull postgres@sha256:d50c84766026d834995ba19d19a02a77f456cc96e17665f3a1ee3354e0576779
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.9 MB (140933986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d7db24fdbde4b67673ccef257fe4b86a071e73e9182348d9abb306f48d6d665`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 27 Jul 2023 23:48:29 GMT
ADD file:53cf36eb7b72a7e970f4b18af1589402b2900f12e30820cdeccc8bb0c166df80 in / 
# Thu, 27 Jul 2023 23:48:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:15:06 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 28 Jul 2023 01:15:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:15:26 GMT
ENV GOSU_VERSION=1.16
# Fri, 28 Jul 2023 01:15:47 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 28 Jul 2023 01:15:58 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Fri, 28 Jul 2023 01:15:58 GMT
ENV LANG=en_US.utf8
# Fri, 28 Jul 2023 01:16:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:16:08 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 28 Jul 2023 01:16:09 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 28 Jul 2023 02:16:37 GMT
ENV PG_MAJOR=14
# Fri, 28 Jul 2023 02:16:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Fri, 28 Jul 2023 02:16:37 GMT
ENV PG_VERSION=14.8-1.pgdg120+1
# Fri, 28 Jul 2023 02:31:06 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 28 Jul 2023 02:31:08 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 28 Jul 2023 02:31:08 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 28 Jul 2023 02:31:08 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 28 Jul 2023 02:31:09 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 28 Jul 2023 02:31:09 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 28 Jul 2023 02:31:09 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Fri, 28 Jul 2023 02:31:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 02:31:09 GMT
STOPSIGNAL SIGINT
# Fri, 28 Jul 2023 02:31:09 GMT
EXPOSE 5432
# Fri, 28 Jul 2023 02:31:09 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:2bd6dfc5281e13a0ca9fb8d9238ac9f14a0de04489913030c8e33b9398b4a4af`  
		Last Modified: Thu, 27 Jul 2023 23:51:28 GMT  
		Size: 27.0 MB (26983508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6950a2bb05c719b562ca3180236d5f0a283b12217fed11cb89218a0d022b62`  
		Last Modified: Fri, 28 Jul 2023 04:03:32 GMT  
		Size: 1.2 KB (1214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c99c1cf0f513bc89dbb127bb91a117945dcd6faab4b048b4abe027e3b62854`  
		Last Modified: Fri, 28 Jul 2023 04:03:32 GMT  
		Size: 4.2 MB (4236816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87280ebc13a247127dfe2cc0df5089ed6b63fd56dd4593eb0ad833ecc7a1f6da`  
		Last Modified: Fri, 28 Jul 2023 04:03:32 GMT  
		Size: 1.4 MB (1422447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f086c85b55d78a462078e5a8b150a82e2f3670c8e09db66313ca139f9f10c411`  
		Last Modified: Fri, 28 Jul 2023 04:03:32 GMT  
		Size: 8.1 MB (8065176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e01c7b334335bd582e3bd9f395b3633965d6c1c09d9cae72dedb9c08465b4ea`  
		Last Modified: Fri, 28 Jul 2023 04:03:30 GMT  
		Size: 1.4 MB (1404143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1c755771bd4b871db1627d4da382dd5166e19791e2d825feb74eb69a2d5aad`  
		Last Modified: Fri, 28 Jul 2023 04:03:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb41b0dd67db99200fbbdec607bcfe73c16bd0c24706813608de12c67edf862c`  
		Last Modified: Fri, 28 Jul 2023 04:03:29 GMT  
		Size: 3.2 KB (3202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5618583b535a0bf439137213968aedd7c065ddd463ed7e36efbadf7ba48800e4`  
		Last Modified: Fri, 28 Jul 2023 04:05:39 GMT  
		Size: 98.8 MB (98802675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c2c2cee45836d8b854a03bd2ac5bd065a7c2c61fc83b91da7fe84e280fbf6d9`  
		Last Modified: Fri, 28 Jul 2023 04:05:22 GMT  
		Size: 9.5 KB (9538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d890ec937df92a8b212ce9a558cde561c11a0be6e329723539b03aafcb6f96`  
		Last Modified: Fri, 28 Jul 2023 04:05:23 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61acad469a2a9cf9b2d4529fc4800ef265a2df833a6fe34dd766adae0496ecc2`  
		Last Modified: Fri, 28 Jul 2023 04:05:22 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3381d987a9a78fa18ebd067edaba2ade67cc01c32af89a36e74918eea213d68b`  
		Last Modified: Fri, 28 Jul 2023 04:05:22 GMT  
		Size: 4.8 KB (4787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-bookworm` - linux; arm variant v7

```console
$ docker pull postgres@sha256:019456e0b38c9bf21eddadada2132764f9116afc3081458823b8191318df1485
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.8 MB (135810845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab6c57efe880485054595f22a383f8d481eda498040f322ea843fc21dfcc5e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 04 Jul 2023 00:57:54 GMT
ADD file:d168d1710cbca4edb322c26348dafaf2b3a64980f52b8b790f334cdbd6a7047e in / 
# Tue, 04 Jul 2023 00:57:55 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:46:28 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 04 Jul 2023 01:46:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 01:46:39 GMT
ENV GOSU_VERSION=1.16
# Tue, 04 Jul 2023 01:46:48 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 01:46:54 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 04 Jul 2023 01:46:54 GMT
ENV LANG=en_US.utf8
# Tue, 04 Jul 2023 01:46:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 01:46:59 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 01:47:00 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 04 Jul 2023 02:50:49 GMT
ENV PG_MAJOR=14
# Tue, 04 Jul 2023 02:50:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Tue, 04 Jul 2023 02:50:49 GMT
ENV PG_VERSION=14.8-1.pgdg120+1
# Tue, 04 Jul 2023 03:04:41 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 04 Jul 2023 03:04:42 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 04 Jul 2023 03:04:43 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 04 Jul 2023 03:04:43 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 04 Jul 2023 03:04:44 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 04 Jul 2023 03:04:44 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 04 Jul 2023 03:04:44 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Tue, 04 Jul 2023 03:04:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 03:04:44 GMT
STOPSIGNAL SIGINT
# Tue, 04 Jul 2023 03:04:44 GMT
EXPOSE 5432
# Tue, 04 Jul 2023 03:04:44 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:340ace0baa422f18db718d7634c1c88a9650f4871dda2630ef15577120aa6816`  
		Last Modified: Tue, 04 Jul 2023 01:02:50 GMT  
		Size: 24.8 MB (24801264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30bf1169413903f011722804d0aa32f2ff77bc975517bb5037ccec5a4acc3ded`  
		Last Modified: Tue, 04 Jul 2023 04:33:28 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a737009bf990aff94219f6eb74883512379c6b53284af3d5f02928e297fffbd`  
		Last Modified: Tue, 04 Jul 2023 04:33:28 GMT  
		Size: 3.8 MB (3839459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c94d04093aa7424ae7d299175451e55983929ee5232c7f1176e200fb1b512ba`  
		Last Modified: Tue, 04 Jul 2023 04:33:28 GMT  
		Size: 1.4 MB (1411903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c5b708892f996f33049dd2bcfe2723671c0ceec3d268131d46a7c42789f847`  
		Last Modified: Tue, 04 Jul 2023 04:33:27 GMT  
		Size: 8.1 MB (8065057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4274fbe730308a909f8c492f8a5f4a65e662dab613848d65ec8896e5b707d10a`  
		Last Modified: Tue, 04 Jul 2023 04:33:25 GMT  
		Size: 1.3 MB (1277609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4819b71c63c9711a1ba1707229574e6b382df766e924b6e22ac26c0ab210469b`  
		Last Modified: Tue, 04 Jul 2023 04:33:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf322bf97eee11e7ccaadbf34c333604acce40558b4eb5c2d402a104b7ef59a`  
		Last Modified: Tue, 04 Jul 2023 04:33:25 GMT  
		Size: 3.2 KB (3193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df1964ffac8d918eb559b0d08d45c2e6b028f2795752b5733ea7687559f237b`  
		Last Modified: Tue, 04 Jul 2023 04:36:04 GMT  
		Size: 96.4 MB (96396366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4877cb8d451106c0dda6f3fb1e009fddf683ab0ad4d47bb7cdc6aff94a173ec`  
		Last Modified: Tue, 04 Jul 2023 04:35:49 GMT  
		Size: 9.5 KB (9526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf591d7fdd50d18cb402627662fd7107f9bec11837e0dfb35c0d4bb30716bbf`  
		Last Modified: Tue, 04 Jul 2023 04:35:49 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b91292aa59a360437d3a844125d596ee0ac1811629041628c8cb77471a3b439`  
		Last Modified: Tue, 04 Jul 2023 04:35:49 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e557f3ff6a5112a198de1f50f0b90429e33c87398ee28a9fa930303de9f608f`  
		Last Modified: Tue, 04 Jul 2023 04:35:49 GMT  
		Size: 4.8 KB (4784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-bookworm` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:1050153f46ad3fa89c27f3002e6ebf15fef0ceedf1d21f49a982e1364a6c2e3d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.9 MB (145871744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07336019987162ade7661828bcd57fbeb37adea6f106c9c22aecbb434eb36326`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:00 GMT
ADD file:1de2ba0dc88aa343332814e19adc6b850d08e62c31589fe902b8eb2cb465934e in / 
# Thu, 27 Jul 2023 23:43:00 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 06:27:53 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 28 Jul 2023 06:27:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 06:27:58 GMT
ENV GOSU_VERSION=1.16
# Fri, 28 Jul 2023 06:28:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 28 Jul 2023 06:28:11 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Fri, 28 Jul 2023 06:28:11 GMT
ENV LANG=en_US.utf8
# Fri, 28 Jul 2023 06:28:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 06:28:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 28 Jul 2023 06:28:16 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 28 Jul 2023 06:30:31 GMT
ENV PG_MAJOR=14
# Fri, 28 Jul 2023 06:30:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Fri, 28 Jul 2023 06:30:31 GMT
ENV PG_VERSION=14.8-1.pgdg120+1
# Fri, 28 Jul 2023 06:30:47 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 28 Jul 2023 06:30:49 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 28 Jul 2023 06:30:49 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 28 Jul 2023 06:30:49 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 28 Jul 2023 06:30:50 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 28 Jul 2023 06:30:50 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 28 Jul 2023 06:30:50 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Fri, 28 Jul 2023 06:30:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 06:30:50 GMT
STOPSIGNAL SIGINT
# Fri, 28 Jul 2023 06:30:50 GMT
EXPOSE 5432
# Fri, 28 Jul 2023 06:30:50 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:90524f7dc01b4ce9b387992acc6cbdbcc2a9ee8c6addfd632429ca06ea18751e`  
		Last Modified: Thu, 27 Jul 2023 23:46:17 GMT  
		Size: 29.2 MB (29157226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7240014a472438ad2cc69dbf1875ba58bb60de7e1628eb80856e59fe105439`  
		Last Modified: Fri, 28 Jul 2023 06:34:30 GMT  
		Size: 1.2 KB (1215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d2c856d78465db6762de3837a65afac229998326f631762a65ff15e71c17f9`  
		Last Modified: Fri, 28 Jul 2023 06:34:31 GMT  
		Size: 4.6 MB (4578225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:885c9ba4e584d12b1ba2d08b155e7a8cbc11fa0745a8579a2fab36ef07487d06`  
		Last Modified: Fri, 28 Jul 2023 06:34:30 GMT  
		Size: 1.4 MB (1376534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f003c5d3c778ab5990731175017d97e7a66d616dd51f6c224402637f47c9b3c`  
		Last Modified: Fri, 28 Jul 2023 06:34:29 GMT  
		Size: 8.1 MB (8065106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c86f7fa28743824f47cbfb3790e55abdcf38cfb035a8f5a116b3cc6c622c6cc`  
		Last Modified: Fri, 28 Jul 2023 06:34:28 GMT  
		Size: 1.3 MB (1317878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa86bc459ff8dfccb17d57fe1a383d843160b21c22684d452a7a6772bec6637d`  
		Last Modified: Fri, 28 Jul 2023 06:34:28 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd6da0c1c546a31bcb5b5b4814d6f8a57f2bc49b570f948fb352cfaa7dca682`  
		Last Modified: Fri, 28 Jul 2023 06:34:28 GMT  
		Size: 3.2 KB (3199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3601f2fb8f0dc84bb73f246aadb2e06b1ce738fefb1e104ce47061b1f40c89c2`  
		Last Modified: Fri, 28 Jul 2023 06:36:10 GMT  
		Size: 101.4 MB (101357563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a637ba48b5cae1ed8f4b3b0289244236efbf69f973d629a9da80f99af55f4dd`  
		Last Modified: Fri, 28 Jul 2023 06:35:59 GMT  
		Size: 9.5 KB (9531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64154edb9a936722288c347f0b160cd7aa18bab41cbeea52940fa9a4136b59d2`  
		Last Modified: Fri, 28 Jul 2023 06:35:59 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:190658377d5f0023802847b199d26f2b7c0ae39df9fe01af05a46c4d6fb56431`  
		Last Modified: Fri, 28 Jul 2023 06:35:59 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7bd2bf25c0ea84e34e28f49904ae2c211591d0fd916fc16055cfc67c5033ad`  
		Last Modified: Fri, 28 Jul 2023 06:35:59 GMT  
		Size: 4.8 KB (4789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-bookworm` - linux; 386

```console
$ docker pull postgres@sha256:d4eb1d4106de0024eee03ed2bd2d248f447603be549c1eca243df6ccd6b4f161
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155052087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c495c21bc1c975f70bef6fcc163485f39b06b84a24e95e9741aada6740a4995`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 27 Jul 2023 23:38:56 GMT
ADD file:3d6e6f3e900e480a7e060fcaf57313c0f954bf906967a7fa0317567c387cf5aa in / 
# Thu, 27 Jul 2023 23:38:57 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 09:53:03 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 28 Jul 2023 09:53:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 09:53:10 GMT
ENV GOSU_VERSION=1.16
# Fri, 28 Jul 2023 09:53:21 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 28 Jul 2023 09:53:28 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Fri, 28 Jul 2023 09:53:28 GMT
ENV LANG=en_US.utf8
# Fri, 28 Jul 2023 09:53:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 09:53:34 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 28 Jul 2023 09:53:35 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 28 Jul 2023 10:55:28 GMT
ENV PG_MAJOR=14
# Fri, 28 Jul 2023 10:55:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Fri, 28 Jul 2023 10:55:28 GMT
ENV PG_VERSION=14.8-1.pgdg120+1
# Fri, 28 Jul 2023 11:10:18 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 28 Jul 2023 11:10:20 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 28 Jul 2023 11:10:21 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 28 Jul 2023 11:10:21 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 28 Jul 2023 11:10:21 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 28 Jul 2023 11:10:21 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 28 Jul 2023 11:10:22 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Fri, 28 Jul 2023 11:10:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 11:10:22 GMT
STOPSIGNAL SIGINT
# Fri, 28 Jul 2023 11:10:22 GMT
EXPOSE 5432
# Fri, 28 Jul 2023 11:10:22 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:3a8b0c4b1a83609d978d576be6174f951ff27084d7c9aef91892b60b223a5104`  
		Last Modified: Thu, 27 Jul 2023 23:43:26 GMT  
		Size: 30.1 MB (30141788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096d4d1f1233ed790606e4fb1ee8341e03f400beb2d65ff9ee52c6f6c88b60ea`  
		Last Modified: Fri, 28 Jul 2023 12:46:14 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f6edbf97a1cf6888c4f00b80e49070ce4725078a3ff4bd7e870932b6058e88`  
		Last Modified: Fri, 28 Jul 2023 12:46:15 GMT  
		Size: 5.0 MB (5039474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904c905d637603ae1d7400e0bf5ef5c89b4ed57d303f50b6dcc45267f2d5ce03`  
		Last Modified: Fri, 28 Jul 2023 12:46:14 GMT  
		Size: 1.4 MB (1420351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:051ce4fec4fae3d465939a504293fa27d40a67eaa8992abb8370a5a1b1532435`  
		Last Modified: Fri, 28 Jul 2023 12:46:14 GMT  
		Size: 8.1 MB (8065046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61e3edfb73ae61999aaf26c4e608527f4cc0b6ad53c49f8cdea8604b247f990`  
		Last Modified: Fri, 28 Jul 2023 12:46:12 GMT  
		Size: 1.3 MB (1346493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03009c6a383d7b218ffe5a1b195ac9be43892444635636786325668b5b73ee8a`  
		Last Modified: Fri, 28 Jul 2023 12:46:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab1cd45a3ae848f8ce13e20c8e3e1f61642e6869861d1c26fbc6591d52f9c82`  
		Last Modified: Fri, 28 Jul 2023 12:46:11 GMT  
		Size: 3.2 KB (3196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a31c79cfacdb49b2d099f9149dee862ba5afc808f1216c93fa1eaa03c2e334`  
		Last Modified: Fri, 28 Jul 2023 12:48:39 GMT  
		Size: 109.0 MB (109019719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dd8716972eafcfe870ebaf8a60eb713c7c55ac92464f9caa3378c20a86ba39`  
		Last Modified: Fri, 28 Jul 2023 12:48:19 GMT  
		Size: 9.5 KB (9538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d29e9c742b7879b5c8c52ae24aef1c1fbfc79d05c1b7bd74be20e47c041b4d9`  
		Last Modified: Fri, 28 Jul 2023 12:48:19 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a5436d028bd6fa7f826483e074ced6fe3f7ce4f577fdd36331118542375da8`  
		Last Modified: Fri, 28 Jul 2023 12:48:19 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08d48a1e7ee5227b50994f9e8cd4a4037e03c46c05a41d738585945d7d9ad12`  
		Last Modified: Fri, 28 Jul 2023 12:48:19 GMT  
		Size: 4.8 KB (4789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-bookworm` - linux; mips64le

```console
$ docker pull postgres@sha256:630fc68c54e28de5a23a4f2ed4e5bd35b5f931f6d9bbc149418f366934bdb3e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.7 MB (143676463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6e164de7a434e61f19402e12d2cb0ad4ad246a28099ccf5f3922839f3cf7dee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 04 Jul 2023 01:09:28 GMT
ADD file:cf4b72a35644a7b9f5f1ca39a54e484822f408f6821f0800f1167ae48ad6e38e in / 
# Tue, 04 Jul 2023 01:09:32 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:54:47 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 04 Jul 2023 01:55:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 01:55:27 GMT
ENV GOSU_VERSION=1.16
# Tue, 04 Jul 2023 01:56:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 04 Jul 2023 01:56:30 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 04 Jul 2023 01:56:33 GMT
ENV LANG=en_US.utf8
# Tue, 04 Jul 2023 01:56:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 01:56:56 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 04 Jul 2023 01:57:02 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 04 Jul 2023 06:15:21 GMT
ENV PG_MAJOR=14
# Tue, 04 Jul 2023 06:15:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Tue, 04 Jul 2023 06:15:26 GMT
ENV PG_VERSION=14.8-1.pgdg120+1
# Tue, 04 Jul 2023 07:17:23 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 04 Jul 2023 07:17:29 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 04 Jul 2023 07:17:35 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 04 Jul 2023 07:17:38 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 04 Jul 2023 07:17:44 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 04 Jul 2023 07:17:47 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 04 Jul 2023 07:17:50 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Tue, 04 Jul 2023 07:17:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jul 2023 07:17:57 GMT
STOPSIGNAL SIGINT
# Tue, 04 Jul 2023 07:18:00 GMT
EXPOSE 5432
# Tue, 04 Jul 2023 07:18:04 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:502a81d5004983c2a770a910286271410d8e2b20d0cb61ef7397e664e1e72654`  
		Last Modified: Tue, 04 Jul 2023 01:19:57 GMT  
		Size: 29.1 MB (29118201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4214fd0953e1de08d6b701710ddf147eb769c7c0bdc0b39e4fe957e17cc01f6`  
		Last Modified: Tue, 04 Jul 2023 14:00:12 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16472607cea5fa601c76d37cc263c4422257547672cad6477b7d8aaf96547afa`  
		Last Modified: Tue, 04 Jul 2023 14:00:15 GMT  
		Size: 4.4 MB (4355644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4350b9f4a7a844be6f01f23d6e874c3604151a855a873617de49cca982fdf895`  
		Last Modified: Tue, 04 Jul 2023 14:00:12 GMT  
		Size: 1.3 MB (1331408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea06d6188b5ca703692f4157c8957f67fb133b5d0463516cfc6bf50a107850d6`  
		Last Modified: Tue, 04 Jul 2023 14:00:16 GMT  
		Size: 8.1 MB (8064810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbca4ca0657f22bf5578ea6f2d715c2e1467839d06baddff04fff2c8e6e028d7`  
		Last Modified: Tue, 04 Jul 2023 14:00:09 GMT  
		Size: 1.2 MB (1181482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bb6198f5f88dc20164c340b50c3de273d0f14985d4a2fdd77bdb0ba363653a`  
		Last Modified: Tue, 04 Jul 2023 14:00:09 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf39e09515527257eda211039e55ad5ac0e26aba158cabb7c6f0719426710f4`  
		Last Modified: Tue, 04 Jul 2023 14:00:08 GMT  
		Size: 3.1 KB (3137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef1120cbe4a3e1ec49c8710c99650206be044cf4928079628e21c5b25983ca0`  
		Last Modified: Tue, 04 Jul 2023 14:06:13 GMT  
		Size: 99.6 MB (99605923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d9f6ea0325730304dcd80e220363bac72e9bfa95db639cba227a8d1c4f4dc4`  
		Last Modified: Tue, 04 Jul 2023 14:05:10 GMT  
		Size: 9.5 KB (9527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e6ec69074edc46547e813cc632e39aee52fd6cb2e0368f52dfe11cebc74bef`  
		Last Modified: Tue, 04 Jul 2023 14:05:10 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c40b506283c19f8303ddda2d8670c2b8a0170612d8a0756f7b9fd715e1e2b708`  
		Last Modified: Tue, 04 Jul 2023 14:05:10 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62eded965b5dab37a9aba2abe692726031795b477fd414f7a90e47aa5f46b6c4`  
		Last Modified: Tue, 04 Jul 2023 14:05:10 GMT  
		Size: 4.8 KB (4786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-bookworm` - linux; ppc64le

```console
$ docker pull postgres@sha256:3a78bd69927a7f60b963e264ac834b1746d6d00822fa04086d470c867f7488db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.7 MB (159661319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:441940e66fa0074baaefa0f5f22e2ad6a905c23bacc0a983cbdd2354935ef61e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 27 Jul 2023 23:23:01 GMT
ADD file:774a99e5c40757d27c981eb5ad6e03eb72970bb0c54f799eab1442624238ea3e in / 
# Thu, 27 Jul 2023 23:23:03 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 04:15:52 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 28 Jul 2023 04:16:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 04:16:13 GMT
ENV GOSU_VERSION=1.16
# Fri, 28 Jul 2023 04:16:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 28 Jul 2023 04:16:53 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Fri, 28 Jul 2023 04:16:55 GMT
ENV LANG=en_US.utf8
# Fri, 28 Jul 2023 04:17:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 04:17:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 28 Jul 2023 04:17:09 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 28 Jul 2023 04:23:51 GMT
ENV PG_MAJOR=14
# Fri, 28 Jul 2023 04:23:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Fri, 28 Jul 2023 04:23:52 GMT
ENV PG_VERSION=14.8-1.pgdg120+1
# Fri, 28 Jul 2023 04:24:53 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 28 Jul 2023 04:25:00 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 28 Jul 2023 04:25:03 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 28 Jul 2023 04:25:04 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 28 Jul 2023 04:25:06 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 28 Jul 2023 04:25:06 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 28 Jul 2023 04:25:07 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Fri, 28 Jul 2023 04:25:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 04:25:08 GMT
STOPSIGNAL SIGINT
# Fri, 28 Jul 2023 04:25:09 GMT
EXPOSE 5432
# Fri, 28 Jul 2023 04:25:10 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:ad974e0ada84177d519dec70d0d7d9ff6a4f468bc7306425feb8429bc276bd8a`  
		Last Modified: Thu, 27 Jul 2023 23:29:24 GMT  
		Size: 33.1 MB (33119211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83fbde5c945e871360e8cb398fd1db475b6634bd1200164834524029a407032b`  
		Last Modified: Fri, 28 Jul 2023 04:36:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0511a8f404d7e17f9ba13ce967de818440ab80e85a880c0cd063b31eecf73986`  
		Last Modified: Fri, 28 Jul 2023 04:36:48 GMT  
		Size: 5.4 MB (5433699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6056b4d51ca10cb9d049abcd2399ec0e1863f1cc3cde44fb05af52194b4c21`  
		Last Modified: Fri, 28 Jul 2023 04:36:47 GMT  
		Size: 1.4 MB (1367280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9b886e865159b9b47ba204855c72293cb57869ec9175ebbb512b213566a486`  
		Last Modified: Fri, 28 Jul 2023 04:36:47 GMT  
		Size: 8.1 MB (8065165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e34d347cb25c3beba9102be490110151bc9be20968019d1e015e8156646ee1`  
		Last Modified: Fri, 28 Jul 2023 04:36:45 GMT  
		Size: 1.5 MB (1494547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08cd635a2f7a12ed97921ee20fd306861e74f3b252484e64c7c3e7037cb41f55`  
		Last Modified: Fri, 28 Jul 2023 04:36:44 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca51d30a7065d38900cd63f5d7352fc9c3019ec7a3009eb40fda58563ebf470`  
		Last Modified: Fri, 28 Jul 2023 04:36:44 GMT  
		Size: 3.2 KB (3199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05ad29054c313e01e90ab852d9ff8c5496bbca4bd5cf5687a893811885f5f`  
		Last Modified: Fri, 28 Jul 2023 04:40:04 GMT  
		Size: 110.2 MB (110162201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ba737624449ccf556674fc1d16df492b5ce01989100cf964c7e1e0e8645bad`  
		Last Modified: Fri, 28 Jul 2023 04:39:38 GMT  
		Size: 9.5 KB (9533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fc87c5931105e2d5ec72524a9f768a0c878b184c5d926d0deeec3027fdc76e`  
		Last Modified: Fri, 28 Jul 2023 04:39:38 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c5067cff4599e4085d37e7358b85a8de822f96c7ef8828cd585a233c2cad70`  
		Last Modified: Fri, 28 Jul 2023 04:39:38 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e31375b2b037c5dd7f7b71c9fcb745b3c3525ef68f2720eae52f4dece7f1062`  
		Last Modified: Fri, 28 Jul 2023 04:39:38 GMT  
		Size: 4.8 KB (4790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:14-bookworm` - linux; s390x

```console
$ docker pull postgres@sha256:5af81ae1ab30a4c9a4cdca2416c56327e0a44f12af04e510a484c57fe5a79cf6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.2 MB (153224254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:989f308ead2ad584c97a940c9f142a3441dd1b21b383d9a465ab92adea775fea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 27 Jul 2023 23:47:11 GMT
ADD file:0a5e1e86b375d60637d0829f77a12085777cf2ca07495b0f6249d8efea84e958 in / 
# Thu, 27 Jul 2023 23:47:13 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 09:36:30 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Fri, 28 Jul 2023 09:36:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 09:36:35 GMT
ENV GOSU_VERSION=1.16
# Fri, 28 Jul 2023 09:36:41 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 28 Jul 2023 09:36:47 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Fri, 28 Jul 2023 09:36:48 GMT
ENV LANG=en_US.utf8
# Fri, 28 Jul 2023 09:36:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 09:36:52 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Fri, 28 Jul 2023 09:36:53 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Fri, 28 Jul 2023 09:39:49 GMT
ENV PG_MAJOR=14
# Fri, 28 Jul 2023 09:39:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/14/bin
# Fri, 28 Jul 2023 09:39:50 GMT
ENV PG_VERSION=14.8-1.pgdg120+1
# Fri, 28 Jul 2023 09:40:10 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 28 Jul 2023 09:40:15 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 28 Jul 2023 09:40:15 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 28 Jul 2023 09:40:15 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 28 Jul 2023 09:40:16 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 28 Jul 2023 09:40:16 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 28 Jul 2023 09:40:16 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Fri, 28 Jul 2023 09:40:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 09:40:16 GMT
STOPSIGNAL SIGINT
# Fri, 28 Jul 2023 09:40:16 GMT
EXPOSE 5432
# Fri, 28 Jul 2023 09:40:16 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f4301d25bb1bea85fcc5b364aec84ff58274f714cea191ab22d9b1b1e4f78527`  
		Last Modified: Thu, 27 Jul 2023 23:52:17 GMT  
		Size: 27.5 MB (27489697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b5780f07b300ba585e3cb596361f2bb24f923e72af1521d9258bff53e93054`  
		Last Modified: Fri, 28 Jul 2023 09:46:01 GMT  
		Size: 1.2 KB (1215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:619389542bf4d20923b62d5f47ce106d5fa370188b9ad4d0d3e6402685b177c5`  
		Last Modified: Fri, 28 Jul 2023 09:46:01 GMT  
		Size: 4.5 MB (4474571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26a9633ba1507903ade8b0913ad572656bf9a6fb287a4ebb0794297e801f986`  
		Last Modified: Fri, 28 Jul 2023 09:46:00 GMT  
		Size: 1.4 MB (1410631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39aeba3023f1deb04a422096e9e4081fbbf757791f088152ae4b614a8d3eb0f2`  
		Last Modified: Fri, 28 Jul 2023 09:46:00 GMT  
		Size: 8.1 MB (8119472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c16cfd2d3de496036054d4ab8b22816861c1f331238159c80925f0ea701f4e0`  
		Last Modified: Fri, 28 Jul 2023 09:45:59 GMT  
		Size: 1.3 MB (1307745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4088675631b4487d166ffa50d5f6a22325f4cb859888e26b13657f265aa00cfa`  
		Last Modified: Fri, 28 Jul 2023 09:45:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205d44667d955ac4d1e54914316deebb9e815440de6b03013f926f6042457d7f`  
		Last Modified: Fri, 28 Jul 2023 09:45:59 GMT  
		Size: 3.2 KB (3201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179805b93372ad2f1cc2000dadf0d928e0b052f3d304f91d187c3d42e8ac4a89`  
		Last Modified: Fri, 28 Jul 2023 09:47:37 GMT  
		Size: 110.4 MB (110402921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210746c326235a366902bed90f9eeb7cffa23df3ad658179f6c198d83b31a6fa`  
		Last Modified: Fri, 28 Jul 2023 09:47:22 GMT  
		Size: 9.5 KB (9535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e95056c0c020c725a2473e647b5e87fa35a1abdd5227cd569f35f7a53a896bee`  
		Last Modified: Fri, 28 Jul 2023 09:47:23 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f02d22f4708a695a541a045d0e226fae3c37536d2335e48b6e9627c9e4a040`  
		Last Modified: Fri, 28 Jul 2023 09:47:22 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f0e4bf1f1b8fbaa40ae017db4bdd5bb1da091f85dbae0df8f88b53b831a8c9`  
		Last Modified: Fri, 28 Jul 2023 09:47:22 GMT  
		Size: 4.8 KB (4786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
