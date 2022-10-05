<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `couchdb`

-	[`couchdb:2`](#couchdb2)
-	[`couchdb:2.3`](#couchdb23)
-	[`couchdb:2.3.1`](#couchdb231)
-	[`couchdb:3`](#couchdb3)
-	[`couchdb:3.1`](#couchdb31)
-	[`couchdb:3.1.2`](#couchdb312)
-	[`couchdb:3.2`](#couchdb32)
-	[`couchdb:3.2.2`](#couchdb322)
-	[`couchdb:latest`](#couchdblatest)

## `couchdb:2`

```console
$ docker pull couchdb@sha256:e8885a73041d303b37bfd493d7deb8e057e834429df127dd5ee0e950fac5b534
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2` - linux; amd64

```console
$ docker pull couchdb@sha256:fdd360c2699c5ccce0e926e64e111ac1ddbeea91ae06bd8c8342deab8bbece81
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84521637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ea24299b2688202b1f16bf104a8edd9d9d3620e72226b286c744b41527dd3c1`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:48 GMT
ADD file:782d864aa72c2d5fb599311ebae56db4067d2e91ff532c1aaf1a291c3dbce5bb in / 
# Tue, 13 Sep 2022 00:56:49 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:54:33 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Sep 2022 03:54:34 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Sep 2022 03:54:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:54:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 13 Sep 2022 03:54:45 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Sep 2022 03:54:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:55:14 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 13 Sep 2022 03:55:14 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Sep 2022 03:55:32 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Sep 2022 03:55:32 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Sep 2022 03:55:32 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 13 Sep 2022 03:55:32 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 13 Sep 2022 03:55:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 03:55:33 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Sep 2022 03:55:33 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Sep 2022 03:55:33 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Sep 2022 03:55:33 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:4b7b4a8876e2f677668e51b8473f97a237d3d4df201b9df4031bcaa8068370b1`  
		Last Modified: Tue, 13 Sep 2022 01:01:16 GMT  
		Size: 27.1 MB (27130552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c088c3a03bf60b8f0b3b24363efbc28aef3c87451537b97521bfbf1f2aa13199`  
		Last Modified: Tue, 13 Sep 2022 03:56:21 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65e6c9d6ee4b135545b364dd8b30be2b91e27e6b1e62addf07801a90a90ac96f`  
		Last Modified: Tue, 13 Sep 2022 03:56:20 GMT  
		Size: 6.7 MB (6698707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e1633127944965c144a64754b6a92bf6622c1de73c33716a59ca7f9ef1baca`  
		Last Modified: Tue, 13 Sep 2022 03:56:19 GMT  
		Size: 1.3 MB (1258362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61a40f9af1917164479b4fc40fc1f8fa2db40005957a46bb7b167f3a6f2724c`  
		Last Modified: Tue, 13 Sep 2022 03:56:18 GMT  
		Size: 293.1 KB (293062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d24fe37ce953bdb8931392614becce928b2547796764bddd9f88e56c6ed97d8`  
		Last Modified: Tue, 13 Sep 2022 03:56:34 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283af9663b67d645492bd442d5e7cbc4a46b247238ff7aed93a0483c77310649`  
		Last Modified: Tue, 13 Sep 2022 03:56:38 GMT  
		Size: 49.1 MB (49133940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4788d07645893982eb35d79013264bcb958817cb4c1c0e52f0254f8de7e34c33`  
		Last Modified: Tue, 13 Sep 2022 03:56:32 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e97b88ff5fd41abb9abad7b6ce9c27f883f8df6819b6074f7e6732f3e396ce`  
		Last Modified: Tue, 13 Sep 2022 03:56:32 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6073742d94dc8629793832fe392891511bc2c7fa5be1aa13b87b50d0d956c430`  
		Last Modified: Tue, 13 Sep 2022 03:56:32 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f3d38689c87981ca7f5c0ace468c72ed5ff7a897ed74b8d86386db94be8d949`  
		Last Modified: Tue, 13 Sep 2022 03:56:32 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:b5f6db08e39cf0632d9bed88436c31f501c02d7ecb7b0863ed2efb9076420334
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72533691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56458d08878446377adc3bfd36d6cd5a04d270972781aa4c5ed74934ec852107`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 04 Oct 2022 23:45:10 GMT
ADD file:5395cc8536f80a7cce6fbae552f35b892b152e1db2fce6274fc514d8fc77d7c9 in / 
# Tue, 04 Oct 2022 23:45:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:49:20 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 05 Oct 2022 00:49:21 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 05 Oct 2022 00:49:29 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:49:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 05 Oct 2022 00:49:34 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 05 Oct 2022 00:49:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:50:12 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 05 Oct 2022 00:50:13 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 05 Oct 2022 00:50:30 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Oct 2022 00:50:32 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 05 Oct 2022 00:50:33 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 05 Oct 2022 00:50:34 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 05 Oct 2022 00:50:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 00:50:35 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 00:50:36 GMT
VOLUME [/opt/couchdb/data]
# Wed, 05 Oct 2022 00:50:37 GMT
EXPOSE 4369 5984 9100
# Wed, 05 Oct 2022 00:50:38 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:2c1ba50780a9bc2b2a8f3d639ceca4285c97f51fd1c51c783fe34e150ff35e60`  
		Last Modified: Tue, 04 Oct 2022 23:51:14 GMT  
		Size: 25.9 MB (25911903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9d52fabe092940bc792dd8f1bb4e6f129488b391d08ebeefd1d7627f6e1b40`  
		Last Modified: Wed, 05 Oct 2022 00:51:34 GMT  
		Size: 3.3 KB (3323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eae867bf6785dc23f4882f13570fde4a0fc1da95016048a19775019c9ad55e4`  
		Last Modified: Wed, 05 Oct 2022 00:51:33 GMT  
		Size: 6.6 MB (6557121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b2fdd67a8553ce64d8858fe406d0f214004cfb0222e37a7aa224f69c75e84d4`  
		Last Modified: Wed, 05 Oct 2022 00:51:32 GMT  
		Size: 951.2 KB (951173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2886035e065831ccb1a14acc93cdefbbb3c9b0093f3d65bb42f3aea88ace6fe`  
		Last Modified: Wed, 05 Oct 2022 00:51:32 GMT  
		Size: 79.9 KB (79932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01fdbbddab8b088fc36beac4ab9ce6dcb2a7fa1a02e928a68ab47cac43db4675`  
		Last Modified: Wed, 05 Oct 2022 00:51:48 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce419a04f9915966cd0cc9b92a2305ea04ff48f6beb5631c8e995de5010fe04`  
		Last Modified: Wed, 05 Oct 2022 00:51:51 GMT  
		Size: 39.0 MB (39026632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47fec2de36e7db36c1d653abb7b2ca6aa5be09113df1324f9983d3bb776fee87`  
		Last Modified: Wed, 05 Oct 2022 00:51:46 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135b343d09d36b63515856502bfa78d3394de0ae50cd664422d0f8ac886cd888`  
		Last Modified: Wed, 05 Oct 2022 00:51:46 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058b2a8902bc82279819fef135fdfe5f1558c76392dd78c98c383b4675e4e92a`  
		Last Modified: Wed, 05 Oct 2022 00:51:46 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6aec47116b5ea1a6b81c00b1fbb37932e2535a55569e3775d8891b31418ef85`  
		Last Modified: Wed, 05 Oct 2022 00:51:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3`

```console
$ docker pull couchdb@sha256:e8885a73041d303b37bfd493d7deb8e057e834429df127dd5ee0e950fac5b534
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:fdd360c2699c5ccce0e926e64e111ac1ddbeea91ae06bd8c8342deab8bbece81
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84521637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ea24299b2688202b1f16bf104a8edd9d9d3620e72226b286c744b41527dd3c1`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:48 GMT
ADD file:782d864aa72c2d5fb599311ebae56db4067d2e91ff532c1aaf1a291c3dbce5bb in / 
# Tue, 13 Sep 2022 00:56:49 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:54:33 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Sep 2022 03:54:34 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Sep 2022 03:54:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:54:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 13 Sep 2022 03:54:45 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Sep 2022 03:54:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:55:14 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 13 Sep 2022 03:55:14 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Sep 2022 03:55:32 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Sep 2022 03:55:32 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Sep 2022 03:55:32 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 13 Sep 2022 03:55:32 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 13 Sep 2022 03:55:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 03:55:33 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Sep 2022 03:55:33 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Sep 2022 03:55:33 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Sep 2022 03:55:33 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:4b7b4a8876e2f677668e51b8473f97a237d3d4df201b9df4031bcaa8068370b1`  
		Last Modified: Tue, 13 Sep 2022 01:01:16 GMT  
		Size: 27.1 MB (27130552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c088c3a03bf60b8f0b3b24363efbc28aef3c87451537b97521bfbf1f2aa13199`  
		Last Modified: Tue, 13 Sep 2022 03:56:21 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65e6c9d6ee4b135545b364dd8b30be2b91e27e6b1e62addf07801a90a90ac96f`  
		Last Modified: Tue, 13 Sep 2022 03:56:20 GMT  
		Size: 6.7 MB (6698707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e1633127944965c144a64754b6a92bf6622c1de73c33716a59ca7f9ef1baca`  
		Last Modified: Tue, 13 Sep 2022 03:56:19 GMT  
		Size: 1.3 MB (1258362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61a40f9af1917164479b4fc40fc1f8fa2db40005957a46bb7b167f3a6f2724c`  
		Last Modified: Tue, 13 Sep 2022 03:56:18 GMT  
		Size: 293.1 KB (293062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d24fe37ce953bdb8931392614becce928b2547796764bddd9f88e56c6ed97d8`  
		Last Modified: Tue, 13 Sep 2022 03:56:34 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283af9663b67d645492bd442d5e7cbc4a46b247238ff7aed93a0483c77310649`  
		Last Modified: Tue, 13 Sep 2022 03:56:38 GMT  
		Size: 49.1 MB (49133940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4788d07645893982eb35d79013264bcb958817cb4c1c0e52f0254f8de7e34c33`  
		Last Modified: Tue, 13 Sep 2022 03:56:32 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e97b88ff5fd41abb9abad7b6ce9c27f883f8df6819b6074f7e6732f3e396ce`  
		Last Modified: Tue, 13 Sep 2022 03:56:32 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6073742d94dc8629793832fe392891511bc2c7fa5be1aa13b87b50d0d956c430`  
		Last Modified: Tue, 13 Sep 2022 03:56:32 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f3d38689c87981ca7f5c0ace468c72ed5ff7a897ed74b8d86386db94be8d949`  
		Last Modified: Tue, 13 Sep 2022 03:56:32 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:b5f6db08e39cf0632d9bed88436c31f501c02d7ecb7b0863ed2efb9076420334
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72533691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56458d08878446377adc3bfd36d6cd5a04d270972781aa4c5ed74934ec852107`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 04 Oct 2022 23:45:10 GMT
ADD file:5395cc8536f80a7cce6fbae552f35b892b152e1db2fce6274fc514d8fc77d7c9 in / 
# Tue, 04 Oct 2022 23:45:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:49:20 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 05 Oct 2022 00:49:21 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 05 Oct 2022 00:49:29 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:49:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 05 Oct 2022 00:49:34 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 05 Oct 2022 00:49:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:50:12 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 05 Oct 2022 00:50:13 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 05 Oct 2022 00:50:30 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Oct 2022 00:50:32 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 05 Oct 2022 00:50:33 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 05 Oct 2022 00:50:34 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 05 Oct 2022 00:50:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 00:50:35 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 00:50:36 GMT
VOLUME [/opt/couchdb/data]
# Wed, 05 Oct 2022 00:50:37 GMT
EXPOSE 4369 5984 9100
# Wed, 05 Oct 2022 00:50:38 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:2c1ba50780a9bc2b2a8f3d639ceca4285c97f51fd1c51c783fe34e150ff35e60`  
		Last Modified: Tue, 04 Oct 2022 23:51:14 GMT  
		Size: 25.9 MB (25911903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9d52fabe092940bc792dd8f1bb4e6f129488b391d08ebeefd1d7627f6e1b40`  
		Last Modified: Wed, 05 Oct 2022 00:51:34 GMT  
		Size: 3.3 KB (3323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eae867bf6785dc23f4882f13570fde4a0fc1da95016048a19775019c9ad55e4`  
		Last Modified: Wed, 05 Oct 2022 00:51:33 GMT  
		Size: 6.6 MB (6557121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b2fdd67a8553ce64d8858fe406d0f214004cfb0222e37a7aa224f69c75e84d4`  
		Last Modified: Wed, 05 Oct 2022 00:51:32 GMT  
		Size: 951.2 KB (951173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2886035e065831ccb1a14acc93cdefbbb3c9b0093f3d65bb42f3aea88ace6fe`  
		Last Modified: Wed, 05 Oct 2022 00:51:32 GMT  
		Size: 79.9 KB (79932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01fdbbddab8b088fc36beac4ab9ce6dcb2a7fa1a02e928a68ab47cac43db4675`  
		Last Modified: Wed, 05 Oct 2022 00:51:48 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce419a04f9915966cd0cc9b92a2305ea04ff48f6beb5631c8e995de5010fe04`  
		Last Modified: Wed, 05 Oct 2022 00:51:51 GMT  
		Size: 39.0 MB (39026632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47fec2de36e7db36c1d653abb7b2ca6aa5be09113df1324f9983d3bb776fee87`  
		Last Modified: Wed, 05 Oct 2022 00:51:46 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135b343d09d36b63515856502bfa78d3394de0ae50cd664422d0f8ac886cd888`  
		Last Modified: Wed, 05 Oct 2022 00:51:46 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058b2a8902bc82279819fef135fdfe5f1558c76392dd78c98c383b4675e4e92a`  
		Last Modified: Wed, 05 Oct 2022 00:51:46 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6aec47116b5ea1a6b81c00b1fbb37932e2535a55569e3775d8891b31418ef85`  
		Last Modified: Wed, 05 Oct 2022 00:51:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3.1`

```console
$ docker pull couchdb@sha256:e8885a73041d303b37bfd493d7deb8e057e834429df127dd5ee0e950fac5b534
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:fdd360c2699c5ccce0e926e64e111ac1ddbeea91ae06bd8c8342deab8bbece81
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84521637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ea24299b2688202b1f16bf104a8edd9d9d3620e72226b286c744b41527dd3c1`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:48 GMT
ADD file:782d864aa72c2d5fb599311ebae56db4067d2e91ff532c1aaf1a291c3dbce5bb in / 
# Tue, 13 Sep 2022 00:56:49 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:54:33 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Sep 2022 03:54:34 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Sep 2022 03:54:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:54:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 13 Sep 2022 03:54:45 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Sep 2022 03:54:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:55:14 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 13 Sep 2022 03:55:14 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Sep 2022 03:55:32 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Sep 2022 03:55:32 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Sep 2022 03:55:32 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 13 Sep 2022 03:55:32 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 13 Sep 2022 03:55:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 03:55:33 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Sep 2022 03:55:33 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Sep 2022 03:55:33 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Sep 2022 03:55:33 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:4b7b4a8876e2f677668e51b8473f97a237d3d4df201b9df4031bcaa8068370b1`  
		Last Modified: Tue, 13 Sep 2022 01:01:16 GMT  
		Size: 27.1 MB (27130552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c088c3a03bf60b8f0b3b24363efbc28aef3c87451537b97521bfbf1f2aa13199`  
		Last Modified: Tue, 13 Sep 2022 03:56:21 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65e6c9d6ee4b135545b364dd8b30be2b91e27e6b1e62addf07801a90a90ac96f`  
		Last Modified: Tue, 13 Sep 2022 03:56:20 GMT  
		Size: 6.7 MB (6698707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e1633127944965c144a64754b6a92bf6622c1de73c33716a59ca7f9ef1baca`  
		Last Modified: Tue, 13 Sep 2022 03:56:19 GMT  
		Size: 1.3 MB (1258362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61a40f9af1917164479b4fc40fc1f8fa2db40005957a46bb7b167f3a6f2724c`  
		Last Modified: Tue, 13 Sep 2022 03:56:18 GMT  
		Size: 293.1 KB (293062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d24fe37ce953bdb8931392614becce928b2547796764bddd9f88e56c6ed97d8`  
		Last Modified: Tue, 13 Sep 2022 03:56:34 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283af9663b67d645492bd442d5e7cbc4a46b247238ff7aed93a0483c77310649`  
		Last Modified: Tue, 13 Sep 2022 03:56:38 GMT  
		Size: 49.1 MB (49133940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4788d07645893982eb35d79013264bcb958817cb4c1c0e52f0254f8de7e34c33`  
		Last Modified: Tue, 13 Sep 2022 03:56:32 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e97b88ff5fd41abb9abad7b6ce9c27f883f8df6819b6074f7e6732f3e396ce`  
		Last Modified: Tue, 13 Sep 2022 03:56:32 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6073742d94dc8629793832fe392891511bc2c7fa5be1aa13b87b50d0d956c430`  
		Last Modified: Tue, 13 Sep 2022 03:56:32 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f3d38689c87981ca7f5c0ace468c72ed5ff7a897ed74b8d86386db94be8d949`  
		Last Modified: Tue, 13 Sep 2022 03:56:32 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:b5f6db08e39cf0632d9bed88436c31f501c02d7ecb7b0863ed2efb9076420334
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72533691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56458d08878446377adc3bfd36d6cd5a04d270972781aa4c5ed74934ec852107`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 04 Oct 2022 23:45:10 GMT
ADD file:5395cc8536f80a7cce6fbae552f35b892b152e1db2fce6274fc514d8fc77d7c9 in / 
# Tue, 04 Oct 2022 23:45:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:49:20 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 05 Oct 2022 00:49:21 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 05 Oct 2022 00:49:29 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:49:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 05 Oct 2022 00:49:34 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 05 Oct 2022 00:49:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:50:12 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 05 Oct 2022 00:50:13 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 05 Oct 2022 00:50:30 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Oct 2022 00:50:32 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 05 Oct 2022 00:50:33 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 05 Oct 2022 00:50:34 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 05 Oct 2022 00:50:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 00:50:35 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 00:50:36 GMT
VOLUME [/opt/couchdb/data]
# Wed, 05 Oct 2022 00:50:37 GMT
EXPOSE 4369 5984 9100
# Wed, 05 Oct 2022 00:50:38 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:2c1ba50780a9bc2b2a8f3d639ceca4285c97f51fd1c51c783fe34e150ff35e60`  
		Last Modified: Tue, 04 Oct 2022 23:51:14 GMT  
		Size: 25.9 MB (25911903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9d52fabe092940bc792dd8f1bb4e6f129488b391d08ebeefd1d7627f6e1b40`  
		Last Modified: Wed, 05 Oct 2022 00:51:34 GMT  
		Size: 3.3 KB (3323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eae867bf6785dc23f4882f13570fde4a0fc1da95016048a19775019c9ad55e4`  
		Last Modified: Wed, 05 Oct 2022 00:51:33 GMT  
		Size: 6.6 MB (6557121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b2fdd67a8553ce64d8858fe406d0f214004cfb0222e37a7aa224f69c75e84d4`  
		Last Modified: Wed, 05 Oct 2022 00:51:32 GMT  
		Size: 951.2 KB (951173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2886035e065831ccb1a14acc93cdefbbb3c9b0093f3d65bb42f3aea88ace6fe`  
		Last Modified: Wed, 05 Oct 2022 00:51:32 GMT  
		Size: 79.9 KB (79932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01fdbbddab8b088fc36beac4ab9ce6dcb2a7fa1a02e928a68ab47cac43db4675`  
		Last Modified: Wed, 05 Oct 2022 00:51:48 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce419a04f9915966cd0cc9b92a2305ea04ff48f6beb5631c8e995de5010fe04`  
		Last Modified: Wed, 05 Oct 2022 00:51:51 GMT  
		Size: 39.0 MB (39026632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47fec2de36e7db36c1d653abb7b2ca6aa5be09113df1324f9983d3bb776fee87`  
		Last Modified: Wed, 05 Oct 2022 00:51:46 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135b343d09d36b63515856502bfa78d3394de0ae50cd664422d0f8ac886cd888`  
		Last Modified: Wed, 05 Oct 2022 00:51:46 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058b2a8902bc82279819fef135fdfe5f1558c76392dd78c98c383b4675e4e92a`  
		Last Modified: Wed, 05 Oct 2022 00:51:46 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6aec47116b5ea1a6b81c00b1fbb37932e2535a55569e3775d8891b31418ef85`  
		Last Modified: Wed, 05 Oct 2022 00:51:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3`

```console
$ docker pull couchdb@sha256:934ae4b7e2b88d4cb6b2cca03cb5c39d955cef2ffeb258d9b6511302e55716be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3` - linux; amd64

```console
$ docker pull couchdb@sha256:ac5c57c4df9f9d0129390f652b62dfa348a1b383c458841010ad52abbb6c8f0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87530196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9292db79eb5d3107963496f664c9764d4974a423cff1612702d8ca782a888f5`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:29 GMT
ADD file:5bd53bff884e470b3c12425132975ab9c6f99002c62c43bca1ff5cde9d863b92 in / 
# Tue, 13 Sep 2022 00:56:29 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:53:59 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Sep 2022 03:54:00 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Sep 2022 03:54:07 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:54:10 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 13 Sep 2022 03:54:10 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Sep 2022 03:54:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:54:16 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 13 Sep 2022 03:54:16 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Sep 2022 03:54:29 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Sep 2022 03:54:30 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Sep 2022 03:54:30 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 13 Sep 2022 03:54:30 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 13 Sep 2022 03:54:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 03:54:30 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Sep 2022 03:54:31 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Sep 2022 03:54:31 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Sep 2022 03:54:31 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:31b3f1ad4ce1f369084d0f959813c51df0ca17d9877d5ee88c2db6ff88341430`  
		Last Modified: Tue, 13 Sep 2022 01:00:29 GMT  
		Size: 31.4 MB (31404121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9775a4fbb4b5564bbc1ec8e077d317b8745a7598e059365241ddc1a9766c129c`  
		Last Modified: Tue, 13 Sep 2022 03:55:55 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d707a0a4de816f6a35046bed27c3bd025081394b651fd4b339188a4e19967c4`  
		Last Modified: Tue, 13 Sep 2022 03:55:54 GMT  
		Size: 5.2 MB (5224215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c15634eb84187cbacfe864298c664c5eb740aa1a455a39e64f4f6a94c0f07a14`  
		Last Modified: Tue, 13 Sep 2022 03:55:53 GMT  
		Size: 1.6 MB (1553277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59f0fe4ba863352dbd7372301d2eae5be8cd69838e66876a65c5c0b1666de8c`  
		Last Modified: Tue, 13 Sep 2022 03:55:53 GMT  
		Size: 295.6 KB (295573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f507b233637bff8bdab3e80909e9dcdcc02a11efcca3f242c4ae8bf410296bbe`  
		Last Modified: Tue, 13 Sep 2022 03:55:53 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a76624d812c6c764f46d961f80510fa92e7512419c528ba6ab86e250d365d8`  
		Last Modified: Tue, 13 Sep 2022 03:55:56 GMT  
		Size: 49.0 MB (49045868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6166f23a925f2a6a18aa9efa186271f01020d8fd5d40d7a307cb02d6172974`  
		Last Modified: Tue, 13 Sep 2022 03:55:50 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc867e39bf60d67febf095d33500f8b30b51f6edbef26bd9d37b7a38a9bfaebc`  
		Last Modified: Tue, 13 Sep 2022 03:55:50 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5bc74ba5f149b1005fb23f07d5b84e4946fc31381d124892f99322b8c9a202`  
		Last Modified: Tue, 13 Sep 2022 03:55:50 GMT  
		Size: 2.2 KB (2187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ff75922f5a116b20c00eabe11b5280455fc7c77595f4ae03ed74a4e45ffb41`  
		Last Modified: Tue, 13 Sep 2022 03:55:50 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:15b86d4a7e914f5cb43435066ca4bab8cbcdaebe90b368ddd84e62b1276707cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.4 MB (85431442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c8d97bc3ed2957b5104f353e1f2c8a556ce0578fef9ea833e20f12084ffd785`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:48:29 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 05 Oct 2022 00:48:30 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 05 Oct 2022 00:48:37 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:48:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 05 Oct 2022 00:48:42 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 05 Oct 2022 00:48:48 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:48:48 GMT
ENV COUCHDB_VERSION=3.2.2
# Wed, 05 Oct 2022 00:48:49 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 05 Oct 2022 00:49:07 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Oct 2022 00:49:08 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 05 Oct 2022 00:49:09 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 05 Oct 2022 00:49:10 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 05 Oct 2022 00:49:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 00:49:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 00:49:12 GMT
VOLUME [/opt/couchdb/data]
# Wed, 05 Oct 2022 00:49:13 GMT
EXPOSE 4369 5984 9100
# Wed, 05 Oct 2022 00:49:14 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f51811668444e3b968d7a39cc5de30342e106eb12a367f9df356df8bbcf389`  
		Last Modified: Wed, 05 Oct 2022 00:51:09 GMT  
		Size: 3.3 KB (3323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3647d34c5a0150082687be7055d489b6b82a1373a51288e0ac2f96eb14d14bba`  
		Last Modified: Wed, 05 Oct 2022 00:51:08 GMT  
		Size: 5.0 MB (5003078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede8dd5eef52dc53a17137c8f44a05bdbb7d3051469c807a72604863295b68ef`  
		Last Modified: Wed, 05 Oct 2022 00:51:07 GMT  
		Size: 1.2 MB (1221098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7805f556f9096b24a1f655412b3e107a441d7f80ca8784574468f3b5af237e3c`  
		Last Modified: Wed, 05 Oct 2022 00:51:07 GMT  
		Size: 79.2 KB (79188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f2666158c95d59c0c61ac764acbb74e7454790953711cef91637f157db1029`  
		Last Modified: Wed, 05 Oct 2022 00:51:07 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34690541f949f6b1d8f46ae836e345d751c04b0aba8e1b09d9cbfd1b9d76e99a`  
		Last Modified: Wed, 05 Oct 2022 00:51:11 GMT  
		Size: 49.1 MB (49056628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4dc122dca5acda98426bf931c79625fad8ae9c9ce8ff53b480fd2b23f38203`  
		Last Modified: Wed, 05 Oct 2022 00:51:05 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:709b165a3a0c88c48e1537f0235f679a4473e281e80fc901b01c9a606b09fa21`  
		Last Modified: Wed, 05 Oct 2022 00:51:05 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b953f92a10f1393fe7e947f8523a7c20861b1e924f68da4b7ef27f6fd772ca`  
		Last Modified: Wed, 05 Oct 2022 00:51:05 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:923cca80d418f57784d23718f6af544e71daf08c5f06dafd817982538a7b0c82`  
		Last Modified: Wed, 05 Oct 2022 00:51:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; ppc64le

```console
$ docker pull couchdb@sha256:143e3cd2945cb48d796d2278db9557504a800c77299549c9ac183576f1b6c918
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93229895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7711c8b3c5ab31870f4215b49471ddd8fa0a590d524a9b20be6af5f450232aa`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 04 Oct 2022 23:18:04 GMT
ADD file:66a0f55a4b4dfbb5d64082ffdb24751f20c5773039277ba278fdb4ce4a538c33 in / 
# Tue, 04 Oct 2022 23:18:06 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:08:24 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 05 Oct 2022 00:08:26 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 05 Oct 2022 00:08:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:08:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 05 Oct 2022 00:08:50 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 05 Oct 2022 00:09:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:09:02 GMT
ENV COUCHDB_VERSION=3.2.2
# Wed, 05 Oct 2022 00:09:03 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 05 Oct 2022 00:09:26 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Oct 2022 00:09:28 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 05 Oct 2022 00:09:28 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 05 Oct 2022 00:09:29 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 05 Oct 2022 00:09:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 00:09:30 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 00:09:31 GMT
VOLUME [/opt/couchdb/data]
# Wed, 05 Oct 2022 00:09:31 GMT
EXPOSE 4369 5984 9100
# Wed, 05 Oct 2022 00:09:31 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:4e001127162dd884a6f7bd2e6f74215816d325bebb3a374ae9fcee9f038f99b8`  
		Last Modified: Tue, 04 Oct 2022 23:24:13 GMT  
		Size: 35.3 MB (35290584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381109cbfbaaa798f564a18947f6c0f1dd5910da0234beab17bd5819ea39399d`  
		Last Modified: Wed, 05 Oct 2022 00:09:54 GMT  
		Size: 3.4 KB (3410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395cceb53989fdd5e1a8a72b46ca77b7d6663f50db82d16939a22fc6bc490b0d`  
		Last Modified: Wed, 05 Oct 2022 00:09:54 GMT  
		Size: 6.0 MB (6043722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c601f28412075f4767666bf160d562b535fd07b9fb959ef7ff65f470e5554bb`  
		Last Modified: Wed, 05 Oct 2022 00:09:52 GMT  
		Size: 1.5 MB (1509160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908145ec6ae093dd2fcc342bd38df282b5851f529d6b3a835ac93d69aaa33424`  
		Last Modified: Wed, 05 Oct 2022 00:09:52 GMT  
		Size: 295.5 KB (295506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f5839c8ec51b87036b5260c4c50c7b68102134e73a620710ba0c6c551e02cc`  
		Last Modified: Wed, 05 Oct 2022 00:09:52 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf4fabbea2bc9c827bf92aa5c2f2d24249508e1f71a1228e328d2611e0d899c`  
		Last Modified: Wed, 05 Oct 2022 00:09:59 GMT  
		Size: 50.1 MB (50083786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:435f63e26726324a42486d58656d232b9a7a902119575252fbd7326ff3e78f12`  
		Last Modified: Wed, 05 Oct 2022 00:09:50 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d3b1210769a993aa36f893916060dffb032025964550b36c01181138dc64f74`  
		Last Modified: Wed, 05 Oct 2022 00:09:49 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ab88b6abdfeff6d61bc12392dd5649756851f5b7dda2e77bea1bbea2f90038`  
		Last Modified: Wed, 05 Oct 2022 00:09:50 GMT  
		Size: 2.2 KB (2187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2fcd7203df115c27ce9f60eea1502476c8d59cc71edf4c6f0994b0a78b200c`  
		Last Modified: Wed, 05 Oct 2022 00:09:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1`

```console
$ docker pull couchdb@sha256:02685ca17100dff3c3e0f9a81ef160ca3e52065cba742dd21d47d3b9e1051072
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:56f710e313037efd3c25fa4b49915b84d702a31381fc38a43762e6bac60c74a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80004867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f48f1d73bb2abbf3e60211207f5d416c139ea8d36c4bf9360874811baabfbca6`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:48 GMT
ADD file:782d864aa72c2d5fb599311ebae56db4067d2e91ff532c1aaf1a291c3dbce5bb in / 
# Tue, 13 Sep 2022 00:56:49 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:54:33 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Sep 2022 03:54:34 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Sep 2022 03:54:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:54:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 13 Sep 2022 03:54:45 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Sep 2022 03:54:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:54:51 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 13 Sep 2022 03:54:52 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Sep 2022 03:55:05 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Sep 2022 03:55:06 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Sep 2022 03:55:06 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 13 Sep 2022 03:55:06 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 13 Sep 2022 03:55:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 03:55:07 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Sep 2022 03:55:07 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Sep 2022 03:55:07 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Sep 2022 03:55:07 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:4b7b4a8876e2f677668e51b8473f97a237d3d4df201b9df4031bcaa8068370b1`  
		Last Modified: Tue, 13 Sep 2022 01:01:16 GMT  
		Size: 27.1 MB (27130552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c088c3a03bf60b8f0b3b24363efbc28aef3c87451537b97521bfbf1f2aa13199`  
		Last Modified: Tue, 13 Sep 2022 03:56:21 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65e6c9d6ee4b135545b364dd8b30be2b91e27e6b1e62addf07801a90a90ac96f`  
		Last Modified: Tue, 13 Sep 2022 03:56:20 GMT  
		Size: 6.7 MB (6698707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e1633127944965c144a64754b6a92bf6622c1de73c33716a59ca7f9ef1baca`  
		Last Modified: Tue, 13 Sep 2022 03:56:19 GMT  
		Size: 1.3 MB (1258362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61a40f9af1917164479b4fc40fc1f8fa2db40005957a46bb7b167f3a6f2724c`  
		Last Modified: Tue, 13 Sep 2022 03:56:18 GMT  
		Size: 293.1 KB (293062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7eae00d81a619c1b8d71dc8e8b6a2318e06ce5afeafd58b6b0d9552f09261d2`  
		Last Modified: Tue, 13 Sep 2022 03:56:18 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75278761418a6e65c5ef254f72d0a496d0637be7e24631aa0fc31e7e365c080d`  
		Last Modified: Tue, 13 Sep 2022 03:56:21 GMT  
		Size: 44.6 MB (44617172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5b505f864f3542ade296e07b2aeddd0672c1c1e23b3274b9a3a4f9db90256a`  
		Last Modified: Tue, 13 Sep 2022 03:56:17 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5311452d93f303af98096fadb36f8010feea220fb6988b8ccb03e4de55fde725`  
		Last Modified: Tue, 13 Sep 2022 03:56:16 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cc94873d6f1ffc6ef99804d2418b5444f939646feac9f991cf58c41442b91e`  
		Last Modified: Tue, 13 Sep 2022 03:56:16 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81cfa86b5c94ad137436fdbbbe1db947123cedb91147470f17111fc67173907`  
		Last Modified: Tue, 13 Sep 2022 03:56:16 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:9511b39dd90ece04c657df86f985fc32e1c2515ec760fd073bf897df93e061e3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74623799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b144bac68cc54d86cef7bec6c633434d00bd48e6678fa31f17cae380bcbc2a61`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 04 Oct 2022 23:45:10 GMT
ADD file:5395cc8536f80a7cce6fbae552f35b892b152e1db2fce6274fc514d8fc77d7c9 in / 
# Tue, 04 Oct 2022 23:45:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:49:20 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 05 Oct 2022 00:49:21 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 05 Oct 2022 00:49:29 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:49:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 05 Oct 2022 00:49:34 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 05 Oct 2022 00:49:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:49:41 GMT
ENV COUCHDB_VERSION=3.1.2
# Wed, 05 Oct 2022 00:49:42 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 05 Oct 2022 00:49:59 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Oct 2022 00:50:00 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 05 Oct 2022 00:50:01 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 05 Oct 2022 00:50:02 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 05 Oct 2022 00:50:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 00:50:03 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 00:50:04 GMT
VOLUME [/opt/couchdb/data]
# Wed, 05 Oct 2022 00:50:05 GMT
EXPOSE 4369 5984 9100
# Wed, 05 Oct 2022 00:50:06 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:2c1ba50780a9bc2b2a8f3d639ceca4285c97f51fd1c51c783fe34e150ff35e60`  
		Last Modified: Tue, 04 Oct 2022 23:51:14 GMT  
		Size: 25.9 MB (25911903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9d52fabe092940bc792dd8f1bb4e6f129488b391d08ebeefd1d7627f6e1b40`  
		Last Modified: Wed, 05 Oct 2022 00:51:34 GMT  
		Size: 3.3 KB (3323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eae867bf6785dc23f4882f13570fde4a0fc1da95016048a19775019c9ad55e4`  
		Last Modified: Wed, 05 Oct 2022 00:51:33 GMT  
		Size: 6.6 MB (6557121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b2fdd67a8553ce64d8858fe406d0f214004cfb0222e37a7aa224f69c75e84d4`  
		Last Modified: Wed, 05 Oct 2022 00:51:32 GMT  
		Size: 951.2 KB (951173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2886035e065831ccb1a14acc93cdefbbb3c9b0093f3d65bb42f3aea88ace6fe`  
		Last Modified: Wed, 05 Oct 2022 00:51:32 GMT  
		Size: 79.9 KB (79932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:868db392d530fda8de08df63262729f5aba0a2616b58f8b2b1c4c489fce87605`  
		Last Modified: Wed, 05 Oct 2022 00:51:32 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c8a687b92d4ca6aa00bc648f5ee2baa91b526c07eeb85a0776143bcf066870`  
		Last Modified: Wed, 05 Oct 2022 00:51:35 GMT  
		Size: 41.1 MB (41116753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32dec1f2479dbac1b6ae9d61eec6a4e26b8cfcd1f83b71666bcb273c0e6aa128`  
		Last Modified: Wed, 05 Oct 2022 00:51:29 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f26f385cd05d1ccb7b9599d9bedaf6fb60f0a77ea192913ab5498a742054b1`  
		Last Modified: Wed, 05 Oct 2022 00:51:29 GMT  
		Size: 761.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d2727503716141f749ba450d1152366c9320353f47a70e49df42540423a3eb6`  
		Last Modified: Wed, 05 Oct 2022 00:51:29 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031434fe63244ec3e4cf2f40b150f851388a693fbd1f97a88f71e2337e0d270f`  
		Last Modified: Wed, 05 Oct 2022 00:51:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1.2`

```console
$ docker pull couchdb@sha256:02685ca17100dff3c3e0f9a81ef160ca3e52065cba742dd21d47d3b9e1051072
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1.2` - linux; amd64

```console
$ docker pull couchdb@sha256:56f710e313037efd3c25fa4b49915b84d702a31381fc38a43762e6bac60c74a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80004867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f48f1d73bb2abbf3e60211207f5d416c139ea8d36c4bf9360874811baabfbca6`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:48 GMT
ADD file:782d864aa72c2d5fb599311ebae56db4067d2e91ff532c1aaf1a291c3dbce5bb in / 
# Tue, 13 Sep 2022 00:56:49 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:54:33 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Sep 2022 03:54:34 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Sep 2022 03:54:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:54:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 13 Sep 2022 03:54:45 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Sep 2022 03:54:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:54:51 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 13 Sep 2022 03:54:52 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Sep 2022 03:55:05 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Sep 2022 03:55:06 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Sep 2022 03:55:06 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 13 Sep 2022 03:55:06 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 13 Sep 2022 03:55:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 03:55:07 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Sep 2022 03:55:07 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Sep 2022 03:55:07 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Sep 2022 03:55:07 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:4b7b4a8876e2f677668e51b8473f97a237d3d4df201b9df4031bcaa8068370b1`  
		Last Modified: Tue, 13 Sep 2022 01:01:16 GMT  
		Size: 27.1 MB (27130552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c088c3a03bf60b8f0b3b24363efbc28aef3c87451537b97521bfbf1f2aa13199`  
		Last Modified: Tue, 13 Sep 2022 03:56:21 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65e6c9d6ee4b135545b364dd8b30be2b91e27e6b1e62addf07801a90a90ac96f`  
		Last Modified: Tue, 13 Sep 2022 03:56:20 GMT  
		Size: 6.7 MB (6698707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e1633127944965c144a64754b6a92bf6622c1de73c33716a59ca7f9ef1baca`  
		Last Modified: Tue, 13 Sep 2022 03:56:19 GMT  
		Size: 1.3 MB (1258362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61a40f9af1917164479b4fc40fc1f8fa2db40005957a46bb7b167f3a6f2724c`  
		Last Modified: Tue, 13 Sep 2022 03:56:18 GMT  
		Size: 293.1 KB (293062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7eae00d81a619c1b8d71dc8e8b6a2318e06ce5afeafd58b6b0d9552f09261d2`  
		Last Modified: Tue, 13 Sep 2022 03:56:18 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75278761418a6e65c5ef254f72d0a496d0637be7e24631aa0fc31e7e365c080d`  
		Last Modified: Tue, 13 Sep 2022 03:56:21 GMT  
		Size: 44.6 MB (44617172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5b505f864f3542ade296e07b2aeddd0672c1c1e23b3274b9a3a4f9db90256a`  
		Last Modified: Tue, 13 Sep 2022 03:56:17 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5311452d93f303af98096fadb36f8010feea220fb6988b8ccb03e4de55fde725`  
		Last Modified: Tue, 13 Sep 2022 03:56:16 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cc94873d6f1ffc6ef99804d2418b5444f939646feac9f991cf58c41442b91e`  
		Last Modified: Tue, 13 Sep 2022 03:56:16 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81cfa86b5c94ad137436fdbbbe1db947123cedb91147470f17111fc67173907`  
		Last Modified: Tue, 13 Sep 2022 03:56:16 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:9511b39dd90ece04c657df86f985fc32e1c2515ec760fd073bf897df93e061e3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74623799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b144bac68cc54d86cef7bec6c633434d00bd48e6678fa31f17cae380bcbc2a61`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 04 Oct 2022 23:45:10 GMT
ADD file:5395cc8536f80a7cce6fbae552f35b892b152e1db2fce6274fc514d8fc77d7c9 in / 
# Tue, 04 Oct 2022 23:45:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:49:20 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 05 Oct 2022 00:49:21 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 05 Oct 2022 00:49:29 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:49:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 05 Oct 2022 00:49:34 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 05 Oct 2022 00:49:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:49:41 GMT
ENV COUCHDB_VERSION=3.1.2
# Wed, 05 Oct 2022 00:49:42 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 05 Oct 2022 00:49:59 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Oct 2022 00:50:00 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 05 Oct 2022 00:50:01 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 05 Oct 2022 00:50:02 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 05 Oct 2022 00:50:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 00:50:03 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 00:50:04 GMT
VOLUME [/opt/couchdb/data]
# Wed, 05 Oct 2022 00:50:05 GMT
EXPOSE 4369 5984 9100
# Wed, 05 Oct 2022 00:50:06 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:2c1ba50780a9bc2b2a8f3d639ceca4285c97f51fd1c51c783fe34e150ff35e60`  
		Last Modified: Tue, 04 Oct 2022 23:51:14 GMT  
		Size: 25.9 MB (25911903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9d52fabe092940bc792dd8f1bb4e6f129488b391d08ebeefd1d7627f6e1b40`  
		Last Modified: Wed, 05 Oct 2022 00:51:34 GMT  
		Size: 3.3 KB (3323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eae867bf6785dc23f4882f13570fde4a0fc1da95016048a19775019c9ad55e4`  
		Last Modified: Wed, 05 Oct 2022 00:51:33 GMT  
		Size: 6.6 MB (6557121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b2fdd67a8553ce64d8858fe406d0f214004cfb0222e37a7aa224f69c75e84d4`  
		Last Modified: Wed, 05 Oct 2022 00:51:32 GMT  
		Size: 951.2 KB (951173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2886035e065831ccb1a14acc93cdefbbb3c9b0093f3d65bb42f3aea88ace6fe`  
		Last Modified: Wed, 05 Oct 2022 00:51:32 GMT  
		Size: 79.9 KB (79932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:868db392d530fda8de08df63262729f5aba0a2616b58f8b2b1c4c489fce87605`  
		Last Modified: Wed, 05 Oct 2022 00:51:32 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c8a687b92d4ca6aa00bc648f5ee2baa91b526c07eeb85a0776143bcf066870`  
		Last Modified: Wed, 05 Oct 2022 00:51:35 GMT  
		Size: 41.1 MB (41116753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32dec1f2479dbac1b6ae9d61eec6a4e26b8cfcd1f83b71666bcb273c0e6aa128`  
		Last Modified: Wed, 05 Oct 2022 00:51:29 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f26f385cd05d1ccb7b9599d9bedaf6fb60f0a77ea192913ab5498a742054b1`  
		Last Modified: Wed, 05 Oct 2022 00:51:29 GMT  
		Size: 761.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d2727503716141f749ba450d1152366c9320353f47a70e49df42540423a3eb6`  
		Last Modified: Wed, 05 Oct 2022 00:51:29 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031434fe63244ec3e4cf2f40b150f851388a693fbd1f97a88f71e2337e0d270f`  
		Last Modified: Wed, 05 Oct 2022 00:51:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2`

```console
$ docker pull couchdb@sha256:934ae4b7e2b88d4cb6b2cca03cb5c39d955cef2ffeb258d9b6511302e55716be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2` - linux; amd64

```console
$ docker pull couchdb@sha256:ac5c57c4df9f9d0129390f652b62dfa348a1b383c458841010ad52abbb6c8f0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87530196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9292db79eb5d3107963496f664c9764d4974a423cff1612702d8ca782a888f5`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:29 GMT
ADD file:5bd53bff884e470b3c12425132975ab9c6f99002c62c43bca1ff5cde9d863b92 in / 
# Tue, 13 Sep 2022 00:56:29 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:53:59 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Sep 2022 03:54:00 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Sep 2022 03:54:07 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:54:10 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 13 Sep 2022 03:54:10 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Sep 2022 03:54:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:54:16 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 13 Sep 2022 03:54:16 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Sep 2022 03:54:29 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Sep 2022 03:54:30 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Sep 2022 03:54:30 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 13 Sep 2022 03:54:30 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 13 Sep 2022 03:54:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 03:54:30 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Sep 2022 03:54:31 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Sep 2022 03:54:31 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Sep 2022 03:54:31 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:31b3f1ad4ce1f369084d0f959813c51df0ca17d9877d5ee88c2db6ff88341430`  
		Last Modified: Tue, 13 Sep 2022 01:00:29 GMT  
		Size: 31.4 MB (31404121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9775a4fbb4b5564bbc1ec8e077d317b8745a7598e059365241ddc1a9766c129c`  
		Last Modified: Tue, 13 Sep 2022 03:55:55 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d707a0a4de816f6a35046bed27c3bd025081394b651fd4b339188a4e19967c4`  
		Last Modified: Tue, 13 Sep 2022 03:55:54 GMT  
		Size: 5.2 MB (5224215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c15634eb84187cbacfe864298c664c5eb740aa1a455a39e64f4f6a94c0f07a14`  
		Last Modified: Tue, 13 Sep 2022 03:55:53 GMT  
		Size: 1.6 MB (1553277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59f0fe4ba863352dbd7372301d2eae5be8cd69838e66876a65c5c0b1666de8c`  
		Last Modified: Tue, 13 Sep 2022 03:55:53 GMT  
		Size: 295.6 KB (295573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f507b233637bff8bdab3e80909e9dcdcc02a11efcca3f242c4ae8bf410296bbe`  
		Last Modified: Tue, 13 Sep 2022 03:55:53 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a76624d812c6c764f46d961f80510fa92e7512419c528ba6ab86e250d365d8`  
		Last Modified: Tue, 13 Sep 2022 03:55:56 GMT  
		Size: 49.0 MB (49045868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6166f23a925f2a6a18aa9efa186271f01020d8fd5d40d7a307cb02d6172974`  
		Last Modified: Tue, 13 Sep 2022 03:55:50 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc867e39bf60d67febf095d33500f8b30b51f6edbef26bd9d37b7a38a9bfaebc`  
		Last Modified: Tue, 13 Sep 2022 03:55:50 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5bc74ba5f149b1005fb23f07d5b84e4946fc31381d124892f99322b8c9a202`  
		Last Modified: Tue, 13 Sep 2022 03:55:50 GMT  
		Size: 2.2 KB (2187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ff75922f5a116b20c00eabe11b5280455fc7c77595f4ae03ed74a4e45ffb41`  
		Last Modified: Tue, 13 Sep 2022 03:55:50 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:15b86d4a7e914f5cb43435066ca4bab8cbcdaebe90b368ddd84e62b1276707cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.4 MB (85431442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c8d97bc3ed2957b5104f353e1f2c8a556ce0578fef9ea833e20f12084ffd785`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:48:29 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 05 Oct 2022 00:48:30 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 05 Oct 2022 00:48:37 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:48:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 05 Oct 2022 00:48:42 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 05 Oct 2022 00:48:48 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:48:48 GMT
ENV COUCHDB_VERSION=3.2.2
# Wed, 05 Oct 2022 00:48:49 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 05 Oct 2022 00:49:07 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Oct 2022 00:49:08 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 05 Oct 2022 00:49:09 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 05 Oct 2022 00:49:10 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 05 Oct 2022 00:49:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 00:49:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 00:49:12 GMT
VOLUME [/opt/couchdb/data]
# Wed, 05 Oct 2022 00:49:13 GMT
EXPOSE 4369 5984 9100
# Wed, 05 Oct 2022 00:49:14 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f51811668444e3b968d7a39cc5de30342e106eb12a367f9df356df8bbcf389`  
		Last Modified: Wed, 05 Oct 2022 00:51:09 GMT  
		Size: 3.3 KB (3323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3647d34c5a0150082687be7055d489b6b82a1373a51288e0ac2f96eb14d14bba`  
		Last Modified: Wed, 05 Oct 2022 00:51:08 GMT  
		Size: 5.0 MB (5003078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede8dd5eef52dc53a17137c8f44a05bdbb7d3051469c807a72604863295b68ef`  
		Last Modified: Wed, 05 Oct 2022 00:51:07 GMT  
		Size: 1.2 MB (1221098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7805f556f9096b24a1f655412b3e107a441d7f80ca8784574468f3b5af237e3c`  
		Last Modified: Wed, 05 Oct 2022 00:51:07 GMT  
		Size: 79.2 KB (79188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f2666158c95d59c0c61ac764acbb74e7454790953711cef91637f157db1029`  
		Last Modified: Wed, 05 Oct 2022 00:51:07 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34690541f949f6b1d8f46ae836e345d751c04b0aba8e1b09d9cbfd1b9d76e99a`  
		Last Modified: Wed, 05 Oct 2022 00:51:11 GMT  
		Size: 49.1 MB (49056628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4dc122dca5acda98426bf931c79625fad8ae9c9ce8ff53b480fd2b23f38203`  
		Last Modified: Wed, 05 Oct 2022 00:51:05 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:709b165a3a0c88c48e1537f0235f679a4473e281e80fc901b01c9a606b09fa21`  
		Last Modified: Wed, 05 Oct 2022 00:51:05 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b953f92a10f1393fe7e947f8523a7c20861b1e924f68da4b7ef27f6fd772ca`  
		Last Modified: Wed, 05 Oct 2022 00:51:05 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:923cca80d418f57784d23718f6af544e71daf08c5f06dafd817982538a7b0c82`  
		Last Modified: Wed, 05 Oct 2022 00:51:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; ppc64le

```console
$ docker pull couchdb@sha256:143e3cd2945cb48d796d2278db9557504a800c77299549c9ac183576f1b6c918
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93229895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7711c8b3c5ab31870f4215b49471ddd8fa0a590d524a9b20be6af5f450232aa`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 04 Oct 2022 23:18:04 GMT
ADD file:66a0f55a4b4dfbb5d64082ffdb24751f20c5773039277ba278fdb4ce4a538c33 in / 
# Tue, 04 Oct 2022 23:18:06 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:08:24 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 05 Oct 2022 00:08:26 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 05 Oct 2022 00:08:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:08:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 05 Oct 2022 00:08:50 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 05 Oct 2022 00:09:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:09:02 GMT
ENV COUCHDB_VERSION=3.2.2
# Wed, 05 Oct 2022 00:09:03 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 05 Oct 2022 00:09:26 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Oct 2022 00:09:28 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 05 Oct 2022 00:09:28 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 05 Oct 2022 00:09:29 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 05 Oct 2022 00:09:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 00:09:30 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 00:09:31 GMT
VOLUME [/opt/couchdb/data]
# Wed, 05 Oct 2022 00:09:31 GMT
EXPOSE 4369 5984 9100
# Wed, 05 Oct 2022 00:09:31 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:4e001127162dd884a6f7bd2e6f74215816d325bebb3a374ae9fcee9f038f99b8`  
		Last Modified: Tue, 04 Oct 2022 23:24:13 GMT  
		Size: 35.3 MB (35290584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381109cbfbaaa798f564a18947f6c0f1dd5910da0234beab17bd5819ea39399d`  
		Last Modified: Wed, 05 Oct 2022 00:09:54 GMT  
		Size: 3.4 KB (3410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395cceb53989fdd5e1a8a72b46ca77b7d6663f50db82d16939a22fc6bc490b0d`  
		Last Modified: Wed, 05 Oct 2022 00:09:54 GMT  
		Size: 6.0 MB (6043722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c601f28412075f4767666bf160d562b535fd07b9fb959ef7ff65f470e5554bb`  
		Last Modified: Wed, 05 Oct 2022 00:09:52 GMT  
		Size: 1.5 MB (1509160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908145ec6ae093dd2fcc342bd38df282b5851f529d6b3a835ac93d69aaa33424`  
		Last Modified: Wed, 05 Oct 2022 00:09:52 GMT  
		Size: 295.5 KB (295506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f5839c8ec51b87036b5260c4c50c7b68102134e73a620710ba0c6c551e02cc`  
		Last Modified: Wed, 05 Oct 2022 00:09:52 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf4fabbea2bc9c827bf92aa5c2f2d24249508e1f71a1228e328d2611e0d899c`  
		Last Modified: Wed, 05 Oct 2022 00:09:59 GMT  
		Size: 50.1 MB (50083786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:435f63e26726324a42486d58656d232b9a7a902119575252fbd7326ff3e78f12`  
		Last Modified: Wed, 05 Oct 2022 00:09:50 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d3b1210769a993aa36f893916060dffb032025964550b36c01181138dc64f74`  
		Last Modified: Wed, 05 Oct 2022 00:09:49 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ab88b6abdfeff6d61bc12392dd5649756851f5b7dda2e77bea1bbea2f90038`  
		Last Modified: Wed, 05 Oct 2022 00:09:50 GMT  
		Size: 2.2 KB (2187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2fcd7203df115c27ce9f60eea1502476c8d59cc71edf4c6f0994b0a78b200c`  
		Last Modified: Wed, 05 Oct 2022 00:09:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2.2`

```console
$ docker pull couchdb@sha256:934ae4b7e2b88d4cb6b2cca03cb5c39d955cef2ffeb258d9b6511302e55716be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2.2` - linux; amd64

```console
$ docker pull couchdb@sha256:ac5c57c4df9f9d0129390f652b62dfa348a1b383c458841010ad52abbb6c8f0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87530196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9292db79eb5d3107963496f664c9764d4974a423cff1612702d8ca782a888f5`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:29 GMT
ADD file:5bd53bff884e470b3c12425132975ab9c6f99002c62c43bca1ff5cde9d863b92 in / 
# Tue, 13 Sep 2022 00:56:29 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:53:59 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Sep 2022 03:54:00 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Sep 2022 03:54:07 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:54:10 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 13 Sep 2022 03:54:10 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Sep 2022 03:54:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:54:16 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 13 Sep 2022 03:54:16 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Sep 2022 03:54:29 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Sep 2022 03:54:30 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Sep 2022 03:54:30 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 13 Sep 2022 03:54:30 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 13 Sep 2022 03:54:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 03:54:30 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Sep 2022 03:54:31 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Sep 2022 03:54:31 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Sep 2022 03:54:31 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:31b3f1ad4ce1f369084d0f959813c51df0ca17d9877d5ee88c2db6ff88341430`  
		Last Modified: Tue, 13 Sep 2022 01:00:29 GMT  
		Size: 31.4 MB (31404121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9775a4fbb4b5564bbc1ec8e077d317b8745a7598e059365241ddc1a9766c129c`  
		Last Modified: Tue, 13 Sep 2022 03:55:55 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d707a0a4de816f6a35046bed27c3bd025081394b651fd4b339188a4e19967c4`  
		Last Modified: Tue, 13 Sep 2022 03:55:54 GMT  
		Size: 5.2 MB (5224215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c15634eb84187cbacfe864298c664c5eb740aa1a455a39e64f4f6a94c0f07a14`  
		Last Modified: Tue, 13 Sep 2022 03:55:53 GMT  
		Size: 1.6 MB (1553277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59f0fe4ba863352dbd7372301d2eae5be8cd69838e66876a65c5c0b1666de8c`  
		Last Modified: Tue, 13 Sep 2022 03:55:53 GMT  
		Size: 295.6 KB (295573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f507b233637bff8bdab3e80909e9dcdcc02a11efcca3f242c4ae8bf410296bbe`  
		Last Modified: Tue, 13 Sep 2022 03:55:53 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a76624d812c6c764f46d961f80510fa92e7512419c528ba6ab86e250d365d8`  
		Last Modified: Tue, 13 Sep 2022 03:55:56 GMT  
		Size: 49.0 MB (49045868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6166f23a925f2a6a18aa9efa186271f01020d8fd5d40d7a307cb02d6172974`  
		Last Modified: Tue, 13 Sep 2022 03:55:50 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc867e39bf60d67febf095d33500f8b30b51f6edbef26bd9d37b7a38a9bfaebc`  
		Last Modified: Tue, 13 Sep 2022 03:55:50 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5bc74ba5f149b1005fb23f07d5b84e4946fc31381d124892f99322b8c9a202`  
		Last Modified: Tue, 13 Sep 2022 03:55:50 GMT  
		Size: 2.2 KB (2187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ff75922f5a116b20c00eabe11b5280455fc7c77595f4ae03ed74a4e45ffb41`  
		Last Modified: Tue, 13 Sep 2022 03:55:50 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:15b86d4a7e914f5cb43435066ca4bab8cbcdaebe90b368ddd84e62b1276707cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.4 MB (85431442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c8d97bc3ed2957b5104f353e1f2c8a556ce0578fef9ea833e20f12084ffd785`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:48:29 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 05 Oct 2022 00:48:30 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 05 Oct 2022 00:48:37 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:48:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 05 Oct 2022 00:48:42 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 05 Oct 2022 00:48:48 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:48:48 GMT
ENV COUCHDB_VERSION=3.2.2
# Wed, 05 Oct 2022 00:48:49 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 05 Oct 2022 00:49:07 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Oct 2022 00:49:08 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 05 Oct 2022 00:49:09 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 05 Oct 2022 00:49:10 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 05 Oct 2022 00:49:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 00:49:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 00:49:12 GMT
VOLUME [/opt/couchdb/data]
# Wed, 05 Oct 2022 00:49:13 GMT
EXPOSE 4369 5984 9100
# Wed, 05 Oct 2022 00:49:14 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f51811668444e3b968d7a39cc5de30342e106eb12a367f9df356df8bbcf389`  
		Last Modified: Wed, 05 Oct 2022 00:51:09 GMT  
		Size: 3.3 KB (3323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3647d34c5a0150082687be7055d489b6b82a1373a51288e0ac2f96eb14d14bba`  
		Last Modified: Wed, 05 Oct 2022 00:51:08 GMT  
		Size: 5.0 MB (5003078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede8dd5eef52dc53a17137c8f44a05bdbb7d3051469c807a72604863295b68ef`  
		Last Modified: Wed, 05 Oct 2022 00:51:07 GMT  
		Size: 1.2 MB (1221098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7805f556f9096b24a1f655412b3e107a441d7f80ca8784574468f3b5af237e3c`  
		Last Modified: Wed, 05 Oct 2022 00:51:07 GMT  
		Size: 79.2 KB (79188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f2666158c95d59c0c61ac764acbb74e7454790953711cef91637f157db1029`  
		Last Modified: Wed, 05 Oct 2022 00:51:07 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34690541f949f6b1d8f46ae836e345d751c04b0aba8e1b09d9cbfd1b9d76e99a`  
		Last Modified: Wed, 05 Oct 2022 00:51:11 GMT  
		Size: 49.1 MB (49056628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4dc122dca5acda98426bf931c79625fad8ae9c9ce8ff53b480fd2b23f38203`  
		Last Modified: Wed, 05 Oct 2022 00:51:05 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:709b165a3a0c88c48e1537f0235f679a4473e281e80fc901b01c9a606b09fa21`  
		Last Modified: Wed, 05 Oct 2022 00:51:05 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b953f92a10f1393fe7e947f8523a7c20861b1e924f68da4b7ef27f6fd772ca`  
		Last Modified: Wed, 05 Oct 2022 00:51:05 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:923cca80d418f57784d23718f6af544e71daf08c5f06dafd817982538a7b0c82`  
		Last Modified: Wed, 05 Oct 2022 00:51:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2.2` - linux; ppc64le

```console
$ docker pull couchdb@sha256:143e3cd2945cb48d796d2278db9557504a800c77299549c9ac183576f1b6c918
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93229895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7711c8b3c5ab31870f4215b49471ddd8fa0a590d524a9b20be6af5f450232aa`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 04 Oct 2022 23:18:04 GMT
ADD file:66a0f55a4b4dfbb5d64082ffdb24751f20c5773039277ba278fdb4ce4a538c33 in / 
# Tue, 04 Oct 2022 23:18:06 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:08:24 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 05 Oct 2022 00:08:26 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 05 Oct 2022 00:08:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:08:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 05 Oct 2022 00:08:50 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 05 Oct 2022 00:09:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:09:02 GMT
ENV COUCHDB_VERSION=3.2.2
# Wed, 05 Oct 2022 00:09:03 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 05 Oct 2022 00:09:26 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Oct 2022 00:09:28 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 05 Oct 2022 00:09:28 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 05 Oct 2022 00:09:29 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 05 Oct 2022 00:09:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 00:09:30 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 00:09:31 GMT
VOLUME [/opt/couchdb/data]
# Wed, 05 Oct 2022 00:09:31 GMT
EXPOSE 4369 5984 9100
# Wed, 05 Oct 2022 00:09:31 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:4e001127162dd884a6f7bd2e6f74215816d325bebb3a374ae9fcee9f038f99b8`  
		Last Modified: Tue, 04 Oct 2022 23:24:13 GMT  
		Size: 35.3 MB (35290584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381109cbfbaaa798f564a18947f6c0f1dd5910da0234beab17bd5819ea39399d`  
		Last Modified: Wed, 05 Oct 2022 00:09:54 GMT  
		Size: 3.4 KB (3410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395cceb53989fdd5e1a8a72b46ca77b7d6663f50db82d16939a22fc6bc490b0d`  
		Last Modified: Wed, 05 Oct 2022 00:09:54 GMT  
		Size: 6.0 MB (6043722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c601f28412075f4767666bf160d562b535fd07b9fb959ef7ff65f470e5554bb`  
		Last Modified: Wed, 05 Oct 2022 00:09:52 GMT  
		Size: 1.5 MB (1509160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908145ec6ae093dd2fcc342bd38df282b5851f529d6b3a835ac93d69aaa33424`  
		Last Modified: Wed, 05 Oct 2022 00:09:52 GMT  
		Size: 295.5 KB (295506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f5839c8ec51b87036b5260c4c50c7b68102134e73a620710ba0c6c551e02cc`  
		Last Modified: Wed, 05 Oct 2022 00:09:52 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf4fabbea2bc9c827bf92aa5c2f2d24249508e1f71a1228e328d2611e0d899c`  
		Last Modified: Wed, 05 Oct 2022 00:09:59 GMT  
		Size: 50.1 MB (50083786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:435f63e26726324a42486d58656d232b9a7a902119575252fbd7326ff3e78f12`  
		Last Modified: Wed, 05 Oct 2022 00:09:50 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d3b1210769a993aa36f893916060dffb032025964550b36c01181138dc64f74`  
		Last Modified: Wed, 05 Oct 2022 00:09:49 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ab88b6abdfeff6d61bc12392dd5649756851f5b7dda2e77bea1bbea2f90038`  
		Last Modified: Wed, 05 Oct 2022 00:09:50 GMT  
		Size: 2.2 KB (2187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2fcd7203df115c27ce9f60eea1502476c8d59cc71edf4c6f0994b0a78b200c`  
		Last Modified: Wed, 05 Oct 2022 00:09:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:latest`

```console
$ docker pull couchdb@sha256:934ae4b7e2b88d4cb6b2cca03cb5c39d955cef2ffeb258d9b6511302e55716be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:ac5c57c4df9f9d0129390f652b62dfa348a1b383c458841010ad52abbb6c8f0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87530196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9292db79eb5d3107963496f664c9764d4974a423cff1612702d8ca782a888f5`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:29 GMT
ADD file:5bd53bff884e470b3c12425132975ab9c6f99002c62c43bca1ff5cde9d863b92 in / 
# Tue, 13 Sep 2022 00:56:29 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:53:59 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Sep 2022 03:54:00 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Sep 2022 03:54:07 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:54:10 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 13 Sep 2022 03:54:10 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Sep 2022 03:54:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:54:16 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 13 Sep 2022 03:54:16 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Sep 2022 03:54:29 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Sep 2022 03:54:30 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Sep 2022 03:54:30 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 13 Sep 2022 03:54:30 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 13 Sep 2022 03:54:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 03:54:30 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Sep 2022 03:54:31 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Sep 2022 03:54:31 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Sep 2022 03:54:31 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:31b3f1ad4ce1f369084d0f959813c51df0ca17d9877d5ee88c2db6ff88341430`  
		Last Modified: Tue, 13 Sep 2022 01:00:29 GMT  
		Size: 31.4 MB (31404121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9775a4fbb4b5564bbc1ec8e077d317b8745a7598e059365241ddc1a9766c129c`  
		Last Modified: Tue, 13 Sep 2022 03:55:55 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d707a0a4de816f6a35046bed27c3bd025081394b651fd4b339188a4e19967c4`  
		Last Modified: Tue, 13 Sep 2022 03:55:54 GMT  
		Size: 5.2 MB (5224215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c15634eb84187cbacfe864298c664c5eb740aa1a455a39e64f4f6a94c0f07a14`  
		Last Modified: Tue, 13 Sep 2022 03:55:53 GMT  
		Size: 1.6 MB (1553277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59f0fe4ba863352dbd7372301d2eae5be8cd69838e66876a65c5c0b1666de8c`  
		Last Modified: Tue, 13 Sep 2022 03:55:53 GMT  
		Size: 295.6 KB (295573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f507b233637bff8bdab3e80909e9dcdcc02a11efcca3f242c4ae8bf410296bbe`  
		Last Modified: Tue, 13 Sep 2022 03:55:53 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a76624d812c6c764f46d961f80510fa92e7512419c528ba6ab86e250d365d8`  
		Last Modified: Tue, 13 Sep 2022 03:55:56 GMT  
		Size: 49.0 MB (49045868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6166f23a925f2a6a18aa9efa186271f01020d8fd5d40d7a307cb02d6172974`  
		Last Modified: Tue, 13 Sep 2022 03:55:50 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc867e39bf60d67febf095d33500f8b30b51f6edbef26bd9d37b7a38a9bfaebc`  
		Last Modified: Tue, 13 Sep 2022 03:55:50 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5bc74ba5f149b1005fb23f07d5b84e4946fc31381d124892f99322b8c9a202`  
		Last Modified: Tue, 13 Sep 2022 03:55:50 GMT  
		Size: 2.2 KB (2187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ff75922f5a116b20c00eabe11b5280455fc7c77595f4ae03ed74a4e45ffb41`  
		Last Modified: Tue, 13 Sep 2022 03:55:50 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:15b86d4a7e914f5cb43435066ca4bab8cbcdaebe90b368ddd84e62b1276707cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.4 MB (85431442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c8d97bc3ed2957b5104f353e1f2c8a556ce0578fef9ea833e20f12084ffd785`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:48:29 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 05 Oct 2022 00:48:30 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 05 Oct 2022 00:48:37 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:48:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 05 Oct 2022 00:48:42 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 05 Oct 2022 00:48:48 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:48:48 GMT
ENV COUCHDB_VERSION=3.2.2
# Wed, 05 Oct 2022 00:48:49 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 05 Oct 2022 00:49:07 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Oct 2022 00:49:08 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 05 Oct 2022 00:49:09 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 05 Oct 2022 00:49:10 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 05 Oct 2022 00:49:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 00:49:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 00:49:12 GMT
VOLUME [/opt/couchdb/data]
# Wed, 05 Oct 2022 00:49:13 GMT
EXPOSE 4369 5984 9100
# Wed, 05 Oct 2022 00:49:14 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f51811668444e3b968d7a39cc5de30342e106eb12a367f9df356df8bbcf389`  
		Last Modified: Wed, 05 Oct 2022 00:51:09 GMT  
		Size: 3.3 KB (3323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3647d34c5a0150082687be7055d489b6b82a1373a51288e0ac2f96eb14d14bba`  
		Last Modified: Wed, 05 Oct 2022 00:51:08 GMT  
		Size: 5.0 MB (5003078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede8dd5eef52dc53a17137c8f44a05bdbb7d3051469c807a72604863295b68ef`  
		Last Modified: Wed, 05 Oct 2022 00:51:07 GMT  
		Size: 1.2 MB (1221098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7805f556f9096b24a1f655412b3e107a441d7f80ca8784574468f3b5af237e3c`  
		Last Modified: Wed, 05 Oct 2022 00:51:07 GMT  
		Size: 79.2 KB (79188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f2666158c95d59c0c61ac764acbb74e7454790953711cef91637f157db1029`  
		Last Modified: Wed, 05 Oct 2022 00:51:07 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34690541f949f6b1d8f46ae836e345d751c04b0aba8e1b09d9cbfd1b9d76e99a`  
		Last Modified: Wed, 05 Oct 2022 00:51:11 GMT  
		Size: 49.1 MB (49056628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4dc122dca5acda98426bf931c79625fad8ae9c9ce8ff53b480fd2b23f38203`  
		Last Modified: Wed, 05 Oct 2022 00:51:05 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:709b165a3a0c88c48e1537f0235f679a4473e281e80fc901b01c9a606b09fa21`  
		Last Modified: Wed, 05 Oct 2022 00:51:05 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b953f92a10f1393fe7e947f8523a7c20861b1e924f68da4b7ef27f6fd772ca`  
		Last Modified: Wed, 05 Oct 2022 00:51:05 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:923cca80d418f57784d23718f6af544e71daf08c5f06dafd817982538a7b0c82`  
		Last Modified: Wed, 05 Oct 2022 00:51:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; ppc64le

```console
$ docker pull couchdb@sha256:143e3cd2945cb48d796d2278db9557504a800c77299549c9ac183576f1b6c918
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93229895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7711c8b3c5ab31870f4215b49471ddd8fa0a590d524a9b20be6af5f450232aa`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 04 Oct 2022 23:18:04 GMT
ADD file:66a0f55a4b4dfbb5d64082ffdb24751f20c5773039277ba278fdb4ce4a538c33 in / 
# Tue, 04 Oct 2022 23:18:06 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:08:24 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 05 Oct 2022 00:08:26 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 05 Oct 2022 00:08:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:08:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 05 Oct 2022 00:08:50 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 05 Oct 2022 00:09:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:09:02 GMT
ENV COUCHDB_VERSION=3.2.2
# Wed, 05 Oct 2022 00:09:03 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 05 Oct 2022 00:09:26 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Oct 2022 00:09:28 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 05 Oct 2022 00:09:28 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 05 Oct 2022 00:09:29 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 05 Oct 2022 00:09:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 00:09:30 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 00:09:31 GMT
VOLUME [/opt/couchdb/data]
# Wed, 05 Oct 2022 00:09:31 GMT
EXPOSE 4369 5984 9100
# Wed, 05 Oct 2022 00:09:31 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:4e001127162dd884a6f7bd2e6f74215816d325bebb3a374ae9fcee9f038f99b8`  
		Last Modified: Tue, 04 Oct 2022 23:24:13 GMT  
		Size: 35.3 MB (35290584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381109cbfbaaa798f564a18947f6c0f1dd5910da0234beab17bd5819ea39399d`  
		Last Modified: Wed, 05 Oct 2022 00:09:54 GMT  
		Size: 3.4 KB (3410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395cceb53989fdd5e1a8a72b46ca77b7d6663f50db82d16939a22fc6bc490b0d`  
		Last Modified: Wed, 05 Oct 2022 00:09:54 GMT  
		Size: 6.0 MB (6043722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c601f28412075f4767666bf160d562b535fd07b9fb959ef7ff65f470e5554bb`  
		Last Modified: Wed, 05 Oct 2022 00:09:52 GMT  
		Size: 1.5 MB (1509160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908145ec6ae093dd2fcc342bd38df282b5851f529d6b3a835ac93d69aaa33424`  
		Last Modified: Wed, 05 Oct 2022 00:09:52 GMT  
		Size: 295.5 KB (295506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f5839c8ec51b87036b5260c4c50c7b68102134e73a620710ba0c6c551e02cc`  
		Last Modified: Wed, 05 Oct 2022 00:09:52 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf4fabbea2bc9c827bf92aa5c2f2d24249508e1f71a1228e328d2611e0d899c`  
		Last Modified: Wed, 05 Oct 2022 00:09:59 GMT  
		Size: 50.1 MB (50083786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:435f63e26726324a42486d58656d232b9a7a902119575252fbd7326ff3e78f12`  
		Last Modified: Wed, 05 Oct 2022 00:09:50 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d3b1210769a993aa36f893916060dffb032025964550b36c01181138dc64f74`  
		Last Modified: Wed, 05 Oct 2022 00:09:49 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ab88b6abdfeff6d61bc12392dd5649756851f5b7dda2e77bea1bbea2f90038`  
		Last Modified: Wed, 05 Oct 2022 00:09:50 GMT  
		Size: 2.2 KB (2187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2fcd7203df115c27ce9f60eea1502476c8d59cc71edf4c6f0994b0a78b200c`  
		Last Modified: Wed, 05 Oct 2022 00:09:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
