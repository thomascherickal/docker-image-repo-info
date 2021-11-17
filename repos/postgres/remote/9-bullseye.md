## `postgres:9-bullseye`

```console
$ docker pull postgres@sha256:389cbf94445d807ce91ee421d9659b94d7dbfd580a00e1046c8448324ccbae15
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

### `postgres:9-bullseye` - linux; amd64

```console
$ docker pull postgres@sha256:2bc295a7fa5b573929a8f845471f64395dab8a4b84378b43b8c56f8294690ad9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.9 MB (84872069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a88b2dfdaad0b893629458cce4ceee2f7e9c3701a32239a15b2a045249a2c033`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:42 GMT
ADD file:16dc2c6d1932194edec28d730b004fd6deca3d0f0e1a07bc5b8b6e8a1662f7af in / 
# Tue, 12 Oct 2021 01:20:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 12:16:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 12:16:10 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 12 Oct 2021 12:16:10 GMT
ENV GOSU_VERSION=1.12
# Tue, 12 Oct 2021 12:16:24 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Oct 2021 12:16:33 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 12 Oct 2021 12:16:33 GMT
ENV LANG=en_US.utf8
# Tue, 12 Oct 2021 12:16:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:16:40 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 12 Oct 2021 12:16:49 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 12 Oct 2021 12:22:29 GMT
ENV PG_MAJOR=9.6
# Tue, 12 Oct 2021 12:22:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Thu, 11 Nov 2021 22:49:42 GMT
ENV PG_VERSION=9.6.24-1.pgdg110+1
# Thu, 11 Nov 2021 22:49:59 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 11 Nov 2021 22:50:00 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 11 Nov 2021 22:50:01 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 11 Nov 2021 22:50:01 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 11 Nov 2021 22:50:02 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 11 Nov 2021 22:50:02 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 11 Nov 2021 22:50:02 GMT
COPY file:73785d4a64e88cd001941f2d0fb17c583e6d98ffda704b27106f5ef128737e5b in /usr/local/bin/ 
# Thu, 11 Nov 2021 22:50:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 11 Nov 2021 22:50:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Nov 2021 22:50:04 GMT
STOPSIGNAL SIGINT
# Thu, 11 Nov 2021 22:50:04 GMT
EXPOSE 5432
# Thu, 11 Nov 2021 22:50:04 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:7d63c13d9b9b6ec5f05a2b07daadacaa9c610d01102a662ae9b1d082105f1ffa`  
		Last Modified: Tue, 12 Oct 2021 01:26:05 GMT  
		Size: 31.4 MB (31357311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad0f9d5f5fe21c0fa3ac99c08cf068480bdd2ebc09adce4b81767b0df509bd7`  
		Last Modified: Tue, 12 Oct 2021 12:24:27 GMT  
		Size: 4.4 MB (4414499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff74a7a559cbdfbf9d23234053849d1056dae0e2e7f69671d5bec47661a0d4ef`  
		Last Modified: Tue, 12 Oct 2021 12:24:25 GMT  
		Size: 1.8 KB (1799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43dfd845683c4cebbcd3cbdb95bf611fc7a7e88ce3fc709c9675380153a9379`  
		Last Modified: Tue, 12 Oct 2021 12:24:25 GMT  
		Size: 1.5 MB (1450540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e554331369f5844d7ddd374c4536d8e26d0ef0df5d35ff87993f2c8fe6eb74bd`  
		Last Modified: Tue, 12 Oct 2021 12:24:25 GMT  
		Size: 8.0 MB (8045166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25d54a3ac3a7d1bae47256b879f56f92f3f36ef4801e6d5f27300b1449d5035`  
		Last Modified: Tue, 12 Oct 2021 12:24:23 GMT  
		Size: 441.6 KB (441564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc6df00588cd9e292196b96ffb30750e92b07f02165662b35a21a3ae965c291`  
		Last Modified: Tue, 12 Oct 2021 12:24:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4deb2e8648094c506b62bb26ea709e6845b5ab79bef7820be29f959a4ebf8e0`  
		Last Modified: Tue, 12 Oct 2021 12:24:23 GMT  
		Size: 3.1 KB (3051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c219883cc8500d7a0a9c660c94619ca18787f6583fae85456a16c1a347f136`  
		Last Modified: Thu, 11 Nov 2021 23:00:51 GMT  
		Size: 39.1 MB (39144954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f17993adc6a80ccf60dcee220bb21a8c31aa35a22587ee335b81ff6d2bd724`  
		Last Modified: Thu, 11 Nov 2021 23:00:41 GMT  
		Size: 7.9 KB (7867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1befec750b045210f69ed4a914ae8f5a23f95e26019ccaecf5a576c8ab56686`  
		Last Modified: Thu, 11 Nov 2021 23:00:41 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f275a480b1e47ab15794ab580d27462251a7c63a024dc845b4c7d2a8a1b015b`  
		Last Modified: Thu, 11 Nov 2021 23:00:41 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a6b40bcc8b16db3594e786a9846c64626fadd059941e431ff551b658ca5e5c`  
		Last Modified: Thu, 11 Nov 2021 23:00:42 GMT  
		Size: 4.7 KB (4719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315ea279429a81c2a9b7894e28ef46ed166eadd04271bf6e4ab42894bfb36b6b`  
		Last Modified: Thu, 11 Nov 2021 23:00:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-bullseye` - linux; arm variant v5

```console
$ docker pull postgres@sha256:9c015810fab94f29e92961979264ebc189d4ecaaeba8c5e3df16971938113c74
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.8 MB (80776602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c393c7db8ece82dbbafe90788337e8ae28c5e8537f7ca11efed2f3a48039952`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 17 Nov 2021 02:50:37 GMT
ADD file:738a04a17bdb9077594ad9a847333abe28216a7f04d3058718a5e21c236c24bb in / 
# Wed, 17 Nov 2021 02:50:38 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 07:04:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 07:04:32 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 17 Nov 2021 07:04:32 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Nov 2021 07:04:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Nov 2021 07:05:18 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 17 Nov 2021 07:05:19 GMT
ENV LANG=en_US.utf8
# Wed, 17 Nov 2021 07:05:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 07:05:31 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Nov 2021 07:05:35 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Wed, 17 Nov 2021 10:47:00 GMT
ENV PG_MAJOR=9.6
# Wed, 17 Nov 2021 10:47:00 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Wed, 17 Nov 2021 10:47:01 GMT
ENV PG_VERSION=9.6.24-1.pgdg110+1
# Wed, 17 Nov 2021 11:09:21 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 17 Nov 2021 11:09:23 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 17 Nov 2021 11:09:25 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 17 Nov 2021 11:09:25 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 17 Nov 2021 11:09:27 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 17 Nov 2021 11:09:27 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 17 Nov 2021 11:09:28 GMT
COPY file:73785d4a64e88cd001941f2d0fb17c583e6d98ffda704b27106f5ef128737e5b in /usr/local/bin/ 
# Wed, 17 Nov 2021 11:09:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 17 Nov 2021 11:09:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 11:09:30 GMT
STOPSIGNAL SIGINT
# Wed, 17 Nov 2021 11:09:31 GMT
EXPOSE 5432
# Wed, 17 Nov 2021 11:09:31 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:a960a56baa1baffbe2aa1e0c1fb02f9ee4816337d02fec259b312c409d77fafc`  
		Last Modified: Wed, 17 Nov 2021 03:06:09 GMT  
		Size: 28.9 MB (28911006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2ac9e3ed26a54de75a39a02c813343c2f2da6d330db5aedec6ce0c53224e9c`  
		Last Modified: Wed, 17 Nov 2021 11:38:04 GMT  
		Size: 4.1 MB (4096446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940c573b71bfb0dc5d6257ac0a038c717a7659ce616e33ce43ab01fe09be44ec`  
		Last Modified: Wed, 17 Nov 2021 11:38:01 GMT  
		Size: 1.8 KB (1791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2545e4aff5b41c80c355e8088b768e10f7848e4652b57e0c6d48639489f88ec`  
		Last Modified: Wed, 17 Nov 2021 11:38:02 GMT  
		Size: 1.4 MB (1409841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab777c351898461b61f20cbcf50cfa59138624e65d888861239e5ac45a1fdb8`  
		Last Modified: Wed, 17 Nov 2021 11:38:05 GMT  
		Size: 8.0 MB (8045268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0164b8561fc75365f2de2e4e19f1158cb443328ceea58ce251c7dea783bd89b5`  
		Last Modified: Wed, 17 Nov 2021 11:38:00 GMT  
		Size: 439.8 KB (439832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592ecb945403cba2d03a3ffc6503faef393710ceb4ceda8c441c5ba42ccd2dcf`  
		Last Modified: Wed, 17 Nov 2021 11:37:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:917bd638f9752fef8f0ce6e3b4b327079b3e3f574a92901d04196a8161454044`  
		Last Modified: Wed, 17 Nov 2021 11:37:59 GMT  
		Size: 3.1 KB (3056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21b1a96ceab1f951886cd848b37aa09fe3b03ad66c08c49e1cb166b0559dba7`  
		Last Modified: Wed, 17 Nov 2021 11:45:38 GMT  
		Size: 37.9 MB (37856165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768bd613953c1e1217980b912e5bbdd2268651efb7668b660066fec7fddd61aa`  
		Last Modified: Wed, 17 Nov 2021 11:45:13 GMT  
		Size: 7.9 KB (7875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0b4108c3089b6eb5424c33b9935212960a0a0eb86924749dd7aff59886999d`  
		Last Modified: Wed, 17 Nov 2021 11:45:14 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676e844ec2472a1f36608ddd0782db1abbff2c8d466293dc89ef7e04a3bd3be0`  
		Last Modified: Wed, 17 Nov 2021 11:45:13 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:820b9def578bffba2e1b5798355469083ac5e704c60b6f2be7e525a95ed9526e`  
		Last Modified: Wed, 17 Nov 2021 11:45:13 GMT  
		Size: 4.7 KB (4721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161fda7ba00e723c297d9d828ea8ab9c960e10a42bee008b1f38d78c9caf05c2`  
		Last Modified: Wed, 17 Nov 2021 11:45:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-bullseye` - linux; arm variant v7

```console
$ docker pull postgres@sha256:cec32a7f4a81f818a25568e605c6ffd5b0889b4e4e5fc1ddbd8f8b890d178358
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77083189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6e06a502a7f0c8ac4c8f8162ba3c1e8a98334316ba628cb110a9fe0d7cafa77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 12 Oct 2021 01:28:36 GMT
ADD file:89eac94007ac04f9168737686fa0a6c737f2c28fc9e5918d4d512924fe1973be in / 
# Tue, 12 Oct 2021 01:28:37 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 19:45:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 19:45:19 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 12 Oct 2021 19:45:20 GMT
ENV GOSU_VERSION=1.12
# Tue, 12 Oct 2021 19:45:39 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Oct 2021 19:45:59 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 12 Oct 2021 19:45:59 GMT
ENV LANG=en_US.utf8
# Tue, 12 Oct 2021 19:46:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 19:46:10 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 12 Oct 2021 19:46:18 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 12 Oct 2021 23:07:09 GMT
ENV PG_MAJOR=9.6
# Tue, 12 Oct 2021 23:07:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Fri, 12 Nov 2021 04:24:49 GMT
ENV PG_VERSION=9.6.24-1.pgdg110+1
# Fri, 12 Nov 2021 04:45:20 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 12 Nov 2021 04:45:23 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 12 Nov 2021 04:45:24 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 12 Nov 2021 04:45:25 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 12 Nov 2021 04:45:26 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 12 Nov 2021 04:45:27 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 12 Nov 2021 04:45:27 GMT
COPY file:73785d4a64e88cd001941f2d0fb17c583e6d98ffda704b27106f5ef128737e5b in /usr/local/bin/ 
# Fri, 12 Nov 2021 04:45:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 12 Nov 2021 04:45:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 04:45:30 GMT
STOPSIGNAL SIGINT
# Fri, 12 Nov 2021 04:45:30 GMT
EXPOSE 5432
# Fri, 12 Nov 2021 04:45:31 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:4e5300249f84466df4dc73ea0ce09938ca00c1718bb12619c4f26bd936162331`  
		Last Modified: Tue, 12 Oct 2021 01:44:28 GMT  
		Size: 26.6 MB (26561058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97cba707aae3987e29b0a8890362bb7f8aeb98e2b95d2ead33fb2a0e6026721a`  
		Last Modified: Tue, 12 Oct 2021 23:55:46 GMT  
		Size: 3.7 MB (3717133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdb41d616591151f010658ddfaf59999a7e915a2ca3555f2fc87bf162dd9306`  
		Last Modified: Tue, 12 Oct 2021 23:55:44 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6032407c0d7c3ab05ba475ed2ba7c9a7dbdaedfb04fab35e2e7a5ce40d3a33b6`  
		Last Modified: Tue, 12 Oct 2021 23:55:44 GMT  
		Size: 1.4 MB (1402411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afb522a8b87e3489e1108844c8598a6d0a0c905ba159060d0bcba643e58cd0c`  
		Last Modified: Tue, 12 Oct 2021 23:55:48 GMT  
		Size: 8.0 MB (8045250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b26989d9dd05a24ab44e3cfbf09e139fe7c6364fee7bfaed7b34c1dec78d01`  
		Last Modified: Tue, 12 Oct 2021 23:55:42 GMT  
		Size: 434.5 KB (434519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51d834dc810ead99fd22be336ececec175225a25a7dbcf1824eef9e9b00a59d`  
		Last Modified: Tue, 12 Oct 2021 23:55:42 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d15c7b10005bfdc938618081172d76fe94133713590cf57d0a6069ce2e0697a`  
		Last Modified: Tue, 12 Oct 2021 23:55:42 GMT  
		Size: 3.1 KB (3056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c467acad975fcc2bec9b8d8415e3339fb5a270512cbd2543bbeed7c36718e7cf`  
		Last Modified: Fri, 12 Nov 2021 05:28:34 GMT  
		Size: 36.9 MB (36904779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e246f732686773aeb0c8e1b9413f46de4964d04ad38ac9d4e72952af084e586`  
		Last Modified: Fri, 12 Nov 2021 05:28:07 GMT  
		Size: 7.9 KB (7874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:308646eb87fdbc711f3a1dcb040752da25266b41625374528eeaa82c4efccdfc`  
		Last Modified: Fri, 12 Nov 2021 05:28:07 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32e63891dbe322c3285e1c11567501ce0583f4c19fba692de0470d6f627ce68`  
		Last Modified: Fri, 12 Nov 2021 05:28:07 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6752342921e8b7c0a720c3cf406cc3d1085b7d4b8f2e3078436a8f86567d1fde`  
		Last Modified: Fri, 12 Nov 2021 05:28:07 GMT  
		Size: 4.7 KB (4720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9fa5ef3f8b7ca937ba9acb2af38fc888edbacd7d9a952d33270a1a3c40eaab6`  
		Last Modified: Fri, 12 Nov 2021 05:28:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-bullseye` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:3b87505f5a9c4a01b19ebad5e2be2d5852365777ce3665949d0ca56e29d95d6b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.8 MB (82830727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2915c31cafe66dbd57d093df2be41ec3f3ffd046df6a2092960f4a87a3af7c4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:15 GMT
ADD file:4203242b2b09a65239092c4780b59181da7b861b3c0be40810b3588aa200f72c in / 
# Wed, 17 Nov 2021 02:40:16 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 10:56:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 10:56:35 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 17 Nov 2021 10:56:36 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Nov 2021 10:56:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Nov 2021 10:56:52 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 17 Nov 2021 10:56:53 GMT
ENV LANG=en_US.utf8
# Wed, 17 Nov 2021 10:56:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 10:56:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Nov 2021 10:57:05 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Wed, 17 Nov 2021 11:22:24 GMT
ENV PG_MAJOR=9.6
# Wed, 17 Nov 2021 11:22:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Wed, 17 Nov 2021 11:22:26 GMT
ENV PG_VERSION=9.6.24-1.pgdg110+1
# Wed, 17 Nov 2021 11:22:41 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 17 Nov 2021 11:22:42 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 17 Nov 2021 11:22:43 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 17 Nov 2021 11:22:44 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 17 Nov 2021 11:22:45 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 17 Nov 2021 11:22:46 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 17 Nov 2021 11:22:48 GMT
COPY file:73785d4a64e88cd001941f2d0fb17c583e6d98ffda704b27106f5ef128737e5b in /usr/local/bin/ 
# Wed, 17 Nov 2021 11:22:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 17 Nov 2021 11:22:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 11:22:50 GMT
STOPSIGNAL SIGINT
# Wed, 17 Nov 2021 11:22:51 GMT
EXPOSE 5432
# Wed, 17 Nov 2021 11:22:52 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:eb9a2845ed124d072b117aba4f0508e00c1ecd0d147dc324d14b00d24092046c`  
		Last Modified: Wed, 17 Nov 2021 02:47:17 GMT  
		Size: 30.1 MB (30056521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0a8f5dc8469747b817020b211885445957c2ebbb768fc67891799e36e47cb8`  
		Last Modified: Wed, 17 Nov 2021 11:35:10 GMT  
		Size: 4.2 MB (4208882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d8025a640ac47adb95ca00802aa24eee591c5cf682195cd62eed14df139a1e`  
		Last Modified: Wed, 17 Nov 2021 11:35:09 GMT  
		Size: 1.6 KB (1649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d76080820eaf4434ad6a27aa329f5470b8f0a84db83709240b2effda215888`  
		Last Modified: Wed, 17 Nov 2021 11:35:09 GMT  
		Size: 1.4 MB (1386357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7ecf182a3e52de7c86a35c8b1e09d8fe1934ef7eefc56b305f2a36b3eb305a`  
		Last Modified: Wed, 17 Nov 2021 11:35:08 GMT  
		Size: 8.0 MB (8043386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f006f2874091466c12bfce62b64b72df9259372caae65b4541532aac1acfb9cb`  
		Last Modified: Wed, 17 Nov 2021 11:35:07 GMT  
		Size: 218.6 KB (218596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f107f00cd284556028168c8f445cc3e6f9c255cee49d1f2135a46e9b6ea9a0`  
		Last Modified: Wed, 17 Nov 2021 11:35:07 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377bbaec8727cb50aa749bb95f8d0b2690979eb4de1e753079c74667e9ec1262`  
		Last Modified: Wed, 17 Nov 2021 11:35:06 GMT  
		Size: 3.0 KB (3033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9270898cfc3fe870d2bad9baa06c326d3fa20db496debf96c1bddba841b23db0`  
		Last Modified: Wed, 17 Nov 2021 11:38:47 GMT  
		Size: 38.9 MB (38899168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7469c1402568308844543003e63ae96bf3207dfdd065d1e9f85effee8185f893`  
		Last Modified: Wed, 17 Nov 2021 11:38:38 GMT  
		Size: 7.9 KB (7880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f38fa7b872c632cdc501a3204af3cd2678001ca168b61097ffed4b33767e15`  
		Last Modified: Wed, 17 Nov 2021 11:38:38 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbf8845c117ad860aece270d647e45feb822b8a6da61c0ce347ed6eb00db86c`  
		Last Modified: Wed, 17 Nov 2021 11:38:38 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d452380b6dc3a4505ee54e6c9a88d10477727bad143255f502d46c007b0f18a`  
		Last Modified: Wed, 17 Nov 2021 11:38:39 GMT  
		Size: 4.7 KB (4718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:487246caedac3123f0629a09b8a48131a3ffe4b06049e9fb4ced11de41d61061`  
		Last Modified: Wed, 17 Nov 2021 11:38:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-bullseye` - linux; 386

```console
$ docker pull postgres@sha256:af5215556d8374fa39418f6f25f7fe07ff905a9735bf0e4ee00657476ebeb6c6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.6 MB (86587289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:891fa3b0214979b3910f6bd3636d2e61de00a0af58cdf05b3c88315e022e6193`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 12 Oct 2021 01:39:47 GMT
ADD file:42196ffa4c70af8d9f1e7b74edb3bb92d47296acf989adf615e8208230f8bd0c in / 
# Tue, 12 Oct 2021 01:39:47 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:43:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 16:43:33 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 12 Oct 2021 16:43:33 GMT
ENV GOSU_VERSION=1.12
# Tue, 12 Oct 2021 16:43:43 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Oct 2021 16:43:52 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 12 Oct 2021 16:43:52 GMT
ENV LANG=en_US.utf8
# Tue, 12 Oct 2021 16:43:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:43:58 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 12 Oct 2021 16:44:07 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 12 Oct 2021 17:56:46 GMT
ENV PG_MAJOR=9.6
# Tue, 12 Oct 2021 17:56:46 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Fri, 12 Nov 2021 01:15:20 GMT
ENV PG_VERSION=9.6.24-1.pgdg110+1
# Fri, 12 Nov 2021 01:24:59 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 12 Nov 2021 01:25:00 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 12 Nov 2021 01:25:01 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 12 Nov 2021 01:25:01 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 12 Nov 2021 01:25:03 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 12 Nov 2021 01:25:03 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 12 Nov 2021 01:25:03 GMT
COPY file:73785d4a64e88cd001941f2d0fb17c583e6d98ffda704b27106f5ef128737e5b in /usr/local/bin/ 
# Fri, 12 Nov 2021 01:25:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 12 Nov 2021 01:25:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 01:25:05 GMT
STOPSIGNAL SIGINT
# Fri, 12 Nov 2021 01:25:05 GMT
EXPOSE 5432
# Fri, 12 Nov 2021 01:25:05 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:87318d165b5c0fdf05c8ccf97d83084f56b4608075a3335b1a46c76295b82753`  
		Last Modified: Tue, 12 Oct 2021 01:47:39 GMT  
		Size: 32.4 MB (32370344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ab187160d0847ea1ec672c159e4652606a33d6ac53e1816ac02dc97cefc33a`  
		Last Modified: Tue, 12 Oct 2021 18:09:23 GMT  
		Size: 4.8 MB (4812830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c68d74945aa5d3a843a3b94fe6bd21653c594d1b2ef8605506ae2ed2917bab`  
		Last Modified: Tue, 12 Oct 2021 18:09:20 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a8ab909d4ef7fb1ec08a61993371c7139b708b1281e3dfa919afac68ddcd0c`  
		Last Modified: Tue, 12 Oct 2021 18:09:21 GMT  
		Size: 1.4 MB (1420908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c14538c32215beb917823b160441889ddb7495eac8d152fd14c0beec4d394d`  
		Last Modified: Tue, 12 Oct 2021 18:09:21 GMT  
		Size: 8.0 MB (8045095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa5563cc4981619d36b455a2de82c6933337c1d2f846aed365d7d09e064e4a2`  
		Last Modified: Tue, 12 Oct 2021 18:09:19 GMT  
		Size: 448.0 KB (447955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a162ed101b940f05dd8d8b640c51b488072f773e109d8b189909050c2905b3`  
		Last Modified: Tue, 12 Oct 2021 18:09:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be68e76c56b5050145b971db5c0a9024251277ef45970cd6731ca51f939ea518`  
		Last Modified: Tue, 12 Oct 2021 18:09:18 GMT  
		Size: 3.1 KB (3057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17452def5b07b034397d9a51b766cd02a5f2d3e04797c9a6c33f38c097cd194c`  
		Last Modified: Fri, 12 Nov 2021 01:39:33 GMT  
		Size: 39.5 MB (39472119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb880bdf78275fa898fb73fccfdfe5a8b06b75bddf04fbfc9dceaab223178d66`  
		Last Modified: Fri, 12 Nov 2021 01:39:21 GMT  
		Size: 7.9 KB (7877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae7a3db0bbf34af77e0e5ec894ed3aaab0cd14188a5eb222cc689739194775d`  
		Last Modified: Fri, 12 Nov 2021 01:39:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8844effa7dacfc3e03419a539386941ae3e684852cac29c32f1a61b80ae85660`  
		Last Modified: Fri, 12 Nov 2021 01:39:21 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c20e4d02d11ca894cb4652783734a38b5afa7ed83509b0b3f5ea2feef4f5cd`  
		Last Modified: Fri, 12 Nov 2021 01:39:21 GMT  
		Size: 4.7 KB (4717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14cf58467ae120731ec4ad50a86e8f75b0f73e0b7b3fe7decf35a0575ae081b3`  
		Last Modified: Fri, 12 Nov 2021 01:39:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-bullseye` - linux; mips64le

```console
$ docker pull postgres@sha256:e591bae11b6dd3a3390a07e73e1d01523accf848fc8421cc1af56bfbfb2ab6c1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.1 MB (82060790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b483075b0eaf9b57f12b62c0394d2afdeb640b63437ad5051268ef9a504f6936`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 17 Nov 2021 02:10:13 GMT
ADD file:10bc783d286d0a800f59d5009e87ecb4651659c82cae1325132756c7c8b1dec0 in / 
# Wed, 17 Nov 2021 02:10:13 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:38:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:38:48 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 17 Nov 2021 03:38:48 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Nov 2021 03:39:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Nov 2021 03:39:33 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 17 Nov 2021 03:39:34 GMT
ENV LANG=en_US.utf8
# Wed, 17 Nov 2021 03:39:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:39:48 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Nov 2021 03:39:51 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Wed, 17 Nov 2021 07:45:16 GMT
ENV PG_MAJOR=9.6
# Wed, 17 Nov 2021 07:45:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Wed, 17 Nov 2021 07:45:17 GMT
ENV PG_VERSION=9.6.24-1.pgdg110+1
# Wed, 17 Nov 2021 08:19:36 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 17 Nov 2021 08:19:38 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 17 Nov 2021 08:19:40 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 17 Nov 2021 08:19:41 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 17 Nov 2021 08:19:43 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 17 Nov 2021 08:19:43 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 17 Nov 2021 08:19:44 GMT
COPY file:73785d4a64e88cd001941f2d0fb17c583e6d98ffda704b27106f5ef128737e5b in /usr/local/bin/ 
# Wed, 17 Nov 2021 08:19:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 17 Nov 2021 08:19:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 08:19:46 GMT
STOPSIGNAL SIGINT
# Wed, 17 Nov 2021 08:19:47 GMT
EXPOSE 5432
# Wed, 17 Nov 2021 08:19:47 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:08bca22fbffb4e58224e9e4f6a56f1ca5099c002b1aeb6181df63af308a3da58`  
		Last Modified: Wed, 17 Nov 2021 02:19:09 GMT  
		Size: 29.6 MB (29630388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173240a7e67fd44ecc0ad5edd818557628d50f00c5d2a5f3d580e0a2ac091610`  
		Last Modified: Wed, 17 Nov 2021 08:20:21 GMT  
		Size: 4.4 MB (4402817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5442a27e75e2c0fbbf3bcf39b1c33f75d31863490f96ba2f0f1921ef6da25caf`  
		Last Modified: Wed, 17 Nov 2021 08:20:17 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a05b937ee3b119c0e6374cd0714d487d3e7d316cd28fc27fb4e5f39db8599763`  
		Last Modified: Wed, 17 Nov 2021 08:20:18 GMT  
		Size: 1.3 MB (1339348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9fe5fe83dffd40efe580e890c0a431b321561937529823e2e956ac2f72caca7`  
		Last Modified: Wed, 17 Nov 2021 08:20:23 GMT  
		Size: 8.0 MB (8043928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03edfb8f51563dcfa34d0b6309748f3fdad25b9228618d34d46b730988e02ea8`  
		Last Modified: Wed, 17 Nov 2021 08:20:15 GMT  
		Size: 439.2 KB (439151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93775bff4a0726e00590a3612932eaf2ff62a0af78998a1f470019ab95d62158`  
		Last Modified: Wed, 17 Nov 2021 08:20:14 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a285cfb90ec68b7c4601ff2fd7ae8045d7ee5bb8d909ec598250ad0e8008586`  
		Last Modified: Wed, 17 Nov 2021 08:20:15 GMT  
		Size: 3.1 KB (3054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18efd40dfdb26efcff42424acaf7ded291df18ec9ff32c7994054f6326b609e6`  
		Last Modified: Wed, 17 Nov 2021 08:26:35 GMT  
		Size: 38.2 MB (38187208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356a49c48210c5f57417ddc20eb0e6866750a5e6c310d96dabfce793c8b5c237`  
		Last Modified: Wed, 17 Nov 2021 08:26:04 GMT  
		Size: 7.9 KB (7877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05fd6b4d0acb8bb2108517207b51f319b855a56c839584d9cace0552844e2a7d`  
		Last Modified: Wed, 17 Nov 2021 08:26:04 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f95f7c7db1ae96ce5d163cf12a7653edbc1cb17c95a389e36b8d0e1ebc03b5a`  
		Last Modified: Wed, 17 Nov 2021 08:26:04 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67348030d70371078225f0b41d323868fddea18acd15543a2b9938ac1d08884`  
		Last Modified: Wed, 17 Nov 2021 08:26:04 GMT  
		Size: 4.7 KB (4717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3bd3188b11dde87f68fb85a8578b5c812974f2fa287fc88a58bd961a3d97cea`  
		Last Modified: Wed, 17 Nov 2021 08:26:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-bullseye` - linux; ppc64le

```console
$ docker pull postgres@sha256:f730486d95e66282cdc278b40648c67a50ba7b06bcb76bdac1108b65c3488ada
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.1 MB (91093591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:884a042655ff6db32d48ea3e2ecfdd4399f8bfc5b3d6a68de8586c906829f142`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 12 Oct 2021 01:25:45 GMT
ADD file:d8794fadf16c9948c3574ba28740d08393eca57766340333ad91f9c2a33eb719 in / 
# Tue, 12 Oct 2021 01:25:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 14:55:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 14:55:19 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 12 Oct 2021 14:55:25 GMT
ENV GOSU_VERSION=1.12
# Tue, 12 Oct 2021 14:56:03 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Oct 2021 14:56:32 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 12 Oct 2021 14:56:37 GMT
ENV LANG=en_US.utf8
# Tue, 12 Oct 2021 14:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 14:57:02 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 12 Oct 2021 14:57:21 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 12 Oct 2021 15:22:18 GMT
ENV PG_MAJOR=9.6
# Tue, 12 Oct 2021 15:22:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Fri, 12 Nov 2021 02:29:13 GMT
ENV PG_VERSION=9.6.24-1.pgdg110+1
# Fri, 12 Nov 2021 02:31:04 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 12 Nov 2021 02:31:13 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 12 Nov 2021 02:31:23 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 12 Nov 2021 02:31:26 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 12 Nov 2021 02:31:34 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 12 Nov 2021 02:31:37 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 12 Nov 2021 02:31:41 GMT
COPY file:73785d4a64e88cd001941f2d0fb17c583e6d98ffda704b27106f5ef128737e5b in /usr/local/bin/ 
# Fri, 12 Nov 2021 02:31:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 12 Nov 2021 02:31:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 02:32:00 GMT
STOPSIGNAL SIGINT
# Fri, 12 Nov 2021 02:32:04 GMT
EXPOSE 5432
# Fri, 12 Nov 2021 02:32:07 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:6c28c1405c677dd809094d06190225b38cee3d24f18da38d287ef5bcc67884d6`  
		Last Modified: Tue, 12 Oct 2021 01:37:00 GMT  
		Size: 35.3 MB (35258729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9e316c6ef33eec8142585314b9d0470aa0571ca6823736415d5690b498cf4e`  
		Last Modified: Tue, 12 Oct 2021 15:28:24 GMT  
		Size: 5.2 MB (5222851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1400a742c256b3741eb48f35fdf894551f242a23597eb4c1a39f564294588e7a`  
		Last Modified: Tue, 12 Oct 2021 15:28:21 GMT  
		Size: 1.8 KB (1811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37a720bcb97007805a78a8d5d6dbf546425e80a37f9b7b2a2a4da15e17a5104e`  
		Last Modified: Tue, 12 Oct 2021 15:28:21 GMT  
		Size: 1.4 MB (1369932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18a10b53c0b91dd4a3cec4e8c6abc43ee9a2b64ba342ec6a6387580889054e4`  
		Last Modified: Tue, 12 Oct 2021 15:28:21 GMT  
		Size: 8.0 MB (8045430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09824599989746e9afe2f80874ce0a07790006377c2a01c5804ee52f1da5ce54`  
		Last Modified: Tue, 12 Oct 2021 15:28:19 GMT  
		Size: 451.5 KB (451527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6996fb3321c0ac34b6cb6834c455670afb7f617c598c5a4bd6ddcedb559050f`  
		Last Modified: Tue, 12 Oct 2021 15:28:19 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a98de73b59c9a342634f8ad9e220cc81956836793dd6c73dbd78a54ce34c9c`  
		Last Modified: Tue, 12 Oct 2021 15:28:18 GMT  
		Size: 3.1 KB (3054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7cb05067628e052bfd86c957a9050e63f36cb3989b591bce4f503569d24ed83`  
		Last Modified: Fri, 12 Nov 2021 03:08:08 GMT  
		Size: 40.7 MB (40727060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4610ddb4cc54d0b0e0949316b1446222e48e3790c8ff9df97c248081af06911`  
		Last Modified: Fri, 12 Nov 2021 03:07:57 GMT  
		Size: 7.9 KB (7877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d798be767c11458c2e23582c09702014ada0b5eed5bbe54aed9a62317da65e13`  
		Last Modified: Fri, 12 Nov 2021 03:07:57 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd68e8f6ed240419295149e405667ddcea0fe16db57e59e49c533ea5ee7a150e`  
		Last Modified: Fri, 12 Nov 2021 03:07:57 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa4ad2a97a0f3c26c548bc476931edf063ec47e62bbeb4a8af3b0c0d88085d7`  
		Last Modified: Fri, 12 Nov 2021 03:07:57 GMT  
		Size: 4.7 KB (4721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42117007bde63ee8970c18245632f934445003f1c4d9a90ad8f9210bb1a2a766`  
		Last Modified: Fri, 12 Nov 2021 03:07:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-bullseye` - linux; s390x

```console
$ docker pull postgres@sha256:77e7c3bb1e77438fbd75cdd0f575870afde3e358e4c05e5b4254f3c8904c302d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.3 MB (83337605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94b34ccedadcab7ff482a7bc50f16a9b646980ef269be553852703c2b213db2a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:27 GMT
ADD file:42f73dac307a6a5232e3100f3d3b36e8125f73a4ca504b106e60e2b66d242b2f in / 
# Wed, 17 Nov 2021 02:42:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 04:19:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 04:19:51 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 17 Nov 2021 04:19:51 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Nov 2021 04:19:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Nov 2021 04:20:03 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 17 Nov 2021 04:20:03 GMT
ENV LANG=en_US.utf8
# Wed, 17 Nov 2021 04:20:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 04:20:07 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Nov 2021 04:20:13 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Wed, 17 Nov 2021 04:59:51 GMT
ENV PG_MAJOR=9.6
# Wed, 17 Nov 2021 04:59:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Wed, 17 Nov 2021 04:59:51 GMT
ENV PG_VERSION=9.6.24-1.pgdg110+1
# Wed, 17 Nov 2021 05:05:32 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ bullseye-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 17 Nov 2021 05:05:34 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 17 Nov 2021 05:05:35 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 17 Nov 2021 05:05:35 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 17 Nov 2021 05:05:35 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 17 Nov 2021 05:05:35 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 17 Nov 2021 05:05:35 GMT
COPY file:73785d4a64e88cd001941f2d0fb17c583e6d98ffda704b27106f5ef128737e5b in /usr/local/bin/ 
# Wed, 17 Nov 2021 05:05:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 17 Nov 2021 05:05:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 05:05:36 GMT
STOPSIGNAL SIGINT
# Wed, 17 Nov 2021 05:05:36 GMT
EXPOSE 5432
# Wed, 17 Nov 2021 05:05:36 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:8d71e885edf612b507bbdcc48a970548d436b8709eeedfc2c98f6843a214b5e2`  
		Last Modified: Wed, 17 Nov 2021 02:48:25 GMT  
		Size: 29.7 MB (29650960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f117b4d1df6500c1b1b8489bf7f0c4a49ebfed67aa499b78150ab0fdf26ef25`  
		Last Modified: Wed, 17 Nov 2021 05:07:31 GMT  
		Size: 4.3 MB (4302200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6121d676711df302dfeaa794390cdb627d2ce10fe23004c4dca743581730c9`  
		Last Modified: Wed, 17 Nov 2021 05:07:30 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fefdece5a4cdb8fc01771c3a85779ad92ff8fe65fe48c2ec4065ff1c956695`  
		Last Modified: Wed, 17 Nov 2021 05:07:30 GMT  
		Size: 1.4 MB (1437313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8868560824c1a5c168802ec7ce901a9e3c2dbb619656a28f0051623b39a829da`  
		Last Modified: Wed, 17 Nov 2021 05:07:30 GMT  
		Size: 8.1 MB (8099059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffdb275ebdf0f2decbd9af88ca3d704d4dbf8c5516ba17cb2d51aa9f156a1067`  
		Last Modified: Wed, 17 Nov 2021 05:07:29 GMT  
		Size: 438.3 KB (438293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843bf84eff8691e3a11499f4e05a4033b4b03f1a70e001280f0451198bbd5af0`  
		Last Modified: Wed, 17 Nov 2021 05:07:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf5933791b8a2696c52a08c9d0c72cad1c5630107bc8bbb5c5d3407905cf1cc`  
		Last Modified: Wed, 17 Nov 2021 05:07:29 GMT  
		Size: 3.1 KB (3054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8a00530955cbbdea3287d97099f7dcd6f1face6e8f039f5b5414487e24f28e`  
		Last Modified: Wed, 17 Nov 2021 05:09:40 GMT  
		Size: 39.4 MB (39391729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265faabbdddeef6c95123f0130aa4f0d19dae7f8ae15493c59ad0b6a55800d45`  
		Last Modified: Wed, 17 Nov 2021 05:09:33 GMT  
		Size: 7.9 KB (7874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c952e3ff39dcf7c684cae077829a5802a03ae9cc65f12952cc5e8d16433fd22`  
		Last Modified: Wed, 17 Nov 2021 05:09:33 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f822afd51e200c8d9c07228bcf42873215ec9363c7e45f6d0bdb464cf3763116`  
		Last Modified: Wed, 17 Nov 2021 05:09:33 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e985cfaf6f63a1001b3dd684005f76b9686c1c395f06084e0bb824de670b6ab`  
		Last Modified: Wed, 17 Nov 2021 05:09:33 GMT  
		Size: 4.7 KB (4719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba62a27e69133c8e1fb1f839257e40b33694ae2685c31fd6d3527155236f767e`  
		Last Modified: Wed, 17 Nov 2021 05:09:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
