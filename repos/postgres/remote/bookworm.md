## `postgres:bookworm`

```console
$ docker pull postgres@sha256:d0c68cd506cde10ddd890e77f98339a4f05810ffba99c881061a12b30a0525c9
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

### `postgres:bookworm` - linux; amd64

```console
$ docker pull postgres@sha256:190f2f092ceb28b08e70f4b223bffb0dfe407d5e5f9730c5aedc19f9cab4a494
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.9 MB (148903900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69e765e8cdbefcc310a57c0d5344bd0db05b182e9807b473c1deb8f424066084`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 07 Sep 2023 00:20:51 GMT
ADD file:3a8cd4de7f163d93718670f4db1de49045f5e04af3a8aa27d81c0f14647db707 in / 
# Thu, 07 Sep 2023 00:20:51 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 14:22:15 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 07 Sep 2023 14:22:21 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 14:22:21 GMT
ENV GOSU_VERSION=1.16
# Thu, 07 Sep 2023 14:22:30 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 07 Sep 2023 14:22:36 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 07 Sep 2023 14:22:36 GMT
ENV LANG=en_US.utf8
# Thu, 07 Sep 2023 14:22:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 14:22:41 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 07 Sep 2023 14:22:42 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 07 Sep 2023 14:24:16 GMT
ENV PG_MAJOR=15
# Thu, 07 Sep 2023 14:24:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Thu, 07 Sep 2023 14:24:16 GMT
ENV PG_VERSION=15.4-1.pgdg120+1
# Thu, 07 Sep 2023 14:24:35 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 07 Sep 2023 14:24:37 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 07 Sep 2023 14:24:37 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 07 Sep 2023 14:24:37 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 07 Sep 2023 14:24:38 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 07 Sep 2023 14:24:38 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 07 Sep 2023 14:24:38 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Thu, 07 Sep 2023 14:24:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Sep 2023 14:24:38 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 14:24:38 GMT
EXPOSE 5432
# Thu, 07 Sep 2023 14:24:38 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:360eba32fa65016e0d558c6af176db31a202e9a6071666f9b629cb8ba6ccedf0`  
		Last Modified: Thu, 07 Sep 2023 00:25:22 GMT  
		Size: 29.1 MB (29124494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6987678f9780a65e1300c3d532de110c386c1c31426a9d58bf6a89064dc5891e`  
		Last Modified: Thu, 07 Sep 2023 14:29:42 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42299245e9050289da4064333ed9c50baa15c2d2e2553c5c63cd61f1cd58d913`  
		Last Modified: Thu, 07 Sep 2023 14:29:43 GMT  
		Size: 4.6 MB (4618729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afcda32ad76a6ffb6b64cdd88d736e02ed9061da715f6e1ace084917f1545a57`  
		Last Modified: Thu, 07 Sep 2023 14:29:42 GMT  
		Size: 1.4 MB (1444748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d81c7506667f1840cfec9f2300f7c8e2fd339b8dc75d994b56510fea75220d`  
		Last Modified: Thu, 07 Sep 2023 14:29:41 GMT  
		Size: 8.1 MB (8065033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7813914a8b7e2fce2df17d99844729d113fe54db71504972e23f275adac38d6`  
		Last Modified: Thu, 07 Sep 2023 14:29:40 GMT  
		Size: 1.4 MB (1405696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:876fecb4c432d062ffcc214cbdec029ffe9455f30f3e591f5c9680322f52c963`  
		Last Modified: Thu, 07 Sep 2023 14:29:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8727713246ed1e93b83ea6566473f0e49d331d6bd78d495a25921149423e7f`  
		Last Modified: Thu, 07 Sep 2023 14:29:39 GMT  
		Size: 3.2 KB (3200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd55a69456f7dbeefa051cdfb51f20e3917466e404530f6e793c5d59c6a27798`  
		Last Modified: Thu, 07 Sep 2023 14:30:35 GMT  
		Size: 104.2 MB (104225743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a9c6f88b3ac0d34a58c6cacd68ece1c4d7f53b0e1d7017edead031d087050f`  
		Last Modified: Thu, 07 Sep 2023 14:30:22 GMT  
		Size: 9.8 KB (9781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8b906dc57f465d053a04ed809cfa8d5fab25f4357707e9ed6b375d7696c901`  
		Last Modified: Thu, 07 Sep 2023 14:30:22 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa3ed8d50472d219b0a54f2a27594e240fcba78705c16737d3eda4e4053fd22`  
		Last Modified: Thu, 07 Sep 2023 14:30:22 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae8c52f27323035d588de8dfb1c943442bd741da263b49ae02dac4ac8f5c78d`  
		Last Modified: Thu, 07 Sep 2023 14:30:22 GMT  
		Size: 4.8 KB (4785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:bookworm` - linux; arm variant v5

```console
$ docker pull postgres@sha256:eb166517b9afdb3026bd0c8d200b24498cff3764172d304cec329e12d494c0c3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.9 MB (141873334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3f69dc17b096fd8de34dd98d4b9d125589787bd7a10bb11f96de0110309e78a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 07 Sep 2023 00:48:30 GMT
ADD file:e7b77e5797ddb7e058507462fd5f5aad6864ba08ebc4a6c2743dae81ed0f445d in / 
# Thu, 07 Sep 2023 00:48:31 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 02:53:45 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 07 Sep 2023 02:53:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:53:53 GMT
ENV GOSU_VERSION=1.16
# Thu, 07 Sep 2023 02:54:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 07 Sep 2023 02:54:15 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 07 Sep 2023 02:54:15 GMT
ENV LANG=en_US.utf8
# Thu, 07 Sep 2023 02:54:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 02:54:22 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 07 Sep 2023 02:54:23 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 07 Sep 2023 03:30:01 GMT
ENV PG_MAJOR=15
# Thu, 07 Sep 2023 03:30:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Thu, 07 Sep 2023 03:30:02 GMT
ENV PG_VERSION=15.4-1.pgdg120+1
# Thu, 07 Sep 2023 03:45:07 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 07 Sep 2023 03:45:09 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 07 Sep 2023 03:45:10 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 07 Sep 2023 03:45:10 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 07 Sep 2023 03:45:10 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 07 Sep 2023 03:45:10 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 07 Sep 2023 03:45:10 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Thu, 07 Sep 2023 03:45:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Sep 2023 03:45:11 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 03:45:11 GMT
EXPOSE 5432
# Thu, 07 Sep 2023 03:45:11 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:d971e043cc5e8068fe39c736806d279b128c720a08d2e0d41002dcf027787939`  
		Last Modified: Thu, 07 Sep 2023 00:51:35 GMT  
		Size: 27.0 MB (26983530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de8b047558c321f3d85dac362acc6b5be2ef1a63e1228dcc312fe0349e7368d`  
		Last Modified: Thu, 07 Sep 2023 05:51:18 GMT  
		Size: 1.2 KB (1211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a001ee6f62d264464ebac6fa7957af0eef9f2b372d086b3ceb5ca0716d4a7c`  
		Last Modified: Thu, 07 Sep 2023 05:51:20 GMT  
		Size: 4.2 MB (4236742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088a29538691f49cbe34a2b6ad563f1906160e4d50d03209b0060a3ea384a736`  
		Last Modified: Thu, 07 Sep 2023 05:51:18 GMT  
		Size: 1.4 MB (1422349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5642e454380eb8686c56be7ecce79209c1bbf2b5e9e29d5d0155e611b336f2e2`  
		Last Modified: Thu, 07 Sep 2023 05:51:19 GMT  
		Size: 8.1 MB (8065171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b620324ad132460ef93d433f9180591c03a526c710577816ef1644bec32ddd70`  
		Last Modified: Thu, 07 Sep 2023 05:51:16 GMT  
		Size: 1.4 MB (1404068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4ffcb4a7cd4a043e5b402406876a8cf7b66de35c58e3d7ceb859398ba7d5ee`  
		Last Modified: Thu, 07 Sep 2023 05:51:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef49764891b3f19a655bc08ffff0cc05e87eecd546576c26e55740dcea514f0a`  
		Last Modified: Thu, 07 Sep 2023 05:51:15 GMT  
		Size: 3.2 KB (3201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:163d8890aed0e61554de10b278e4e526cafaab144060eb567f20bff94a99cee9`  
		Last Modified: Thu, 07 Sep 2023 05:52:21 GMT  
		Size: 99.7 MB (99742008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d32e9996be49193bbc50198363e9cf86fb8b5e5784265aa6c2b8c8a2f28849e`  
		Last Modified: Thu, 07 Sep 2023 05:52:03 GMT  
		Size: 9.8 KB (9788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f677ed8e3ab39ae0338fad103225b4bf6e5d68935e8ca39c29f97909ae56521`  
		Last Modified: Thu, 07 Sep 2023 05:52:03 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e51381d43203240e0f5650cf57b1ed8fd21ba1d5d627b1de5aa413e309ee71`  
		Last Modified: Thu, 07 Sep 2023 05:52:03 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ae96759e535a41f7f26366fc130a33b087a5a1cac26cd48facc538aec473d6`  
		Last Modified: Thu, 07 Sep 2023 05:52:03 GMT  
		Size: 4.8 KB (4787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:bookworm` - linux; arm variant v7

```console
$ docker pull postgres@sha256:1e2a88236ee8148caeceab5b65459d1aa5a28f60e7567d68107c20a470040ec9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136737618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea312e82fb7b61e0bab66f534a2aa6b3ff39d32ce9d8c2ff67ae21c77adda663`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 07 Sep 2023 00:57:48 GMT
ADD file:5775cb975a13a9e48198190564cd469f115a433dabc5c3406c45e1ef0b1ccdf0 in / 
# Thu, 07 Sep 2023 00:57:49 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 04:11:32 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 07 Sep 2023 04:11:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 04:11:39 GMT
ENV GOSU_VERSION=1.16
# Thu, 07 Sep 2023 04:11:48 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 07 Sep 2023 04:11:55 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 07 Sep 2023 04:11:55 GMT
ENV LANG=en_US.utf8
# Thu, 07 Sep 2023 04:11:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 04:12:00 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 07 Sep 2023 04:12:01 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 07 Sep 2023 04:41:52 GMT
ENV PG_MAJOR=15
# Thu, 07 Sep 2023 04:41:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Thu, 07 Sep 2023 04:41:52 GMT
ENV PG_VERSION=15.4-1.pgdg120+1
# Thu, 07 Sep 2023 04:56:20 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 07 Sep 2023 04:56:22 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 07 Sep 2023 04:56:23 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 07 Sep 2023 04:56:23 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 07 Sep 2023 04:56:24 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 07 Sep 2023 04:56:24 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 07 Sep 2023 04:56:24 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Thu, 07 Sep 2023 04:56:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Sep 2023 04:56:24 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 04:56:24 GMT
EXPOSE 5432
# Thu, 07 Sep 2023 04:56:25 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:6a9fec8868f77cdcda1bf847be168c1d104031ca6c8edc961bc7f76e3a4bf54b`  
		Last Modified: Thu, 07 Sep 2023 01:02:31 GMT  
		Size: 24.8 MB (24805221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999d6861171255263f391e61de575844c466d1febd75af8fa5d511fac54e3cfc`  
		Last Modified: Thu, 07 Sep 2023 06:55:41 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53577034808c93e57db36b89db59aa949c0fbc412ce574993eca6d27b888334e`  
		Last Modified: Thu, 07 Sep 2023 06:55:41 GMT  
		Size: 3.8 MB (3839571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eaf7a366d36d9a45c69a4e4c643b64dd1a52c041349f4725afdb533c28841a2`  
		Last Modified: Thu, 07 Sep 2023 06:55:41 GMT  
		Size: 1.4 MB (1411957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffa833623bff42fe1cb8cbdffb7fadba5270226da7af67adfca20c4602aa02c`  
		Last Modified: Thu, 07 Sep 2023 06:55:41 GMT  
		Size: 8.1 MB (8065045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc754d0b977295419a2f915ff581a2f9bc3b02899e96adebf5124b5eccc19fe7`  
		Last Modified: Thu, 07 Sep 2023 06:55:39 GMT  
		Size: 1.3 MB (1277643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec504dc35e1c85529fedf0ada8ee845054a2b940034afd8184ce27cfecd9f1a`  
		Last Modified: Thu, 07 Sep 2023 06:55:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cccd2df8625a79b96543f30d28afd1ed156b2c0db4639d8a890ab84923a6b0`  
		Last Modified: Thu, 07 Sep 2023 06:55:38 GMT  
		Size: 3.2 KB (3198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c8abce3f98ca32ed2a416acb99b5db4fe08a6bd017f1a3ea4807afff98343c`  
		Last Modified: Thu, 07 Sep 2023 06:56:42 GMT  
		Size: 97.3 MB (97318720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc17a3911609a2d38f5bbed16be15263d569fcdee39760d53e3c5caa9617425`  
		Last Modified: Thu, 07 Sep 2023 06:56:25 GMT  
		Size: 9.8 KB (9789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6d03f1f0b4c3d0c8b33798f45a6e05c6494f0d2b4aee1ecdcd23750cde87d4`  
		Last Modified: Thu, 07 Sep 2023 06:56:26 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092f44b5a4e8699f7da08c7f057a7b6ae80778de9a3a7114780fdf24d461bc61`  
		Last Modified: Thu, 07 Sep 2023 06:56:25 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21811e021547b97edda3c58fe6a101fe41ba8fac258338c892da82254c7e0ae2`  
		Last Modified: Thu, 07 Sep 2023 06:56:26 GMT  
		Size: 4.8 KB (4786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:bookworm` - linux; arm64 variant v8

```console
$ docker pull postgres@sha256:fbe5c7dcac8d88393f773df3eeeee9a0b84a694015777f7a09dab67ba5459aa0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.8 MB (146821288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e9c7a43157267165cdd2f1d96791a1e2c14a4cfaf6a2cb7f23f68cb5085e9a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:39 GMT
ADD file:fb5c8f411c4a1e06c25ac32455221938386907d0b4782fc228ca67de63a7e9de in / 
# Thu, 07 Sep 2023 00:39:39 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 05:48:59 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 07 Sep 2023 05:49:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 05:49:04 GMT
ENV GOSU_VERSION=1.16
# Thu, 07 Sep 2023 05:49:12 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 07 Sep 2023 05:49:17 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 07 Sep 2023 05:49:17 GMT
ENV LANG=en_US.utf8
# Thu, 07 Sep 2023 05:49:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 05:49:21 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 07 Sep 2023 05:49:22 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 07 Sep 2023 05:50:38 GMT
ENV PG_MAJOR=15
# Thu, 07 Sep 2023 05:50:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Thu, 07 Sep 2023 05:50:38 GMT
ENV PG_VERSION=15.4-1.pgdg120+1
# Thu, 07 Sep 2023 05:50:53 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 07 Sep 2023 05:50:55 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 07 Sep 2023 05:50:55 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 07 Sep 2023 05:50:55 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 07 Sep 2023 05:50:55 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 07 Sep 2023 05:50:56 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 07 Sep 2023 05:50:56 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Thu, 07 Sep 2023 05:50:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Sep 2023 05:50:56 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 05:50:56 GMT
EXPOSE 5432
# Thu, 07 Sep 2023 05:50:56 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:155eab17d86c47443adc8cebe7fc62c847c03db8cfb1ca53aa6276564fff23ef`  
		Last Modified: Thu, 07 Sep 2023 00:43:02 GMT  
		Size: 29.2 MB (29157149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55722f192d83c20c8f76ea6e4a67442422f4e3b267cf5bb52fab9574a8a823e`  
		Last Modified: Thu, 07 Sep 2023 05:55:26 GMT  
		Size: 1.2 KB (1211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ba17ccdd1c8e7039acb98c0b4a8cd5032a8e24401a3a41051b5cee8fff3e10`  
		Last Modified: Thu, 07 Sep 2023 05:55:27 GMT  
		Size: 4.6 MB (4578373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18dfde5d5395194e4bd8d2acfa1fbfb6f7fb981552740db93ef72532f54105fe`  
		Last Modified: Thu, 07 Sep 2023 05:55:26 GMT  
		Size: 1.4 MB (1376571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e1089c0d388aca82bdb508c841d9f075b32ef2f15363741feb9ff244dd966b`  
		Last Modified: Thu, 07 Sep 2023 05:55:26 GMT  
		Size: 8.1 MB (8065199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d777fedefbac0ed8c7489beb6415c5d956cdcb3735bf2ebebe57c34cbe311a63`  
		Last Modified: Thu, 07 Sep 2023 05:55:24 GMT  
		Size: 1.3 MB (1317866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f0a37cd4f7f3593b3341ef531274d82c2b6d39d815735f96d83e088d21b185d`  
		Last Modified: Thu, 07 Sep 2023 05:55:24 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d24f0e05805b51cca91a59256efc113f3c1c534404287899152d50e9b03ea7`  
		Last Modified: Thu, 07 Sep 2023 05:55:24 GMT  
		Size: 3.2 KB (3200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34466a80c9764f275d591aed50958da4e348a8a4edc8e807842c0487e75eacdf`  
		Last Modified: Thu, 07 Sep 2023 05:56:08 GMT  
		Size: 102.3 MB (102306676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2dc7454877a681a9779d1403687f28b9aaef789ebb68243bafd920862af7590`  
		Last Modified: Thu, 07 Sep 2023 05:55:57 GMT  
		Size: 9.8 KB (9781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad478a2aa98215ec23c3649b239d6a5a932ecc825e27084a947d82b02f222978`  
		Last Modified: Thu, 07 Sep 2023 05:55:57 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd605ff234cd454377420132d241b991bd23ddfb22399a3c4bfe7cafefb4642`  
		Last Modified: Thu, 07 Sep 2023 05:55:57 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d24de45b25a03287beb312d90bbc699cefa77b7f74e39b411c6e4e49469a4262`  
		Last Modified: Thu, 07 Sep 2023 05:55:57 GMT  
		Size: 4.8 KB (4786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:bookworm` - linux; 386

```console
$ docker pull postgres@sha256:a178759239b057330399b9e3c32b98382812c977ff42cbf147b3c33ba900b7b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.0 MB (156044493 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4cf57d7c38a73ac2b86d9ab90a6d61acf472aef7febf0ba5b2ebca854481935`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:00 GMT
ADD file:0952a54f5474629ed000e89bfd1b8827e49b63270932e45ed8d953a2676ac79c in / 
# Thu, 07 Sep 2023 00:39:00 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:08:48 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 07 Sep 2023 01:08:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:08:56 GMT
ENV GOSU_VERSION=1.16
# Thu, 07 Sep 2023 01:09:08 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 07 Sep 2023 01:09:17 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 07 Sep 2023 01:09:17 GMT
ENV LANG=en_US.utf8
# Thu, 07 Sep 2023 01:09:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:09:23 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 07 Sep 2023 01:09:24 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 07 Sep 2023 01:48:53 GMT
ENV PG_MAJOR=15
# Thu, 07 Sep 2023 01:48:53 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Thu, 07 Sep 2023 01:48:53 GMT
ENV PG_VERSION=15.4-1.pgdg120+1
# Thu, 07 Sep 2023 02:07:12 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 07 Sep 2023 02:07:15 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 07 Sep 2023 02:07:15 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 07 Sep 2023 02:07:15 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 07 Sep 2023 02:07:16 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 07 Sep 2023 02:07:16 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 07 Sep 2023 02:07:16 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Thu, 07 Sep 2023 02:07:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Sep 2023 02:07:16 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 02:07:16 GMT
EXPOSE 5432
# Thu, 07 Sep 2023 02:07:16 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:30ae0f429560d1effd0839849ab7780512b72d9fbc09a6cec67e03092a85a1d1`  
		Last Modified: Thu, 07 Sep 2023 00:43:48 GMT  
		Size: 30.1 MB (30141753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f46dbec3f5e6f4c75ea8d19dae300dcffbb4aa5d5d46b76033825d46bd8c262`  
		Last Modified: Thu, 07 Sep 2023 04:40:03 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8d71699dabe1c5baf4a11e8c37292bc4f8d1ad9f7800643542f194795389bd`  
		Last Modified: Thu, 07 Sep 2023 04:40:04 GMT  
		Size: 5.0 MB (5039432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40dcb44c9c86789af1867251d6aaa55a0f5626ba1a4d55c7bf0babd8d0ce993a`  
		Last Modified: Thu, 07 Sep 2023 04:40:03 GMT  
		Size: 1.4 MB (1420316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa64f3aa56ca13d5ede15422c423d1e5f8280cf13302284230e2dc05348c81f`  
		Last Modified: Thu, 07 Sep 2023 04:40:04 GMT  
		Size: 8.1 MB (8065077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0143e5ca7ce1c66755ed946ffd59d214d6d446df619144f1a167b2d04f4f77fa`  
		Last Modified: Thu, 07 Sep 2023 04:40:01 GMT  
		Size: 1.3 MB (1346477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e61f6dd5a6b813733d4817d4e1b6dbc03aca80351b3d802637529dbcf5d1a6d`  
		Last Modified: Thu, 07 Sep 2023 04:40:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f517a716c661221e613e926a9a1e5802d4976be5e9465314f7392dda961c4aed`  
		Last Modified: Thu, 07 Sep 2023 04:40:00 GMT  
		Size: 3.2 KB (3200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfcaaa2fdd66835b7b0df156f1a1d17fddacfe7f15e46b9fa677cad76964552f`  
		Last Modified: Thu, 07 Sep 2023 04:41:21 GMT  
		Size: 110.0 MB (110011973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8455ea8b1f7671f87bf86bd50d42c97d9f97803a2de263978f9916a060abe37a`  
		Last Modified: Thu, 07 Sep 2023 04:40:59 GMT  
		Size: 9.8 KB (9788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2880399fdec33bafff40db6c2af58df160afc327b4bc4a2906050b66c92fa21`  
		Last Modified: Thu, 07 Sep 2023 04:40:59 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565c35b3e53658175b159899b2e2902628528bc3071659d77972c0e67c69356d`  
		Last Modified: Thu, 07 Sep 2023 04:40:59 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6c57b706ce33980a78393250b84e34de5bc9c59818e9796f9a6272b04687b7`  
		Last Modified: Thu, 07 Sep 2023 04:40:59 GMT  
		Size: 4.8 KB (4790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:bookworm` - linux; mips64le

```console
$ docker pull postgres@sha256:8ea71f5b11082c8df68fe131da5813ee81a440b4e2762e953bf529f8c9ee795d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.6 MB (144636782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43585a2de0b9d813a35411cbc87f16da5d8de37f913dff5eeab7ab2cbbb3aaad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 07 Sep 2023 01:09:11 GMT
ADD file:263719948aa8496c0852aa2ef6c6660c25ce35618af5b1c5bc35c901d853bcf8 in / 
# Thu, 07 Sep 2023 01:09:17 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 19:44:23 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 07 Sep 2023 19:44:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 19:44:58 GMT
ENV GOSU_VERSION=1.16
# Thu, 07 Sep 2023 19:45:30 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 07 Sep 2023 19:45:58 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 07 Sep 2023 19:46:01 GMT
ENV LANG=en_US.utf8
# Thu, 07 Sep 2023 19:46:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 19:46:25 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 07 Sep 2023 19:46:31 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 07 Sep 2023 21:58:37 GMT
ENV PG_MAJOR=15
# Thu, 07 Sep 2023 21:58:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Thu, 07 Sep 2023 21:58:42 GMT
ENV PG_VERSION=15.4-1.pgdg120+1
# Thu, 07 Sep 2023 23:00:57 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 07 Sep 2023 23:01:03 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 07 Sep 2023 23:01:09 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 07 Sep 2023 23:01:12 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 07 Sep 2023 23:01:18 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 07 Sep 2023 23:01:21 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 07 Sep 2023 23:01:24 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Thu, 07 Sep 2023 23:01:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Sep 2023 23:01:30 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 23:01:33 GMT
EXPOSE 5432
# Thu, 07 Sep 2023 23:01:37 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:a6519d39af9071c1099bd2a01d04c824d095fb31f439e10814371707227802ae`  
		Last Modified: Thu, 07 Sep 2023 01:20:14 GMT  
		Size: 29.1 MB (29121387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18af474dc84f99261867730073661aba1d2fd9557be2b13b58d9d24d8c73f066`  
		Last Modified: Fri, 08 Sep 2023 07:46:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:618cd013a798c25885029837623a9d7847c3f015faa81eadab5587c131ca35fd`  
		Last Modified: Fri, 08 Sep 2023 07:46:26 GMT  
		Size: 4.4 MB (4355627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185fcc2cb22a64b3b53aa8d284136774bbdfd422831194549af977436c982c69`  
		Last Modified: Fri, 08 Sep 2023 07:46:24 GMT  
		Size: 1.3 MB (1331491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c9d587d20dea2a5f0ae108d5ca0e269cca19f1a107b3a17a2b0758d1bdbd7f`  
		Last Modified: Fri, 08 Sep 2023 07:46:28 GMT  
		Size: 8.1 MB (8064894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffacf3d23809923d6c0de9ea58fa547184988d38fe6c224e52670a7ccd2c750`  
		Last Modified: Fri, 08 Sep 2023 07:46:21 GMT  
		Size: 1.2 MB (1181558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb738a4bc28ff81d76098f725a2f84a8990d65f0f427abf798f41ff01e7eb4a5`  
		Last Modified: Fri, 08 Sep 2023 07:46:20 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b888b5bb2dc1d7c10d07be463e3f579c948ee61267c232ea1de55cde8a16a40f`  
		Last Modified: Fri, 08 Sep 2023 07:46:19 GMT  
		Size: 3.1 KB (3139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a604eb00156b3482cb59108be0864df3436a3d529c1afcf178ba151ba2c440fc`  
		Last Modified: Fri, 08 Sep 2023 07:49:44 GMT  
		Size: 100.6 MB (100562563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107a0625382844a6f0b2b72e1f6f7ad22278e8678d0a5bdc5f2a764402ace38a`  
		Last Modified: Fri, 08 Sep 2023 07:48:40 GMT  
		Size: 9.8 KB (9788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8cec4c3f7007510d8313b40b09fa2ad44310644ed61dc29a5e8f05448a911fa`  
		Last Modified: Fri, 08 Sep 2023 07:48:40 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e8d17593505bf3954818daa621e32b430f888b8414e2a280d24fa88d888e840`  
		Last Modified: Fri, 08 Sep 2023 07:48:40 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94cc626680c381f182b92bd4a3dc85355f05aa745b5cc73245428b224c55288c`  
		Last Modified: Fri, 08 Sep 2023 07:48:40 GMT  
		Size: 4.8 KB (4790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:bookworm` - linux; ppc64le

```console
$ docker pull postgres@sha256:d64738a8433215b94d7338f4ef3f2fa4af16bcdedb1c8ee487ba6f10c2d2d674
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.7 MB (160680235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abcc884c479b9f5185479b514511bdfd8a1753c729aceca3e3f2305e3b67ace8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 07 Sep 2023 00:17:29 GMT
ADD file:c5cce4a01995fb11fea5067fdf342af046481b4869e8e858a85986686f68ef2a in / 
# Thu, 07 Sep 2023 00:17:32 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 16:25:14 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 07 Sep 2023 16:25:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 16:25:32 GMT
ENV GOSU_VERSION=1.16
# Thu, 07 Sep 2023 16:25:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 07 Sep 2023 16:26:07 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 07 Sep 2023 16:26:08 GMT
ENV LANG=en_US.utf8
# Thu, 07 Sep 2023 16:26:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 16:26:20 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 07 Sep 2023 16:26:22 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 07 Sep 2023 16:29:51 GMT
ENV PG_MAJOR=15
# Thu, 07 Sep 2023 16:29:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Thu, 07 Sep 2023 16:29:52 GMT
ENV PG_VERSION=15.4-1.pgdg120+1
# Thu, 07 Sep 2023 16:30:40 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 07 Sep 2023 16:30:46 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 07 Sep 2023 16:30:47 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 07 Sep 2023 16:30:48 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 07 Sep 2023 16:30:49 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 07 Sep 2023 16:30:50 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 07 Sep 2023 16:30:50 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Thu, 07 Sep 2023 16:30:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Sep 2023 16:30:52 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 16:30:52 GMT
EXPOSE 5432
# Thu, 07 Sep 2023 16:30:53 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:1db76043538a495ac265ef61277e1a2137637bebdc1ffa7712108b3efe4a4d33`  
		Last Modified: Thu, 07 Sep 2023 00:23:29 GMT  
		Size: 33.1 MB (33119207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca4407b91945cefaf57592756b201b9bbed2e8dc33baa9972abb512406c06da`  
		Last Modified: Thu, 07 Sep 2023 16:42:09 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e17881de676d15d36eae9d56f24ca1f069cb1abda2d5a5cc896a2f9782d673`  
		Last Modified: Thu, 07 Sep 2023 16:42:10 GMT  
		Size: 5.4 MB (5433636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039c3785da844676d84eda8a89b711923496f248b15dfce8ceca922006528c59`  
		Last Modified: Thu, 07 Sep 2023 16:42:09 GMT  
		Size: 1.4 MB (1367241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c566d192e2b6d880fef53c3ee90831024c62f21caf5d5935c24daf0fc89c1e89`  
		Last Modified: Thu, 07 Sep 2023 16:42:09 GMT  
		Size: 8.1 MB (8065164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e12edd582ad487fdd333d82dd17da5ef809694798fae513d639fb9c5f7dedd3`  
		Last Modified: Thu, 07 Sep 2023 16:42:07 GMT  
		Size: 1.5 MB (1494542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d381305b9544768a35acc06d02a8ade09c3437f15a4b55bfbb9f4d781b89fb9`  
		Last Modified: Thu, 07 Sep 2023 16:42:07 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b58c5d8694270b75bf48e1e4ab863e482aab47b9deb973e3b855beea679ef9`  
		Last Modified: Thu, 07 Sep 2023 16:42:07 GMT  
		Size: 3.2 KB (3200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0692766adae57aac5f60065d5f160594c4e87f870f30266cf0f6f999dc324d83`  
		Last Modified: Thu, 07 Sep 2023 16:43:39 GMT  
		Size: 111.2 MB (111180990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd2d60a66c75307dcbc146cf98b7baa55a2efcba503081eeb0a591e4b5a57d9`  
		Last Modified: Thu, 07 Sep 2023 16:43:13 GMT  
		Size: 9.8 KB (9778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c692ef7bf614b43c127e5b874358949a9f3f02d4c9cfaca307025d789e907af7`  
		Last Modified: Thu, 07 Sep 2023 16:43:13 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149c2da3be7cc479191b5f943d26746fcf4a9b582adddffec399486d5f5e7b76`  
		Last Modified: Thu, 07 Sep 2023 16:43:13 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d134baa299fc1923876734236ca38a422c0f9b6e4faa06f1a8e85c476e7dcf4`  
		Last Modified: Thu, 07 Sep 2023 16:43:13 GMT  
		Size: 4.8 KB (4788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postgres:bookworm` - linux; s390x

```console
$ docker pull postgres@sha256:3890ea25c56265f60352d9cc5528711722374f546d5b82e4be1415ab04090b9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.2 MB (154199240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1ac3f15270ed789f14ddcd14cbde490535d43bd90b2ce417825c5d5850fa2aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["postgres"]`

```dockerfile
# Thu, 07 Sep 2023 00:43:39 GMT
ADD file:2a617cce71dc34ce7b62d4b1da4b45cca574c219300ba2be25396630f80bb9cd in / 
# Thu, 07 Sep 2023 00:43:47 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 09:43:21 GMT
RUN set -eux; 	groupadd -r postgres --gid=999; 	useradd -r -g postgres --uid=999 --home-dir=/var/lib/postgresql --shell=/bin/bash postgres; 	mkdir -p /var/lib/postgresql; 	chown -R postgres:postgres /var/lib/postgresql
# Thu, 07 Sep 2023 09:43:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 09:43:26 GMT
ENV GOSU_VERSION=1.16
# Thu, 07 Sep 2023 09:43:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 07 Sep 2023 09:43:40 GMT
RUN set -eux; 	if [ -f /etc/dpkg/dpkg.cfg.d/docker ]; then 		grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 		sed -ri '/\/usr\/share\/locale/d' /etc/dpkg/dpkg.cfg.d/docker; 		! grep -q '/usr/share/locale' /etc/dpkg/dpkg.cfg.d/docker; 	fi; 	apt-get update; apt-get install -y --no-install-recommends locales; rm -rf /var/lib/apt/lists/*; 	localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
# Thu, 07 Sep 2023 09:43:40 GMT
ENV LANG=en_US.utf8
# Thu, 07 Sep 2023 09:43:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libnss-wrapper 		xz-utils 		zstd 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 09:43:44 GMT
RUN mkdir /docker-entrypoint-initdb.d
# Thu, 07 Sep 2023 09:43:45 GMT
RUN set -ex; 	key='B97B0AFCAA1A47F044F244A07FCC7D46ACCC4CF8'; 	export GNUPGHOME="$(mktemp -d)"; 	mkdir -p /usr/local/share/keyrings/; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	gpg --batch --export --armor "$key" > /usr/local/share/keyrings/postgres.gpg.asc; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME"
# Thu, 07 Sep 2023 09:45:30 GMT
ENV PG_MAJOR=15
# Thu, 07 Sep 2023 09:45:30 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/postgresql/15/bin
# Thu, 07 Sep 2023 09:45:30 GMT
ENV PG_VERSION=15.4-1.pgdg120+1
# Thu, 07 Sep 2023 09:45:52 GMT
RUN set -ex; 		export PYTHONDONTWRITEBYTECODE=1; 		dpkgArch="$(dpkg --print-architecture)"; 	aptRepo="[ signed-by=/usr/local/share/keyrings/postgres.gpg.asc ] http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main $PG_MAJOR"; 	case "$dpkgArch" in 		amd64 | arm64 | ppc64el | s390x) 			echo "deb $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 			apt-get update; 			;; 		*) 			echo "deb-src $aptRepo" > /etc/apt/sources.list.d/pgdg.list; 						savedAptMark="$(apt-mark showmanual)"; 						tempDir="$(mktemp -d)"; 			cd "$tempDir"; 						apt-get update; 			apt-get install -y --no-install-recommends dpkg-dev; 			echo "deb [ trusted=yes ] file://$tempDir ./" > /etc/apt/sources.list.d/temp.list; 			_update_repo() { 				dpkg-scanpackages . > Packages; 				apt-get -o Acquire::GzipIndexes=false update; 			}; 			_update_repo; 						nproc="$(nproc)"; 			export DEB_BUILD_OPTIONS="nocheck parallel=$nproc"; 			apt-get build-dep -y postgresql-common pgdg-keyring; 			apt-get source --compile postgresql-common pgdg-keyring; 			_update_repo; 			apt-get build-dep -y "postgresql-$PG_MAJOR=$PG_VERSION"; 			apt-get source --compile "postgresql-$PG_MAJOR=$PG_VERSION"; 									apt-mark showmanual | xargs apt-mark auto > /dev/null; 			apt-mark manual $savedAptMark; 						ls -lAFh; 			_update_repo; 			grep '^Package: ' Packages; 			cd /; 			;; 	esac; 		apt-get install -y --no-install-recommends postgresql-common; 	sed -ri 's/#(create_main_cluster) .*$/\1 = false/' /etc/postgresql-common/createcluster.conf; 	apt-get install -y --no-install-recommends 		"postgresql-$PG_MAJOR=$PG_VERSION" 	; 		rm -rf /var/lib/apt/lists/*; 		if [ -n "$tempDir" ]; then 		apt-get purge -y --auto-remove; 		rm -rf "$tempDir" /etc/apt/sources.list.d/temp.list; 	fi; 		find /usr -name '*.pyc' -type f -exec bash -c 'for pyc; do dpkg -S "$pyc" &> /dev/null || rm -vf "$pyc"; done' -- '{}' +; 		postgres --version
# Thu, 07 Sep 2023 09:45:59 GMT
RUN set -eux; 	dpkg-divert --add --rename --divert "/usr/share/postgresql/postgresql.conf.sample.dpkg" "/usr/share/postgresql/$PG_MAJOR/postgresql.conf.sample"; 	cp -v /usr/share/postgresql/postgresql.conf.sample.dpkg /usr/share/postgresql/postgresql.conf.sample; 	ln -sv ../postgresql.conf.sample "/usr/share/postgresql/$PG_MAJOR/"; 	sed -ri "s!^#?(listen_addresses)\s*=\s*\S+.*!\1 = '*'!" /usr/share/postgresql/postgresql.conf.sample; 	grep -F "listen_addresses = '*'" /usr/share/postgresql/postgresql.conf.sample
# Thu, 07 Sep 2023 09:45:59 GMT
RUN mkdir -p /var/run/postgresql && chown -R postgres:postgres /var/run/postgresql && chmod 2777 /var/run/postgresql
# Thu, 07 Sep 2023 09:45:59 GMT
ENV PGDATA=/var/lib/postgresql/data
# Thu, 07 Sep 2023 09:46:00 GMT
RUN mkdir -p "$PGDATA" && chown -R postgres:postgres "$PGDATA" && chmod 777 "$PGDATA"
# Thu, 07 Sep 2023 09:46:00 GMT
VOLUME [/var/lib/postgresql/data]
# Thu, 07 Sep 2023 09:46:00 GMT
COPY file:512acb0aab31f9e5d908f16e2f4478f65cddd5d4e555a02a1551074bb16f54d7 in /usr/local/bin/ 
# Thu, 07 Sep 2023 09:46:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Sep 2023 09:46:01 GMT
STOPSIGNAL SIGINT
# Thu, 07 Sep 2023 09:46:01 GMT
EXPOSE 5432
# Thu, 07 Sep 2023 09:46:01 GMT
CMD ["postgres"]
```

-	Layers:
	-	`sha256:68043338ec5d8515f0dcc40f82eb11d30dd8539a1d30984e4b157df8779f6d53`  
		Last Modified: Thu, 07 Sep 2023 00:49:40 GMT  
		Size: 27.5 MB (27489648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47ff2b4de49c4c26503044f9c80367bcea18c867befe09b99cce4ebc2edd8cf`  
		Last Modified: Thu, 07 Sep 2023 09:54:48 GMT  
		Size: 1.2 KB (1211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3709e147d007a9416b5d5c525e0407cb89d479abc59ef6e4190e5654674740be`  
		Last Modified: Thu, 07 Sep 2023 09:54:48 GMT  
		Size: 4.5 MB (4474543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5d2e99909cd167970fb123f11ffaaf2ccd3e2220db859d8682f85175bb264d`  
		Last Modified: Thu, 07 Sep 2023 09:54:47 GMT  
		Size: 1.4 MB (1410596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15e0461a9395a1992567658cfe4a86ba3d72ffe923713c674ef726e86c8d928`  
		Last Modified: Thu, 07 Sep 2023 09:54:47 GMT  
		Size: 8.1 MB (8119622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ed487407e3f8279ef057a42a0f127fd6232bfe32efc6f00719b74d8f6aeab7`  
		Last Modified: Thu, 07 Sep 2023 09:54:46 GMT  
		Size: 1.3 MB (1307758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08560e87a93355c4c4c871dc754a38ec33527ba5c306f9ac90765a421009b2c2`  
		Last Modified: Thu, 07 Sep 2023 09:54:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe713cb98eb252c0f75a308e583accad73d821271550d4d7c20e53aa2697f811`  
		Last Modified: Thu, 07 Sep 2023 09:54:46 GMT  
		Size: 3.2 KB (3193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aece52fbe46eca83c8c9c337a117a9d7869901df65a0ed3044c13ee88fe5ff29`  
		Last Modified: Thu, 07 Sep 2023 09:55:37 GMT  
		Size: 111.4 MB (111377623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e729a15b60d50a9f833eae83e47760a7560b757044bd14fa845b1a58a34efb7`  
		Last Modified: Thu, 07 Sep 2023 09:55:22 GMT  
		Size: 9.8 KB (9779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7e0e915c01ccc7ca27c2607c48375b0b014c0f6324c4e47980cab38fdf61f6`  
		Last Modified: Thu, 07 Sep 2023 09:55:22 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73246c8228321475191f9905d155c956b4d0c766f3f22e797a0b00fff98f91d`  
		Last Modified: Thu, 07 Sep 2023 09:55:22 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1ddb7fe066728471b3d0dc580bd42973c16c7e382b21b2839fef95d8a2f412`  
		Last Modified: Thu, 07 Sep 2023 09:55:22 GMT  
		Size: 4.8 KB (4787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
