<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `couchdb`

-	[`couchdb:2`](#couchdb2)
-	[`couchdb:2.3`](#couchdb23)
-	[`couchdb:2.3.1`](#couchdb231)
-	[`couchdb:3`](#couchdb3)
-	[`couchdb:3.1`](#couchdb31)
-	[`couchdb:3.1.2`](#couchdb312)
-	[`couchdb:3.2`](#couchdb32)
-	[`couchdb:3.2.3`](#couchdb323)
-	[`couchdb:3.3`](#couchdb33)
-	[`couchdb:3.3.2`](#couchdb332)
-	[`couchdb:latest`](#couchdblatest)

## `couchdb:2`

```console
$ docker pull couchdb@sha256:0b99b61fd66e0c5e93fd70f5478171c688e1f299890f8fe36b5f27cb523ec6e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2` - linux; amd64

```console
$ docker pull couchdb@sha256:f530aa464748189fb4cb9437f146f4a77054c49b01eec23326fc1ff901ce69df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84536131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96918c3fb276e53901e03168afdd8764c82624f3e73fd11835f262ce2d5f05eb`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:32 GMT
ADD file:2818e508d01da2188fb234b38fb19aa1ea9eeeae92d361ecdf49318d949f51a9 in / 
# Mon, 12 Jun 2023 23:21:32 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:02:48 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Jun 2023 04:02:49 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Jun 2023 04:02:59 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:03:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 13 Jun 2023 04:03:04 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Jun 2023 04:03:11 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:03:29 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 13 Jun 2023 04:03:30 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Jun 2023 04:03:48 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Jun 2023 04:03:48 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Jun 2023 04:03:49 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 13 Jun 2023 04:03:49 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 13 Jun 2023 04:03:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 04:03:49 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:03:49 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Jun 2023 04:03:49 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Jun 2023 04:03:50 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:8b91b88d557765cd8c6802668755a3f6dc4337b6ce15a17e4857139e5fc964f3`  
		Last Modified: Mon, 12 Jun 2023 23:27:09 GMT  
		Size: 27.1 MB (27138450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19dce64dc1d986fe2a02da40cd4c32ca008166442ea4db561eab33b63f7cd126`  
		Last Modified: Tue, 13 Jun 2023 04:04:37 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6fb99156553b37b2d58e9a39225c37af49c63cfcc5f03833fd34bb10d34268`  
		Last Modified: Tue, 13 Jun 2023 04:04:36 GMT  
		Size: 6.7 MB (6704288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a50c5202daac6c76c5bd1d96dffd366da65456eddc306a8a77ef3de4a2cbb59`  
		Last Modified: Tue, 13 Jun 2023 04:04:35 GMT  
		Size: 1.3 MB (1259685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd650c9b2081d19a80d278a6396c0cbbdd34b45d6447ce293c4f8a5717981d54`  
		Last Modified: Tue, 13 Jun 2023 04:04:35 GMT  
		Size: 294.4 KB (294395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf42c30bc28466dc973f38316c0950f5661394dd2b9939b61540ca72422691a1`  
		Last Modified: Tue, 13 Jun 2023 04:04:48 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04306ba85711b8ab93c1b6a2c2e1319a6b9f032234fddce3fd1b2c09e59d6d4`  
		Last Modified: Tue, 13 Jun 2023 04:04:52 GMT  
		Size: 49.1 MB (49132304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85de8b774141c1c61eaa4be3d8a6b61262b278d238b20dc74f8c3bddb14aaa3`  
		Last Modified: Tue, 13 Jun 2023 04:04:46 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0d32f382de9d38f161ab52ccc6bd07bb3e3cc5a8046165fd6b42194c1a374a`  
		Last Modified: Tue, 13 Jun 2023 04:04:46 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adfdaf2d05607fa689935da29d8df4caa92273cd94634bd3ae59a9461fdb79a`  
		Last Modified: Tue, 13 Jun 2023 04:04:46 GMT  
		Size: 2.1 KB (2056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ff3919f1c9f0c5ffb9d0415ced2e37ee361789a966cb0fe250695bc547cbfc`  
		Last Modified: Tue, 13 Jun 2023 04:04:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:02057eeb80a595623788c49882979da93370f58e965daa36fce407651c7a58a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72994192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:071172ca5f921f5d94ab53a2cc1eff20dd8cbe37f8c65d1dd1b3f6ed45f907df`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:52 GMT
ADD file:d4a87f28032264e15d38bdd7efb6ffca8deadeb5388758f243e4866b360324c2 in / 
# Mon, 12 Jun 2023 23:40:52 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:11:57 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Jun 2023 03:11:58 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Jun 2023 03:12:04 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:12:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 13 Jun 2023 03:12:08 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Jun 2023 03:12:13 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:12:30 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 13 Jun 2023 03:12:31 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Jun 2023 03:12:42 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Jun 2023 03:12:43 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Jun 2023 03:12:43 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 13 Jun 2023 03:12:43 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 13 Jun 2023 03:12:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 03:12:43 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 03:12:43 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Jun 2023 03:12:44 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Jun 2023 03:12:44 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:d191be7a3c9fa95847a482db8211b6f85b45096c7817fdad4d7661ee7ff1a421`  
		Last Modified: Mon, 12 Jun 2023 23:45:21 GMT  
		Size: 25.9 MB (25921353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2213f55567f81f08bc5ba23f2f3c6222351ff646159063e2848c4a2dfc1ded`  
		Last Modified: Tue, 13 Jun 2023 03:13:16 GMT  
		Size: 3.4 KB (3433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92dc5471d249752ca5ec5b8fb080807fcc215bb6c19b55f7f87a04df41bdffd0`  
		Last Modified: Tue, 13 Jun 2023 03:13:15 GMT  
		Size: 6.6 MB (6577394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84eec32c687f2b22b459509b84844998435fb99ff588b07a339fb6535e257eda`  
		Last Modified: Tue, 13 Jun 2023 03:13:14 GMT  
		Size: 1.2 MB (1164584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf99775bdab8813fecf587e6a196f5c0f43b10f9b434652d160e0ff7040bc77`  
		Last Modified: Tue, 13 Jun 2023 03:13:14 GMT  
		Size: 294.2 KB (294224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c085b5208c57cf42e11e07dda04eedee7c048de3fc7df97f7b5a66fa1deb598c`  
		Last Modified: Tue, 13 Jun 2023 03:13:26 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c97d22258ae2941e86d3ab1290e900713c7e5fa34b14204fcaf0612497a3e6a7`  
		Last Modified: Tue, 13 Jun 2023 03:13:28 GMT  
		Size: 39.0 MB (39029605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa74f4d8727bf0ad49720e2fcfe1c66f6fa446a3e3ca810f37c618b5fd346d3`  
		Last Modified: Tue, 13 Jun 2023 03:13:24 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114bb35468b163fe4994a91a53b1b318ecac713936e4d2255e6bd3ffc493ab87`  
		Last Modified: Tue, 13 Jun 2023 03:13:24 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324b52e0f256b68cec535956d1627433e7525ea2cdae8cd9e73b5e501a876bfc`  
		Last Modified: Tue, 13 Jun 2023 03:13:24 GMT  
		Size: 2.1 KB (2056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9096ecbebafc651dee0df1e0f2e4ad41990c102040c491d353b55c0981d6697`  
		Last Modified: Tue, 13 Jun 2023 03:13:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3`

```console
$ docker pull couchdb@sha256:0b99b61fd66e0c5e93fd70f5478171c688e1f299890f8fe36b5f27cb523ec6e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:f530aa464748189fb4cb9437f146f4a77054c49b01eec23326fc1ff901ce69df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84536131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96918c3fb276e53901e03168afdd8764c82624f3e73fd11835f262ce2d5f05eb`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:32 GMT
ADD file:2818e508d01da2188fb234b38fb19aa1ea9eeeae92d361ecdf49318d949f51a9 in / 
# Mon, 12 Jun 2023 23:21:32 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:02:48 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Jun 2023 04:02:49 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Jun 2023 04:02:59 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:03:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 13 Jun 2023 04:03:04 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Jun 2023 04:03:11 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:03:29 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 13 Jun 2023 04:03:30 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Jun 2023 04:03:48 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Jun 2023 04:03:48 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Jun 2023 04:03:49 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 13 Jun 2023 04:03:49 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 13 Jun 2023 04:03:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 04:03:49 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:03:49 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Jun 2023 04:03:49 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Jun 2023 04:03:50 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:8b91b88d557765cd8c6802668755a3f6dc4337b6ce15a17e4857139e5fc964f3`  
		Last Modified: Mon, 12 Jun 2023 23:27:09 GMT  
		Size: 27.1 MB (27138450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19dce64dc1d986fe2a02da40cd4c32ca008166442ea4db561eab33b63f7cd126`  
		Last Modified: Tue, 13 Jun 2023 04:04:37 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6fb99156553b37b2d58e9a39225c37af49c63cfcc5f03833fd34bb10d34268`  
		Last Modified: Tue, 13 Jun 2023 04:04:36 GMT  
		Size: 6.7 MB (6704288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a50c5202daac6c76c5bd1d96dffd366da65456eddc306a8a77ef3de4a2cbb59`  
		Last Modified: Tue, 13 Jun 2023 04:04:35 GMT  
		Size: 1.3 MB (1259685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd650c9b2081d19a80d278a6396c0cbbdd34b45d6447ce293c4f8a5717981d54`  
		Last Modified: Tue, 13 Jun 2023 04:04:35 GMT  
		Size: 294.4 KB (294395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf42c30bc28466dc973f38316c0950f5661394dd2b9939b61540ca72422691a1`  
		Last Modified: Tue, 13 Jun 2023 04:04:48 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04306ba85711b8ab93c1b6a2c2e1319a6b9f032234fddce3fd1b2c09e59d6d4`  
		Last Modified: Tue, 13 Jun 2023 04:04:52 GMT  
		Size: 49.1 MB (49132304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85de8b774141c1c61eaa4be3d8a6b61262b278d238b20dc74f8c3bddb14aaa3`  
		Last Modified: Tue, 13 Jun 2023 04:04:46 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0d32f382de9d38f161ab52ccc6bd07bb3e3cc5a8046165fd6b42194c1a374a`  
		Last Modified: Tue, 13 Jun 2023 04:04:46 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adfdaf2d05607fa689935da29d8df4caa92273cd94634bd3ae59a9461fdb79a`  
		Last Modified: Tue, 13 Jun 2023 04:04:46 GMT  
		Size: 2.1 KB (2056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ff3919f1c9f0c5ffb9d0415ced2e37ee361789a966cb0fe250695bc547cbfc`  
		Last Modified: Tue, 13 Jun 2023 04:04:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:02057eeb80a595623788c49882979da93370f58e965daa36fce407651c7a58a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72994192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:071172ca5f921f5d94ab53a2cc1eff20dd8cbe37f8c65d1dd1b3f6ed45f907df`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:52 GMT
ADD file:d4a87f28032264e15d38bdd7efb6ffca8deadeb5388758f243e4866b360324c2 in / 
# Mon, 12 Jun 2023 23:40:52 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:11:57 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Jun 2023 03:11:58 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Jun 2023 03:12:04 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:12:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 13 Jun 2023 03:12:08 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Jun 2023 03:12:13 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:12:30 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 13 Jun 2023 03:12:31 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Jun 2023 03:12:42 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Jun 2023 03:12:43 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Jun 2023 03:12:43 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 13 Jun 2023 03:12:43 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 13 Jun 2023 03:12:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 03:12:43 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 03:12:43 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Jun 2023 03:12:44 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Jun 2023 03:12:44 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:d191be7a3c9fa95847a482db8211b6f85b45096c7817fdad4d7661ee7ff1a421`  
		Last Modified: Mon, 12 Jun 2023 23:45:21 GMT  
		Size: 25.9 MB (25921353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2213f55567f81f08bc5ba23f2f3c6222351ff646159063e2848c4a2dfc1ded`  
		Last Modified: Tue, 13 Jun 2023 03:13:16 GMT  
		Size: 3.4 KB (3433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92dc5471d249752ca5ec5b8fb080807fcc215bb6c19b55f7f87a04df41bdffd0`  
		Last Modified: Tue, 13 Jun 2023 03:13:15 GMT  
		Size: 6.6 MB (6577394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84eec32c687f2b22b459509b84844998435fb99ff588b07a339fb6535e257eda`  
		Last Modified: Tue, 13 Jun 2023 03:13:14 GMT  
		Size: 1.2 MB (1164584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf99775bdab8813fecf587e6a196f5c0f43b10f9b434652d160e0ff7040bc77`  
		Last Modified: Tue, 13 Jun 2023 03:13:14 GMT  
		Size: 294.2 KB (294224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c085b5208c57cf42e11e07dda04eedee7c048de3fc7df97f7b5a66fa1deb598c`  
		Last Modified: Tue, 13 Jun 2023 03:13:26 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c97d22258ae2941e86d3ab1290e900713c7e5fa34b14204fcaf0612497a3e6a7`  
		Last Modified: Tue, 13 Jun 2023 03:13:28 GMT  
		Size: 39.0 MB (39029605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa74f4d8727bf0ad49720e2fcfe1c66f6fa446a3e3ca810f37c618b5fd346d3`  
		Last Modified: Tue, 13 Jun 2023 03:13:24 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114bb35468b163fe4994a91a53b1b318ecac713936e4d2255e6bd3ffc493ab87`  
		Last Modified: Tue, 13 Jun 2023 03:13:24 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324b52e0f256b68cec535956d1627433e7525ea2cdae8cd9e73b5e501a876bfc`  
		Last Modified: Tue, 13 Jun 2023 03:13:24 GMT  
		Size: 2.1 KB (2056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9096ecbebafc651dee0df1e0f2e4ad41990c102040c491d353b55c0981d6697`  
		Last Modified: Tue, 13 Jun 2023 03:13:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3.1`

```console
$ docker pull couchdb@sha256:0b99b61fd66e0c5e93fd70f5478171c688e1f299890f8fe36b5f27cb523ec6e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:f530aa464748189fb4cb9437f146f4a77054c49b01eec23326fc1ff901ce69df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84536131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96918c3fb276e53901e03168afdd8764c82624f3e73fd11835f262ce2d5f05eb`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:32 GMT
ADD file:2818e508d01da2188fb234b38fb19aa1ea9eeeae92d361ecdf49318d949f51a9 in / 
# Mon, 12 Jun 2023 23:21:32 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:02:48 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Jun 2023 04:02:49 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Jun 2023 04:02:59 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:03:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 13 Jun 2023 04:03:04 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Jun 2023 04:03:11 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:03:29 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 13 Jun 2023 04:03:30 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Jun 2023 04:03:48 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Jun 2023 04:03:48 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Jun 2023 04:03:49 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 13 Jun 2023 04:03:49 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 13 Jun 2023 04:03:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 04:03:49 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:03:49 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Jun 2023 04:03:49 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Jun 2023 04:03:50 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:8b91b88d557765cd8c6802668755a3f6dc4337b6ce15a17e4857139e5fc964f3`  
		Last Modified: Mon, 12 Jun 2023 23:27:09 GMT  
		Size: 27.1 MB (27138450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19dce64dc1d986fe2a02da40cd4c32ca008166442ea4db561eab33b63f7cd126`  
		Last Modified: Tue, 13 Jun 2023 04:04:37 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6fb99156553b37b2d58e9a39225c37af49c63cfcc5f03833fd34bb10d34268`  
		Last Modified: Tue, 13 Jun 2023 04:04:36 GMT  
		Size: 6.7 MB (6704288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a50c5202daac6c76c5bd1d96dffd366da65456eddc306a8a77ef3de4a2cbb59`  
		Last Modified: Tue, 13 Jun 2023 04:04:35 GMT  
		Size: 1.3 MB (1259685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd650c9b2081d19a80d278a6396c0cbbdd34b45d6447ce293c4f8a5717981d54`  
		Last Modified: Tue, 13 Jun 2023 04:04:35 GMT  
		Size: 294.4 KB (294395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf42c30bc28466dc973f38316c0950f5661394dd2b9939b61540ca72422691a1`  
		Last Modified: Tue, 13 Jun 2023 04:04:48 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04306ba85711b8ab93c1b6a2c2e1319a6b9f032234fddce3fd1b2c09e59d6d4`  
		Last Modified: Tue, 13 Jun 2023 04:04:52 GMT  
		Size: 49.1 MB (49132304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85de8b774141c1c61eaa4be3d8a6b61262b278d238b20dc74f8c3bddb14aaa3`  
		Last Modified: Tue, 13 Jun 2023 04:04:46 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0d32f382de9d38f161ab52ccc6bd07bb3e3cc5a8046165fd6b42194c1a374a`  
		Last Modified: Tue, 13 Jun 2023 04:04:46 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1adfdaf2d05607fa689935da29d8df4caa92273cd94634bd3ae59a9461fdb79a`  
		Last Modified: Tue, 13 Jun 2023 04:04:46 GMT  
		Size: 2.1 KB (2056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ff3919f1c9f0c5ffb9d0415ced2e37ee361789a966cb0fe250695bc547cbfc`  
		Last Modified: Tue, 13 Jun 2023 04:04:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:02057eeb80a595623788c49882979da93370f58e965daa36fce407651c7a58a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72994192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:071172ca5f921f5d94ab53a2cc1eff20dd8cbe37f8c65d1dd1b3f6ed45f907df`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:52 GMT
ADD file:d4a87f28032264e15d38bdd7efb6ffca8deadeb5388758f243e4866b360324c2 in / 
# Mon, 12 Jun 2023 23:40:52 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:11:57 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Jun 2023 03:11:58 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Jun 2023 03:12:04 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:12:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 13 Jun 2023 03:12:08 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Jun 2023 03:12:13 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:12:30 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 13 Jun 2023 03:12:31 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Jun 2023 03:12:42 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Jun 2023 03:12:43 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Jun 2023 03:12:43 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 13 Jun 2023 03:12:43 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 13 Jun 2023 03:12:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 03:12:43 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 03:12:43 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Jun 2023 03:12:44 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Jun 2023 03:12:44 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:d191be7a3c9fa95847a482db8211b6f85b45096c7817fdad4d7661ee7ff1a421`  
		Last Modified: Mon, 12 Jun 2023 23:45:21 GMT  
		Size: 25.9 MB (25921353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2213f55567f81f08bc5ba23f2f3c6222351ff646159063e2848c4a2dfc1ded`  
		Last Modified: Tue, 13 Jun 2023 03:13:16 GMT  
		Size: 3.4 KB (3433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92dc5471d249752ca5ec5b8fb080807fcc215bb6c19b55f7f87a04df41bdffd0`  
		Last Modified: Tue, 13 Jun 2023 03:13:15 GMT  
		Size: 6.6 MB (6577394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84eec32c687f2b22b459509b84844998435fb99ff588b07a339fb6535e257eda`  
		Last Modified: Tue, 13 Jun 2023 03:13:14 GMT  
		Size: 1.2 MB (1164584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf99775bdab8813fecf587e6a196f5c0f43b10f9b434652d160e0ff7040bc77`  
		Last Modified: Tue, 13 Jun 2023 03:13:14 GMT  
		Size: 294.2 KB (294224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c085b5208c57cf42e11e07dda04eedee7c048de3fc7df97f7b5a66fa1deb598c`  
		Last Modified: Tue, 13 Jun 2023 03:13:26 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c97d22258ae2941e86d3ab1290e900713c7e5fa34b14204fcaf0612497a3e6a7`  
		Last Modified: Tue, 13 Jun 2023 03:13:28 GMT  
		Size: 39.0 MB (39029605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa74f4d8727bf0ad49720e2fcfe1c66f6fa446a3e3ca810f37c618b5fd346d3`  
		Last Modified: Tue, 13 Jun 2023 03:13:24 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114bb35468b163fe4994a91a53b1b318ecac713936e4d2255e6bd3ffc493ab87`  
		Last Modified: Tue, 13 Jun 2023 03:13:24 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324b52e0f256b68cec535956d1627433e7525ea2cdae8cd9e73b5e501a876bfc`  
		Last Modified: Tue, 13 Jun 2023 03:13:24 GMT  
		Size: 2.1 KB (2056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9096ecbebafc651dee0df1e0f2e4ad41990c102040c491d353b55c0981d6697`  
		Last Modified: Tue, 13 Jun 2023 03:13:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3`

```console
$ docker pull couchdb@sha256:b889ec0dba71a167320a6e90a9198ee13d382bbfc9c3913f405a2f6a7dedc44f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `couchdb:3` - linux; amd64

```console
$ docker pull couchdb@sha256:40016f83b61df0ac945f1536e3a52e6ea2761a18326933513bbe358e5f787102
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90239977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b725f6b2513a8b4ec7c8b706aed6ac7a7166a5c833b1a23dd2f559310808110`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:01:57 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Jun 2023 04:01:58 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Jun 2023 04:02:05 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:02:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 13 Jun 2023 04:02:09 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Jun 2023 04:02:13 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:02:14 GMT
ENV COUCHDB_VERSION=3.3.2
# Tue, 13 Jun 2023 04:02:14 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Jun 2023 04:02:27 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Jun 2023 04:02:27 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Jun 2023 04:02:27 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 13 Jun 2023 04:02:27 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 13 Jun 2023 04:02:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 04:02:28 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:02:28 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Jun 2023 04:02:28 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Jun 2023 04:02:28 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56fa5a08f48785d08765b7746d507926063e6ab14084ec52c45ad658c9900e2`  
		Last Modified: Tue, 13 Jun 2023 04:04:05 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:effeea359db8a5b5241e47adb1070cec93345c3cc2011db12b74a56d6cec9151`  
		Last Modified: Tue, 13 Jun 2023 04:04:04 GMT  
		Size: 5.2 MB (5224468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b83a1bd5e8dd69f1172af3053ab31900973778718afe1abb82dd6d9cf4075a`  
		Last Modified: Tue, 13 Jun 2023 04:04:03 GMT  
		Size: 610.3 KB (610265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d5ee803171a181293d9529fab444ccda628ce617e53d52acb7bbd34e1dbe3f`  
		Last Modified: Tue, 13 Jun 2023 04:04:03 GMT  
		Size: 294.4 KB (294377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abff9bf83b2eee5ea095f234f197ed3bdc13ba5c1d9d27e366d814ca232560d3`  
		Last Modified: Tue, 13 Jun 2023 04:04:03 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1c0289451f671b5a57844126e484dc7f940b217bdd9badb059bda68d8764ab`  
		Last Modified: Tue, 13 Jun 2023 04:04:07 GMT  
		Size: 52.7 MB (52686042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f7f7afef66f9db1812bc4358426b2221d5126baecd2715d01530d1fa9ea2e86`  
		Last Modified: Tue, 13 Jun 2023 04:04:01 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d22413df733620c7d50f6db00f44e8dd5cd48ae5343fcbb767b482c4f0f9ad`  
		Last Modified: Tue, 13 Jun 2023 04:04:01 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7983d64b4de2667bb5662734e159cb3529658b676c0c32a3e5906a4a26d27ce3`  
		Last Modified: Tue, 13 Jun 2023 04:04:01 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf22f027705f7c7b494a7c2f2bd1d7b88f54297a0cd015536fdf35b915ace46`  
		Last Modified: Tue, 13 Jun 2023 04:04:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:141772490f9958ea64a517669cb9f3284f540ab4ec5486e2e685f63f0d080f51
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88684701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5caf00b8d2804b512825d7ae87ef5c0320c191a123d13c11a57b1e2e079bd70d`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:11:13 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Jun 2023 03:11:13 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Jun 2023 03:11:20 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:11:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 13 Jun 2023 03:11:23 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Jun 2023 03:11:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:11:27 GMT
ENV COUCHDB_VERSION=3.3.2
# Tue, 13 Jun 2023 03:11:28 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Jun 2023 03:11:39 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Jun 2023 03:11:40 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Jun 2023 03:11:40 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 13 Jun 2023 03:11:40 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 13 Jun 2023 03:11:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 03:11:40 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 03:11:40 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Jun 2023 03:11:40 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Jun 2023 03:11:40 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e233a96952e1934fa67393b0643bae29d210a5989e09f4b7f420b079982c96c4`  
		Last Modified: Tue, 13 Jun 2023 03:12:58 GMT  
		Size: 3.4 KB (3425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c60a62bf69974ac716a93c155b419669eaac5acbbcc214c6c211667ab267c9`  
		Last Modified: Tue, 13 Jun 2023 03:12:57 GMT  
		Size: 5.2 MB (5209604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750b53c5b967617f8b2ff9cb0ecc88700772caab48f3b4f59f6d1e9a844e427a`  
		Last Modified: Tue, 13 Jun 2023 03:12:56 GMT  
		Size: 566.3 KB (566262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c843fecc8eafd5a7c37f7c3329458c4bb1cc58d6836fee8d9e8acff6f9b38c0`  
		Last Modified: Tue, 13 Jun 2023 03:12:56 GMT  
		Size: 294.3 KB (294347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c90431247a4ed342f9d684e9b04bb9bfc5dda7118d4267e7b3f23bd59ad4fd`  
		Last Modified: Tue, 13 Jun 2023 03:12:56 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f35924c1a48bb2edaa217e033e1fbee469d6e11c805e338939f681aaefbf34`  
		Last Modified: Tue, 13 Jun 2023 03:12:59 GMT  
		Size: 52.5 MB (52544231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471f7004fd790c6758674730bf2f9bd8fdabf72eca171b74caa8ef1744fece7e`  
		Last Modified: Tue, 13 Jun 2023 03:12:54 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d386b3f9b6664b042d1774b40dff2342b3c02d82cade1337f63021606bd299e6`  
		Last Modified: Tue, 13 Jun 2023 03:12:54 GMT  
		Size: 998.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b370d69da1a2a4adc59447af4f255ae1ec356c733e4b73d3b96b7761810229dc`  
		Last Modified: Tue, 13 Jun 2023 03:12:54 GMT  
		Size: 2.2 KB (2227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77933cca358498c1f5feb64dd9ed2c965d85c8d49fdb7db2e72e68bd245712f3`  
		Last Modified: Tue, 13 Jun 2023 03:12:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; ppc64le

```console
$ docker pull couchdb@sha256:c399e90a9b1b305e1b72125a4905ae3c51db4be6dff26c4a78bc27e759035a00
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.0 MB (95961503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ca27ec01131c11c250078f1488ed292338f0ceeefadde47ac20108c3e7e4b4b`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Mon, 12 Jun 2023 23:18:20 GMT
ADD file:b17eabe509462fa1a2e4c5421e877e3e4149085e3da07a421a66c7b06566c457 in / 
# Mon, 12 Jun 2023 23:18:22 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 09:45:19 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Jun 2023 09:45:20 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Jun 2023 09:45:36 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 09:45:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 13 Jun 2023 09:45:44 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Jun 2023 09:45:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 09:45:56 GMT
ENV COUCHDB_VERSION=3.3.2
# Tue, 13 Jun 2023 09:45:57 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Jun 2023 09:46:20 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Jun 2023 09:46:22 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Jun 2023 09:46:22 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 13 Jun 2023 09:46:23 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 13 Jun 2023 09:46:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 09:46:24 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 09:46:24 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Jun 2023 09:46:25 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Jun 2023 09:46:25 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:2973ac0be4a80a6cecbb73370e92810a6f67a98e12e61b3044aa63a322dab03a`  
		Last Modified: Mon, 12 Jun 2023 23:25:03 GMT  
		Size: 35.3 MB (35290790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7a4c14920d3766677c031be9ca45255dc9e4840b301c89d08bbab6c0c829b8`  
		Last Modified: Tue, 13 Jun 2023 09:47:05 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ee15726d36a785865415f386f34e9c4214a817d6dc79aec252811407ced685`  
		Last Modified: Tue, 13 Jun 2023 09:47:05 GMT  
		Size: 6.0 MB (6044040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a5cfeef71b924481f431fd94af56f33ccc02f4fcd0ce1b39afedb3168bd228a`  
		Last Modified: Tue, 13 Jun 2023 09:47:03 GMT  
		Size: 662.1 KB (662089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:799b3ab5e90729432923cecf21aad2ed782c84206d9d207078011186642aad90`  
		Last Modified: Tue, 13 Jun 2023 09:47:03 GMT  
		Size: 294.3 KB (294296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd6815c4999f2fa98c8cf4608b23fa063cf5a774c83160b584f54643a784eb0`  
		Last Modified: Tue, 13 Jun 2023 09:47:03 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea7c054364d04ef4b21f2a283c8ab5a0d200b3dfc983a9d4efd4c9b00c744a5c`  
		Last Modified: Tue, 13 Jun 2023 09:47:11 GMT  
		Size: 53.7 MB (53662870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76fc449be4ce6b84b9700f3c78608d408a725c28dc094af606d988eb350474da`  
		Last Modified: Tue, 13 Jun 2023 09:47:01 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064cc07cec794834bfcdae6cc7830104662247eeb39c275d846db362bc91301d`  
		Last Modified: Tue, 13 Jun 2023 09:47:01 GMT  
		Size: 999.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:214dfd321091da26c6f756ee7d21328d6e12653fd1acb75f40dfaf0063174b67`  
		Last Modified: Tue, 13 Jun 2023 09:47:01 GMT  
		Size: 2.2 KB (2228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03afeadee0940c842a4ed2c86ddb83b2a9fce341219595a1b84ffb0c299fe48f`  
		Last Modified: Tue, 13 Jun 2023 09:47:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; s390x

```console
$ docker pull couchdb@sha256:27f57b5ffc3a8799873fd57224eb642f883f404866610dbabd7710e700fa7d55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.0 MB (86982637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9c3afe9604f8597d2587042e19236a4a9af934cb69c067b9eb73e86501d11aa`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 23 May 2023 00:42:52 GMT
ADD file:23b1e12559302529556a94a1d4098dbdb454e263265258b940c2b2d23a97c121 in / 
# Tue, 23 May 2023 00:42:54 GMT
CMD ["bash"]
# Wed, 31 May 2023 23:41:40 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 31 May 2023 23:41:41 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 31 May 2023 23:41:47 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 31 May 2023 23:41:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 31 May 2023 23:41:50 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 31 May 2023 23:41:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 31 May 2023 23:41:55 GMT
ENV COUCHDB_VERSION=3.3.2
# Wed, 31 May 2023 23:41:55 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 31 May 2023 23:42:11 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 31 May 2023 23:42:12 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 31 May 2023 23:42:12 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 31 May 2023 23:42:13 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 31 May 2023 23:42:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 31 May 2023 23:42:13 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 31 May 2023 23:42:13 GMT
VOLUME [/opt/couchdb/data]
# Wed, 31 May 2023 23:42:13 GMT
EXPOSE 4369 5984 9100
# Wed, 31 May 2023 23:42:13 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:9c24ec455bdb6a9ad0d033c7cce8e71dd5bdbbe53a86d5feeb8d4cb7804fb8e5`  
		Last Modified: Tue, 23 May 2023 00:45:47 GMT  
		Size: 29.6 MB (29642170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79369d7477079fd194a68b466dff2d8edc280d261dc304b2567bfb55973c870b`  
		Last Modified: Wed, 31 May 2023 23:42:31 GMT  
		Size: 3.4 KB (3433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bea484bba066eb8863a66dcecc668d69aec750f8d1c0ad9325cc89b8210d148`  
		Last Modified: Wed, 31 May 2023 23:42:30 GMT  
		Size: 5.1 MB (5110473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5297b03b741ba1714084f21808e891def15cc57d292f901233aa010d56eda78e`  
		Last Modified: Wed, 31 May 2023 23:42:30 GMT  
		Size: 573.0 KB (573029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c1c59cdce3bf8d5680cb008d32bc45637f344c162a7912c90d5bbb3d0c753d`  
		Last Modified: Wed, 31 May 2023 23:42:30 GMT  
		Size: 294.5 KB (294451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89faeb4398086a27f7d1c2cfd535d3d86db34051276853757976607b8e6697e6`  
		Last Modified: Wed, 31 May 2023 23:42:30 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d08b9ecfe40b07d3aac1d314249e9c5843ce52edc2bea23828d62981849ff18`  
		Last Modified: Wed, 31 May 2023 23:42:34 GMT  
		Size: 51.4 MB (51355073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a8e6b453b90234fdb6dd9135a15beae0f3ba97050c5bd98264e1564f32386f`  
		Last Modified: Wed, 31 May 2023 23:42:28 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce5dd09ac3c1e930fd074767a97609f55cca10e5f1c213a684236bf7d4852b0`  
		Last Modified: Wed, 31 May 2023 23:42:28 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c7c51f86fe82775ec0e610e7ee7e3bf2e4ec64fe2d2a9ac042c388b5a61810`  
		Last Modified: Wed, 31 May 2023 23:42:28 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36cb0e3d58be45185e1df3bd73ef5f6906dad6517350c73fab6653744a44d7c`  
		Last Modified: Wed, 31 May 2023 23:42:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1`

```console
$ docker pull couchdb@sha256:9f3e6bf527b7075d72dfac1d1d1dd722cbe5597b3b9d69dd25a68108899726b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:2a2307415ded35db033de3738950a0cbb9b17dadee7f140896f31b1d8ad5ce9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80023796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:134062f2fcc091d3d855826efe96aa5309b7c4dbd1d3da286cd66d09fa01d8bd`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:32 GMT
ADD file:2818e508d01da2188fb234b38fb19aa1ea9eeeae92d361ecdf49318d949f51a9 in / 
# Mon, 12 Jun 2023 23:21:32 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:02:48 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Jun 2023 04:02:49 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Jun 2023 04:02:59 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:03:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 13 Jun 2023 04:03:04 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Jun 2023 04:03:11 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:03:11 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 13 Jun 2023 04:03:12 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Jun 2023 04:03:25 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Jun 2023 04:03:25 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Jun 2023 04:03:25 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 13 Jun 2023 04:03:25 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 13 Jun 2023 04:03:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 04:03:26 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:03:26 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Jun 2023 04:03:26 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Jun 2023 04:03:26 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:8b91b88d557765cd8c6802668755a3f6dc4337b6ce15a17e4857139e5fc964f3`  
		Last Modified: Mon, 12 Jun 2023 23:27:09 GMT  
		Size: 27.1 MB (27138450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19dce64dc1d986fe2a02da40cd4c32ca008166442ea4db561eab33b63f7cd126`  
		Last Modified: Tue, 13 Jun 2023 04:04:37 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6fb99156553b37b2d58e9a39225c37af49c63cfcc5f03833fd34bb10d34268`  
		Last Modified: Tue, 13 Jun 2023 04:04:36 GMT  
		Size: 6.7 MB (6704288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a50c5202daac6c76c5bd1d96dffd366da65456eddc306a8a77ef3de4a2cbb59`  
		Last Modified: Tue, 13 Jun 2023 04:04:35 GMT  
		Size: 1.3 MB (1259685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd650c9b2081d19a80d278a6396c0cbbdd34b45d6447ce293c4f8a5717981d54`  
		Last Modified: Tue, 13 Jun 2023 04:04:35 GMT  
		Size: 294.4 KB (294395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22c2981ce802ff3af09597af4c3d5fa3c00b9c1d470c90e0be6e3040d1cffcc`  
		Last Modified: Tue, 13 Jun 2023 04:04:35 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81596bdfad922a44b726226abb7db7f4c97c88ec16e805ac13cbdd5b5ec125a6`  
		Last Modified: Tue, 13 Jun 2023 04:04:38 GMT  
		Size: 44.6 MB (44619975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c0b99740b533501ceaad0807cd7be644e8aa431d479aecaff8cd03f9f9296d`  
		Last Modified: Tue, 13 Jun 2023 04:04:33 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c86518fe5107ac033c504c023a35d97166b8f64e9e1450a55cf79bf2c060c1`  
		Last Modified: Tue, 13 Jun 2023 04:04:33 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3dc7f68ec827cd8a7c6b88ccc917646e5872f284e9ec624daf6949faa2147aa`  
		Last Modified: Tue, 13 Jun 2023 04:04:33 GMT  
		Size: 2.1 KB (2055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d80149eff3a59dbc742ea73df38ce43e01cc9beb72aca8d415e20ae25a11d9`  
		Last Modified: Tue, 13 Jun 2023 04:04:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:50b83c69fe20e483ff670d196e0cd34f321dbd53a5d7a0daabcb82edc0a8ea29
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75090906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f317e85c3e007697b8816f7006950bd61ed2460a215c8f1e11109df29f4a9a74`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:52 GMT
ADD file:d4a87f28032264e15d38bdd7efb6ffca8deadeb5388758f243e4866b360324c2 in / 
# Mon, 12 Jun 2023 23:40:52 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:11:57 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Jun 2023 03:11:58 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Jun 2023 03:12:04 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:12:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 13 Jun 2023 03:12:08 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Jun 2023 03:12:13 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:12:14 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 13 Jun 2023 03:12:14 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Jun 2023 03:12:26 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Jun 2023 03:12:26 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Jun 2023 03:12:26 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 13 Jun 2023 03:12:26 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 13 Jun 2023 03:12:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 03:12:27 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 03:12:27 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Jun 2023 03:12:27 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Jun 2023 03:12:27 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:d191be7a3c9fa95847a482db8211b6f85b45096c7817fdad4d7661ee7ff1a421`  
		Last Modified: Mon, 12 Jun 2023 23:45:21 GMT  
		Size: 25.9 MB (25921353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2213f55567f81f08bc5ba23f2f3c6222351ff646159063e2848c4a2dfc1ded`  
		Last Modified: Tue, 13 Jun 2023 03:13:16 GMT  
		Size: 3.4 KB (3433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92dc5471d249752ca5ec5b8fb080807fcc215bb6c19b55f7f87a04df41bdffd0`  
		Last Modified: Tue, 13 Jun 2023 03:13:15 GMT  
		Size: 6.6 MB (6577394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84eec32c687f2b22b459509b84844998435fb99ff588b07a339fb6535e257eda`  
		Last Modified: Tue, 13 Jun 2023 03:13:14 GMT  
		Size: 1.2 MB (1164584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf99775bdab8813fecf587e6a196f5c0f43b10f9b434652d160e0ff7040bc77`  
		Last Modified: Tue, 13 Jun 2023 03:13:14 GMT  
		Size: 294.2 KB (294224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:799efcdc71b4eb17ebe4419cc2a5a995c62ccd9e800cc9af3b78c5f657b6cdb5`  
		Last Modified: Tue, 13 Jun 2023 03:13:13 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0b61c1568ef1f3dbed3e64c516ce8985d29f7208590bd2f9d72839c3b6b523`  
		Last Modified: Tue, 13 Jun 2023 03:13:15 GMT  
		Size: 41.1 MB (41126321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81968efaf0aaa5a3053771d4e64bbe4154a9319410ca02498d8c063159829b80`  
		Last Modified: Tue, 13 Jun 2023 03:13:12 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49a184256086427df0b8d942c5c7b5c73e4109d1a72fc0ba5dcd1b9e4c80a85`  
		Last Modified: Tue, 13 Jun 2023 03:13:12 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312bf3ffed99f9f12009bc5db0cefff3195e6f1069eeeb102dad19c066e3e58a`  
		Last Modified: Tue, 13 Jun 2023 03:13:12 GMT  
		Size: 2.1 KB (2055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc91fd03927356accbc0142ab952fd6bc351ab894b9afd161088b4200116168`  
		Last Modified: Tue, 13 Jun 2023 03:13:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1.2`

```console
$ docker pull couchdb@sha256:9f3e6bf527b7075d72dfac1d1d1dd722cbe5597b3b9d69dd25a68108899726b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1.2` - linux; amd64

```console
$ docker pull couchdb@sha256:2a2307415ded35db033de3738950a0cbb9b17dadee7f140896f31b1d8ad5ce9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80023796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:134062f2fcc091d3d855826efe96aa5309b7c4dbd1d3da286cd66d09fa01d8bd`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:32 GMT
ADD file:2818e508d01da2188fb234b38fb19aa1ea9eeeae92d361ecdf49318d949f51a9 in / 
# Mon, 12 Jun 2023 23:21:32 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:02:48 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Jun 2023 04:02:49 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Jun 2023 04:02:59 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:03:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 13 Jun 2023 04:03:04 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Jun 2023 04:03:11 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:03:11 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 13 Jun 2023 04:03:12 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Jun 2023 04:03:25 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Jun 2023 04:03:25 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Jun 2023 04:03:25 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 13 Jun 2023 04:03:25 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 13 Jun 2023 04:03:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 04:03:26 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:03:26 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Jun 2023 04:03:26 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Jun 2023 04:03:26 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:8b91b88d557765cd8c6802668755a3f6dc4337b6ce15a17e4857139e5fc964f3`  
		Last Modified: Mon, 12 Jun 2023 23:27:09 GMT  
		Size: 27.1 MB (27138450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19dce64dc1d986fe2a02da40cd4c32ca008166442ea4db561eab33b63f7cd126`  
		Last Modified: Tue, 13 Jun 2023 04:04:37 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6fb99156553b37b2d58e9a39225c37af49c63cfcc5f03833fd34bb10d34268`  
		Last Modified: Tue, 13 Jun 2023 04:04:36 GMT  
		Size: 6.7 MB (6704288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a50c5202daac6c76c5bd1d96dffd366da65456eddc306a8a77ef3de4a2cbb59`  
		Last Modified: Tue, 13 Jun 2023 04:04:35 GMT  
		Size: 1.3 MB (1259685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd650c9b2081d19a80d278a6396c0cbbdd34b45d6447ce293c4f8a5717981d54`  
		Last Modified: Tue, 13 Jun 2023 04:04:35 GMT  
		Size: 294.4 KB (294395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22c2981ce802ff3af09597af4c3d5fa3c00b9c1d470c90e0be6e3040d1cffcc`  
		Last Modified: Tue, 13 Jun 2023 04:04:35 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81596bdfad922a44b726226abb7db7f4c97c88ec16e805ac13cbdd5b5ec125a6`  
		Last Modified: Tue, 13 Jun 2023 04:04:38 GMT  
		Size: 44.6 MB (44619975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c0b99740b533501ceaad0807cd7be644e8aa431d479aecaff8cd03f9f9296d`  
		Last Modified: Tue, 13 Jun 2023 04:04:33 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c86518fe5107ac033c504c023a35d97166b8f64e9e1450a55cf79bf2c060c1`  
		Last Modified: Tue, 13 Jun 2023 04:04:33 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3dc7f68ec827cd8a7c6b88ccc917646e5872f284e9ec624daf6949faa2147aa`  
		Last Modified: Tue, 13 Jun 2023 04:04:33 GMT  
		Size: 2.1 KB (2055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d80149eff3a59dbc742ea73df38ce43e01cc9beb72aca8d415e20ae25a11d9`  
		Last Modified: Tue, 13 Jun 2023 04:04:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:50b83c69fe20e483ff670d196e0cd34f321dbd53a5d7a0daabcb82edc0a8ea29
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75090906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f317e85c3e007697b8816f7006950bd61ed2460a215c8f1e11109df29f4a9a74`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:52 GMT
ADD file:d4a87f28032264e15d38bdd7efb6ffca8deadeb5388758f243e4866b360324c2 in / 
# Mon, 12 Jun 2023 23:40:52 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:11:57 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Jun 2023 03:11:58 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Jun 2023 03:12:04 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:12:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 13 Jun 2023 03:12:08 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Jun 2023 03:12:13 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:12:14 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 13 Jun 2023 03:12:14 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Jun 2023 03:12:26 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Jun 2023 03:12:26 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Jun 2023 03:12:26 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 13 Jun 2023 03:12:26 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 13 Jun 2023 03:12:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 03:12:27 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 03:12:27 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Jun 2023 03:12:27 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Jun 2023 03:12:27 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:d191be7a3c9fa95847a482db8211b6f85b45096c7817fdad4d7661ee7ff1a421`  
		Last Modified: Mon, 12 Jun 2023 23:45:21 GMT  
		Size: 25.9 MB (25921353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2213f55567f81f08bc5ba23f2f3c6222351ff646159063e2848c4a2dfc1ded`  
		Last Modified: Tue, 13 Jun 2023 03:13:16 GMT  
		Size: 3.4 KB (3433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92dc5471d249752ca5ec5b8fb080807fcc215bb6c19b55f7f87a04df41bdffd0`  
		Last Modified: Tue, 13 Jun 2023 03:13:15 GMT  
		Size: 6.6 MB (6577394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84eec32c687f2b22b459509b84844998435fb99ff588b07a339fb6535e257eda`  
		Last Modified: Tue, 13 Jun 2023 03:13:14 GMT  
		Size: 1.2 MB (1164584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf99775bdab8813fecf587e6a196f5c0f43b10f9b434652d160e0ff7040bc77`  
		Last Modified: Tue, 13 Jun 2023 03:13:14 GMT  
		Size: 294.2 KB (294224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:799efcdc71b4eb17ebe4419cc2a5a995c62ccd9e800cc9af3b78c5f657b6cdb5`  
		Last Modified: Tue, 13 Jun 2023 03:13:13 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0b61c1568ef1f3dbed3e64c516ce8985d29f7208590bd2f9d72839c3b6b523`  
		Last Modified: Tue, 13 Jun 2023 03:13:15 GMT  
		Size: 41.1 MB (41126321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81968efaf0aaa5a3053771d4e64bbe4154a9319410ca02498d8c063159829b80`  
		Last Modified: Tue, 13 Jun 2023 03:13:12 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49a184256086427df0b8d942c5c7b5c73e4109d1a72fc0ba5dcd1b9e4c80a85`  
		Last Modified: Tue, 13 Jun 2023 03:13:12 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312bf3ffed99f9f12009bc5db0cefff3195e6f1069eeeb102dad19c066e3e58a`  
		Last Modified: Tue, 13 Jun 2023 03:13:12 GMT  
		Size: 2.1 KB (2055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc91fd03927356accbc0142ab952fd6bc351ab894b9afd161088b4200116168`  
		Last Modified: Tue, 13 Jun 2023 03:13:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2`

```console
$ docker pull couchdb@sha256:d86c0902299a50886c853fb3c4e15fb9168c42fbe2edb9f14c2f683f3920028c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2` - linux; amd64

```console
$ docker pull couchdb@sha256:22fdd25d4eef5d0385853f6079463a23ca52bfcbd8d0dc7092dbd9797adf897d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.7 MB (89740540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a70f12d6bc5aa3e6c706277ff2c517d3bfcd6bc7dcdff28e99c7318d0c5f318`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:01:57 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Jun 2023 04:01:58 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Jun 2023 04:02:05 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:02:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 13 Jun 2023 04:02:09 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Jun 2023 04:02:13 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:02:32 GMT
ENV COUCHDB_VERSION=3.2.3
# Tue, 13 Jun 2023 04:02:32 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Jun 2023 04:02:44 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Jun 2023 04:02:45 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Jun 2023 04:02:45 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 13 Jun 2023 04:02:45 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 13 Jun 2023 04:02:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 04:02:46 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:02:46 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Jun 2023 04:02:46 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Jun 2023 04:02:46 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56fa5a08f48785d08765b7746d507926063e6ab14084ec52c45ad658c9900e2`  
		Last Modified: Tue, 13 Jun 2023 04:04:05 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:effeea359db8a5b5241e47adb1070cec93345c3cc2011db12b74a56d6cec9151`  
		Last Modified: Tue, 13 Jun 2023 04:04:04 GMT  
		Size: 5.2 MB (5224468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b83a1bd5e8dd69f1172af3053ab31900973778718afe1abb82dd6d9cf4075a`  
		Last Modified: Tue, 13 Jun 2023 04:04:03 GMT  
		Size: 610.3 KB (610265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d5ee803171a181293d9529fab444ccda628ce617e53d52acb7bbd34e1dbe3f`  
		Last Modified: Tue, 13 Jun 2023 04:04:03 GMT  
		Size: 294.4 KB (294377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7bcd34bc103365c025d56bb91321fb3f909de9d2d8a3f86e2e42840dd5c967`  
		Last Modified: Tue, 13 Jun 2023 04:04:21 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c75aaa8226bcf8bd5abde0889b8926be9f496fb20715116927c48c9805a805`  
		Last Modified: Tue, 13 Jun 2023 04:04:25 GMT  
		Size: 52.2 MB (52186611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80869518eed6425bb6d52d653b7eafa53284cb556b9cc2d90b6ed8cd003dc773`  
		Last Modified: Tue, 13 Jun 2023 04:04:20 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c58c4494b65a294c8086500f80de0b3f1f88777384b4a0bf59f39d1374bb32`  
		Last Modified: Tue, 13 Jun 2023 04:04:20 GMT  
		Size: 999.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0453ee6f28c2aca08755a0990b9e7e89af4760c203915d0701b6e041498a0b1`  
		Last Modified: Tue, 13 Jun 2023 04:04:20 GMT  
		Size: 2.2 KB (2226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e1a0063344ada8ed441664af0f10f3f8e507014eeeeb1f145a78b67931ec74`  
		Last Modified: Tue, 13 Jun 2023 04:04:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:960305e9b35826163f173e8b89eab4112410bee3725c3f0773140932dd9f7877
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.2 MB (85205205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:352add31bc606968e9b4695dc003a06de6c7ca3682ea0d3145b972feb8dabfee`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:33:39 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 12 Apr 2023 01:33:39 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 12 Apr 2023 01:33:45 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:33:48 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 12 Apr 2023 01:33:48 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 12 Apr 2023 01:33:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:34:12 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Wed, 12 Apr 2023 01:34:12 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 12 Apr 2023 01:34:24 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 12 Apr 2023 01:34:24 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 12 Apr 2023 01:34:24 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 12 Apr 2023 01:34:24 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 12 Apr 2023 01:34:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 12 Apr 2023 01:34:25 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 01:34:25 GMT
VOLUME [/opt/couchdb/data]
# Wed, 12 Apr 2023 01:34:25 GMT
EXPOSE 4369 5984 9100
# Wed, 12 Apr 2023 01:34:25 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f522824805b9b3818de882a514dd5454399e3c21b512a09e64274bf12d18ab4`  
		Last Modified: Wed, 12 Apr 2023 01:35:29 GMT  
		Size: 3.4 KB (3434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdfaf598c101b0427a73a7b5a1edb3b6229985b64794e6d215eb049125bbd25`  
		Last Modified: Wed, 12 Apr 2023 01:35:27 GMT  
		Size: 5.2 MB (5209561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc33796685833f0fdacecb6c4f2078915729822d8fb7a21aada1b767c48b377`  
		Last Modified: Wed, 12 Apr 2023 01:35:27 GMT  
		Size: 566.3 KB (566295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356323e70f7127294f4bee19c211582a4af79acc6d1f696d70fc94229c84aa52`  
		Last Modified: Wed, 12 Apr 2023 01:35:27 GMT  
		Size: 294.3 KB (294328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9652526d42f149093060de62ac3b39905fb0bfb8457d6148e4314ef71058a153`  
		Last Modified: Wed, 12 Apr 2023 01:35:44 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d95be693dac094ea4fe70ff2bd1f44b66a9ede007474a31cafcb829c361429`  
		Last Modified: Wed, 12 Apr 2023 01:35:47 GMT  
		Size: 49.1 MB (49063995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61eb7f6826c8440901fb275f2b3c5f6be3e97d95482db6770215d5bd31899ed1`  
		Last Modified: Wed, 12 Apr 2023 01:35:42 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d81fa00cdd93053287b1afda2f3cfda4475c6ac6307dc22125a76f843f21415`  
		Last Modified: Wed, 12 Apr 2023 01:35:43 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16e726b19dd008ea8df7bf3ce90fa1947f685d2f6fdd3caa36e1f3b6e40526d0`  
		Last Modified: Wed, 12 Apr 2023 01:35:43 GMT  
		Size: 2.2 KB (2227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c78146fce98da16e884fde6d22f444849c69c3da90555e336827ceb2b6a039`  
		Last Modified: Wed, 12 Apr 2023 01:35:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; ppc64le

```console
$ docker pull couchdb@sha256:90a95123b16f3f08c9e3b862a7e628ead429c8602d5dc110db1b038b5b47db9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.4 MB (92383985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7c0714b286e5789d8b829c846536d1f8a5308d8cf419fa60995af8b91ab3b55`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 12 Apr 2023 00:08:20 GMT
ADD file:63eb52aaff02c15bceabb87a78eb1b36389066ff4774cf8a754160ca7d509816 in / 
# Wed, 12 Apr 2023 00:08:23 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:23:31 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 12 Apr 2023 01:23:35 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 12 Apr 2023 01:23:57 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:24:07 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 12 Apr 2023 01:24:08 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 12 Apr 2023 01:24:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:25:25 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Wed, 12 Apr 2023 01:25:27 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 12 Apr 2023 01:25:58 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 12 Apr 2023 01:26:02 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 12 Apr 2023 01:26:02 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 12 Apr 2023 01:26:03 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 12 Apr 2023 01:26:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 12 Apr 2023 01:26:05 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 01:26:06 GMT
VOLUME [/opt/couchdb/data]
# Wed, 12 Apr 2023 01:26:06 GMT
EXPOSE 4369 5984 9100
# Wed, 12 Apr 2023 01:26:07 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:5b41d5ec640939cf684959234ad3b80909268a32bfd520a31c6720a91521c2fa`  
		Last Modified: Wed, 12 Apr 2023 00:13:13 GMT  
		Size: 35.3 MB (35291995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7569dcea363c11bb071b416ea27193dbe62d8a210fa1f829efabb35b46600dae`  
		Last Modified: Wed, 12 Apr 2023 01:26:25 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a685c575c0e899abc0410edf84715dd5cf4184fcbd447fdbbcac069795eadd05`  
		Last Modified: Wed, 12 Apr 2023 01:26:26 GMT  
		Size: 6.0 MB (6044117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0283a2882808914c7a35f392d4ad2d2921ccf8b8855ab399e2998c22d061f16e`  
		Last Modified: Wed, 12 Apr 2023 01:26:24 GMT  
		Size: 662.1 KB (662116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17deb4c48f5c43beee592bed99d27502afe8c8f60cde1cb4bebb7dce00e877c`  
		Last Modified: Wed, 12 Apr 2023 01:26:24 GMT  
		Size: 294.3 KB (294319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7661a9384c6767a073bc8e86df2ec2c60bef8bad55fac7ab22d7ecffcdb1f1`  
		Last Modified: Wed, 12 Apr 2023 01:26:48 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74733b44093de42db86284861068e909838a6bca4f3ecf0bfd04eb99d5bf8c79`  
		Last Modified: Wed, 12 Apr 2023 01:26:56 GMT  
		Size: 50.1 MB (50084252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c567dbfb6ac3167b1cd2d6532940fd6fb66d9b5b6a1dedf22d61b92a7b4095eb`  
		Last Modified: Wed, 12 Apr 2023 01:26:46 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf08299e06354b4674e5fabd7e99da65832d26bc98826c051d261e7a03195099`  
		Last Modified: Wed, 12 Apr 2023 01:26:46 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5861e0f3152c23eda58111aaac02f82ed4973711f9a55c51cb55ebb9af6220`  
		Last Modified: Wed, 12 Apr 2023 01:26:46 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54774512e47b4b9a6dee9f79bf7ec483b3c7c234e949bc4f6c96fb22a3e8237`  
		Last Modified: Wed, 12 Apr 2023 01:26:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2.3`

```console
$ docker pull couchdb@sha256:f230dbb6694e33b90b1c48782b20b1d71f7fb42c7b2099818d9c39782e60d380
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchdb:3.2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:22fdd25d4eef5d0385853f6079463a23ca52bfcbd8d0dc7092dbd9797adf897d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.7 MB (89740540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a70f12d6bc5aa3e6c706277ff2c517d3bfcd6bc7dcdff28e99c7318d0c5f318`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:01:57 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Jun 2023 04:01:58 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Jun 2023 04:02:05 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:02:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 13 Jun 2023 04:02:09 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Jun 2023 04:02:13 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:02:32 GMT
ENV COUCHDB_VERSION=3.2.3
# Tue, 13 Jun 2023 04:02:32 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Jun 2023 04:02:44 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Jun 2023 04:02:45 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Jun 2023 04:02:45 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 13 Jun 2023 04:02:45 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 13 Jun 2023 04:02:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 04:02:46 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:02:46 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Jun 2023 04:02:46 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Jun 2023 04:02:46 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56fa5a08f48785d08765b7746d507926063e6ab14084ec52c45ad658c9900e2`  
		Last Modified: Tue, 13 Jun 2023 04:04:05 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:effeea359db8a5b5241e47adb1070cec93345c3cc2011db12b74a56d6cec9151`  
		Last Modified: Tue, 13 Jun 2023 04:04:04 GMT  
		Size: 5.2 MB (5224468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b83a1bd5e8dd69f1172af3053ab31900973778718afe1abb82dd6d9cf4075a`  
		Last Modified: Tue, 13 Jun 2023 04:04:03 GMT  
		Size: 610.3 KB (610265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d5ee803171a181293d9529fab444ccda628ce617e53d52acb7bbd34e1dbe3f`  
		Last Modified: Tue, 13 Jun 2023 04:04:03 GMT  
		Size: 294.4 KB (294377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7bcd34bc103365c025d56bb91321fb3f909de9d2d8a3f86e2e42840dd5c967`  
		Last Modified: Tue, 13 Jun 2023 04:04:21 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c75aaa8226bcf8bd5abde0889b8926be9f496fb20715116927c48c9805a805`  
		Last Modified: Tue, 13 Jun 2023 04:04:25 GMT  
		Size: 52.2 MB (52186611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80869518eed6425bb6d52d653b7eafa53284cb556b9cc2d90b6ed8cd003dc773`  
		Last Modified: Tue, 13 Jun 2023 04:04:20 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c58c4494b65a294c8086500f80de0b3f1f88777384b4a0bf59f39d1374bb32`  
		Last Modified: Tue, 13 Jun 2023 04:04:20 GMT  
		Size: 999.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0453ee6f28c2aca08755a0990b9e7e89af4760c203915d0701b6e041498a0b1`  
		Last Modified: Tue, 13 Jun 2023 04:04:20 GMT  
		Size: 2.2 KB (2226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e1a0063344ada8ed441664af0f10f3f8e507014eeeeb1f145a78b67931ec74`  
		Last Modified: Tue, 13 Jun 2023 04:04:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.3`

```console
$ docker pull couchdb@sha256:b889ec0dba71a167320a6e90a9198ee13d382bbfc9c3913f405a2f6a7dedc44f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `couchdb:3.3` - linux; amd64

```console
$ docker pull couchdb@sha256:40016f83b61df0ac945f1536e3a52e6ea2761a18326933513bbe358e5f787102
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90239977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b725f6b2513a8b4ec7c8b706aed6ac7a7166a5c833b1a23dd2f559310808110`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:01:57 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Jun 2023 04:01:58 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Jun 2023 04:02:05 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:02:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 13 Jun 2023 04:02:09 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Jun 2023 04:02:13 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:02:14 GMT
ENV COUCHDB_VERSION=3.3.2
# Tue, 13 Jun 2023 04:02:14 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Jun 2023 04:02:27 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Jun 2023 04:02:27 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Jun 2023 04:02:27 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 13 Jun 2023 04:02:27 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 13 Jun 2023 04:02:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 04:02:28 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:02:28 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Jun 2023 04:02:28 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Jun 2023 04:02:28 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56fa5a08f48785d08765b7746d507926063e6ab14084ec52c45ad658c9900e2`  
		Last Modified: Tue, 13 Jun 2023 04:04:05 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:effeea359db8a5b5241e47adb1070cec93345c3cc2011db12b74a56d6cec9151`  
		Last Modified: Tue, 13 Jun 2023 04:04:04 GMT  
		Size: 5.2 MB (5224468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b83a1bd5e8dd69f1172af3053ab31900973778718afe1abb82dd6d9cf4075a`  
		Last Modified: Tue, 13 Jun 2023 04:04:03 GMT  
		Size: 610.3 KB (610265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d5ee803171a181293d9529fab444ccda628ce617e53d52acb7bbd34e1dbe3f`  
		Last Modified: Tue, 13 Jun 2023 04:04:03 GMT  
		Size: 294.4 KB (294377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abff9bf83b2eee5ea095f234f197ed3bdc13ba5c1d9d27e366d814ca232560d3`  
		Last Modified: Tue, 13 Jun 2023 04:04:03 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1c0289451f671b5a57844126e484dc7f940b217bdd9badb059bda68d8764ab`  
		Last Modified: Tue, 13 Jun 2023 04:04:07 GMT  
		Size: 52.7 MB (52686042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f7f7afef66f9db1812bc4358426b2221d5126baecd2715d01530d1fa9ea2e86`  
		Last Modified: Tue, 13 Jun 2023 04:04:01 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d22413df733620c7d50f6db00f44e8dd5cd48ae5343fcbb767b482c4f0f9ad`  
		Last Modified: Tue, 13 Jun 2023 04:04:01 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7983d64b4de2667bb5662734e159cb3529658b676c0c32a3e5906a4a26d27ce3`  
		Last Modified: Tue, 13 Jun 2023 04:04:01 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf22f027705f7c7b494a7c2f2bd1d7b88f54297a0cd015536fdf35b915ace46`  
		Last Modified: Tue, 13 Jun 2023 04:04:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:141772490f9958ea64a517669cb9f3284f540ab4ec5486e2e685f63f0d080f51
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88684701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5caf00b8d2804b512825d7ae87ef5c0320c191a123d13c11a57b1e2e079bd70d`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:11:13 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Jun 2023 03:11:13 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Jun 2023 03:11:20 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:11:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 13 Jun 2023 03:11:23 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Jun 2023 03:11:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:11:27 GMT
ENV COUCHDB_VERSION=3.3.2
# Tue, 13 Jun 2023 03:11:28 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Jun 2023 03:11:39 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Jun 2023 03:11:40 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Jun 2023 03:11:40 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 13 Jun 2023 03:11:40 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 13 Jun 2023 03:11:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 03:11:40 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 03:11:40 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Jun 2023 03:11:40 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Jun 2023 03:11:40 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e233a96952e1934fa67393b0643bae29d210a5989e09f4b7f420b079982c96c4`  
		Last Modified: Tue, 13 Jun 2023 03:12:58 GMT  
		Size: 3.4 KB (3425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c60a62bf69974ac716a93c155b419669eaac5acbbcc214c6c211667ab267c9`  
		Last Modified: Tue, 13 Jun 2023 03:12:57 GMT  
		Size: 5.2 MB (5209604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750b53c5b967617f8b2ff9cb0ecc88700772caab48f3b4f59f6d1e9a844e427a`  
		Last Modified: Tue, 13 Jun 2023 03:12:56 GMT  
		Size: 566.3 KB (566262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c843fecc8eafd5a7c37f7c3329458c4bb1cc58d6836fee8d9e8acff6f9b38c0`  
		Last Modified: Tue, 13 Jun 2023 03:12:56 GMT  
		Size: 294.3 KB (294347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c90431247a4ed342f9d684e9b04bb9bfc5dda7118d4267e7b3f23bd59ad4fd`  
		Last Modified: Tue, 13 Jun 2023 03:12:56 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f35924c1a48bb2edaa217e033e1fbee469d6e11c805e338939f681aaefbf34`  
		Last Modified: Tue, 13 Jun 2023 03:12:59 GMT  
		Size: 52.5 MB (52544231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471f7004fd790c6758674730bf2f9bd8fdabf72eca171b74caa8ef1744fece7e`  
		Last Modified: Tue, 13 Jun 2023 03:12:54 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d386b3f9b6664b042d1774b40dff2342b3c02d82cade1337f63021606bd299e6`  
		Last Modified: Tue, 13 Jun 2023 03:12:54 GMT  
		Size: 998.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b370d69da1a2a4adc59447af4f255ae1ec356c733e4b73d3b96b7761810229dc`  
		Last Modified: Tue, 13 Jun 2023 03:12:54 GMT  
		Size: 2.2 KB (2227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77933cca358498c1f5feb64dd9ed2c965d85c8d49fdb7db2e72e68bd245712f3`  
		Last Modified: Tue, 13 Jun 2023 03:12:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3` - linux; ppc64le

```console
$ docker pull couchdb@sha256:c399e90a9b1b305e1b72125a4905ae3c51db4be6dff26c4a78bc27e759035a00
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.0 MB (95961503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ca27ec01131c11c250078f1488ed292338f0ceeefadde47ac20108c3e7e4b4b`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Mon, 12 Jun 2023 23:18:20 GMT
ADD file:b17eabe509462fa1a2e4c5421e877e3e4149085e3da07a421a66c7b06566c457 in / 
# Mon, 12 Jun 2023 23:18:22 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 09:45:19 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Jun 2023 09:45:20 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Jun 2023 09:45:36 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 09:45:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 13 Jun 2023 09:45:44 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Jun 2023 09:45:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 09:45:56 GMT
ENV COUCHDB_VERSION=3.3.2
# Tue, 13 Jun 2023 09:45:57 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Jun 2023 09:46:20 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Jun 2023 09:46:22 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Jun 2023 09:46:22 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 13 Jun 2023 09:46:23 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 13 Jun 2023 09:46:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 09:46:24 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 09:46:24 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Jun 2023 09:46:25 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Jun 2023 09:46:25 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:2973ac0be4a80a6cecbb73370e92810a6f67a98e12e61b3044aa63a322dab03a`  
		Last Modified: Mon, 12 Jun 2023 23:25:03 GMT  
		Size: 35.3 MB (35290790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7a4c14920d3766677c031be9ca45255dc9e4840b301c89d08bbab6c0c829b8`  
		Last Modified: Tue, 13 Jun 2023 09:47:05 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ee15726d36a785865415f386f34e9c4214a817d6dc79aec252811407ced685`  
		Last Modified: Tue, 13 Jun 2023 09:47:05 GMT  
		Size: 6.0 MB (6044040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a5cfeef71b924481f431fd94af56f33ccc02f4fcd0ce1b39afedb3168bd228a`  
		Last Modified: Tue, 13 Jun 2023 09:47:03 GMT  
		Size: 662.1 KB (662089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:799b3ab5e90729432923cecf21aad2ed782c84206d9d207078011186642aad90`  
		Last Modified: Tue, 13 Jun 2023 09:47:03 GMT  
		Size: 294.3 KB (294296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd6815c4999f2fa98c8cf4608b23fa063cf5a774c83160b584f54643a784eb0`  
		Last Modified: Tue, 13 Jun 2023 09:47:03 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea7c054364d04ef4b21f2a283c8ab5a0d200b3dfc983a9d4efd4c9b00c744a5c`  
		Last Modified: Tue, 13 Jun 2023 09:47:11 GMT  
		Size: 53.7 MB (53662870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76fc449be4ce6b84b9700f3c78608d408a725c28dc094af606d988eb350474da`  
		Last Modified: Tue, 13 Jun 2023 09:47:01 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064cc07cec794834bfcdae6cc7830104662247eeb39c275d846db362bc91301d`  
		Last Modified: Tue, 13 Jun 2023 09:47:01 GMT  
		Size: 999.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:214dfd321091da26c6f756ee7d21328d6e12653fd1acb75f40dfaf0063174b67`  
		Last Modified: Tue, 13 Jun 2023 09:47:01 GMT  
		Size: 2.2 KB (2228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03afeadee0940c842a4ed2c86ddb83b2a9fce341219595a1b84ffb0c299fe48f`  
		Last Modified: Tue, 13 Jun 2023 09:47:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3` - linux; s390x

```console
$ docker pull couchdb@sha256:27f57b5ffc3a8799873fd57224eb642f883f404866610dbabd7710e700fa7d55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.0 MB (86982637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9c3afe9604f8597d2587042e19236a4a9af934cb69c067b9eb73e86501d11aa`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 23 May 2023 00:42:52 GMT
ADD file:23b1e12559302529556a94a1d4098dbdb454e263265258b940c2b2d23a97c121 in / 
# Tue, 23 May 2023 00:42:54 GMT
CMD ["bash"]
# Wed, 31 May 2023 23:41:40 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 31 May 2023 23:41:41 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 31 May 2023 23:41:47 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 31 May 2023 23:41:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 31 May 2023 23:41:50 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 31 May 2023 23:41:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 31 May 2023 23:41:55 GMT
ENV COUCHDB_VERSION=3.3.2
# Wed, 31 May 2023 23:41:55 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 31 May 2023 23:42:11 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 31 May 2023 23:42:12 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 31 May 2023 23:42:12 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 31 May 2023 23:42:13 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 31 May 2023 23:42:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 31 May 2023 23:42:13 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 31 May 2023 23:42:13 GMT
VOLUME [/opt/couchdb/data]
# Wed, 31 May 2023 23:42:13 GMT
EXPOSE 4369 5984 9100
# Wed, 31 May 2023 23:42:13 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:9c24ec455bdb6a9ad0d033c7cce8e71dd5bdbbe53a86d5feeb8d4cb7804fb8e5`  
		Last Modified: Tue, 23 May 2023 00:45:47 GMT  
		Size: 29.6 MB (29642170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79369d7477079fd194a68b466dff2d8edc280d261dc304b2567bfb55973c870b`  
		Last Modified: Wed, 31 May 2023 23:42:31 GMT  
		Size: 3.4 KB (3433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bea484bba066eb8863a66dcecc668d69aec750f8d1c0ad9325cc89b8210d148`  
		Last Modified: Wed, 31 May 2023 23:42:30 GMT  
		Size: 5.1 MB (5110473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5297b03b741ba1714084f21808e891def15cc57d292f901233aa010d56eda78e`  
		Last Modified: Wed, 31 May 2023 23:42:30 GMT  
		Size: 573.0 KB (573029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c1c59cdce3bf8d5680cb008d32bc45637f344c162a7912c90d5bbb3d0c753d`  
		Last Modified: Wed, 31 May 2023 23:42:30 GMT  
		Size: 294.5 KB (294451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89faeb4398086a27f7d1c2cfd535d3d86db34051276853757976607b8e6697e6`  
		Last Modified: Wed, 31 May 2023 23:42:30 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d08b9ecfe40b07d3aac1d314249e9c5843ce52edc2bea23828d62981849ff18`  
		Last Modified: Wed, 31 May 2023 23:42:34 GMT  
		Size: 51.4 MB (51355073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a8e6b453b90234fdb6dd9135a15beae0f3ba97050c5bd98264e1564f32386f`  
		Last Modified: Wed, 31 May 2023 23:42:28 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce5dd09ac3c1e930fd074767a97609f55cca10e5f1c213a684236bf7d4852b0`  
		Last Modified: Wed, 31 May 2023 23:42:28 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c7c51f86fe82775ec0e610e7ee7e3bf2e4ec64fe2d2a9ac042c388b5a61810`  
		Last Modified: Wed, 31 May 2023 23:42:28 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36cb0e3d58be45185e1df3bd73ef5f6906dad6517350c73fab6653744a44d7c`  
		Last Modified: Wed, 31 May 2023 23:42:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.3.2`

```console
$ docker pull couchdb@sha256:b889ec0dba71a167320a6e90a9198ee13d382bbfc9c3913f405a2f6a7dedc44f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `couchdb:3.3.2` - linux; amd64

```console
$ docker pull couchdb@sha256:40016f83b61df0ac945f1536e3a52e6ea2761a18326933513bbe358e5f787102
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90239977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b725f6b2513a8b4ec7c8b706aed6ac7a7166a5c833b1a23dd2f559310808110`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:01:57 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Jun 2023 04:01:58 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Jun 2023 04:02:05 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:02:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 13 Jun 2023 04:02:09 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Jun 2023 04:02:13 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:02:14 GMT
ENV COUCHDB_VERSION=3.3.2
# Tue, 13 Jun 2023 04:02:14 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Jun 2023 04:02:27 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Jun 2023 04:02:27 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Jun 2023 04:02:27 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 13 Jun 2023 04:02:27 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 13 Jun 2023 04:02:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 04:02:28 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:02:28 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Jun 2023 04:02:28 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Jun 2023 04:02:28 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56fa5a08f48785d08765b7746d507926063e6ab14084ec52c45ad658c9900e2`  
		Last Modified: Tue, 13 Jun 2023 04:04:05 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:effeea359db8a5b5241e47adb1070cec93345c3cc2011db12b74a56d6cec9151`  
		Last Modified: Tue, 13 Jun 2023 04:04:04 GMT  
		Size: 5.2 MB (5224468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b83a1bd5e8dd69f1172af3053ab31900973778718afe1abb82dd6d9cf4075a`  
		Last Modified: Tue, 13 Jun 2023 04:04:03 GMT  
		Size: 610.3 KB (610265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d5ee803171a181293d9529fab444ccda628ce617e53d52acb7bbd34e1dbe3f`  
		Last Modified: Tue, 13 Jun 2023 04:04:03 GMT  
		Size: 294.4 KB (294377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abff9bf83b2eee5ea095f234f197ed3bdc13ba5c1d9d27e366d814ca232560d3`  
		Last Modified: Tue, 13 Jun 2023 04:04:03 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1c0289451f671b5a57844126e484dc7f940b217bdd9badb059bda68d8764ab`  
		Last Modified: Tue, 13 Jun 2023 04:04:07 GMT  
		Size: 52.7 MB (52686042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f7f7afef66f9db1812bc4358426b2221d5126baecd2715d01530d1fa9ea2e86`  
		Last Modified: Tue, 13 Jun 2023 04:04:01 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d22413df733620c7d50f6db00f44e8dd5cd48ae5343fcbb767b482c4f0f9ad`  
		Last Modified: Tue, 13 Jun 2023 04:04:01 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7983d64b4de2667bb5662734e159cb3529658b676c0c32a3e5906a4a26d27ce3`  
		Last Modified: Tue, 13 Jun 2023 04:04:01 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf22f027705f7c7b494a7c2f2bd1d7b88f54297a0cd015536fdf35b915ace46`  
		Last Modified: Tue, 13 Jun 2023 04:04:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:141772490f9958ea64a517669cb9f3284f540ab4ec5486e2e685f63f0d080f51
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88684701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5caf00b8d2804b512825d7ae87ef5c0320c191a123d13c11a57b1e2e079bd70d`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:11:13 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Jun 2023 03:11:13 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Jun 2023 03:11:20 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:11:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 13 Jun 2023 03:11:23 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Jun 2023 03:11:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:11:27 GMT
ENV COUCHDB_VERSION=3.3.2
# Tue, 13 Jun 2023 03:11:28 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Jun 2023 03:11:39 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Jun 2023 03:11:40 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Jun 2023 03:11:40 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 13 Jun 2023 03:11:40 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 13 Jun 2023 03:11:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 03:11:40 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 03:11:40 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Jun 2023 03:11:40 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Jun 2023 03:11:40 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e233a96952e1934fa67393b0643bae29d210a5989e09f4b7f420b079982c96c4`  
		Last Modified: Tue, 13 Jun 2023 03:12:58 GMT  
		Size: 3.4 KB (3425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c60a62bf69974ac716a93c155b419669eaac5acbbcc214c6c211667ab267c9`  
		Last Modified: Tue, 13 Jun 2023 03:12:57 GMT  
		Size: 5.2 MB (5209604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750b53c5b967617f8b2ff9cb0ecc88700772caab48f3b4f59f6d1e9a844e427a`  
		Last Modified: Tue, 13 Jun 2023 03:12:56 GMT  
		Size: 566.3 KB (566262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c843fecc8eafd5a7c37f7c3329458c4bb1cc58d6836fee8d9e8acff6f9b38c0`  
		Last Modified: Tue, 13 Jun 2023 03:12:56 GMT  
		Size: 294.3 KB (294347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c90431247a4ed342f9d684e9b04bb9bfc5dda7118d4267e7b3f23bd59ad4fd`  
		Last Modified: Tue, 13 Jun 2023 03:12:56 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f35924c1a48bb2edaa217e033e1fbee469d6e11c805e338939f681aaefbf34`  
		Last Modified: Tue, 13 Jun 2023 03:12:59 GMT  
		Size: 52.5 MB (52544231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471f7004fd790c6758674730bf2f9bd8fdabf72eca171b74caa8ef1744fece7e`  
		Last Modified: Tue, 13 Jun 2023 03:12:54 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d386b3f9b6664b042d1774b40dff2342b3c02d82cade1337f63021606bd299e6`  
		Last Modified: Tue, 13 Jun 2023 03:12:54 GMT  
		Size: 998.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b370d69da1a2a4adc59447af4f255ae1ec356c733e4b73d3b96b7761810229dc`  
		Last Modified: Tue, 13 Jun 2023 03:12:54 GMT  
		Size: 2.2 KB (2227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77933cca358498c1f5feb64dd9ed2c965d85c8d49fdb7db2e72e68bd245712f3`  
		Last Modified: Tue, 13 Jun 2023 03:12:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3.2` - linux; ppc64le

```console
$ docker pull couchdb@sha256:c399e90a9b1b305e1b72125a4905ae3c51db4be6dff26c4a78bc27e759035a00
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.0 MB (95961503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ca27ec01131c11c250078f1488ed292338f0ceeefadde47ac20108c3e7e4b4b`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Mon, 12 Jun 2023 23:18:20 GMT
ADD file:b17eabe509462fa1a2e4c5421e877e3e4149085e3da07a421a66c7b06566c457 in / 
# Mon, 12 Jun 2023 23:18:22 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 09:45:19 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Jun 2023 09:45:20 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Jun 2023 09:45:36 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 09:45:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 13 Jun 2023 09:45:44 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Jun 2023 09:45:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 09:45:56 GMT
ENV COUCHDB_VERSION=3.3.2
# Tue, 13 Jun 2023 09:45:57 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Jun 2023 09:46:20 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Jun 2023 09:46:22 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Jun 2023 09:46:22 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 13 Jun 2023 09:46:23 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 13 Jun 2023 09:46:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 09:46:24 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 09:46:24 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Jun 2023 09:46:25 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Jun 2023 09:46:25 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:2973ac0be4a80a6cecbb73370e92810a6f67a98e12e61b3044aa63a322dab03a`  
		Last Modified: Mon, 12 Jun 2023 23:25:03 GMT  
		Size: 35.3 MB (35290790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7a4c14920d3766677c031be9ca45255dc9e4840b301c89d08bbab6c0c829b8`  
		Last Modified: Tue, 13 Jun 2023 09:47:05 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ee15726d36a785865415f386f34e9c4214a817d6dc79aec252811407ced685`  
		Last Modified: Tue, 13 Jun 2023 09:47:05 GMT  
		Size: 6.0 MB (6044040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a5cfeef71b924481f431fd94af56f33ccc02f4fcd0ce1b39afedb3168bd228a`  
		Last Modified: Tue, 13 Jun 2023 09:47:03 GMT  
		Size: 662.1 KB (662089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:799b3ab5e90729432923cecf21aad2ed782c84206d9d207078011186642aad90`  
		Last Modified: Tue, 13 Jun 2023 09:47:03 GMT  
		Size: 294.3 KB (294296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd6815c4999f2fa98c8cf4608b23fa063cf5a774c83160b584f54643a784eb0`  
		Last Modified: Tue, 13 Jun 2023 09:47:03 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea7c054364d04ef4b21f2a283c8ab5a0d200b3dfc983a9d4efd4c9b00c744a5c`  
		Last Modified: Tue, 13 Jun 2023 09:47:11 GMT  
		Size: 53.7 MB (53662870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76fc449be4ce6b84b9700f3c78608d408a725c28dc094af606d988eb350474da`  
		Last Modified: Tue, 13 Jun 2023 09:47:01 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064cc07cec794834bfcdae6cc7830104662247eeb39c275d846db362bc91301d`  
		Last Modified: Tue, 13 Jun 2023 09:47:01 GMT  
		Size: 999.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:214dfd321091da26c6f756ee7d21328d6e12653fd1acb75f40dfaf0063174b67`  
		Last Modified: Tue, 13 Jun 2023 09:47:01 GMT  
		Size: 2.2 KB (2228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03afeadee0940c842a4ed2c86ddb83b2a9fce341219595a1b84ffb0c299fe48f`  
		Last Modified: Tue, 13 Jun 2023 09:47:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3.2` - linux; s390x

```console
$ docker pull couchdb@sha256:27f57b5ffc3a8799873fd57224eb642f883f404866610dbabd7710e700fa7d55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.0 MB (86982637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9c3afe9604f8597d2587042e19236a4a9af934cb69c067b9eb73e86501d11aa`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 23 May 2023 00:42:52 GMT
ADD file:23b1e12559302529556a94a1d4098dbdb454e263265258b940c2b2d23a97c121 in / 
# Tue, 23 May 2023 00:42:54 GMT
CMD ["bash"]
# Wed, 31 May 2023 23:41:40 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 31 May 2023 23:41:41 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 31 May 2023 23:41:47 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 31 May 2023 23:41:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 31 May 2023 23:41:50 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 31 May 2023 23:41:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 31 May 2023 23:41:55 GMT
ENV COUCHDB_VERSION=3.3.2
# Wed, 31 May 2023 23:41:55 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 31 May 2023 23:42:11 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 31 May 2023 23:42:12 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 31 May 2023 23:42:12 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 31 May 2023 23:42:13 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 31 May 2023 23:42:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 31 May 2023 23:42:13 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 31 May 2023 23:42:13 GMT
VOLUME [/opt/couchdb/data]
# Wed, 31 May 2023 23:42:13 GMT
EXPOSE 4369 5984 9100
# Wed, 31 May 2023 23:42:13 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:9c24ec455bdb6a9ad0d033c7cce8e71dd5bdbbe53a86d5feeb8d4cb7804fb8e5`  
		Last Modified: Tue, 23 May 2023 00:45:47 GMT  
		Size: 29.6 MB (29642170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79369d7477079fd194a68b466dff2d8edc280d261dc304b2567bfb55973c870b`  
		Last Modified: Wed, 31 May 2023 23:42:31 GMT  
		Size: 3.4 KB (3433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bea484bba066eb8863a66dcecc668d69aec750f8d1c0ad9325cc89b8210d148`  
		Last Modified: Wed, 31 May 2023 23:42:30 GMT  
		Size: 5.1 MB (5110473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5297b03b741ba1714084f21808e891def15cc57d292f901233aa010d56eda78e`  
		Last Modified: Wed, 31 May 2023 23:42:30 GMT  
		Size: 573.0 KB (573029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c1c59cdce3bf8d5680cb008d32bc45637f344c162a7912c90d5bbb3d0c753d`  
		Last Modified: Wed, 31 May 2023 23:42:30 GMT  
		Size: 294.5 KB (294451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89faeb4398086a27f7d1c2cfd535d3d86db34051276853757976607b8e6697e6`  
		Last Modified: Wed, 31 May 2023 23:42:30 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d08b9ecfe40b07d3aac1d314249e9c5843ce52edc2bea23828d62981849ff18`  
		Last Modified: Wed, 31 May 2023 23:42:34 GMT  
		Size: 51.4 MB (51355073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a8e6b453b90234fdb6dd9135a15beae0f3ba97050c5bd98264e1564f32386f`  
		Last Modified: Wed, 31 May 2023 23:42:28 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce5dd09ac3c1e930fd074767a97609f55cca10e5f1c213a684236bf7d4852b0`  
		Last Modified: Wed, 31 May 2023 23:42:28 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c7c51f86fe82775ec0e610e7ee7e3bf2e4ec64fe2d2a9ac042c388b5a61810`  
		Last Modified: Wed, 31 May 2023 23:42:28 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36cb0e3d58be45185e1df3bd73ef5f6906dad6517350c73fab6653744a44d7c`  
		Last Modified: Wed, 31 May 2023 23:42:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:latest`

```console
$ docker pull couchdb@sha256:b889ec0dba71a167320a6e90a9198ee13d382bbfc9c3913f405a2f6a7dedc44f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:40016f83b61df0ac945f1536e3a52e6ea2761a18326933513bbe358e5f787102
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90239977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b725f6b2513a8b4ec7c8b706aed6ac7a7166a5c833b1a23dd2f559310808110`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:07 GMT
ADD file:5ab44909c2983e19ab6596e7e4ee9ad80e48afeb9dfe0e7224afdae7cafd25ef in / 
# Mon, 12 Jun 2023 23:21:08 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:01:57 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Jun 2023 04:01:58 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Jun 2023 04:02:05 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:02:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 13 Jun 2023 04:02:09 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Jun 2023 04:02:13 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 04:02:14 GMT
ENV COUCHDB_VERSION=3.3.2
# Tue, 13 Jun 2023 04:02:14 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Jun 2023 04:02:27 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Jun 2023 04:02:27 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Jun 2023 04:02:27 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 13 Jun 2023 04:02:27 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 13 Jun 2023 04:02:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 04:02:28 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 04:02:28 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Jun 2023 04:02:28 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Jun 2023 04:02:28 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:759700526b7894aa9c150feb2ebfcd00cf06d2890df739e71555edcfd13669e3`  
		Last Modified: Mon, 12 Jun 2023 23:26:30 GMT  
		Size: 31.4 MB (31417410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56fa5a08f48785d08765b7746d507926063e6ab14084ec52c45ad658c9900e2`  
		Last Modified: Tue, 13 Jun 2023 04:04:05 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:effeea359db8a5b5241e47adb1070cec93345c3cc2011db12b74a56d6cec9151`  
		Last Modified: Tue, 13 Jun 2023 04:04:04 GMT  
		Size: 5.2 MB (5224468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b83a1bd5e8dd69f1172af3053ab31900973778718afe1abb82dd6d9cf4075a`  
		Last Modified: Tue, 13 Jun 2023 04:04:03 GMT  
		Size: 610.3 KB (610265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d5ee803171a181293d9529fab444ccda628ce617e53d52acb7bbd34e1dbe3f`  
		Last Modified: Tue, 13 Jun 2023 04:04:03 GMT  
		Size: 294.4 KB (294377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abff9bf83b2eee5ea095f234f197ed3bdc13ba5c1d9d27e366d814ca232560d3`  
		Last Modified: Tue, 13 Jun 2023 04:04:03 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1c0289451f671b5a57844126e484dc7f940b217bdd9badb059bda68d8764ab`  
		Last Modified: Tue, 13 Jun 2023 04:04:07 GMT  
		Size: 52.7 MB (52686042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f7f7afef66f9db1812bc4358426b2221d5126baecd2715d01530d1fa9ea2e86`  
		Last Modified: Tue, 13 Jun 2023 04:04:01 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d22413df733620c7d50f6db00f44e8dd5cd48ae5343fcbb767b482c4f0f9ad`  
		Last Modified: Tue, 13 Jun 2023 04:04:01 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7983d64b4de2667bb5662734e159cb3529658b676c0c32a3e5906a4a26d27ce3`  
		Last Modified: Tue, 13 Jun 2023 04:04:01 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cf22f027705f7c7b494a7c2f2bd1d7b88f54297a0cd015536fdf35b915ace46`  
		Last Modified: Tue, 13 Jun 2023 04:04:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:141772490f9958ea64a517669cb9f3284f540ab4ec5486e2e685f63f0d080f51
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88684701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5caf00b8d2804b512825d7ae87ef5c0320c191a123d13c11a57b1e2e079bd70d`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:33 GMT
ADD file:10af42ddb9f028c5418d370fe2b841aa61e81f37de1ffe76900a783ba3926646 in / 
# Mon, 12 Jun 2023 23:40:33 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:11:13 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Jun 2023 03:11:13 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Jun 2023 03:11:20 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:11:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 13 Jun 2023 03:11:23 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Jun 2023 03:11:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:11:27 GMT
ENV COUCHDB_VERSION=3.3.2
# Tue, 13 Jun 2023 03:11:28 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Jun 2023 03:11:39 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Jun 2023 03:11:40 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Jun 2023 03:11:40 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 13 Jun 2023 03:11:40 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 13 Jun 2023 03:11:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 03:11:40 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 03:11:40 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Jun 2023 03:11:40 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Jun 2023 03:11:40 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:92ad4775570054c645678402c8b75eb489b8e05313c9ccd7867bb591266db4d8`  
		Last Modified: Mon, 12 Jun 2023 23:44:45 GMT  
		Size: 30.1 MB (30062834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e233a96952e1934fa67393b0643bae29d210a5989e09f4b7f420b079982c96c4`  
		Last Modified: Tue, 13 Jun 2023 03:12:58 GMT  
		Size: 3.4 KB (3425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c60a62bf69974ac716a93c155b419669eaac5acbbcc214c6c211667ab267c9`  
		Last Modified: Tue, 13 Jun 2023 03:12:57 GMT  
		Size: 5.2 MB (5209604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750b53c5b967617f8b2ff9cb0ecc88700772caab48f3b4f59f6d1e9a844e427a`  
		Last Modified: Tue, 13 Jun 2023 03:12:56 GMT  
		Size: 566.3 KB (566262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c843fecc8eafd5a7c37f7c3329458c4bb1cc58d6836fee8d9e8acff6f9b38c0`  
		Last Modified: Tue, 13 Jun 2023 03:12:56 GMT  
		Size: 294.3 KB (294347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c90431247a4ed342f9d684e9b04bb9bfc5dda7118d4267e7b3f23bd59ad4fd`  
		Last Modified: Tue, 13 Jun 2023 03:12:56 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f35924c1a48bb2edaa217e033e1fbee469d6e11c805e338939f681aaefbf34`  
		Last Modified: Tue, 13 Jun 2023 03:12:59 GMT  
		Size: 52.5 MB (52544231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471f7004fd790c6758674730bf2f9bd8fdabf72eca171b74caa8ef1744fece7e`  
		Last Modified: Tue, 13 Jun 2023 03:12:54 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d386b3f9b6664b042d1774b40dff2342b3c02d82cade1337f63021606bd299e6`  
		Last Modified: Tue, 13 Jun 2023 03:12:54 GMT  
		Size: 998.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b370d69da1a2a4adc59447af4f255ae1ec356c733e4b73d3b96b7761810229dc`  
		Last Modified: Tue, 13 Jun 2023 03:12:54 GMT  
		Size: 2.2 KB (2227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77933cca358498c1f5feb64dd9ed2c965d85c8d49fdb7db2e72e68bd245712f3`  
		Last Modified: Tue, 13 Jun 2023 03:12:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; ppc64le

```console
$ docker pull couchdb@sha256:c399e90a9b1b305e1b72125a4905ae3c51db4be6dff26c4a78bc27e759035a00
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.0 MB (95961503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ca27ec01131c11c250078f1488ed292338f0ceeefadde47ac20108c3e7e4b4b`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Mon, 12 Jun 2023 23:18:20 GMT
ADD file:b17eabe509462fa1a2e4c5421e877e3e4149085e3da07a421a66c7b06566c457 in / 
# Mon, 12 Jun 2023 23:18:22 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 09:45:19 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Jun 2023 09:45:20 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Jun 2023 09:45:36 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 09:45:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 13 Jun 2023 09:45:44 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Jun 2023 09:45:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 09:45:56 GMT
ENV COUCHDB_VERSION=3.3.2
# Tue, 13 Jun 2023 09:45:57 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Jun 2023 09:46:20 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Jun 2023 09:46:22 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Jun 2023 09:46:22 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 13 Jun 2023 09:46:23 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 13 Jun 2023 09:46:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Jun 2023 09:46:24 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 09:46:24 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Jun 2023 09:46:25 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Jun 2023 09:46:25 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:2973ac0be4a80a6cecbb73370e92810a6f67a98e12e61b3044aa63a322dab03a`  
		Last Modified: Mon, 12 Jun 2023 23:25:03 GMT  
		Size: 35.3 MB (35290790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7a4c14920d3766677c031be9ca45255dc9e4840b301c89d08bbab6c0c829b8`  
		Last Modified: Tue, 13 Jun 2023 09:47:05 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ee15726d36a785865415f386f34e9c4214a817d6dc79aec252811407ced685`  
		Last Modified: Tue, 13 Jun 2023 09:47:05 GMT  
		Size: 6.0 MB (6044040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a5cfeef71b924481f431fd94af56f33ccc02f4fcd0ce1b39afedb3168bd228a`  
		Last Modified: Tue, 13 Jun 2023 09:47:03 GMT  
		Size: 662.1 KB (662089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:799b3ab5e90729432923cecf21aad2ed782c84206d9d207078011186642aad90`  
		Last Modified: Tue, 13 Jun 2023 09:47:03 GMT  
		Size: 294.3 KB (294296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd6815c4999f2fa98c8cf4608b23fa063cf5a774c83160b584f54643a784eb0`  
		Last Modified: Tue, 13 Jun 2023 09:47:03 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea7c054364d04ef4b21f2a283c8ab5a0d200b3dfc983a9d4efd4c9b00c744a5c`  
		Last Modified: Tue, 13 Jun 2023 09:47:11 GMT  
		Size: 53.7 MB (53662870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76fc449be4ce6b84b9700f3c78608d408a725c28dc094af606d988eb350474da`  
		Last Modified: Tue, 13 Jun 2023 09:47:01 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064cc07cec794834bfcdae6cc7830104662247eeb39c275d846db362bc91301d`  
		Last Modified: Tue, 13 Jun 2023 09:47:01 GMT  
		Size: 999.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:214dfd321091da26c6f756ee7d21328d6e12653fd1acb75f40dfaf0063174b67`  
		Last Modified: Tue, 13 Jun 2023 09:47:01 GMT  
		Size: 2.2 KB (2228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03afeadee0940c842a4ed2c86ddb83b2a9fce341219595a1b84ffb0c299fe48f`  
		Last Modified: Tue, 13 Jun 2023 09:47:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; s390x

```console
$ docker pull couchdb@sha256:27f57b5ffc3a8799873fd57224eb642f883f404866610dbabd7710e700fa7d55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.0 MB (86982637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9c3afe9604f8597d2587042e19236a4a9af934cb69c067b9eb73e86501d11aa`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 23 May 2023 00:42:52 GMT
ADD file:23b1e12559302529556a94a1d4098dbdb454e263265258b940c2b2d23a97c121 in / 
# Tue, 23 May 2023 00:42:54 GMT
CMD ["bash"]
# Wed, 31 May 2023 23:41:40 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 31 May 2023 23:41:41 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 31 May 2023 23:41:47 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 31 May 2023 23:41:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 31 May 2023 23:41:50 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 31 May 2023 23:41:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 31 May 2023 23:41:55 GMT
ENV COUCHDB_VERSION=3.3.2
# Wed, 31 May 2023 23:41:55 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 31 May 2023 23:42:11 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 31 May 2023 23:42:12 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 31 May 2023 23:42:12 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 31 May 2023 23:42:13 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 31 May 2023 23:42:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 31 May 2023 23:42:13 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 31 May 2023 23:42:13 GMT
VOLUME [/opt/couchdb/data]
# Wed, 31 May 2023 23:42:13 GMT
EXPOSE 4369 5984 9100
# Wed, 31 May 2023 23:42:13 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:9c24ec455bdb6a9ad0d033c7cce8e71dd5bdbbe53a86d5feeb8d4cb7804fb8e5`  
		Last Modified: Tue, 23 May 2023 00:45:47 GMT  
		Size: 29.6 MB (29642170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79369d7477079fd194a68b466dff2d8edc280d261dc304b2567bfb55973c870b`  
		Last Modified: Wed, 31 May 2023 23:42:31 GMT  
		Size: 3.4 KB (3433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bea484bba066eb8863a66dcecc668d69aec750f8d1c0ad9325cc89b8210d148`  
		Last Modified: Wed, 31 May 2023 23:42:30 GMT  
		Size: 5.1 MB (5110473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5297b03b741ba1714084f21808e891def15cc57d292f901233aa010d56eda78e`  
		Last Modified: Wed, 31 May 2023 23:42:30 GMT  
		Size: 573.0 KB (573029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c1c59cdce3bf8d5680cb008d32bc45637f344c162a7912c90d5bbb3d0c753d`  
		Last Modified: Wed, 31 May 2023 23:42:30 GMT  
		Size: 294.5 KB (294451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89faeb4398086a27f7d1c2cfd535d3d86db34051276853757976607b8e6697e6`  
		Last Modified: Wed, 31 May 2023 23:42:30 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d08b9ecfe40b07d3aac1d314249e9c5843ce52edc2bea23828d62981849ff18`  
		Last Modified: Wed, 31 May 2023 23:42:34 GMT  
		Size: 51.4 MB (51355073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a8e6b453b90234fdb6dd9135a15beae0f3ba97050c5bd98264e1564f32386f`  
		Last Modified: Wed, 31 May 2023 23:42:28 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce5dd09ac3c1e930fd074767a97609f55cca10e5f1c213a684236bf7d4852b0`  
		Last Modified: Wed, 31 May 2023 23:42:28 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c7c51f86fe82775ec0e610e7ee7e3bf2e4ec64fe2d2a9ac042c388b5a61810`  
		Last Modified: Wed, 31 May 2023 23:42:28 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36cb0e3d58be45185e1df3bd73ef5f6906dad6517350c73fab6653744a44d7c`  
		Last Modified: Wed, 31 May 2023 23:42:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
