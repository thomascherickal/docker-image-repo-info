## `postgres:12-bullseye`

```console
$ docker pull postgres@sha256:f756b2dd95db8c39402c5b0b9327b41ab614e9073821af22f5b8325957cedd12
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
$ docker pull postgres@sha256:b7f707b25e620ba87b85ee02433a7534847c27ec754bc20f0ae3422872b3eea9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.1 MB (136077765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:963b1b753ca652637767d9ba6c94b193a5c11187ba9cfb0e0a0f8a85e142f8e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 01:28:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 02 Mar 2022 01:28:59 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 02 Mar 2022 01:28:59 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Mar 2022 01:29:08 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Mar 2022 01:29:14 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 02 Mar 2022 01:29:14 GMT
ENV LANG=en_US.utf8
# Tue, 08 Mar 2022 19:33:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Mar 2022 19:33:36 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 08 Mar 2022 19:34:20 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 08 Mar 2022 19:46:55 GMT
ENV PG_MAJOR=12
# Tue, 08 Mar 2022 19:46:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Tue, 08 Mar 2022 19:46:56 GMT
ENV PG_VERSION=12.10-1.pgdg110+1
# Tue, 08 Mar 2022 19:47:14 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 08 Mar 2022 19:47:16 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 08 Mar 2022 19:47:16 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 08 Mar 2022 19:47:16 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 08 Mar 2022 19:47:17 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 08 Mar 2022 19:47:17 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 08 Mar 2022 19:47:17 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Tue, 08 Mar 2022 19:47:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Mar 2022 19:47:17 GMT
STOPSIGNAL SIGINT
# Tue, 08 Mar 2022 19:47:18 GMT
EXPOSE 5432
# Tue, 08 Mar 2022 19:47:18 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c22623b5a6a5b3ff505b51cd28af0a29f13da3b4a547b0c91828ab837a322f`  
		Last Modified: Wed, 02 Mar 2022 01:35:40 GMT  
		Size: 4.4 MB (4414417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6a6a85d0141c8ef50d8ee65446beec9e9d833789f250acba597b45a6263940`  
		Last Modified: Wed, 02 Mar 2022 01:35:39 GMT  
		Size: 1.8 KB (1800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6012728e8256730285f52d1f32ea69b1a24636c5dbc10a26376713498a7592d3`  
		Last Modified: Wed, 02 Mar 2022 01:35:39 GMT  
		Size: 1.4 MB (1418354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eca9143e7218b20ea4622cc8923dc00b7f910612c9c9aa30d20cb1f16de5e47`  
		Last Modified: Wed, 02 Mar 2022 01:35:38 GMT  
		Size: 8.0 MB (8045340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9ebd05a23fb460247eeac21972f6b29292c69546fc38126c8d964a170d0037`  
		Last Modified: Tue, 08 Mar 2022 20:06:32 GMT  
		Size: 1.3 MB (1260884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16e63bb90effc502275326045d0aba34b1f0e48d41024b91e123ba8e73ee401c`  
		Last Modified: Tue, 08 Mar 2022 20:06:32 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c15c24115ca4bf23d6e64f0087524312f2dd0d7d8b518bd150192dffdcb8577`  
		Last Modified: Tue, 08 Mar 2022 20:06:32 GMT  
		Size: 3.2 KB (3203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc773987ce60a9840192ec8e3b2e93374bbebd55e6c513642ddfe31a4be4059`  
		Last Modified: Tue, 08 Mar 2022 20:09:11 GMT  
		Size: 89.6 MB (89553164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826ed382a47e1f1242cfd9bfdf2517bfa5b65f191baa822c5f39c85ff624808e`  
		Last Modified: Tue, 08 Mar 2022 20:08:54 GMT  
		Size: 9.0 KB (9031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f354de5e15b7fc61de6c69aed73be4e2becf818926496f24acee1e84775311ca`  
		Last Modified: Tue, 08 Mar 2022 20:08:54 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39177c434ced7b96d812ed0c850fd8459fe1d4a37f0f0a0fcc0d1f057efb91a`  
		Last Modified: Tue, 08 Mar 2022 20:08:54 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf30bc1a15bf6ef444c11fc245fe2129c76b0e3c3996c2838c7c257a5ed56f77`  
		Last Modified: Tue, 08 Mar 2022 20:08:54 GMT  
		Size: 4.7 KB (4696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-bullseye` - linux; arm variant v5

```console
$ docker pull postgres@sha256:5b212e151cc358dc9ab59b3a3b0361f048757b6c81512a09360d5a24013aab13
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128569667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:359632ab33ee0cd3bcdad094071d42cc0ae685440e5a95ca34326de4934b4196`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:53 GMT
ADD file:eb61ee802e5118b26e1fec2c7fc58e34de0de54a5fd47dc6318c11a039ef528f in / 
# Tue, 01 Mar 2022 02:02:53 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 09:22:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 09:22:04 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 01 Mar 2022 09:22:04 GMT
ENV GOSU_VERSION=1.14
# Tue, 01 Mar 2022 09:22:27 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 01 Mar 2022 09:22:49 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 01 Mar 2022 09:22:49 GMT
ENV LANG=en_US.utf8
# Tue, 01 Mar 2022 09:23:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 09:23:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 01 Mar 2022 09:23:15 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 01 Mar 2022 10:38:43 GMT
ENV PG_MAJOR=12
# Tue, 01 Mar 2022 10:38:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Tue, 01 Mar 2022 10:38:44 GMT
ENV PG_VERSION=12.10-1.pgdg110+1
# Tue, 01 Mar 2022 11:14:16 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 01 Mar 2022 11:14:18 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 01 Mar 2022 11:14:20 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 01 Mar 2022 11:14:21 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 01 Mar 2022 11:14:22 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 01 Mar 2022 11:14:23 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 01 Mar 2022 11:14:23 GMT
COPY file:a089d0b5bcabd9529434672fbf8e8d3378ce1f734b4596df5c20c565589c8f01 in /usr/local/bin/ 
# Tue, 01 Mar 2022 11:14:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 11:14:24 GMT
STOPSIGNAL SIGINT
# Tue, 01 Mar 2022 11:14:24 GMT
EXPOSE 5432
# Tue, 01 Mar 2022 11:14:25 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:4aa6e26b4dfdac27e5b5e15b7ebf4366149755a79dd653a5b68d9d93dd94c695`  
		Last Modified: Tue, 01 Mar 2022 02:18:33 GMT  
		Size: 28.9 MB (28909528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bfb4944ed96f352a4ff6d9cc3e6f37a02c9b7196b34e30e69385a0d6af4ee37`  
		Last Modified: Tue, 01 Mar 2022 13:09:41 GMT  
		Size: 4.1 MB (4096513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb094df44e35cf504536e3662bcf7e68155e868e06dd2f454b8f09927a917b0`  
		Last Modified: Tue, 01 Mar 2022 13:09:39 GMT  
		Size: 1.8 KB (1791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d381694ba741048c7b4f8f85d1d7608cf3c1a5b52d84f0ac4c8892dde081ad44`  
		Last Modified: Tue, 01 Mar 2022 13:09:40 GMT  
		Size: 1.4 MB (1382606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66a8daa3ce4e87c5730198c469634d0107b4d3125029d911e93d60e4c3f77cd`  
		Last Modified: Tue, 01 Mar 2022 13:09:43 GMT  
		Size: 8.0 MB (8045231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c755ca0d5e35c60bce61f5dcab069f752c1cf50de8816c5507a92d36fc8a89`  
		Last Modified: Tue, 01 Mar 2022 13:09:37 GMT  
		Size: 439.8 KB (439849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba7aa80b04069b006da74d5c47a37c81cf5bfebd3ce2c7e86c9029ed64c399b`  
		Last Modified: Tue, 01 Mar 2022 13:09:37 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c762403d2eef68231e7bd2cd7470ac12b14f66f511c5f8bc2bbaf80076957b50`  
		Last Modified: Tue, 01 Mar 2022 13:09:37 GMT  
		Size: 3.2 KB (3203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a030bee70b4afc3cba2a787dd015cd5e6a3b13f24517bc5e84f5c26cfd8ee31`  
		Last Modified: Tue, 01 Mar 2022 13:13:13 GMT  
		Size: 85.7 MB (85676753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91aaba11fedac36db75b011efdf5952ae5594638d8e410dae5c428fffe5d30ba`  
		Last Modified: Tue, 01 Mar 2022 13:12:22 GMT  
		Size: 9.0 KB (9034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33728b76ec7316e4d7f2218b3d602bfdbd3859422875f949990495e439f18a64`  
		Last Modified: Tue, 01 Mar 2022 13:12:22 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff59fcc6ffb81b6914e4d56388660ed34d3d2a444557ae109f723e9b902b56f`  
		Last Modified: Tue, 01 Mar 2022 13:12:22 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b4e58588343acf8586b8e5bf658880944c9f885222eef6f5434e45a032a296`  
		Last Modified: Tue, 01 Mar 2022 13:12:22 GMT  
		Size: 4.7 KB (4681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-bullseye` - linux; arm variant v7

```console
$ docker pull postgres@sha256:97d027822f3794fd80267de19afac79b9fb5700678027552af5091a614b510f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.1 MB (124148243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17bc1579d5d754df25e556cd0dd5673ae99a5717ac4eda88a3784d57fb706c06`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:56 GMT
ADD file:c6b519323fd1fa09b9f8c8608778872e8fa6208cb0b42aaccdef4479a469f5f4 in / 
# Tue, 01 Mar 2022 02:02:57 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 13:06:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 02 Mar 2022 13:06:03 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 02 Mar 2022 13:06:03 GMT
ENV GOSU_VERSION=1.14
# Wed, 02 Mar 2022 13:06:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 02 Mar 2022 13:06:43 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 02 Mar 2022 13:06:43 GMT
ENV LANG=en_US.utf8
# Tue, 08 Mar 2022 20:12:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Mar 2022 20:12:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 08 Mar 2022 20:12:35 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 08 Mar 2022 21:31:30 GMT
ENV PG_MAJOR=12
# Tue, 08 Mar 2022 21:31:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Tue, 08 Mar 2022 21:31:31 GMT
ENV PG_VERSION=12.10-1.pgdg110+1
# Tue, 08 Mar 2022 22:03:10 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 08 Mar 2022 22:03:12 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 08 Mar 2022 22:03:14 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 08 Mar 2022 22:03:14 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 08 Mar 2022 22:03:16 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 08 Mar 2022 22:03:16 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 08 Mar 2022 22:03:17 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Tue, 08 Mar 2022 22:03:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Mar 2022 22:03:17 GMT
STOPSIGNAL SIGINT
# Tue, 08 Mar 2022 22:03:18 GMT
EXPOSE 5432
# Tue, 08 Mar 2022 22:03:18 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:59dbb2ac3829352dd707e28e037734c9fbdef5b03aea31e3929ddcead949afee`  
		Last Modified: Tue, 01 Mar 2022 02:19:09 GMT  
		Size: 26.6 MB (26565105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:975c4f43912af76ce914c41ade53c9f99fc0bdf55bacbc0c55b71d6f3593088b`  
		Last Modified: Wed, 02 Mar 2022 16:10:48 GMT  
		Size: 3.7 MB (3717115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6738954b4a8c698826cefa42e66287030036f576d72f05d32a3a7c00dd7bd804`  
		Last Modified: Wed, 02 Mar 2022 16:10:46 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54cbe2ac269d69f85343ed65264c58d0d0c95ebf9f0a817cf2065c94d6526edf`  
		Last Modified: Wed, 02 Mar 2022 16:10:47 GMT  
		Size: 1.4 MB (1375234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1829d5a150885550f05c67a29702a7363168dc175d36d27db53333b1559a492f`  
		Last Modified: Wed, 02 Mar 2022 16:10:51 GMT  
		Size: 8.0 MB (8045344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5068ec92f79339dec94ecd181b2c19a19b996f8c06b0d309fd9a46b5f5bf3d`  
		Last Modified: Wed, 09 Mar 2022 00:01:02 GMT  
		Size: 1.1 MB (1130955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e8e8eccbb89a000a13ab506e2273c2eaae61b4c0f11e9af97875992cfa8d67`  
		Last Modified: Wed, 09 Mar 2022 00:01:02 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26faa757c380f433a74baf912082333ef44f7280a85893290535bea1bce098e9`  
		Last Modified: Wed, 09 Mar 2022 00:01:01 GMT  
		Size: 3.2 KB (3204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9dbf49b76bf1c0fa05908d5521f0c85af7a33109528bee31589b64e8ec03c2`  
		Last Modified: Wed, 09 Mar 2022 00:06:41 GMT  
		Size: 83.3 MB (83295292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1089efa20cb400c9ce1303675c735f8b5dc7e87dbaea302492d0b1554acd19b2`  
		Last Modified: Wed, 09 Mar 2022 00:05:48 GMT  
		Size: 9.0 KB (9028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbe1a2a7e1a0e3b10b093e6ca540d8ee9410e7700d5920cd2a587905c3635337`  
		Last Modified: Wed, 09 Mar 2022 00:05:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47cc7f3dfff4d00887127d27315212bdfb1297c21ee60e18982eb183e27c8ac4`  
		Last Modified: Wed, 09 Mar 2022 00:05:49 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ebc706c721599f2ccbda2f2369796e77d2e6772a99ea5d588014f7b8e7508c0`  
		Last Modified: Wed, 09 Mar 2022 00:05:49 GMT  
		Size: 4.7 KB (4700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-bullseye` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:32b0c20078dc507294b844f8c06715729f75e5177253c9935a9300925e7c505e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.8 MB (130783307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a3562d0044b17225a85bc17e246e7c258a4476b0b7de5806ebb9a7ea456af04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:29 GMT
ADD file:9816c9c29627693c34afda4fa5e1a5e8a0f5aa3c5d5cfd920a4d89c77aab997d in / 
# Tue, 01 Mar 2022 02:11:30 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 18:33:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 18:33:22 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 01 Mar 2022 18:33:22 GMT
ENV GOSU_VERSION=1.14
# Tue, 01 Mar 2022 18:33:30 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 01 Mar 2022 18:33:37 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 01 Mar 2022 18:33:37 GMT
ENV LANG=en_US.utf8
# Tue, 08 Mar 2022 19:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Mar 2022 19:53:19 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 08 Mar 2022 19:53:59 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 08 Mar 2022 20:03:00 GMT
ENV PG_MAJOR=12
# Tue, 08 Mar 2022 20:03:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Tue, 08 Mar 2022 20:03:02 GMT
ENV PG_VERSION=12.10-1.pgdg110+1
# Tue, 08 Mar 2022 20:03:27 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 08 Mar 2022 20:03:28 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 08 Mar 2022 20:03:28 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 08 Mar 2022 20:03:29 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 08 Mar 2022 20:03:30 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 08 Mar 2022 20:03:31 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 08 Mar 2022 20:03:33 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Tue, 08 Mar 2022 20:03:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Mar 2022 20:03:34 GMT
STOPSIGNAL SIGINT
# Tue, 08 Mar 2022 20:03:35 GMT
EXPOSE 5432
# Tue, 08 Mar 2022 20:03:36 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:279a020076a7fbddfc996e4c55e605a8f322810c3eca21cdedbcb06beb0e1305`  
		Last Modified: Tue, 01 Mar 2022 02:18:24 GMT  
		Size: 30.1 MB (30057008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b9fd1723705e278a260ecfdc0ff403e45e81a6b4b0ba2aff3e573175b2b836`  
		Last Modified: Tue, 01 Mar 2022 18:59:38 GMT  
		Size: 4.2 MB (4208882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a892acc309beeb4ab1060f54d801447d2e959f9d3d409a73556be720e4b440ff`  
		Last Modified: Tue, 01 Mar 2022 18:59:36 GMT  
		Size: 1.6 KB (1649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c662a6a1585e383af9123b0f1b450a68480e3268f931cb8832207d298d5fac1a`  
		Last Modified: Tue, 01 Mar 2022 18:59:37 GMT  
		Size: 1.3 MB (1345997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d61f9d15e30c2b3147471f62bae2e68709e45b4295f795d33772f618d2bed1`  
		Last Modified: Tue, 01 Mar 2022 18:59:36 GMT  
		Size: 8.0 MB (8043552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f0e3ed00fb011920b13989fee2a9a2bfce31de1c37e6612fefed4c350f48b41`  
		Last Modified: Tue, 08 Mar 2022 20:35:45 GMT  
		Size: 1.0 MB (1025672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caef23651fbba81466bab3ae23c34492a64564586941d262ebb6e075469e5565`  
		Last Modified: Tue, 08 Mar 2022 20:35:44 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46937ca749035a12cbb1b081e615f104351ee1a3d43d039e24ba73daefc88802`  
		Last Modified: Tue, 08 Mar 2022 20:35:44 GMT  
		Size: 3.1 KB (3146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f211c0d1dd556c9bfc316d174ce4c1fc84482d81a6e1e684a9d16b724dcade`  
		Last Modified: Tue, 08 Mar 2022 20:38:09 GMT  
		Size: 86.1 MB (86083259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb96a9b3480cec093ad7dd94cfc294dfb18d830fe4e178bd7657e55c4ad3139`  
		Last Modified: Tue, 08 Mar 2022 20:37:57 GMT  
		Size: 9.0 KB (9034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e98575570e3393cf4d792088f8297ca2d2adda68462000bef5ffd8925385be`  
		Last Modified: Tue, 08 Mar 2022 20:37:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039f03edbca714d1d894aa6da62d7e0bb83db374ffde01c851b0248c3831cdcd`  
		Last Modified: Tue, 08 Mar 2022 20:37:57 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b4a328f18305625e7d9002e1ad368b868bcc56f4107071e468638aa582c02c0`  
		Last Modified: Tue, 08 Mar 2022 20:37:57 GMT  
		Size: 4.7 KB (4695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-bullseye` - linux; 386

```console
$ docker pull postgres@sha256:d00f9ede362443c739153c6acc4862f7b1fc1e00361795afceae438bb5a25f09
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.3 MB (137328116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8585d3c08dfbe6b550496584f6d8bc593564e52806b234a7f218e1687dfb498d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 01 Mar 2022 02:07:32 GMT
ADD file:e92ab504d4c0d3bd63da83254e6ca400b607c32e0f5037039648559b91770870 in / 
# Tue, 01 Mar 2022 02:07:33 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 19:41:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 19:41:21 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 01 Mar 2022 19:41:22 GMT
ENV GOSU_VERSION=1.14
# Tue, 01 Mar 2022 19:41:37 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 01 Mar 2022 19:41:48 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 01 Mar 2022 19:41:49 GMT
ENV LANG=en_US.utf8
# Tue, 01 Mar 2022 19:41:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 19:41:56 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 01 Mar 2022 19:41:58 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 01 Mar 2022 20:18:37 GMT
ENV PG_MAJOR=12
# Tue, 01 Mar 2022 20:18:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Tue, 01 Mar 2022 20:18:37 GMT
ENV PG_VERSION=12.10-1.pgdg110+1
# Tue, 01 Mar 2022 20:36:00 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 01 Mar 2022 20:36:01 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 01 Mar 2022 20:36:02 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 01 Mar 2022 20:36:02 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 01 Mar 2022 20:36:03 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 01 Mar 2022 20:36:03 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 01 Mar 2022 20:36:03 GMT
COPY file:a089d0b5bcabd9529434672fbf8e8d3378ce1f734b4596df5c20c565589c8f01 in /usr/local/bin/ 
# Tue, 01 Mar 2022 20:36:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 20:36:03 GMT
STOPSIGNAL SIGINT
# Tue, 01 Mar 2022 20:36:03 GMT
EXPOSE 5432
# Tue, 01 Mar 2022 20:36:03 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:04a87e821be7e4b29d48011b7aa4ff884ca57fd36995cb3b99fd2fc24ac562d8`  
		Last Modified: Tue, 01 Mar 2022 02:15:51 GMT  
		Size: 32.4 MB (32377389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1413cd2b1bf19dc897c3353ea7c2684f040e868845616d6d83ad207a560a547`  
		Last Modified: Tue, 01 Mar 2022 21:11:20 GMT  
		Size: 4.8 MB (4812945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb759f45225ffedda25233dafc89b7bfded91e977a3ea137c05e68b0cdc3e367`  
		Last Modified: Tue, 01 Mar 2022 21:11:19 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f40e2c31ccf209c71c3487082dc99346ef03c3fcdec342105266f033c058268`  
		Last Modified: Tue, 01 Mar 2022 21:11:19 GMT  
		Size: 1.4 MB (1385434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f119c2e9750013d27ae6918f9f42fc27b4dbf84ff7886cefcaa2e027b3bfb42`  
		Last Modified: Tue, 01 Mar 2022 21:11:19 GMT  
		Size: 8.0 MB (8045288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14147c502377cab1687da8ffe8690af66a433bc02ce32d4edc1c8c378128f08`  
		Last Modified: Tue, 01 Mar 2022 21:11:17 GMT  
		Size: 448.0 KB (448000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b5c7b74e7e0aee90408523c23b27f5fd8b04f664d0d75305d0cf08495acabc`  
		Last Modified: Tue, 01 Mar 2022 21:11:16 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc7b1ae3f96cce18af6e190b163f663016803b3eac0081ad0110864ce4ad29b`  
		Last Modified: Tue, 01 Mar 2022 21:11:16 GMT  
		Size: 3.2 KB (3193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50f9cbc2b1fba00b064bb5cb37bd8091e17f68868089ebae6cad1f3adaf5fbc`  
		Last Modified: Tue, 01 Mar 2022 21:13:31 GMT  
		Size: 90.2 MB (90239884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f4db98730af97d4f74aac8b05b047c947d48dea4bba8fc4fddf5648cf1480e`  
		Last Modified: Tue, 01 Mar 2022 21:13:03 GMT  
		Size: 9.0 KB (9031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d141089e80ea3e5f7960dd8866305ac1e8c8dc0fe17d39fcf97dfa1f35c00a`  
		Last Modified: Tue, 01 Mar 2022 21:13:03 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af953fa29418a4f43efe0f34f8b66e70c9515f270e2b9f783fcdef0661d647b`  
		Last Modified: Tue, 01 Mar 2022 21:13:03 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa6bc19881b715351dd4d44c98845580ecd17e6b9f336658ba155dd79de3bf9`  
		Last Modified: Tue, 01 Mar 2022 21:13:03 GMT  
		Size: 4.7 KB (4687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-bullseye` - linux; mips64le

```console
$ docker pull postgres@sha256:0f55347608cc26acadd6a323f740a7caa6c6e1dbace5da13f3097d127f85eaab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.7 MB (129708840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c46ddaac741c635a9cc8bb1564813b5840e5f02576c0a205a2f3ef9bd78d4c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:49 GMT
ADD file:1901e1e1292cbfcd557262ec5d08551cecd0070b24928414d220472664fe3fdf in / 
# Tue, 01 Mar 2022 02:02:49 GMT
CMD ["bash"]
# Sat, 05 Mar 2022 09:10:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 05 Mar 2022 09:11:03 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Sat, 05 Mar 2022 09:11:05 GMT
ENV GOSU_VERSION=1.14
# Sat, 05 Mar 2022 09:11:39 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 05 Mar 2022 09:12:11 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Sat, 05 Mar 2022 09:12:14 GMT
ENV LANG=en_US.utf8
# Sat, 05 Mar 2022 09:12:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 05 Mar 2022 09:12:38 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Sat, 05 Mar 2022 09:12:45 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Sat, 05 Mar 2022 11:12:10 GMT
ENV PG_MAJOR=12
# Sat, 05 Mar 2022 11:12:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Sat, 05 Mar 2022 11:12:16 GMT
ENV PG_VERSION=12.10-1.pgdg110+1
# Sat, 05 Mar 2022 12:07:11 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Sat, 05 Mar 2022 12:07:19 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Sat, 05 Mar 2022 12:07:26 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Sat, 05 Mar 2022 12:07:29 GMT
ENV PGDATA=/var/lib/postgresql/data
# Sat, 05 Mar 2022 12:07:36 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Sat, 05 Mar 2022 12:07:39 GMT
VOLUME [/var/lib/postgresql/data]
# Sat, 05 Mar 2022 12:07:42 GMT
COPY file:a089d0b5bcabd9529434672fbf8e8d3378ce1f734b4596df5c20c565589c8f01 in /usr/local/bin/ 
# Sat, 05 Mar 2022 12:07:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 05 Mar 2022 12:07:49 GMT
STOPSIGNAL SIGINT
# Sat, 05 Mar 2022 12:07:53 GMT
EXPOSE 5432
# Sat, 05 Mar 2022 12:07:56 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:3baeb8c34a522fc616f97412d47dc1f665e93552c57aa8237ee1d673f9757cba`  
		Last Modified: Tue, 01 Mar 2022 02:12:25 GMT  
		Size: 29.6 MB (29632966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0723f4f433f2e6d4a82db9f1cf76b246b9d5a301aead35adf8939524deb81b6c`  
		Last Modified: Sat, 05 Mar 2022 13:42:40 GMT  
		Size: 4.2 MB (4196094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4101a9cd5400ceac1f1f17e525dde1982898c0a3937660091a63b3dfd6b78575`  
		Last Modified: Sat, 05 Mar 2022 13:42:36 GMT  
		Size: 1.7 KB (1656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df983545939c4e78054ee7bc09d6ba13a8e3d146386b65a87b5e3a771d5a11f2`  
		Last Modified: Sat, 05 Mar 2022 13:42:37 GMT  
		Size: 1.3 MB (1297927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08575fe34eccc6bd543bcfb24bf76bf7136f932432d63e33c1d66d0bda20a821`  
		Last Modified: Sat, 05 Mar 2022 13:42:41 GMT  
		Size: 8.0 MB (8043969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1c7d906d7bcffcbefc21b3055d8ce9fa536f5cdf2125c9fb7c2df34a3d863e`  
		Last Modified: Sat, 05 Mar 2022 13:42:34 GMT  
		Size: 215.6 KB (215645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb02c2ad9199989bc00c2a55e1a8736b774e9de250cd6d205b06ca4da746e679`  
		Last Modified: Sat, 05 Mar 2022 13:42:34 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1690e4f0f2d03947e2f735c9f5b04c36f77132234103714dd4c0896bf1c774d1`  
		Last Modified: Sat, 05 Mar 2022 13:42:34 GMT  
		Size: 3.1 KB (3146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58644ae333dafc39a44f6d079e3d44ea498f7ced90b1749b1b611fd5cd9ccc9d`  
		Last Modified: Sat, 05 Mar 2022 13:46:01 GMT  
		Size: 86.3 MB (86303311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c65abd27a92e06867451e09831077a5e3ba0065b05c9a437497669048dddc3`  
		Last Modified: Sat, 05 Mar 2022 13:45:05 GMT  
		Size: 9.0 KB (9033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c77d02c287e0a7e0ffbd311839a5dd0e9667b54d13d7659ad724196ef51e21`  
		Last Modified: Sat, 05 Mar 2022 13:45:05 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5799c4c58df07713a9dac493a647c3aaefdad88ebd5f5ee9008be4ccbf9f0497`  
		Last Modified: Sat, 05 Mar 2022 13:45:05 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ebea5589c1b72d59eb96dcdf183d6f603a44a0561bf241d7a26161c6a02f9d`  
		Last Modified: Sat, 05 Mar 2022 13:45:05 GMT  
		Size: 4.7 KB (4679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-bullseye` - linux; ppc64le

```console
$ docker pull postgres@sha256:7f82f5f8ad74a25841953f88a640417da452300a90b13429d2051f1c1964b332
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.0 MB (145013354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf0a2128cd9ee4a84ec3dbbd026fd9ef2d47413a8126ab1e518e9ed3c763b400`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 01 Mar 2022 02:05:07 GMT
ADD file:fc0989685aecf50ec36795d73893c30d9ddd4f946f8c5f4a6d10963f8ab41168 in / 
# Tue, 01 Mar 2022 02:05:12 GMT
CMD ["bash"]
# Tue, 08 Mar 2022 20:21:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 08 Mar 2022 20:21:24 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 08 Mar 2022 20:21:26 GMT
ENV GOSU_VERSION=1.14
# Tue, 08 Mar 2022 20:22:07 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 08 Mar 2022 20:22:35 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 08 Mar 2022 20:22:39 GMT
ENV LANG=en_US.utf8
# Tue, 08 Mar 2022 20:22:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Mar 2022 20:23:03 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 08 Mar 2022 20:23:43 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 08 Mar 2022 20:41:03 GMT
ENV PG_MAJOR=12
# Tue, 08 Mar 2022 20:41:05 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Tue, 08 Mar 2022 20:41:07 GMT
ENV PG_VERSION=12.10-1.pgdg110+1
# Tue, 08 Mar 2022 20:42:16 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 08 Mar 2022 20:42:27 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 08 Mar 2022 20:42:33 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 08 Mar 2022 20:42:36 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 08 Mar 2022 20:42:48 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 08 Mar 2022 20:42:52 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 08 Mar 2022 20:42:54 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Tue, 08 Mar 2022 20:42:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Mar 2022 20:43:06 GMT
STOPSIGNAL SIGINT
# Tue, 08 Mar 2022 20:43:10 GMT
EXPOSE 5432
# Tue, 08 Mar 2022 20:43:18 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:1dde9239ed493e1fe68971baa3f162c734ef0f461ad109e48aeb5b56daa55cc2`  
		Last Modified: Tue, 01 Mar 2022 02:15:19 GMT  
		Size: 35.3 MB (35272910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0e85213528e5b1c423313246151a8d6a58e3d67eedd84746343889730540ab`  
		Last Modified: Tue, 08 Mar 2022 21:07:55 GMT  
		Size: 5.2 MB (5222894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a6eecd8da99a07dcd22c818b8944cca56eb2425bb74a0b1788506338cc4014`  
		Last Modified: Tue, 08 Mar 2022 21:07:54 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990df2a870a68870e1efde36dbb968126ba2543322d47e9044918977292f3548`  
		Last Modified: Tue, 08 Mar 2022 21:07:54 GMT  
		Size: 1.3 MB (1317512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbba78f49993926ce32bd3a36996713b6b6ba615d37adbe7be7f24818c63853`  
		Last Modified: Tue, 08 Mar 2022 21:07:51 GMT  
		Size: 8.0 MB (8045522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0a796a29c72c6f00ba59564e443fab5e953d579b7ea82e0b0a01000db00601`  
		Last Modified: Tue, 08 Mar 2022 21:07:50 GMT  
		Size: 1.4 MB (1420022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66cd0b15e82b9b53b38c5fb3ffaa29ea58f94d110072805fa9b5dea7661d07ce`  
		Last Modified: Tue, 08 Mar 2022 21:07:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66cfc6792d39803affcf94f317e1abb83b2f0c1bfac19361eb1135fb15d5fe39`  
		Last Modified: Tue, 08 Mar 2022 21:07:49 GMT  
		Size: 3.2 KB (3201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d947f561232e66bd222883772de9ee1c4b6992cf11d4df0a661a81d3aad2f5e4`  
		Last Modified: Tue, 08 Mar 2022 21:11:08 GMT  
		Size: 93.7 MB (93715280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14fb57317a40cdfa62f9e7b190795464c793e34e3228c3fa870e47b599f35efd`  
		Last Modified: Tue, 08 Mar 2022 21:10:52 GMT  
		Size: 9.0 KB (9034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d94ccef3a24335463dd51e4956f26b67d484599f528daa1e2eb83cd5cc4a9d`  
		Last Modified: Tue, 08 Mar 2022 21:10:52 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd502a76fc7a97c05e523bc086bdbf694919df9e50033b13cdaa29bbe4051804`  
		Last Modified: Tue, 08 Mar 2022 21:10:52 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4738370fbf790af6c3daf1498a64cff6cc80d394bf28980b129aad89d73cdb6f`  
		Last Modified: Tue, 08 Mar 2022 21:10:52 GMT  
		Size: 4.7 KB (4694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:12-bullseye` - linux; s390x

```console
$ docker pull postgres@sha256:d92bb03cf505ad71929093f10d549fb75c7b1c0391a64ca56df28436e9f968ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.9 MB (139907478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdaa10f32ef1739391ed52eedc0a56d1ed2a4f4a8d958705169dbdd2323e1200`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 01 Mar 2022 02:01:56 GMT
ADD file:d869ad3392a4e752c2f73d08a4cc13594c94bfc050bd037db0ca9827a0207072 in / 
# Tue, 01 Mar 2022 02:01:58 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 09:28:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 09:28:32 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 01 Mar 2022 09:28:32 GMT
ENV GOSU_VERSION=1.14
# Tue, 01 Mar 2022 09:28:39 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 01 Mar 2022 09:28:44 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 01 Mar 2022 09:28:44 GMT
ENV LANG=en_US.utf8
# Tue, 08 Mar 2022 19:48:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 08 Mar 2022 19:48:01 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 08 Mar 2022 19:48:32 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Tue, 08 Mar 2022 20:11:04 GMT
ENV PG_MAJOR=12
# Tue, 08 Mar 2022 20:11:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/12/bin
# Tue, 08 Mar 2022 20:11:04 GMT
ENV PG_VERSION=12.10-1.pgdg110+1
# Tue, 08 Mar 2022 20:19:29 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Tue, 08 Mar 2022 20:19:34 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Tue, 08 Mar 2022 20:19:34 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Tue, 08 Mar 2022 20:19:34 GMT
ENV PGDATA=/var/lib/postgresql/data
# Tue, 08 Mar 2022 20:19:35 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Tue, 08 Mar 2022 20:19:35 GMT
VOLUME [/var/lib/postgresql/data]
# Tue, 08 Mar 2022 20:19:35 GMT
COPY file:3cf28939740c4fc7f2787c08c792133ea7778bcbe5a7254c7efea56f5632f447 in /usr/local/bin/ 
# Tue, 08 Mar 2022 20:19:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Mar 2022 20:19:35 GMT
STOPSIGNAL SIGINT
# Tue, 08 Mar 2022 20:19:35 GMT
EXPOSE 5432
# Tue, 08 Mar 2022 20:19:35 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:f81abce72636770dac4258df46a31beeb6ad81dfddd5b7c9c3fa6942ea074922`  
		Last Modified: Tue, 01 Mar 2022 02:07:33 GMT  
		Size: 29.6 MB (29647132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698e138de522667672d3e84217958de2dd58a50712d15173bc0bd9f30adba1bd`  
		Last Modified: Tue, 01 Mar 2022 10:10:45 GMT  
		Size: 4.3 MB (4302232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0256592c5dd42dac3807b9e4a2ee334c2f7c44b14f75ea31ca8f9611354b61f8`  
		Last Modified: Tue, 01 Mar 2022 10:10:44 GMT  
		Size: 1.8 KB (1802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7045923fdfa4b1f9d44a19502611c5a20a63610a25f20005fa91a19741d9fcb4`  
		Last Modified: Tue, 01 Mar 2022 10:10:44 GMT  
		Size: 1.4 MB (1381418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4412b9ae2c221ffd8c8c5cd4ff5b02da42dfd05f8081edda6d2387c302a3c391`  
		Last Modified: Tue, 01 Mar 2022 10:10:44 GMT  
		Size: 8.1 MB (8099061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d0bf97f125d18c9b7e3fd35e7b91680e7e7b16846b89d69059fd0485845bf3`  
		Last Modified: Tue, 08 Mar 2022 20:44:02 GMT  
		Size: 1.2 MB (1237640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c153a5a318990f24067c3f59e8cce3113b8113aaa6b3acc615394bb7fe3735`  
		Last Modified: Tue, 08 Mar 2022 20:44:02 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d07d41d32515d5e98659ff3df8e0cda9a900d048be6cad1d575efea8f24a61`  
		Last Modified: Tue, 08 Mar 2022 20:44:02 GMT  
		Size: 3.2 KB (3204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa41f4928d52b8532c795ffc24dd1113c0518b52e1c57ab7493dbb9a98e50f5b`  
		Last Modified: Tue, 08 Mar 2022 20:45:43 GMT  
		Size: 95.2 MB (95220779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4ec2f82b3673997204ac2453249832ad5979a7491a335b9501c65ea5f3d026`  
		Last Modified: Tue, 08 Mar 2022 20:45:32 GMT  
		Size: 9.0 KB (9036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e03e9ab0559a62db71a1bc58020e82eb93dcb8f8eee6e9986c5b6dcbac65098`  
		Last Modified: Tue, 08 Mar 2022 20:45:32 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb122fce79eacdfabb506593b7f28d0c0fed7c6b33fc0f2d422da43b2fc1b07`  
		Last Modified: Tue, 08 Mar 2022 20:45:32 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08175eeb08d1e3d9f5c9dcc1a0e4770223299ff92a6ab55a16a17b9eac729e36`  
		Last Modified: Tue, 08 Mar 2022 20:45:32 GMT  
		Size: 4.7 KB (4694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
