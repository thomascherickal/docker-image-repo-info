## `postgres:12-bullseye`

```console
$ docker pull postgres@sha256:c8f4c67b6c078dfa5d1f9a492c37ef367883a4685f75939856bd78fb045f39c4
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

### `postgres:12-bullseye` - linux; amd64

```console
$ docker pull postgres@sha256:d19898e76dea6f3bd0b79fdf95b4b83317d7dba81012616b46524cec801e3fc4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.2 MB (135248368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58bff76313464ab65dcb0b9a2b910c815e8975d827c456ca7f46d69482956d5e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:43 GMT
ADD file:09675d11695f65c55efdc393ff0cd32f30194cd7d0fbef4631eebfed4414ac97 in / 
# Tue, 21 Dec 2021 01:22:43 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 23:31:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 23:31:33 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 21 Dec 2021 23:31:34 GMT
ENV GOSU_VERSION=1.14
# Tue, 21 Dec 2021 23:31:57 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 21 Dec 2021 23:32:11 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 21 Dec 2021 23:32:11 GMT
ENV LANG=en_US.utf8
# Tue, 21 Dec 2021 23:32:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 23:32:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 21 Dec 2021 23:32:29 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 21 Dec 2021 23:33:50 GMT
ENV PG_MAJOR=12
# Tue, 21 Dec 2021 23:33:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Tue, 21 Dec 2021 23:33:51 GMT
ENV PG_VERSION=12.9-1.pgdg110+1
# Tue, 21 Dec 2021 23:34:11 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 21 Dec 2021 23:34:13 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 21 Dec 2021 23:34:14 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 21 Dec 2021 23:34:14 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 21 Dec 2021 23:34:15 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 21 Dec 2021 23:34:15 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 04 Jan 2022 01:20:13 GMT
COPY file:b2fac085615145a2bee98d4185ef0748655fa7c086ca21daef1ca6cac272bf59 in /usr/local/bin/ 
# Tue, 04 Jan 2022 01:20:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jan 2022 01:20:13 GMT
STOPSIGNAL SIGINT
# Tue, 04 Jan 2022 01:20:13 GMT
EXPOSE 5432
# Tue, 04 Jan 2022 01:20:14 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:a2abf6c4d29d43a4bf9fbb769f524d0fb36a2edab49819c1bf3e76f409f953ea`  
		Last Modified: Tue, 21 Dec 2021 01:27:48 GMT  
		Size: 31.4 MB (31357624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1769f49f9101e08b259481961baceea032c026337b960a2737ba58d84c08d5f`  
		Last Modified: Tue, 21 Dec 2021 23:39:01 GMT  
		Size: 4.4 MB (4414603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a59cfee47cee21e9a3725fc141ad856917e95a1817f3719d5e7bae0c4e9515`  
		Last Modified: Tue, 21 Dec 2021 23:38:59 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461b2090c345e5af01940b13f92bcdbd47ef70bd372fd0a565af08f53c0f1601`  
		Last Modified: Tue, 21 Dec 2021 23:39:00 GMT  
		Size: 1.4 MB (1418382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed8ab6290ac04d65ebec4245056773a6679334d17b77a9a6bf1b7f1e26ad08a`  
		Last Modified: Tue, 21 Dec 2021 23:38:59 GMT  
		Size: 8.0 MB (8045343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495e42c822a03224fc27a04cf05716b82a5f1c4c9252cc7457673be355ab12f2`  
		Last Modified: Tue, 21 Dec 2021 23:38:57 GMT  
		Size: 441.7 KB (441681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e858c71c58fe45a750a830bfab4fe11bbd4618ace209d0ad397e4647d648d2`  
		Last Modified: Tue, 21 Dec 2021 23:38:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594792c80d5fa95924c9f7abe6acec205e5db07fc6bd04c299e3cd48174d1fab`  
		Last Modified: Tue, 21 Dec 2021 23:38:57 GMT  
		Size: 3.1 KB (3057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc21527d805918683cae853deb87d4a30477488ee26c9817c2b50dde4a61e64`  
		Last Modified: Tue, 21 Dec 2021 23:40:25 GMT  
		Size: 89.6 MB (89551651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33105c93a6db5806e4b4b8c07e328ec0def1f019ea372a31b0b01dd48ace997`  
		Last Modified: Tue, 21 Dec 2021 23:40:09 GMT  
		Size: 9.0 KB (9027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d44539f7e125063cb80ba8f9d87c44ac4136c37a02afb9761fb971d670db5d`  
		Last Modified: Tue, 21 Dec 2021 23:40:08 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2237b54399af54c19ca329fb833cf09b6d9de94247c603954daaceae89ba340c`  
		Last Modified: Tue, 21 Dec 2021 23:40:08 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59525896cd85cf79324f5e2c4eea62d389f1e73a9e09fe8b73a3e25da197b9bb`  
		Last Modified: Tue, 04 Jan 2022 01:23:16 GMT  
		Size: 4.7 KB (4716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-bullseye` - linux; arm variant v5

```console
$ docker pull postgres@sha256:d191badd021d1c9f78aef75e74a1d74d5593138ce695eac45d68d80da6fe31c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.5 MB (128540250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2617eae76458b280f7f486d0ca7b6fd2b45c7576f4ca38612b359a6b6146a767`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Dec 2021 01:50:31 GMT
ADD file:a3023f71bd93966e7db1419adda3ccde4fcc5e2e8cf58e7b13c51036ed5ff796 in / 
# Tue, 21 Dec 2021 01:50:32 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:30:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 07:30:43 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 21 Dec 2021 07:30:44 GMT
ENV GOSU_VERSION=1.14
# Tue, 21 Dec 2021 07:31:07 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 21 Dec 2021 07:31:30 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 21 Dec 2021 07:31:31 GMT
ENV LANG=en_US.utf8
# Tue, 21 Dec 2021 07:31:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:31:43 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 21 Dec 2021 07:31:46 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 21 Dec 2021 08:46:53 GMT
ENV PG_MAJOR=12
# Tue, 21 Dec 2021 08:46:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Tue, 21 Dec 2021 08:46:54 GMT
ENV PG_VERSION=12.9-1.pgdg110+1
# Tue, 21 Dec 2021 09:22:17 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 21 Dec 2021 09:22:20 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 21 Dec 2021 09:22:22 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 21 Dec 2021 09:22:22 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 21 Dec 2021 09:22:24 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 21 Dec 2021 09:22:24 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 04 Jan 2022 01:49:23 GMT
COPY file:b2fac085615145a2bee98d4185ef0748655fa7c086ca21daef1ca6cac272bf59 in /usr/local/bin/ 
# Tue, 04 Jan 2022 01:49:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jan 2022 01:49:24 GMT
STOPSIGNAL SIGINT
# Tue, 04 Jan 2022 01:49:25 GMT
EXPOSE 5432
# Tue, 04 Jan 2022 01:49:25 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:054429d0cf4038fef39a3b5eb6ce52f600f9a2cbb71a4fb3e95ecf9b2da62581`  
		Last Modified: Tue, 21 Dec 2021 02:05:52 GMT  
		Size: 28.9 MB (28900253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11c3b8663b33872a4cd51280b3b6213125ffb664af3544f78a8c00861d96529`  
		Last Modified: Tue, 21 Dec 2021 12:06:36 GMT  
		Size: 4.1 MB (4096469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7885af84e3728315efcdad4126b9cf21704918c9bd5b532975c20b15618b6d83`  
		Last Modified: Tue, 21 Dec 2021 12:06:31 GMT  
		Size: 1.8 KB (1798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6966bd647e990282b34e4b0ccdcee10086f054b44ed0b3f0133f098b9967b23b`  
		Last Modified: Tue, 21 Dec 2021 12:06:31 GMT  
		Size: 1.4 MB (1382552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a4a1fd7b75dec70f07b372ad523c88e90a1d337f5a2488b84a134db9bbfe15`  
		Last Modified: Tue, 21 Dec 2021 12:06:35 GMT  
		Size: 8.0 MB (8045155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d0038c65b0aafcf1ea56729903d012a7a37126d4900f4861ca4a16d7573fa8`  
		Last Modified: Tue, 21 Dec 2021 12:06:30 GMT  
		Size: 439.8 KB (439838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359b44a703071420b378dcf42f848c5aa8fdf777498ebfb37c8cbe52f38c64b9`  
		Last Modified: Tue, 21 Dec 2021 12:06:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af723b478cfbdf181802077d97fe3ff370c9c0d1505f26ad33f479f19545e442`  
		Last Modified: Tue, 21 Dec 2021 12:06:29 GMT  
		Size: 3.1 KB (3056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38399ed406b35e3c84c6c1e8e7e757631c40a15e3d977367f7514ab9e9118ae`  
		Last Modified: Tue, 21 Dec 2021 12:10:03 GMT  
		Size: 85.7 MB (85656904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680dba6d0fa007cf27b6d1205dc99e886844992833a6bb27f75b542a5ef89e18`  
		Last Modified: Tue, 21 Dec 2021 12:09:08 GMT  
		Size: 9.0 KB (9030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d46cafed138095bf94c8a9472d59eac13fefb91f6355d1cf3b4d2c0c6530c56e`  
		Last Modified: Tue, 21 Dec 2021 12:09:08 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77a56d81964ef5cf2d54d42d2351fd7adf133981e4ccaead4848cc72c69d238`  
		Last Modified: Tue, 21 Dec 2021 12:09:09 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913e3cd70e0749e2213ec0005e2c03e9f0be5a6e58cb8f48fe0161df128f7d6f`  
		Last Modified: Tue, 04 Jan 2022 01:54:35 GMT  
		Size: 4.7 KB (4717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-bullseye` - linux; arm variant v7

```console
$ docker pull postgres@sha256:6ff9af9e20e0f291fad06cbf040a7909a99e9ce11debf15a433ad2822081b985
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.4 MB (123440748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dab4c0b288feb256a0d59709aebc9cf7bfd028c9a33805e46362454c7b6fabc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Dec 2021 01:59:48 GMT
ADD file:6a5555c3e40db91fae5bb112464a4c405a976de17ff64c98f25d3033a6a608d8 in / 
# Tue, 21 Dec 2021 01:59:48 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 13:34:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 13:34:52 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 21 Dec 2021 13:34:53 GMT
ENV GOSU_VERSION=1.14
# Tue, 21 Dec 2021 13:35:15 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 21 Dec 2021 13:35:35 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 21 Dec 2021 13:35:36 GMT
ENV LANG=en_US.utf8
# Tue, 21 Dec 2021 13:35:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 13:35:46 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 21 Dec 2021 13:35:51 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 21 Dec 2021 14:44:25 GMT
ENV PG_MAJOR=12
# Tue, 21 Dec 2021 14:44:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Tue, 21 Dec 2021 14:44:25 GMT
ENV PG_VERSION=12.9-1.pgdg110+1
# Tue, 21 Dec 2021 15:16:16 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 21 Dec 2021 15:16:19 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 21 Dec 2021 15:16:20 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 21 Dec 2021 15:16:21 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 21 Dec 2021 15:16:23 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 21 Dec 2021 15:16:23 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 04 Jan 2022 00:59:12 GMT
COPY file:b2fac085615145a2bee98d4185ef0748655fa7c086ca21daef1ca6cac272bf59 in /usr/local/bin/ 
# Tue, 04 Jan 2022 00:59:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jan 2022 00:59:13 GMT
STOPSIGNAL SIGINT
# Tue, 04 Jan 2022 00:59:13 GMT
EXPOSE 5432
# Tue, 04 Jan 2022 00:59:14 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:d0061d6703dc4975804c3419e00c85efbe3f1b79c86d87e048fa14a683e88e31`  
		Last Modified: Tue, 21 Dec 2021 02:15:26 GMT  
		Size: 26.6 MB (26560815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63faa60732a43e018f66952afb7f45d04d6d4758ee3d81183a163f9b6f804d2a`  
		Last Modified: Tue, 21 Dec 2021 17:48:01 GMT  
		Size: 3.7 MB (3717142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0323b5281fb94b32757850d02213a35a5f22c233d2c30a49504f89067f72f573`  
		Last Modified: Tue, 21 Dec 2021 17:47:59 GMT  
		Size: 1.8 KB (1794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22b25778e1eb533d3a049204db0bd7f35e725b44748eb5b53d7dbcfb5b3adf6`  
		Last Modified: Tue, 21 Dec 2021 17:48:00 GMT  
		Size: 1.4 MB (1375223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89817e68a18fa0bdfc9458a9b332f5b365056be1f503efa9c21faad188af3e92`  
		Last Modified: Tue, 21 Dec 2021 17:48:03 GMT  
		Size: 8.0 MB (8045328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1d4b88549ac5042ce416127fca3eb9ad03134d3f87810ea59ea4234237cfb5`  
		Last Modified: Tue, 21 Dec 2021 17:47:57 GMT  
		Size: 434.5 KB (434535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7fd84c8b77f1bed6ce41ca44ab4fb3dcd41ff89c2536a428f8652b8ddd33a5`  
		Last Modified: Tue, 21 Dec 2021 17:47:57 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0160dd882bce5ce444f89bf8732ff499fc30f3469341d635ea8d721d047c0505`  
		Last Modified: Tue, 21 Dec 2021 17:47:57 GMT  
		Size: 3.1 KB (3058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f79544ee26bf206fa19269f5f7a1ebbde94f2a5bd1656b0ae5f2971d6541bc2`  
		Last Modified: Tue, 21 Dec 2021 17:51:31 GMT  
		Size: 83.3 MB (83288625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eec3e0bbb82724eb4711d2820dfe9e9528a04f699284502c0a58521289481c67`  
		Last Modified: Tue, 21 Dec 2021 17:50:41 GMT  
		Size: 9.0 KB (9033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60474c3ba697da49c7a5a2876f92e59d9016a67c7e49069ad44a5dfdf4231001`  
		Last Modified: Tue, 21 Dec 2021 17:50:41 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb2f2fcde3de0e94da604e20f8b124693d5360709355d8c5f8853f795c45f23`  
		Last Modified: Tue, 21 Dec 2021 17:50:41 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f7c7091186642d54dc77c9d1eaa866bc1b7bdf585e8ead09c184677b19d5eb`  
		Last Modified: Tue, 04 Jan 2022 01:08:35 GMT  
		Size: 4.7 KB (4714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-bullseye` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:b659cf1151444e3fa9f8c1045446fa41ee5180063c2b72ce6ebedfbdf0a283ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (129958291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d078523f99d06ee9202511325bc8498f87fca23f60bb1c89ff062c0ccb0b5c79`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 06:32:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 06:32:16 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 26 Jan 2022 06:32:17 GMT
ENV GOSU_VERSION=1.14
# Wed, 26 Jan 2022 06:32:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 26 Jan 2022 06:32:33 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 26 Jan 2022 06:32:33 GMT
ENV LANG=en_US.utf8
# Wed, 26 Jan 2022 06:32:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 06:32:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 26 Jan 2022 06:33:11 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Wed, 26 Jan 2022 06:34:55 GMT
ENV PG_MAJOR=12
# Wed, 26 Jan 2022 06:34:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Wed, 26 Jan 2022 06:34:57 GMT
ENV PG_VERSION=12.9-1.pgdg110+1
# Wed, 26 Jan 2022 06:35:22 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 26 Jan 2022 06:35:23 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 26 Jan 2022 06:35:23 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 26 Jan 2022 06:35:24 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 26 Jan 2022 06:35:25 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 26 Jan 2022 06:35:26 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 26 Jan 2022 06:35:28 GMT
COPY file:b2fac085615145a2bee98d4185ef0748655fa7c086ca21daef1ca6cac272bf59 in /usr/local/bin/ 
# Wed, 26 Jan 2022 06:35:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 06:35:29 GMT
STOPSIGNAL SIGINT
# Wed, 26 Jan 2022 06:35:30 GMT
EXPOSE 5432
# Wed, 26 Jan 2022 06:35:31 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c57ecc00197f74ecfe5cb4695ff8e4c31d88315d3c8f6b13e57f32b9fb6f2a2`  
		Last Modified: Wed, 26 Jan 2022 07:07:50 GMT  
		Size: 4.2 MB (4208911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1aaa551482e30d108cc7d900e1c329efc065835004868fe1a2f3f19f0a95fb`  
		Last Modified: Wed, 26 Jan 2022 07:07:49 GMT  
		Size: 1.6 KB (1649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409382316c269c57d22fdaa5f25f0738d8914b50707c8983a175dad92d7b4d0d`  
		Last Modified: Wed, 26 Jan 2022 07:07:49 GMT  
		Size: 1.3 MB (1345987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2a428af099e0f069419eb87af03d305891b574838113f91ba44539a05deb4b`  
		Last Modified: Wed, 26 Jan 2022 07:07:48 GMT  
		Size: 8.0 MB (8043388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44b8e834aba8ae7109dbcdff531b91c5939db21d3c6bbffd871e7252c32641a`  
		Last Modified: Wed, 26 Jan 2022 07:07:47 GMT  
		Size: 218.6 KB (218594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1372eb84c820add30aceea443ba9e01d2344f670f92c272837b72f1ad299a0ad`  
		Last Modified: Wed, 26 Jan 2022 07:07:46 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39188dbce14f3aee4c4502bb5b5ccaf9e2ca0ee598f44e6a187a21ab891edfe4`  
		Last Modified: Wed, 26 Jan 2022 07:07:47 GMT  
		Size: 3.0 KB (3032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d5af5dbd4c3ea38f8764e18993f2ecc27b3cd473119570e7964baa056755a0`  
		Last Modified: Wed, 26 Jan 2022 07:09:12 GMT  
		Size: 86.1 MB (86065798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17bbef446d4a7094d65a3fce819772e61df3a399d8e9ba3c2f3b6a65333cf749`  
		Last Modified: Wed, 26 Jan 2022 07:09:00 GMT  
		Size: 9.0 KB (9027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04d11a27cea51b48dbacbc6ad523bbf7eb6a014823cdae743755d932b8fa51e`  
		Last Modified: Wed, 26 Jan 2022 07:09:00 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1529432b2dfdfeda709252935c2a24ac709dd8dbdca11c5d1ff6174f451c2517`  
		Last Modified: Wed, 26 Jan 2022 07:09:00 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c85c0100dcb6571ce9eb4e4e9067b07b9e43cea26cf2a3a842ff16e3da4cd7`  
		Last Modified: Wed, 26 Jan 2022 07:09:00 GMT  
		Size: 4.7 KB (4716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-bullseye` - linux; 386

```console
$ docker pull postgres@sha256:02cc3cc5b47dfad9914033a8aa28916936c40e485fd3240294106a9bb94ffa51
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137290606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16b3ee9e09d5cc18641e11bfd83e8a9a25a02f698c0023b1be915383f09f7242`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:06 GMT
ADD file:6b67a0d4d176747cc8cefbd105facde82f1795467bf02eb45e8385c91cdc9c41 in / 
# Tue, 21 Dec 2021 01:40:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 17:32:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 17:32:31 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 21 Dec 2021 17:32:31 GMT
ENV GOSU_VERSION=1.14
# Tue, 21 Dec 2021 17:32:42 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 21 Dec 2021 17:32:50 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 21 Dec 2021 17:32:51 GMT
ENV LANG=en_US.utf8
# Tue, 21 Dec 2021 17:32:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 17:32:57 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 21 Dec 2021 17:33:04 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 21 Dec 2021 18:14:28 GMT
ENV PG_MAJOR=12
# Tue, 21 Dec 2021 18:14:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Tue, 21 Dec 2021 18:14:28 GMT
ENV PG_VERSION=12.9-1.pgdg110+1
# Tue, 21 Dec 2021 18:30:08 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 21 Dec 2021 18:30:09 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 21 Dec 2021 18:30:10 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 21 Dec 2021 18:30:11 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 21 Dec 2021 18:30:13 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 21 Dec 2021 18:30:13 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 04 Jan 2022 01:39:23 GMT
COPY file:b2fac085615145a2bee98d4185ef0748655fa7c086ca21daef1ca6cac272bf59 in /usr/local/bin/ 
# Tue, 04 Jan 2022 01:39:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jan 2022 01:39:24 GMT
STOPSIGNAL SIGINT
# Tue, 04 Jan 2022 01:39:24 GMT
EXPOSE 5432
# Tue, 04 Jan 2022 01:39:24 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:9b9a100d632569e96aeb2d7b0bc45bc436609bb61335815f207994f3b557f0f7`  
		Last Modified: Tue, 21 Dec 2021 01:48:45 GMT  
		Size: 32.4 MB (32370850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e1cde80251c811d2a11419dd7d755ffd8bb6ee6c48d6c26f4963af66231091`  
		Last Modified: Tue, 21 Dec 2021 19:09:13 GMT  
		Size: 4.8 MB (4812928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e5319205e69940a9e1c4aa2eb8b128ceb099b3b1ff04f95e9b807a57bee635`  
		Last Modified: Tue, 21 Dec 2021 19:09:11 GMT  
		Size: 1.8 KB (1791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:986b5046b42a04043dea030af38801a4786894d4282a6c18ca760a3a7dc08a91`  
		Last Modified: Tue, 21 Dec 2021 19:09:11 GMT  
		Size: 1.4 MB (1385420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69e50d5aff566bb6bc43ae83d6f252488788b3297a5932cd665a9c9df4816a8`  
		Last Modified: Tue, 21 Dec 2021 19:09:12 GMT  
		Size: 8.0 MB (8045063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d4116276636907e25c3224b8a72e1c62e1b6040aae2a429a921513da0d0e4a`  
		Last Modified: Tue, 21 Dec 2021 19:09:09 GMT  
		Size: 448.0 KB (447958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e3213019f61cd51f01af4a70a4182fc67bdd71b82ea07c074f6796d4ff00f6`  
		Last Modified: Tue, 21 Dec 2021 19:09:09 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05967f41fcb3ecba7545ee6ced7b3f5419d14bc5e1fec038363f5e01c268e986`  
		Last Modified: Tue, 21 Dec 2021 19:09:08 GMT  
		Size: 3.1 KB (3053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb46de6d0df59d686a51e7fd0d5423ef792e8ce6a75b3bfa18e46b94ee66012`  
		Last Modified: Tue, 21 Dec 2021 19:10:58 GMT  
		Size: 90.2 MB (90209312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac5e94e8827ade33e8c10dec7740fbd9562c2cf5afc9865e587267f26f0a3df`  
		Last Modified: Tue, 21 Dec 2021 19:10:39 GMT  
		Size: 9.0 KB (9028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb37d8a06d785b16db080403d16be0214fbd7bf6e24ac83c411c7313c86f4c3`  
		Last Modified: Tue, 21 Dec 2021 19:10:39 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83ba1ed7873ad84028a4706166f7af08bdda618ed6f9fc58f5f8a94caa399d2`  
		Last Modified: Tue, 21 Dec 2021 19:10:39 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88eec284b331ea1b43df6a0686dabd137b7dea3eed59dc52ac10a296b1849982`  
		Last Modified: Tue, 04 Jan 2022 01:44:25 GMT  
		Size: 4.7 KB (4724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-bullseye` - linux; mips64le

```console
$ docker pull postgres@sha256:0626c1c3cf6a23e9b2f65d2ce872c6474eb1836af706c5bacee71bce3a1ec0bc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.1 MB (130094519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:054ac9f1196f4e9b01798cf1139b2cdf30b5a7c622e53aac3d6f62d52caad964`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Dec 2021 02:09:07 GMT
ADD file:9e5931d5ed32a23b2e93bd8846258c647613637c581b6813bbc7d7e6b86bbdf5 in / 
# Tue, 21 Dec 2021 02:09:08 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 19:46:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 19:46:42 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 21 Dec 2021 19:46:42 GMT
ENV GOSU_VERSION=1.14
# Tue, 21 Dec 2021 19:47:03 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 21 Dec 2021 19:47:27 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 21 Dec 2021 19:47:27 GMT
ENV LANG=en_US.utf8
# Tue, 21 Dec 2021 19:47:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 19:47:42 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 21 Dec 2021 19:47:45 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 21 Dec 2021 21:37:13 GMT
ENV PG_MAJOR=12
# Tue, 21 Dec 2021 21:37:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Tue, 21 Dec 2021 21:37:14 GMT
ENV PG_VERSION=12.9-1.pgdg110+1
# Tue, 21 Dec 2021 22:28:19 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 21 Dec 2021 22:28:22 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 21 Dec 2021 22:28:24 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 21 Dec 2021 22:28:24 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 21 Dec 2021 22:28:26 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 21 Dec 2021 22:28:27 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 04 Jan 2022 01:07:44 GMT
COPY file:b2fac085615145a2bee98d4185ef0748655fa7c086ca21daef1ca6cac272bf59 in /usr/local/bin/ 
# Tue, 04 Jan 2022 01:07:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jan 2022 01:07:44 GMT
STOPSIGNAL SIGINT
# Tue, 04 Jan 2022 01:07:45 GMT
EXPOSE 5432
# Tue, 04 Jan 2022 01:07:45 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:6a6edb95e2485a5b9b3c44b27b7ebad16384c0e08a3d61b7e48c65d7278763cf`  
		Last Modified: Tue, 21 Dec 2021 02:18:14 GMT  
		Size: 29.6 MB (29619177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653335db2e28f4bfd481492903832070d7b54f24e6dbe67b45fbffb8f93f5f20`  
		Last Modified: Wed, 22 Dec 2021 00:29:22 GMT  
		Size: 4.4 MB (4402849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:383e4074bda5fb21527af7a93e33f31c633e43a90f4e44b18a33310b19b408fb`  
		Last Modified: Wed, 22 Dec 2021 00:29:17 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f76b983b76977ca3c9f7673149aeb74d2c70667cdaa2fd417ad3230f650169`  
		Last Modified: Wed, 22 Dec 2021 00:29:19 GMT  
		Size: 1.3 MB (1298144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7171701033e64ea4d7fa9ccf50c04e53f4dc6c699892fd7e860ea1a5a8909e`  
		Last Modified: Wed, 22 Dec 2021 00:29:23 GMT  
		Size: 8.0 MB (8043972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116ca8f780ee3685a34795364c930ee965bfb719b63da395abf7ffd84fd9b0cd`  
		Last Modified: Wed, 22 Dec 2021 00:29:15 GMT  
		Size: 439.2 KB (439173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87675c81c5f9c9c33f33cb6639eb0d676b031d16b7d33da01e300cb5ac98845c`  
		Last Modified: Wed, 22 Dec 2021 00:29:15 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc52613f4cea3e4b18408762b08e16750865b57c281ec9e1e567fe182a169ea`  
		Last Modified: Wed, 22 Dec 2021 00:29:15 GMT  
		Size: 3.1 KB (3058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f434eaa617ce75e28bc21aaa2b816987e36019f0449172aab32d8185d5f12411`  
		Last Modified: Wed, 22 Dec 2021 00:33:07 GMT  
		Size: 86.3 MB (86272217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f998218918849c3aa870284fb67c1ac7a0390895834ece23f3d6dd73e4d5ae7b`  
		Last Modified: Wed, 22 Dec 2021 00:32:08 GMT  
		Size: 9.0 KB (9029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022611f5ba4acea4bd8cf61cb5972e1f5282b1e87dba28da8c002398ee349bf4`  
		Last Modified: Wed, 22 Dec 2021 00:32:08 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20341891fc24a85aace6858a9bc44a179d3314704d521bf9c00b291b5bdb4425`  
		Last Modified: Wed, 22 Dec 2021 00:32:08 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786752240e3ba0daf46f3979cb20ffed9d733a5827fce7e171e782241223e617`  
		Last Modified: Tue, 04 Jan 2022 01:09:13 GMT  
		Size: 4.7 KB (4715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-bullseye` - linux; ppc64le

```console
$ docker pull postgres@sha256:382c617482f072377a471a872f07f7aa8d3c60ed8f5b3bcb4b4d4fcf930fd807
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.0 MB (144031776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12961bdc82b13380544e867781df7982b2272fa6ecbbbb79f227848bcec08549`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 21 Dec 2021 02:20:24 GMT
ADD file:078a17bf7e519cb7a60fbbf743ba7e5897554201cb44957154ab518d6991a033 in / 
# Tue, 21 Dec 2021 02:20:28 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 19:32:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 19:32:29 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 21 Dec 2021 19:32:32 GMT
ENV GOSU_VERSION=1.14
# Tue, 21 Dec 2021 19:33:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 21 Dec 2021 19:33:41 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 21 Dec 2021 19:33:45 GMT
ENV LANG=en_US.utf8
# Tue, 21 Dec 2021 19:34:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 19:34:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 21 Dec 2021 19:34:32 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 21 Dec 2021 19:40:39 GMT
ENV PG_MAJOR=12
# Tue, 21 Dec 2021 19:40:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Tue, 21 Dec 2021 19:40:51 GMT
ENV PG_VERSION=12.9-1.pgdg110+1
# Tue, 21 Dec 2021 19:43:31 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 21 Dec 2021 19:43:51 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 21 Dec 2021 19:44:01 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 21 Dec 2021 19:44:02 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 21 Dec 2021 19:44:12 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 21 Dec 2021 19:44:17 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 04 Jan 2022 01:18:26 GMT
COPY file:b2fac085615145a2bee98d4185ef0748655fa7c086ca21daef1ca6cac272bf59 in /usr/local/bin/ 
# Tue, 04 Jan 2022 01:18:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 Jan 2022 01:18:31 GMT
STOPSIGNAL SIGINT
# Tue, 04 Jan 2022 01:18:34 GMT
EXPOSE 5432
# Tue, 04 Jan 2022 01:18:36 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:3345479fea0cdce1382b927b0908af4f239b288b30efa203c50edf7ac0cb055e`  
		Last Modified: Tue, 21 Dec 2021 02:29:20 GMT  
		Size: 35.3 MB (35258992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08fad619d5e9b9134c50ee46d26ef57809bfd04852d94a70061b465fedc2585`  
		Last Modified: Tue, 21 Dec 2021 19:55:57 GMT  
		Size: 5.2 MB (5222905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7102b847099d38448e8497d5c9b44e7f49361334982bf01fda2a73889b9878`  
		Last Modified: Tue, 21 Dec 2021 19:55:53 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0c6341861b7e8f732f3cedf24bf499bd159fbeef06cc0fd930903f828d113b`  
		Last Modified: Tue, 21 Dec 2021 19:55:53 GMT  
		Size: 1.3 MB (1317578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371ec02786458e7b7790fdf8d336a55bed62bc6eedbd144764af964a5181ae0e`  
		Last Modified: Tue, 21 Dec 2021 19:55:54 GMT  
		Size: 8.0 MB (8045507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4be2382fa6b141791fb24b126e80a5bee7e0217eee2a2a84108bcf8e3552a59`  
		Last Modified: Tue, 21 Dec 2021 19:55:52 GMT  
		Size: 451.7 KB (451666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89eecb4fbb66e4fea8d2b8dea47313c87717e686ccd4171ca1596bf1105b5558`  
		Last Modified: Tue, 21 Dec 2021 19:55:50 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5242e0f07598b8e0622a3525e3dfeca963999a00291b9d74c727d0c15314f8fe`  
		Last Modified: Tue, 21 Dec 2021 19:55:49 GMT  
		Size: 3.1 KB (3058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd9d204b11ca9587dba2a97c5e50b437d08e2238ed76e4fbfc2f0abe5c07f8f`  
		Last Modified: Tue, 21 Dec 2021 19:57:33 GMT  
		Size: 93.7 MB (93716034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690369f0c81fcc2f6ad214d194b8f4081228eb8bf0efb101e2b1ace966f55e82`  
		Last Modified: Tue, 21 Dec 2021 19:57:16 GMT  
		Size: 9.0 KB (9039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e5331e761e0d410e1a25ca498ad18f564c0e41592fda872cc0b2ae0849ce4e`  
		Last Modified: Tue, 21 Dec 2021 19:57:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0664f3ab7411d7adae57c84a621228a9c4e361e5ff35f3099edf1b611e67314`  
		Last Modified: Tue, 21 Dec 2021 19:57:16 GMT  
		Size: 203.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084a70ba30e4680917e102da81dbfc9c70cdd80e0ebbf8ecf87bbd35e60e887d`  
		Last Modified: Tue, 04 Jan 2022 01:24:13 GMT  
		Size: 4.7 KB (4710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-bullseye` - linux; s390x

```console
$ docker pull postgres@sha256:9006a2b1bd524c55d47d35179a20f6e9bf4faf0c584e735612ee5f34ff08e554
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.8 MB (83797985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae65d2199b101de2381a7a4d982dd8e66c88e952f0718f7e9cac2d564f53baf1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:13 GMT
ADD file:03b224b82f458b08d3b5071e42b67915a3db309332c0fc9229db7cf1148bc1b5 in / 
# Wed, 26 Jan 2022 01:41:15 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 07:32:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 07:32:30 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 26 Jan 2022 07:32:30 GMT
ENV GOSU_VERSION=1.14
# Wed, 26 Jan 2022 07:32:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 26 Jan 2022 07:32:43 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 26 Jan 2022 07:32:44 GMT
ENV LANG=en_US.utf8
# Wed, 26 Jan 2022 07:32:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 07:32:48 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 26 Jan 2022 07:33:20 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Wed, 26 Jan 2022 07:52:15 GMT
ENV PG_MAJOR=12
# Wed, 26 Jan 2022 07:52:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Wed, 26 Jan 2022 07:52:15 GMT
ENV PG_VERSION=12.9-1.pgdg110+1
# Wed, 26 Jan 2022 07:58:24 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 26 Jan 2022 07:58:26 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 26 Jan 2022 07:58:27 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 26 Jan 2022 07:58:27 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 26 Jan 2022 07:58:28 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 26 Jan 2022 07:58:28 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 26 Jan 2022 07:58:28 GMT
COPY file:b2fac085615145a2bee98d4185ef0748655fa7c086ca21daef1ca6cac272bf59 in /usr/local/bin/ 
# Wed, 26 Jan 2022 07:58:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 07:58:28 GMT
STOPSIGNAL SIGINT
# Wed, 26 Jan 2022 07:58:28 GMT
EXPOSE 5432
# Wed, 26 Jan 2022 07:58:28 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:70bed29526f8483937e4d2540d19256d30786007c7c321e717e00d2e74700380`  
		Last Modified: Wed, 26 Jan 2022 01:46:57 GMT  
		Size: 29.6 MB (29647071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adab0b82ec25a88edeaf5e951f0f97b4b3f541b0a9f855ad9bdbab5ec3b82258`  
		Last Modified: Wed, 26 Jan 2022 08:21:41 GMT  
		Size: 4.3 MB (4302200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32845bcd9646d96ac1ebedc163e8b332b93ec5e381b7adb28b4e048446a479c`  
		Last Modified: Wed, 26 Jan 2022 08:21:40 GMT  
		Size: 1.8 KB (1800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db75c1a18cfc37dc49d94fcdf1fe55bf7a3958cd66472580b982daf1dcd60559`  
		Last Modified: Wed, 26 Jan 2022 08:21:40 GMT  
		Size: 1.4 MB (1381382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f042f08b8d2c3c370464daac9b5ca277fd2a7a01d201191427aa3d54d62dcd`  
		Last Modified: Wed, 26 Jan 2022 08:21:40 GMT  
		Size: 8.1 MB (8098986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb531aa668e0f5cb99281939a526713946c9f8b6e071f14fb2a9d9dccdc9fb3`  
		Last Modified: Wed, 26 Jan 2022 08:21:38 GMT  
		Size: 438.3 KB (438285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d904e25ceb71481a5b408ee7254f7e4c6744d23294351859f7ff73ddfeb9f2`  
		Last Modified: Wed, 26 Jan 2022 08:21:39 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce09051744ed10c4ffd4e9537e54551dd68775dcfc11b633dfa6765c67e258c`  
		Last Modified: Wed, 26 Jan 2022 08:21:39 GMT  
		Size: 3.1 KB (3058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9c2ac5127334602e3822a4dd52880be39b3006f3cf9e085a9280ccc138b599`  
		Last Modified: Wed, 26 Jan 2022 08:22:49 GMT  
		Size: 39.9 MB (39910983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9f7f437c2e4067f148e9c0548ce21a4de0d575a945332c6ddd6077e3c51406`  
		Last Modified: Wed, 26 Jan 2022 08:22:44 GMT  
		Size: 9.0 KB (9026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9657f6ea3933fbacec081387e0070d02ea288013af0a7434f25ff5846af6c7fd`  
		Last Modified: Wed, 26 Jan 2022 08:22:44 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a058487abdef7266b2b19d09d52712356f1b097da7eefebd35e8815ad15c395c`  
		Last Modified: Wed, 26 Jan 2022 08:22:44 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66feed4b56699fcbd2cb1058788cd11510444c2fc38159e12497af7d99976af1`  
		Last Modified: Wed, 26 Jan 2022 08:22:44 GMT  
		Size: 4.7 KB (4718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
