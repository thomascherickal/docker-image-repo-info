## `postgres:9-stretch`

```console
$ docker pull postgres@sha256:6f150b7689146ef3642326b8ed96a9124075c004d65fcb99e69d826469952b78
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
$ docker pull postgres@sha256:743305802555b6f1fd3e2fcea59ae65f5dedf257feb63ca0113cbd0300270484
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73582167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27b9ea3cfe700aab15e5265b0d2710bc545d7e451532a162539526743b1636ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 12 Oct 2021 01:22:52 GMT
ADD file:1220579e31585dec45ca8e35874eb689018ed026a1f23b7906f791c0279671e0 in / 
# Tue, 12 Oct 2021 01:22:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 12:20:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 12:20:21 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 12 Oct 2021 12:20:21 GMT
ENV GOSU_VERSION=1.12
# Tue, 12 Oct 2021 12:20:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Oct 2021 12:20:39 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 12 Oct 2021 12:20:39 GMT
ENV LANG=en_US.utf8
# Tue, 12 Oct 2021 12:20:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:20:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 12 Oct 2021 12:20:54 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 12 Oct 2021 12:22:52 GMT
ENV PG_MAJOR=9.6
# Tue, 12 Oct 2021 12:22:53 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Thu, 11 Nov 2021 22:50:10 GMT
ENV PG_VERSION=9.6.24-1.pgdg90+1
# Thu, 11 Nov 2021 22:50:26 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 11 Nov 2021 22:50:27 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 11 Nov 2021 22:50:28 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 11 Nov 2021 22:50:28 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 11 Nov 2021 22:50:29 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 11 Nov 2021 22:50:30 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 11 Nov 2021 22:50:30 GMT
COPY file:73785d4a64e88cd001941f2d0fb17c583e6d98ffda704b27106f5ef128737e5b in /usr/local/bin/ 
# Thu, 11 Nov 2021 22:50:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 11 Nov 2021 22:50:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Nov 2021 22:50:31 GMT
STOPSIGNAL SIGINT
# Thu, 11 Nov 2021 22:50:31 GMT
EXPOSE 5432
# Thu, 11 Nov 2021 22:50:32 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:eec53b8a5053c739b5b685cb372b38eea3286ab6626532bad963291f76357c5f`  
		Last Modified: Tue, 12 Oct 2021 01:29:50 GMT  
		Size: 22.5 MB (22527572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f07e2510c1a2b3be68c27a5849f9c878575e9becb97af6e3b473ecb24748fb`  
		Last Modified: Tue, 12 Oct 2021 12:26:33 GMT  
		Size: 4.5 MB (4503769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1db85978c187782e86129ca29fba157feefbd0d176746e1f280389330894c75`  
		Last Modified: Tue, 12 Oct 2021 12:26:31 GMT  
		Size: 1.8 KB (1810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca900fc1288f10094641c9ec334e6656a3d6fcb81bdb907221e5010d1157c9a`  
		Last Modified: Tue, 12 Oct 2021 12:26:32 GMT  
		Size: 1.4 MB (1412215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12868e60047376773e127d6c2a4eb339ac0067f9737687a0a05a920c9c994aac`  
		Last Modified: Tue, 12 Oct 2021 12:26:31 GMT  
		Size: 6.2 MB (6185363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba54211abe20531ef48c9538c024d87b53dda3236dbc32b2bed1adfed6b7afd5`  
		Last Modified: Tue, 12 Oct 2021 12:26:30 GMT  
		Size: 385.0 KB (385003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d810661b69cb960f1a5a7ead1082aeecf15aeb1d8be1b71da3d9077a0f2e688`  
		Last Modified: Tue, 12 Oct 2021 12:26:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09140fe561abd752e9e3b3c58e080016cc3992ecb1f2af92f88c74496e601f3c`  
		Last Modified: Tue, 12 Oct 2021 12:26:29 GMT  
		Size: 4.8 KB (4792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacf6b420f8dbd4e58e7cc494a41368692cc06019de2236506fa0248f9fc82dc`  
		Last Modified: Thu, 11 Nov 2021 23:01:14 GMT  
		Size: 38.5 MB (38548441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4438479c04f1c02eacb992f6d53d56367320efda52f07aa44509abd2e6e269bd`  
		Last Modified: Thu, 11 Nov 2021 23:01:06 GMT  
		Size: 7.9 KB (7872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f685cf2fd61699a85337a1bd4f495e23d51da9e43551ddf48c062f1b05fa9292`  
		Last Modified: Thu, 11 Nov 2021 23:01:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7614606dfb60bcb92e4ed0be0c03732b294fcb3b7b3e0a260bf396b0a5faaa1`  
		Last Modified: Thu, 11 Nov 2021 23:01:06 GMT  
		Size: 202.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7562dac134613cc41b30b55a2c71defa594353e599a8dea782e2ac0ea2868ac2`  
		Last Modified: Thu, 11 Nov 2021 23:01:06 GMT  
		Size: 4.7 KB (4729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb09a47efe7f3801bd1f3128fe768b743e514e36198f4ad22b397b38d6bca266`  
		Last Modified: Thu, 11 Nov 2021 23:01:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-stretch` - linux; arm variant v5

```console
$ docker pull postgres@sha256:366732ddd3c33f2e55c229969197b13aa07c09417271431ab0bee1307553776a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70604103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55959c53758daafdae8f161b1f4ab349a715b54be9ca601b325d8200819a05c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 17 Nov 2021 02:56:16 GMT
ADD file:b857fb98b0880bbb3add8dd317cd1eb0f339332d4836baaedc8f2f424b5f2c98 in / 
# Wed, 17 Nov 2021 02:56:17 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 09:29:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 09:29:19 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 17 Nov 2021 09:29:20 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Nov 2021 09:29:55 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Nov 2021 09:30:13 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 17 Nov 2021 09:30:14 GMT
ENV LANG=en_US.utf8
# Wed, 17 Nov 2021 09:30:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:30:28 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Nov 2021 09:30:40 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Wed, 17 Nov 2021 11:09:44 GMT
ENV PG_MAJOR=9.6
# Wed, 17 Nov 2021 11:09:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Wed, 17 Nov 2021 11:09:45 GMT
ENV PG_VERSION=9.6.24-1.pgdg90+1
# Wed, 17 Nov 2021 11:35:03 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 17 Nov 2021 11:35:05 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 17 Nov 2021 11:35:06 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 17 Nov 2021 11:35:07 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 17 Nov 2021 11:35:08 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 17 Nov 2021 11:35:09 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 17 Nov 2021 11:35:09 GMT
COPY file:73785d4a64e88cd001941f2d0fb17c583e6d98ffda704b27106f5ef128737e5b in /usr/local/bin/ 
# Wed, 17 Nov 2021 11:35:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 17 Nov 2021 11:35:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 11:35:12 GMT
STOPSIGNAL SIGINT
# Wed, 17 Nov 2021 11:35:12 GMT
EXPOSE 5432
# Wed, 17 Nov 2021 11:35:13 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:ca67a5e1c16d08a9b8520dae81a39d168ef2a816d8905715eb6a328c89a2ce37`  
		Last Modified: Wed, 17 Nov 2021 03:14:12 GMT  
		Size: 21.2 MB (21204234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66becebc6ea2be3de2bc7719b7e2a713bf2841e25347528f0dd43393b518bfee`  
		Last Modified: Wed, 17 Nov 2021 11:43:04 GMT  
		Size: 4.2 MB (4239251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9db125c4534d915cb2f902cd848b367d3ca52e22ab085f28ab02c0c1dfe826`  
		Last Modified: Wed, 17 Nov 2021 11:43:01 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:631ca81a910e378d6e855faf60990f606281ee9dbc05a0727e621ef3770dc652`  
		Last Modified: Wed, 17 Nov 2021 11:43:01 GMT  
		Size: 1.4 MB (1371402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664963e53ff556b1f0b51f962a45b718bd4841af68f53275e9f79e6c1c219dcd`  
		Last Modified: Wed, 17 Nov 2021 11:43:03 GMT  
		Size: 6.2 MB (6185482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e53885ea5db7ff91019cb1f6c2e218dbb5533dcdd7d1191b9c8762263e1f1d`  
		Last Modified: Wed, 17 Nov 2021 11:42:59 GMT  
		Size: 385.0 KB (385043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f91bcbad9cf60309486bd65a1b92ebecc0c022bfe18bb5956e19940632f1e7`  
		Last Modified: Wed, 17 Nov 2021 11:42:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802987e99f265473d4569aa26c3631733bf2e436bb3867d9b7065b73a5b4fce3`  
		Last Modified: Wed, 17 Nov 2021 11:42:59 GMT  
		Size: 5.3 KB (5343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5e6202739b09bf2f172d93e8db0b4acc6d26cb846afb6dfc67f52b71a2fb0c`  
		Last Modified: Wed, 17 Nov 2021 11:46:22 GMT  
		Size: 37.2 MB (37198341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed4d37e76488c177c5f19f3d0734b061a15947118477cbeb3b83e3e6741b6b7`  
		Last Modified: Wed, 17 Nov 2021 11:45:54 GMT  
		Size: 7.9 KB (7874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f3df598611e62a70c022e48759244a90904e285e79c2036d5a97da3239a831`  
		Last Modified: Wed, 17 Nov 2021 11:45:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f80b1125f5c983907a52efd1e412ceb85d3ba5f53a1a5a0b3236d5cc330cd777`  
		Last Modified: Wed, 17 Nov 2021 11:45:54 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460dcb277a087ef9cfe8b010b39c0682e51a68ac0e5549fe7ac5afe7c0fc680e`  
		Last Modified: Wed, 17 Nov 2021 11:45:54 GMT  
		Size: 4.7 KB (4730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fafddb3dc6881243426203a1e45c5b368fb16abf5390fc0b8442573c7b01ba`  
		Last Modified: Wed, 17 Nov 2021 11:45:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-stretch` - linux; arm variant v7

```console
$ docker pull postgres@sha256:e19fcfc02a9aa1c175774a593a40de3f5171028d3656fe2c62ed368808c1f977
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.3 MB (67275061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fd97278b3bbfe1a99d639037cf3c3446f36f334ba77b180953854510b8418ea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 12 Oct 2021 01:34:42 GMT
ADD file:9bfcfd0aaac802b902b0e842e040a6599c461c90b73579bcacc2fbdda7ec39cb in / 
# Tue, 12 Oct 2021 01:34:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 21:57:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 21:57:54 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 12 Oct 2021 21:57:55 GMT
ENV GOSU_VERSION=1.12
# Tue, 12 Oct 2021 21:58:24 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Oct 2021 21:58:40 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 12 Oct 2021 21:58:40 GMT
ENV LANG=en_US.utf8
# Tue, 12 Oct 2021 21:58:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 21:58:51 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 12 Oct 2021 21:59:05 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 12 Oct 2021 23:28:17 GMT
ENV PG_MAJOR=9.6
# Tue, 12 Oct 2021 23:28:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Fri, 12 Nov 2021 04:45:44 GMT
ENV PG_VERSION=9.6.24-1.pgdg90+1
# Fri, 12 Nov 2021 05:07:53 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 12 Nov 2021 05:07:55 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 12 Nov 2021 05:07:57 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 12 Nov 2021 05:07:57 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 12 Nov 2021 05:07:59 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 12 Nov 2021 05:08:00 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 12 Nov 2021 05:08:00 GMT
COPY file:73785d4a64e88cd001941f2d0fb17c583e6d98ffda704b27106f5ef128737e5b in /usr/local/bin/ 
# Fri, 12 Nov 2021 05:08:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 12 Nov 2021 05:08:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 05:08:03 GMT
STOPSIGNAL SIGINT
# Fri, 12 Nov 2021 05:08:03 GMT
EXPOSE 5432
# Fri, 12 Nov 2021 05:08:03 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:a1a3620b17011bd36d6f64dfcc8fd7c4cb3da78d19a59efb1b35afcadaf3f6a8`  
		Last Modified: Tue, 12 Oct 2021 01:51:59 GMT  
		Size: 19.3 MB (19316474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:551b11e6ac4ffc90cd9416856106a0969c3f92ee5dd475a45748f0832d4d1268`  
		Last Modified: Wed, 13 Oct 2021 00:00:45 GMT  
		Size: 3.9 MB (3875492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e15c49bc5ea0c5f135b2fe2eb9326c4a9e2427acec1439b76616f43ce3f9311`  
		Last Modified: Wed, 13 Oct 2021 00:00:43 GMT  
		Size: 1.8 KB (1811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd5ab1ce8ce2584e209d5d850af67102d3692b39fc8645a25094572309ce5b8`  
		Last Modified: Wed, 13 Oct 2021 00:00:44 GMT  
		Size: 1.4 MB (1363842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6ca458a24394f08c06770fcdeade1006e42147036ea609bbbf774009b3f5ff`  
		Last Modified: Wed, 13 Oct 2021 00:00:46 GMT  
		Size: 6.2 MB (6185598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31fba5970bae74f418d3711dbc214f7a1b53473ce3ae217dc31dfad9b77060f`  
		Last Modified: Wed, 13 Oct 2021 00:00:42 GMT  
		Size: 379.1 KB (379150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd1b53946838bd459a2bdac0cdcabefaf6afd6538716c1cfeb40b6855e6fb05`  
		Last Modified: Wed, 13 Oct 2021 00:00:41 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a853d09e19c1300de8fedac88f782e60dec0c2698a4cf16bc46aaf9c74c0f7`  
		Last Modified: Wed, 13 Oct 2021 00:00:41 GMT  
		Size: 5.3 KB (5343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75aa33892233db7ee724f9f079760c74081b603a0d6c29b8922edea5b50617ee`  
		Last Modified: Fri, 12 Nov 2021 05:29:16 GMT  
		Size: 36.1 MB (36134154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b0bbffadae7f559efd8921edc5b13f4e8aa294a9eb67f79c3a683d0926846b4`  
		Last Modified: Fri, 12 Nov 2021 05:28:50 GMT  
		Size: 7.9 KB (7869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a9aad8b5678ee467d7974fe302baf8bde087afdf99faeebd2a5068806b4f67`  
		Last Modified: Fri, 12 Nov 2021 05:28:50 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542ac21630497215af5dabf069792c4b9cd0d5677d8b4a2f6963e400d8fc9329`  
		Last Modified: Fri, 12 Nov 2021 05:28:50 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc0cb248025eba8865f31ff612d4bd9ab9ea62be3cab12d08382bbdd39e7a9a`  
		Last Modified: Fri, 12 Nov 2021 05:28:50 GMT  
		Size: 4.7 KB (4731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363453a886765b614e69033fc2a3b96daa858eb291e5578fbb4616dbe6f4f467`  
		Last Modified: Fri, 12 Nov 2021 05:28:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-stretch` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:d4fc060a34792957fb1efee20e2c7faa4484ea4d321afe9c709f4c7b53db4de3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69488729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72991bbb92eb963128bc65c56fdf70dddc43a3c742142c4614534248e3cda253`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:48 GMT
ADD file:2adad5eee701d55a9f58c07f0706eb574d0ad6b74b0cc52a9e622f50639961c9 in / 
# Wed, 17 Nov 2021 02:42:48 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 11:00:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 11:00:43 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Wed, 17 Nov 2021 11:00:44 GMT
ENV GOSU_VERSION=1.12
# Wed, 17 Nov 2021 11:00:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 17 Nov 2021 11:01:05 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Wed, 17 Nov 2021 11:01:05 GMT
ENV LANG=en_US.utf8
# Wed, 17 Nov 2021 11:01:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 11:01:11 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Wed, 17 Nov 2021 11:01:20 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Wed, 17 Nov 2021 11:23:01 GMT
ENV PG_MAJOR=9.6
# Wed, 17 Nov 2021 11:23:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Wed, 17 Nov 2021 11:23:03 GMT
ENV PG_VERSION=9.6.24-1.pgdg90+1
# Wed, 17 Nov 2021 11:32:45 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 17 Nov 2021 11:32:46 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 17 Nov 2021 11:32:47 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 17 Nov 2021 11:32:48 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 17 Nov 2021 11:32:49 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 17 Nov 2021 11:32:50 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 17 Nov 2021 11:32:52 GMT
COPY file:73785d4a64e88cd001941f2d0fb17c583e6d98ffda704b27106f5ef128737e5b in /usr/local/bin/ 
# Wed, 17 Nov 2021 11:32:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 17 Nov 2021 11:32:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 11:32:54 GMT
STOPSIGNAL SIGINT
# Wed, 17 Nov 2021 11:32:55 GMT
EXPOSE 5432
# Wed, 17 Nov 2021 11:32:56 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:34b92b588f0f390db0d125ab0ee4c85510c52367371c4bcf5af80a6ab18f0a9b`  
		Last Modified: Wed, 17 Nov 2021 02:51:38 GMT  
		Size: 20.4 MB (20389442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89cd8a89c58b4ad8db3feebddf61420fe97f5eb75ff309c706a5c49670a3941`  
		Last Modified: Wed, 17 Nov 2021 11:37:27 GMT  
		Size: 3.9 MB (3890678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed45654da4b113d3ed8b05308e5b46faa991862373d13fddfa4fa71da5058b92`  
		Last Modified: Wed, 17 Nov 2021 11:37:26 GMT  
		Size: 1.7 KB (1662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c1cef042408896a1ceed08aeb4aa7f8e06e001164273890f24b06b10307303`  
		Last Modified: Wed, 17 Nov 2021 11:37:26 GMT  
		Size: 1.3 MB (1346588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14a3c417e1c878b5e6702fd3df7f676ca76a9d843f12d92602362014701b0a4e`  
		Last Modified: Wed, 17 Nov 2021 11:37:24 GMT  
		Size: 6.2 MB (6182437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d2df6610c36d32b855b51da5ed103d2a72d4bafc039abc1ff76d75c6cf25e6`  
		Last Modified: Wed, 17 Nov 2021 11:37:24 GMT  
		Size: 173.4 KB (173418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f657239337b6b1dbb9d1874b1287a090840c1e67bda383b78e62a8b4caeed1`  
		Last Modified: Wed, 17 Nov 2021 11:37:23 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deccc8395759678a9b7b6d14a854eb4ee57d4a72f10e7bcd147d99fe0a92f167`  
		Last Modified: Wed, 17 Nov 2021 11:37:23 GMT  
		Size: 5.3 KB (5316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a484a9724611416d6fd4b58df6465f5897a6b53b4a20998998b266157432310`  
		Last Modified: Wed, 17 Nov 2021 11:39:11 GMT  
		Size: 37.5 MB (37486056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddef05845f311e890476888e41821a71ff043135978c4c1894d066e98971d92d`  
		Last Modified: Wed, 17 Nov 2021 11:39:02 GMT  
		Size: 7.9 KB (7871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0e04b2a605e78b5953babab8bf5acb400b3cf055bdbaab43c97242fd42dda2`  
		Last Modified: Wed, 17 Nov 2021 11:39:02 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be43048612546756ba9968fb4c27b09591669406ca7f71e65bc70bf314b682e4`  
		Last Modified: Wed, 17 Nov 2021 11:39:03 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef2f31390340083f0867ba7d1fe881798ab754a09f94dd7a5e227049d824a38`  
		Last Modified: Wed, 17 Nov 2021 11:39:02 GMT  
		Size: 4.7 KB (4726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf06743a608028a73210cc2fb883c7caa24fe579b66d646d0fb019d1479b3c35`  
		Last Modified: Wed, 17 Nov 2021 11:39:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:9-stretch` - linux; 386

```console
$ docker pull postgres@sha256:042e5daf62c296a7d1d9829c984c8b0f496fa0d657433229318d97e9f9cd90e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74714534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8859590b3f3cf108ef457b4a35edbb35a8da0c2933d3bf502a05dccec0e8ee42`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Tue, 12 Oct 2021 01:42:34 GMT
ADD file:4420d4cd2022d6bad7f61fbfaf16f0759ca6c30424974c6076dc7d5c09910d66 in / 
# Tue, 12 Oct 2021 01:42:34 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 17:43:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 17:43:49 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Tue, 12 Oct 2021 17:43:49 GMT
ENV GOSU_VERSION=1.12
# Tue, 12 Oct 2021 17:44:03 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Oct 2021 17:44:09 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Tue, 12 Oct 2021 17:44:10 GMT
ENV LANG=en_US.utf8
# Tue, 12 Oct 2021 17:44:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 17:44:15 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Tue, 12 Oct 2021 17:44:28 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export "$key" > /etc/apt/trusted.gpg.d/postgres.gpg; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME"; 	apt-key list
# Tue, 12 Oct 2021 18:06:25 GMT
ENV PG_MAJOR=9.6
# Tue, 12 Oct 2021 18:06:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/9.6/bin
# Fri, 12 Nov 2021 01:25:14 GMT
ENV PG_VERSION=9.6.24-1.pgdg90+1
# Fri, 12 Nov 2021 01:25:33 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 		"postgresql-contrib-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 12 Nov 2021 01:25:34 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 12 Nov 2021 01:25:35 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 12 Nov 2021 01:25:36 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 12 Nov 2021 01:25:37 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 12 Nov 2021 01:25:37 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 12 Nov 2021 01:25:37 GMT
COPY file:73785d4a64e88cd001941f2d0fb17c583e6d98ffda704b27106f5ef128737e5b in /usr/local/bin/ 
# Fri, 12 Nov 2021 01:25:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 12 Nov 2021 01:25:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 01:25:39 GMT
STOPSIGNAL SIGINT
# Fri, 12 Nov 2021 01:25:39 GMT
EXPOSE 5432
# Fri, 12 Nov 2021 01:25:39 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:3d6d74524a87c2d3253aea0ad3bc52520036015f508d5b113e4c8c6627e92bc2`  
		Last Modified: Tue, 12 Oct 2021 01:52:28 GMT  
		Size: 23.2 MB (23156692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01b71ba351b729ff06aead26878f02bb87b9b6ac45f63086175bb14a32f1823`  
		Last Modified: Tue, 12 Oct 2021 18:12:17 GMT  
		Size: 4.8 MB (4811926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9678391fbb3aed6cd62fd4866d056d72f14f2d9f4d1c73cb99caea1787d7d6ea`  
		Last Modified: Tue, 12 Oct 2021 18:12:15 GMT  
		Size: 1.8 KB (1800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599258460ebbd57c1c2c475b3e5de2cba0167521a1a828005e36310be5f3bb57`  
		Last Modified: Tue, 12 Oct 2021 18:12:16 GMT  
		Size: 1.4 MB (1382518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189f6193f38cbd3ab3fecdc41282879fc7e97a970a6d3f3913d3d1a655275229`  
		Last Modified: Tue, 12 Oct 2021 18:12:15 GMT  
		Size: 6.2 MB (6185534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c8397c1cce4207420af56bc2c508ba1db3e974a318599f64aeb984377631d9`  
		Last Modified: Tue, 12 Oct 2021 18:12:13 GMT  
		Size: 393.3 KB (393287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63345f2a56e5ee080cae0f56115c3c4f67d716a753d976fbb9d9abd7adb352fe`  
		Last Modified: Tue, 12 Oct 2021 18:12:13 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f7dceeaf3ee720c7be7e21b5a0df7ca5609fd175a125c3af9bc02d7d68cd35`  
		Last Modified: Tue, 12 Oct 2021 18:12:13 GMT  
		Size: 5.3 KB (5347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6038341dd298eb58f83fa59c0c5e2165aa68ed8bd01a9d6bf9a9edd1d14fa6d0`  
		Last Modified: Fri, 12 Nov 2021 01:40:00 GMT  
		Size: 38.8 MB (38764234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aace357e7dc6f2f41258ed0032157408c012f60e54ddc998cd8bc005bf9f5f7`  
		Last Modified: Fri, 12 Nov 2021 01:39:49 GMT  
		Size: 7.9 KB (7870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d545fa57f4aa632b59e10037d5a178c75cb879bd65e952114487684121e31ca`  
		Last Modified: Fri, 12 Nov 2021 01:39:48 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82731d9d52252555e487878cc5e8950b910fbd76f4bbcee3dc4958b07acbabf`  
		Last Modified: Fri, 12 Nov 2021 01:39:48 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810cff8f5c12105350b8640b69088ccda2b09c9da141ad58f9776f0f4eaa2d51`  
		Last Modified: Fri, 12 Nov 2021 01:39:48 GMT  
		Size: 4.7 KB (4727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d1105c13de162a1e2c68eefbd5cbc334ac1b1bfdd475f5bafd21966cd27c20`  
		Last Modified: Fri, 12 Nov 2021 01:39:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
