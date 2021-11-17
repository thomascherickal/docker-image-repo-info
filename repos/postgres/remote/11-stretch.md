## `postgres:11-stretch`

```console
$ docker pull postgres@sha256:1a2fe2166ef542f2e48e66ecb5548208cea1131407cede2a586c05dfedc83721
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `postgres:11-stretch` - linux; amd64

```console
$ docker pull postgres@sha256:e5f273aaaad30e145e51642cff0d3eb249c558a4080a600760585585a6ad6f24
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.6 MB (106551874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f06ac2698ca30bef29a85a4e706e4d0ccdd429ebd5b75b35756e69946a285091`
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
# Tue, 12 Oct 2021 12:20:54 GMT
ENV PG_MAJOR=11
# Tue, 12 Oct 2021 12:20:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Thu, 11 Nov 2021 22:39:01 GMT
ENV PG_VERSION=11.14-1.pgdg90+1
# Thu, 11 Nov 2021 22:39:25 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 11 Nov 2021 22:39:26 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 11 Nov 2021 22:39:27 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 11 Nov 2021 22:39:27 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 11 Nov 2021 22:39:28 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 11 Nov 2021 22:39:28 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 11 Nov 2021 22:39:29 GMT
COPY file:6e4de9271291e4bdd4a40b73fffe4d6d1aeff033460f5b14d74e948686daa095 in /usr/local/bin/ 
# Thu, 11 Nov 2021 22:39:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Nov 2021 22:39:29 GMT
STOPSIGNAL SIGINT
# Thu, 11 Nov 2021 22:39:29 GMT
EXPOSE 5432
# Thu, 11 Nov 2021 22:39:29 GMT
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
	-	`sha256:8a4c34c2408b78f97e7cdb5ebad98d766d94db5d3b3f30226dc2f86a2a437c5f`  
		Last Modified: Thu, 11 Nov 2021 22:58:49 GMT  
		Size: 71.5 MB (71517821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1c38cde394221084c0538e6417c111d9f6aad1166fcbe4b021d62e5914ec09`  
		Last Modified: Thu, 11 Nov 2021 22:58:38 GMT  
		Size: 8.3 KB (8326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f4fee3b9d4538e2a6e70449d6fa18e134574122309736b080fcfcd02d13959`  
		Last Modified: Thu, 11 Nov 2021 22:58:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479df155f72bc4752a5303b4805ba57a56763eb79cbf5bd581661ebc9a6e144f`  
		Last Modified: Thu, 11 Nov 2021 22:58:38 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4445b93894ed2cca29a5ab4e918e109ff8df7f9ed2f4f1c3843fb7fcf411e573`  
		Last Modified: Thu, 11 Nov 2021 22:58:38 GMT  
		Size: 4.7 KB (4727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-stretch` - linux; arm variant v5

```console
$ docker pull postgres@sha256:0d6f2a07b2f3d15aca56a850cd821d8ada563e6bcffe63c200472cec8305845f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70728240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:112099fabfdc511ff9a353073d78e7036d473c7ed2f0c4b61ce9b6249f359447`
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
# Wed, 17 Nov 2021 09:30:40 GMT
ENV PG_MAJOR=11
# Wed, 17 Nov 2021 09:30:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Wed, 17 Nov 2021 09:30:41 GMT
ENV PG_VERSION=11.14-1.pgdg90+1
# Wed, 17 Nov 2021 09:56:55 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 17 Nov 2021 09:56:58 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 17 Nov 2021 09:56:59 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 17 Nov 2021 09:57:00 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 17 Nov 2021 09:57:02 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 17 Nov 2021 09:57:02 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 17 Nov 2021 09:57:03 GMT
COPY file:6e4de9271291e4bdd4a40b73fffe4d6d1aeff033460f5b14d74e948686daa095 in /usr/local/bin/ 
# Wed, 17 Nov 2021 09:57:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 09:57:04 GMT
STOPSIGNAL SIGINT
# Wed, 17 Nov 2021 09:57:04 GMT
EXPOSE 5432
# Wed, 17 Nov 2021 09:57:05 GMT
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
	-	`sha256:a238cb1e3a758d58a2fc64c8bca9c64f1f5c696144095c1bc2e22b27096acb15`  
		Last Modified: Wed, 17 Nov 2021 11:43:23 GMT  
		Size: 37.3 MB (37322145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c867ef685d8f690e63e3c51db8822e03d1d7f59b2cdbe15997dc7ed615333f0a`  
		Last Modified: Wed, 17 Nov 2021 11:42:57 GMT  
		Size: 8.3 KB (8334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7dab2922f3fcbe6f7d4cdd3be41f7ebbd4aafdd2e0239b3f5454697b1c37c8a`  
		Last Modified: Wed, 17 Nov 2021 11:42:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f20879ee57669cdaba33285a5b9d622f46171efe2127a02a82ca176e93637c`  
		Last Modified: Wed, 17 Nov 2021 11:42:57 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34dad57ee9ab073c7e5a3689c5bac01704c331b01c657ff6bda2c68a4d723392`  
		Last Modified: Wed, 17 Nov 2021 11:42:57 GMT  
		Size: 4.7 KB (4725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-stretch` - linux; arm variant v7

```console
$ docker pull postgres@sha256:aa0b8313a78b0eb94ec0a1b33df5e5a15c5800c69010be120e9737b72da81bfc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.4 MB (67373122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54c25f132c30adef0f69ca20aee34239269358a39ab43109eb1136c2b72373ec`
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
# Tue, 12 Oct 2021 21:59:06 GMT
ENV PG_MAJOR=11
# Tue, 12 Oct 2021 21:59:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Fri, 12 Nov 2021 03:08:01 GMT
ENV PG_VERSION=11.14-1.pgdg90+1
# Fri, 12 Nov 2021 03:30:58 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 12 Nov 2021 03:31:01 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 12 Nov 2021 03:31:02 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 12 Nov 2021 03:31:03 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 12 Nov 2021 03:31:04 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 12 Nov 2021 03:31:05 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 12 Nov 2021 03:31:05 GMT
COPY file:6e4de9271291e4bdd4a40b73fffe4d6d1aeff033460f5b14d74e948686daa095 in /usr/local/bin/ 
# Fri, 12 Nov 2021 03:31:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 03:31:06 GMT
STOPSIGNAL SIGINT
# Fri, 12 Nov 2021 03:31:07 GMT
EXPOSE 5432
# Fri, 12 Nov 2021 03:31:07 GMT
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
	-	`sha256:78e37b0505b59a004a099dc69a9f96546762a51ef08f1115d9a8b2b141c1d600`  
		Last Modified: Fri, 12 Nov 2021 05:24:49 GMT  
		Size: 36.2 MB (36231872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41fdba55d5fed12f57a0b919b695bbc1f1ef6d7b0786c41a1d6f38fa29dd862`  
		Last Modified: Fri, 12 Nov 2021 05:24:24 GMT  
		Size: 8.3 KB (8330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c447485ac4584bbc8015de3d5e4d80a5695ee38467ee7594196900c31cb4eee2`  
		Last Modified: Fri, 12 Nov 2021 05:24:24 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddc58613a1937e2d97a7a2a577dd32e89ba3a514629493bd6c9b51b3c32f1f30`  
		Last Modified: Fri, 12 Nov 2021 05:24:24 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1510a73d8fb887ebdb393a134b5b2c57047c406779d19dd861fd2457d58edd`  
		Last Modified: Fri, 12 Nov 2021 05:24:24 GMT  
		Size: 4.7 KB (4730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-stretch` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:220183a9e7dae9776daca9fc24208feae7d9f129148429a738ab629d960ff1c1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69612649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abdc810bf06fcf80c2d963e64f7ed357a1e2ab3848c20154677c0497f9e1bf38`
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
# Wed, 17 Nov 2021 11:01:21 GMT
ENV PG_MAJOR=11
# Wed, 17 Nov 2021 11:01:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Wed, 17 Nov 2021 11:01:23 GMT
ENV PG_VERSION=11.14-1.pgdg90+1
# Wed, 17 Nov 2021 11:11:10 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Wed, 17 Nov 2021 11:11:11 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Wed, 17 Nov 2021 11:11:12 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Wed, 17 Nov 2021 11:11:13 GMT
ENV PGDATA=/var/lib/postgresql/data
# Wed, 17 Nov 2021 11:11:14 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Wed, 17 Nov 2021 11:11:15 GMT
VOLUME [/var/lib/postgresql/data]
# Wed, 17 Nov 2021 11:11:17 GMT
COPY file:6e4de9271291e4bdd4a40b73fffe4d6d1aeff033460f5b14d74e948686daa095 in /usr/local/bin/ 
# Wed, 17 Nov 2021 11:11:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 11:11:18 GMT
STOPSIGNAL SIGINT
# Wed, 17 Nov 2021 11:11:19 GMT
EXPOSE 5432
# Wed, 17 Nov 2021 11:11:20 GMT
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
	-	`sha256:4ffd1f89d82af5402b20dc33e7ce08e808ebead1a2f82b19bcaba73bd851db8e`  
		Last Modified: Wed, 17 Nov 2021 11:37:27 GMT  
		Size: 37.6 MB (37609646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5f7fea371d89f123d9a5537506772b323ebc7e80b6c104421cf491ca860ce3`  
		Last Modified: Wed, 17 Nov 2021 11:37:21 GMT  
		Size: 8.3 KB (8327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf770fd6f759b5acb5a18b4afa418afc40b1e6bee1658c53d9e89cc9742034d`  
		Last Modified: Wed, 17 Nov 2021 11:37:21 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4475e59a14aca3b7d0aecde2d53f7d10a15235c2e941d987158a1f89f978a9f3`  
		Last Modified: Wed, 17 Nov 2021 11:37:21 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b804c62b62277bd8bbe0ca2561fe74338b7b2da49bb52799c0362606d10ee4`  
		Last Modified: Wed, 17 Nov 2021 11:37:21 GMT  
		Size: 4.7 KB (4720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:11-stretch` - linux; 386

```console
$ docker pull postgres@sha256:2974ec7e2aba41f2746cf9e1496d73d224e91c46b9fd8ddba2d7fd55555ea2b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110002168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e1197019d89f0ff0307d66ce4d14fcf111b0f6e537b18d3e8c13f87ee1541b4`
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
# Tue, 12 Oct 2021 17:44:28 GMT
ENV PG_MAJOR=11
# Tue, 12 Oct 2021 17:44:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/11/bin
# Fri, 12 Nov 2021 00:53:04 GMT
ENV PG_VERSION=11.14-1.pgdg90+1
# Fri, 12 Nov 2021 00:53:33 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		amd64 | i386 | ppc64el) 			echo "deb http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src http://apt.postgresql.org/pub/repos/apt/ stretch-pgdg main $PG_MAJOR" > /etc/apt/sources.list.d/pgdg.list; 						echo 'deb http://deb.debian.org/debian stretch-backports main' >> /etc/apt/sources.list.d/pgdg.list; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						savedAptMark="$(apt-mark showmanual)"; 						apt-get update; 			apt-get build-dep -y 				postgresql-common pgdg-keyring 				"postgresql-$PG_MAJOR=$PG_VERSION" 			; 			DEB_BUILD_OPTIONS="nocheck parallel=$(nproc)" 				apt-get source --compile 					postgresql-common pgdg-keyring 					"postgresql-$PG_MAJOR=$PG_VERSION" 			; 						apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			dpkg-scanpackages . > Packages; 			grep '^Package: ' Packages; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			apt-get -o Acquire::GzipIndexes=false update; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Fri, 12 Nov 2021 00:53:34 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Fri, 12 Nov 2021 00:53:36 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Fri, 12 Nov 2021 00:53:36 GMT
ENV PGDATA=/var/lib/postgresql/data
# Fri, 12 Nov 2021 00:53:37 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Fri, 12 Nov 2021 00:53:37 GMT
VOLUME [/var/lib/postgresql/data]
# Fri, 12 Nov 2021 00:53:37 GMT
COPY file:6e4de9271291e4bdd4a40b73fffe4d6d1aeff033460f5b14d74e948686daa095 in /usr/local/bin/ 
# Fri, 12 Nov 2021 00:53:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 00:53:38 GMT
STOPSIGNAL SIGINT
# Fri, 12 Nov 2021 00:53:38 GMT
EXPOSE 5432
# Fri, 12 Nov 2021 00:53:38 GMT
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
	-	`sha256:778eb8534d54062c6083b2453dcca785da71b378fae0c9e6cd39c22a6cd01a2f`  
		Last Modified: Fri, 12 Nov 2021 01:37:09 GMT  
		Size: 74.1 MB (74051531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359bf9d058e38be5d89a808cb3079b662fbbcde80f920d4c6acdbeee9ac16d4a`  
		Last Modified: Fri, 12 Nov 2021 01:36:54 GMT  
		Size: 8.3 KB (8326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43f9860070399582f82bbe7d1503d03fa562f708b5f946f302775d60033380b`  
		Last Modified: Fri, 12 Nov 2021 01:36:54 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba82c140fb65292525a730d1bf76a020c55f6b51fd694e7d0cccd71053cb3b0b`  
		Last Modified: Fri, 12 Nov 2021 01:36:54 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55f7aa0c61ed0426a85801dca8d4266d995a6e11b100bc7a6b91f058adef895`  
		Last Modified: Fri, 12 Nov 2021 01:36:54 GMT  
		Size: 4.7 KB (4728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
