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
$ docker pull couchdb@sha256:15d826c2844f53a0bd6f193c37e2e5a1aeaf6badda3af526b24626d85b45ea05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2` - linux; amd64

```console
$ docker pull couchdb@sha256:63e364a55bdc213af9566ec1724240892cb73b511699100629e35061cd38b7f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.6 MB (84590139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ad4a95121fd0483a15b62d22f065032a5698274d73a9dd84a5fcaf8417fc760`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:31 GMT
ADD file:d4315fd7ceb67a5501410e4392ad3fd73642d6e2490f3626ce20a29321fa3682 in / 
# Wed, 16 Aug 2023 01:00:32 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:55 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 16 Aug 2023 01:46:56 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 16 Aug 2023 01:47:05 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:47:09 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 16 Aug 2023 01:47:09 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 16 Aug 2023 01:47:17 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:47:36 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 16 Aug 2023 01:47:37 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 16 Aug 2023 01:47:56 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 16 Aug 2023 01:47:57 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 16 Aug 2023 01:47:57 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 16 Aug 2023 01:47:57 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 16 Aug 2023 01:47:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 16 Aug 2023 01:47:58 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 01:47:58 GMT
VOLUME [/opt/couchdb/data]
# Wed, 16 Aug 2023 01:47:58 GMT
EXPOSE 4369 5984 9100
# Wed, 16 Aug 2023 01:47:58 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ddade83992f922bd9baa0e67dd5f7e8f518b6ed19c67e2ea076c92a8b38416c0`  
		Last Modified: Wed, 16 Aug 2023 01:05:53 GMT  
		Size: 27.2 MB (27187428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdb67f0bde13bfebd5a0c0957ca03e33e8fd6091372f61ea773900d51fa73b2`  
		Last Modified: Wed, 16 Aug 2023 01:48:51 GMT  
		Size: 3.4 KB (3417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6385c208f7c92df4b22509057f6a449d1ab2579284039131299430c05139541f`  
		Last Modified: Wed, 16 Aug 2023 01:48:50 GMT  
		Size: 6.7 MB (6704577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa5675fd0e6e871a478a47d4bc9a87a01facd68c1fb910b2f1d7a74489fd7fb`  
		Last Modified: Wed, 16 Aug 2023 01:48:49 GMT  
		Size: 1.3 MB (1259878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d18001037e081a3ed8f54e1de10912b457995d2b32c7353c3f2845c1f61e821`  
		Last Modified: Wed, 16 Aug 2023 01:48:49 GMT  
		Size: 294.6 KB (294572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f96d92663321a98f6d826363b563dab4bfe12f6aa1bd59d996c120db20ad6491`  
		Last Modified: Wed, 16 Aug 2023 01:49:02 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc24a5f7a174636bc5ab7a42ee1225f6aa909003c4235205178a92915a2c5755`  
		Last Modified: Wed, 16 Aug 2023 01:49:06 GMT  
		Size: 49.1 MB (49136663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e44842cb443300da6e7a17e69e8c5ec3bb9e0d13f8bb0c4519bec41a250b87`  
		Last Modified: Wed, 16 Aug 2023 01:49:00 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a701cfb7c34b9a2ce17f7a56d43b2b7b4f42436c2f8543bf4e10171a2ca0f57`  
		Last Modified: Wed, 16 Aug 2023 01:49:00 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a9f47d64a4547b9b3ede919da1ec7920f6e1cccef9a5b321d9147efc4ea82c`  
		Last Modified: Wed, 16 Aug 2023 01:49:01 GMT  
		Size: 2.1 KB (2056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a82982b04d4e60e74f988ce0f6ea89adf210c526ef3cd584ef5e98e996527f`  
		Last Modified: Wed, 16 Aug 2023 01:49:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:2fcd7f2a40aacbda5c771df44b1bbe26c6598282049636263b62b08826654bcc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (73041301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ff9e5abc775ae982c50babdc22273cd865a5447576343afc25982839dcd65eb`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:25 GMT
ADD file:cc6c5417b68ddd7a05f4a3896e20ff80bbd9ae8951adb686823f4039db4eba9a in / 
# Tue, 15 Aug 2023 23:40:26 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:07:40 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 16 Aug 2023 01:07:40 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 16 Aug 2023 01:07:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:07:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 16 Aug 2023 01:07:52 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 16 Aug 2023 01:07:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:08:20 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 16 Aug 2023 01:08:21 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 16 Aug 2023 01:08:32 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 16 Aug 2023 01:08:33 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 16 Aug 2023 01:08:33 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 16 Aug 2023 01:08:33 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 16 Aug 2023 01:08:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 16 Aug 2023 01:08:33 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 01:08:33 GMT
VOLUME [/opt/couchdb/data]
# Wed, 16 Aug 2023 01:08:33 GMT
EXPOSE 4369 5984 9100
# Wed, 16 Aug 2023 01:08:34 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:5b18dd3a8fc62fc571f4c7e2207d4072601fe59c0a6d3d739f4fddbff7f0dae3`  
		Last Modified: Tue, 15 Aug 2023 23:44:37 GMT  
		Size: 26.0 MB (25967768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa2eaff7ffcac23c7e7f43d656254fae8cd26f1a32d71f7094da4151e0acb5c`  
		Last Modified: Wed, 16 Aug 2023 01:09:08 GMT  
		Size: 3.4 KB (3437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d318ff6f28c4e31681ae006a971e3764e89587d7cd2d61bf1d94c687b840395f`  
		Last Modified: Wed, 16 Aug 2023 01:09:07 GMT  
		Size: 6.6 MB (6577627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5758ea29bc2ca0c5df4eb91c08975ea8fbdaaf99f8d8185f5dd7bb15aa6342`  
		Last Modified: Wed, 16 Aug 2023 01:09:07 GMT  
		Size: 1.2 MB (1164823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06785c3a618c2299d1c43c6166d218c293154f2b62388308489c543fb468fcc`  
		Last Modified: Wed, 16 Aug 2023 01:09:06 GMT  
		Size: 294.4 KB (294413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f4417b651302759824a7e831699783036288d7ebba9870fdc0949d269aaee9`  
		Last Modified: Wed, 16 Aug 2023 01:09:18 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2493d1574f8170d9eeda3cbff97ad245909908579cbb2282653526938a3c1847`  
		Last Modified: Wed, 16 Aug 2023 01:09:20 GMT  
		Size: 39.0 MB (39029634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96eb73da0cbb8718d9056155ea6d326f55914d6dc23bae2f4aea891fafa156e1`  
		Last Modified: Wed, 16 Aug 2023 01:09:17 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d656aca12a5afbedf32da25c8f2ca355ddb58e915b56851fbc5bd57afd049f0`  
		Last Modified: Wed, 16 Aug 2023 01:09:17 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50610929fac5c8418e73c8997c15b13c382caf512d41501c08361f59f0c684f1`  
		Last Modified: Wed, 16 Aug 2023 01:09:17 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f20b92e1a08ffe59ca2378313657db971ee901ae51e3770ea34f9191d07f83d`  
		Last Modified: Wed, 16 Aug 2023 01:09:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3`

```console
$ docker pull couchdb@sha256:15d826c2844f53a0bd6f193c37e2e5a1aeaf6badda3af526b24626d85b45ea05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:63e364a55bdc213af9566ec1724240892cb73b511699100629e35061cd38b7f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.6 MB (84590139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ad4a95121fd0483a15b62d22f065032a5698274d73a9dd84a5fcaf8417fc760`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:31 GMT
ADD file:d4315fd7ceb67a5501410e4392ad3fd73642d6e2490f3626ce20a29321fa3682 in / 
# Wed, 16 Aug 2023 01:00:32 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:55 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 16 Aug 2023 01:46:56 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 16 Aug 2023 01:47:05 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:47:09 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 16 Aug 2023 01:47:09 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 16 Aug 2023 01:47:17 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:47:36 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 16 Aug 2023 01:47:37 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 16 Aug 2023 01:47:56 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 16 Aug 2023 01:47:57 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 16 Aug 2023 01:47:57 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 16 Aug 2023 01:47:57 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 16 Aug 2023 01:47:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 16 Aug 2023 01:47:58 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 01:47:58 GMT
VOLUME [/opt/couchdb/data]
# Wed, 16 Aug 2023 01:47:58 GMT
EXPOSE 4369 5984 9100
# Wed, 16 Aug 2023 01:47:58 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ddade83992f922bd9baa0e67dd5f7e8f518b6ed19c67e2ea076c92a8b38416c0`  
		Last Modified: Wed, 16 Aug 2023 01:05:53 GMT  
		Size: 27.2 MB (27187428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdb67f0bde13bfebd5a0c0957ca03e33e8fd6091372f61ea773900d51fa73b2`  
		Last Modified: Wed, 16 Aug 2023 01:48:51 GMT  
		Size: 3.4 KB (3417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6385c208f7c92df4b22509057f6a449d1ab2579284039131299430c05139541f`  
		Last Modified: Wed, 16 Aug 2023 01:48:50 GMT  
		Size: 6.7 MB (6704577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa5675fd0e6e871a478a47d4bc9a87a01facd68c1fb910b2f1d7a74489fd7fb`  
		Last Modified: Wed, 16 Aug 2023 01:48:49 GMT  
		Size: 1.3 MB (1259878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d18001037e081a3ed8f54e1de10912b457995d2b32c7353c3f2845c1f61e821`  
		Last Modified: Wed, 16 Aug 2023 01:48:49 GMT  
		Size: 294.6 KB (294572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f96d92663321a98f6d826363b563dab4bfe12f6aa1bd59d996c120db20ad6491`  
		Last Modified: Wed, 16 Aug 2023 01:49:02 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc24a5f7a174636bc5ab7a42ee1225f6aa909003c4235205178a92915a2c5755`  
		Last Modified: Wed, 16 Aug 2023 01:49:06 GMT  
		Size: 49.1 MB (49136663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e44842cb443300da6e7a17e69e8c5ec3bb9e0d13f8bb0c4519bec41a250b87`  
		Last Modified: Wed, 16 Aug 2023 01:49:00 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a701cfb7c34b9a2ce17f7a56d43b2b7b4f42436c2f8543bf4e10171a2ca0f57`  
		Last Modified: Wed, 16 Aug 2023 01:49:00 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a9f47d64a4547b9b3ede919da1ec7920f6e1cccef9a5b321d9147efc4ea82c`  
		Last Modified: Wed, 16 Aug 2023 01:49:01 GMT  
		Size: 2.1 KB (2056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a82982b04d4e60e74f988ce0f6ea89adf210c526ef3cd584ef5e98e996527f`  
		Last Modified: Wed, 16 Aug 2023 01:49:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:2fcd7f2a40aacbda5c771df44b1bbe26c6598282049636263b62b08826654bcc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (73041301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ff9e5abc775ae982c50babdc22273cd865a5447576343afc25982839dcd65eb`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:25 GMT
ADD file:cc6c5417b68ddd7a05f4a3896e20ff80bbd9ae8951adb686823f4039db4eba9a in / 
# Tue, 15 Aug 2023 23:40:26 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:07:40 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 16 Aug 2023 01:07:40 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 16 Aug 2023 01:07:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:07:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 16 Aug 2023 01:07:52 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 16 Aug 2023 01:07:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:08:20 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 16 Aug 2023 01:08:21 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 16 Aug 2023 01:08:32 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 16 Aug 2023 01:08:33 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 16 Aug 2023 01:08:33 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 16 Aug 2023 01:08:33 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 16 Aug 2023 01:08:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 16 Aug 2023 01:08:33 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 01:08:33 GMT
VOLUME [/opt/couchdb/data]
# Wed, 16 Aug 2023 01:08:33 GMT
EXPOSE 4369 5984 9100
# Wed, 16 Aug 2023 01:08:34 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:5b18dd3a8fc62fc571f4c7e2207d4072601fe59c0a6d3d739f4fddbff7f0dae3`  
		Last Modified: Tue, 15 Aug 2023 23:44:37 GMT  
		Size: 26.0 MB (25967768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa2eaff7ffcac23c7e7f43d656254fae8cd26f1a32d71f7094da4151e0acb5c`  
		Last Modified: Wed, 16 Aug 2023 01:09:08 GMT  
		Size: 3.4 KB (3437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d318ff6f28c4e31681ae006a971e3764e89587d7cd2d61bf1d94c687b840395f`  
		Last Modified: Wed, 16 Aug 2023 01:09:07 GMT  
		Size: 6.6 MB (6577627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5758ea29bc2ca0c5df4eb91c08975ea8fbdaaf99f8d8185f5dd7bb15aa6342`  
		Last Modified: Wed, 16 Aug 2023 01:09:07 GMT  
		Size: 1.2 MB (1164823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06785c3a618c2299d1c43c6166d218c293154f2b62388308489c543fb468fcc`  
		Last Modified: Wed, 16 Aug 2023 01:09:06 GMT  
		Size: 294.4 KB (294413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f4417b651302759824a7e831699783036288d7ebba9870fdc0949d269aaee9`  
		Last Modified: Wed, 16 Aug 2023 01:09:18 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2493d1574f8170d9eeda3cbff97ad245909908579cbb2282653526938a3c1847`  
		Last Modified: Wed, 16 Aug 2023 01:09:20 GMT  
		Size: 39.0 MB (39029634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96eb73da0cbb8718d9056155ea6d326f55914d6dc23bae2f4aea891fafa156e1`  
		Last Modified: Wed, 16 Aug 2023 01:09:17 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d656aca12a5afbedf32da25c8f2ca355ddb58e915b56851fbc5bd57afd049f0`  
		Last Modified: Wed, 16 Aug 2023 01:09:17 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50610929fac5c8418e73c8997c15b13c382caf512d41501c08361f59f0c684f1`  
		Last Modified: Wed, 16 Aug 2023 01:09:17 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f20b92e1a08ffe59ca2378313657db971ee901ae51e3770ea34f9191d07f83d`  
		Last Modified: Wed, 16 Aug 2023 01:09:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3.1`

```console
$ docker pull couchdb@sha256:15d826c2844f53a0bd6f193c37e2e5a1aeaf6badda3af526b24626d85b45ea05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:63e364a55bdc213af9566ec1724240892cb73b511699100629e35061cd38b7f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.6 MB (84590139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ad4a95121fd0483a15b62d22f065032a5698274d73a9dd84a5fcaf8417fc760`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:31 GMT
ADD file:d4315fd7ceb67a5501410e4392ad3fd73642d6e2490f3626ce20a29321fa3682 in / 
# Wed, 16 Aug 2023 01:00:32 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:55 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 16 Aug 2023 01:46:56 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 16 Aug 2023 01:47:05 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:47:09 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 16 Aug 2023 01:47:09 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 16 Aug 2023 01:47:17 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:47:36 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 16 Aug 2023 01:47:37 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 16 Aug 2023 01:47:56 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 16 Aug 2023 01:47:57 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 16 Aug 2023 01:47:57 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 16 Aug 2023 01:47:57 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 16 Aug 2023 01:47:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 16 Aug 2023 01:47:58 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 01:47:58 GMT
VOLUME [/opt/couchdb/data]
# Wed, 16 Aug 2023 01:47:58 GMT
EXPOSE 4369 5984 9100
# Wed, 16 Aug 2023 01:47:58 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ddade83992f922bd9baa0e67dd5f7e8f518b6ed19c67e2ea076c92a8b38416c0`  
		Last Modified: Wed, 16 Aug 2023 01:05:53 GMT  
		Size: 27.2 MB (27187428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdb67f0bde13bfebd5a0c0957ca03e33e8fd6091372f61ea773900d51fa73b2`  
		Last Modified: Wed, 16 Aug 2023 01:48:51 GMT  
		Size: 3.4 KB (3417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6385c208f7c92df4b22509057f6a449d1ab2579284039131299430c05139541f`  
		Last Modified: Wed, 16 Aug 2023 01:48:50 GMT  
		Size: 6.7 MB (6704577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa5675fd0e6e871a478a47d4bc9a87a01facd68c1fb910b2f1d7a74489fd7fb`  
		Last Modified: Wed, 16 Aug 2023 01:48:49 GMT  
		Size: 1.3 MB (1259878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d18001037e081a3ed8f54e1de10912b457995d2b32c7353c3f2845c1f61e821`  
		Last Modified: Wed, 16 Aug 2023 01:48:49 GMT  
		Size: 294.6 KB (294572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f96d92663321a98f6d826363b563dab4bfe12f6aa1bd59d996c120db20ad6491`  
		Last Modified: Wed, 16 Aug 2023 01:49:02 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc24a5f7a174636bc5ab7a42ee1225f6aa909003c4235205178a92915a2c5755`  
		Last Modified: Wed, 16 Aug 2023 01:49:06 GMT  
		Size: 49.1 MB (49136663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e44842cb443300da6e7a17e69e8c5ec3bb9e0d13f8bb0c4519bec41a250b87`  
		Last Modified: Wed, 16 Aug 2023 01:49:00 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a701cfb7c34b9a2ce17f7a56d43b2b7b4f42436c2f8543bf4e10171a2ca0f57`  
		Last Modified: Wed, 16 Aug 2023 01:49:00 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a9f47d64a4547b9b3ede919da1ec7920f6e1cccef9a5b321d9147efc4ea82c`  
		Last Modified: Wed, 16 Aug 2023 01:49:01 GMT  
		Size: 2.1 KB (2056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a82982b04d4e60e74f988ce0f6ea89adf210c526ef3cd584ef5e98e996527f`  
		Last Modified: Wed, 16 Aug 2023 01:49:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:2fcd7f2a40aacbda5c771df44b1bbe26c6598282049636263b62b08826654bcc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (73041301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ff9e5abc775ae982c50babdc22273cd865a5447576343afc25982839dcd65eb`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:25 GMT
ADD file:cc6c5417b68ddd7a05f4a3896e20ff80bbd9ae8951adb686823f4039db4eba9a in / 
# Tue, 15 Aug 2023 23:40:26 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:07:40 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 16 Aug 2023 01:07:40 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 16 Aug 2023 01:07:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:07:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 16 Aug 2023 01:07:52 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 16 Aug 2023 01:07:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:08:20 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 16 Aug 2023 01:08:21 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 16 Aug 2023 01:08:32 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 16 Aug 2023 01:08:33 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 16 Aug 2023 01:08:33 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 16 Aug 2023 01:08:33 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 16 Aug 2023 01:08:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 16 Aug 2023 01:08:33 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 01:08:33 GMT
VOLUME [/opt/couchdb/data]
# Wed, 16 Aug 2023 01:08:33 GMT
EXPOSE 4369 5984 9100
# Wed, 16 Aug 2023 01:08:34 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:5b18dd3a8fc62fc571f4c7e2207d4072601fe59c0a6d3d739f4fddbff7f0dae3`  
		Last Modified: Tue, 15 Aug 2023 23:44:37 GMT  
		Size: 26.0 MB (25967768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa2eaff7ffcac23c7e7f43d656254fae8cd26f1a32d71f7094da4151e0acb5c`  
		Last Modified: Wed, 16 Aug 2023 01:09:08 GMT  
		Size: 3.4 KB (3437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d318ff6f28c4e31681ae006a971e3764e89587d7cd2d61bf1d94c687b840395f`  
		Last Modified: Wed, 16 Aug 2023 01:09:07 GMT  
		Size: 6.6 MB (6577627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5758ea29bc2ca0c5df4eb91c08975ea8fbdaaf99f8d8185f5dd7bb15aa6342`  
		Last Modified: Wed, 16 Aug 2023 01:09:07 GMT  
		Size: 1.2 MB (1164823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06785c3a618c2299d1c43c6166d218c293154f2b62388308489c543fb468fcc`  
		Last Modified: Wed, 16 Aug 2023 01:09:06 GMT  
		Size: 294.4 KB (294413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f4417b651302759824a7e831699783036288d7ebba9870fdc0949d269aaee9`  
		Last Modified: Wed, 16 Aug 2023 01:09:18 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2493d1574f8170d9eeda3cbff97ad245909908579cbb2282653526938a3c1847`  
		Last Modified: Wed, 16 Aug 2023 01:09:20 GMT  
		Size: 39.0 MB (39029634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96eb73da0cbb8718d9056155ea6d326f55914d6dc23bae2f4aea891fafa156e1`  
		Last Modified: Wed, 16 Aug 2023 01:09:17 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d656aca12a5afbedf32da25c8f2ca355ddb58e915b56851fbc5bd57afd049f0`  
		Last Modified: Wed, 16 Aug 2023 01:09:17 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50610929fac5c8418e73c8997c15b13c382caf512d41501c08361f59f0c684f1`  
		Last Modified: Wed, 16 Aug 2023 01:09:17 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f20b92e1a08ffe59ca2378313657db971ee901ae51e3770ea34f9191d07f83d`  
		Last Modified: Wed, 16 Aug 2023 01:09:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3`

```console
$ docker pull couchdb@sha256:6187c65b7c07941701ba71695b1102383887056019d421020c455a929e9df20e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `couchdb:3` - linux; amd64

```console
$ docker pull couchdb@sha256:1ec2426cf9d8628f6c7126fb477f51b8c536325289cd02ce93423aaebb274540
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90240695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ca978417950e1e879ab4ddb800644f67dbd2ce4e667da20f62cb3065bba3ef6`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:45:54 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 16 Aug 2023 01:45:54 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 16 Aug 2023 01:46:01 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:46:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 16 Aug 2023 01:46:05 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 16 Aug 2023 01:46:11 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:46:11 GMT
ENV COUCHDB_VERSION=3.3.2
# Wed, 16 Aug 2023 01:46:12 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 16 Aug 2023 01:46:26 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 16 Aug 2023 01:46:26 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 16 Aug 2023 01:46:26 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 16 Aug 2023 01:46:26 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 16 Aug 2023 01:46:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 16 Aug 2023 01:46:27 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 01:46:27 GMT
VOLUME [/opt/couchdb/data]
# Wed, 16 Aug 2023 01:46:27 GMT
EXPOSE 4369 5984 9100
# Wed, 16 Aug 2023 01:46:27 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e683ea8132b62c891a7a7001a4607c52d59cec34fffc7d4c3bf1aa23dd1f8965`  
		Last Modified: Wed, 16 Aug 2023 01:48:14 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd02df917dc89d0c9f2f3b12495a7489bd0e56a9cc24b2293dbfe9d21e97516`  
		Last Modified: Wed, 16 Aug 2023 01:48:14 GMT  
		Size: 5.2 MB (5224576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27e9a0cc8fe852d5144ed084c43083b36f5f25d8c83db408340b31dce9682b3`  
		Last Modified: Wed, 16 Aug 2023 01:48:13 GMT  
		Size: 610.3 KB (610294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91d3a3133f57276711efc489279c7c15c935fe4b9ef5200d4575a884cc2278b`  
		Last Modified: Wed, 16 Aug 2023 01:48:13 GMT  
		Size: 294.5 KB (294462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777caeb656baab6032799b4a60709899a93185ed9c41616fb1d55eb35330da2d`  
		Last Modified: Wed, 16 Aug 2023 01:48:12 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b7d6bbbb71932c5cd4a76f304203e9b46721051d9f9d66bf14767e2245c782`  
		Last Modified: Wed, 16 Aug 2023 01:48:16 GMT  
		Size: 52.7 MB (52686268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ba7d950ec4c78e5f5f1a13c0f11fb294498877976e64b55b5cd1153a4e834d`  
		Last Modified: Wed, 16 Aug 2023 01:48:10 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5e496fb52a8112cf321600bf11ba4269aac657a3e33896481640e379ffc00f`  
		Last Modified: Wed, 16 Aug 2023 01:48:11 GMT  
		Size: 997.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9eec9879e73cae7da79e5eb515359d0f3d64a4ecf49554fc895830759aeb04`  
		Last Modified: Wed, 16 Aug 2023 01:48:11 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32fcbbd11bd218e1902debe81797e81a97a2ec4d352fee88ea4d6ca440127ed`  
		Last Modified: Wed, 16 Aug 2023 01:48:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:30bfee6095c98d4127df9c620886e25c170779d5713ad95fab161d49c76a7717
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88684226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77e27a374b34255c7dce27560b0ad4e0805df34a91fc50eba889ea000cc85961`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:06:55 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 16 Aug 2023 01:06:56 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 16 Aug 2023 01:07:02 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:07:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 16 Aug 2023 01:07:05 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 16 Aug 2023 01:07:09 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:07:09 GMT
ENV COUCHDB_VERSION=3.3.2
# Wed, 16 Aug 2023 01:07:10 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 16 Aug 2023 01:07:22 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 16 Aug 2023 01:07:22 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 16 Aug 2023 01:07:22 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 16 Aug 2023 01:07:22 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 16 Aug 2023 01:07:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 16 Aug 2023 01:07:23 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 01:07:23 GMT
VOLUME [/opt/couchdb/data]
# Wed, 16 Aug 2023 01:07:23 GMT
EXPOSE 4369 5984 9100
# Wed, 16 Aug 2023 01:07:23 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ff9c650b66afcfcf0aecf606a24b4f6267031943f5cb2a9bee414c9b0f89ff`  
		Last Modified: Wed, 16 Aug 2023 01:08:50 GMT  
		Size: 3.4 KB (3436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3110b3b5e035aeab66963dbd48c79553935329f1f627cf3ff4fba44e3b3081`  
		Last Modified: Wed, 16 Aug 2023 01:08:49 GMT  
		Size: 5.2 MB (5209580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0ad12d938d91082a0c04662667c6e63c489ca6b935a55600c3cacd6dfcf6e7`  
		Last Modified: Wed, 16 Aug 2023 01:08:49 GMT  
		Size: 566.3 KB (566309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dcae50ed7b69ad69869743da712f37f818c5a7d003326b5ec9c68cf4c72f7e1`  
		Last Modified: Wed, 16 Aug 2023 01:08:49 GMT  
		Size: 294.3 KB (294339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988571db89e062bd3cc3cc0078fdf2a53dbbbc812ecbc119a71eac500f13a16f`  
		Last Modified: Wed, 16 Aug 2023 01:08:48 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab992810bd02bd6e6909d87fe14dce599f8115a9fb5a7bda65679454f2df3cd8`  
		Last Modified: Wed, 16 Aug 2023 01:08:51 GMT  
		Size: 52.5 MB (52543735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2d794dbe81b85b837cf872688ea211ac7838258ef6d747164c7285fff00580`  
		Last Modified: Wed, 16 Aug 2023 01:08:47 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c31a9ad71eb77b1c29e0cd83b58631175ef07966d3237863d8cacc5d2da53b`  
		Last Modified: Wed, 16 Aug 2023 01:08:47 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0091c75d975b9376b4c8dc194ba8d46241b674cec5dae6d1111cd407f3494e2e`  
		Last Modified: Wed, 16 Aug 2023 01:08:47 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73f0fa03869f341cb2662fad33bf15697269bcb5d7181fee4c6d43032074d7d`  
		Last Modified: Wed, 16 Aug 2023 01:08:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; ppc64le

```console
$ docker pull couchdb@sha256:8e06df720f4e07d7c1aceefc45eb9f61d7d7d61fb5e3de18c1083b2f63b95f3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.0 MB (95962013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7747f406a39fb87acae729b3f33ef6b5ce3045b048a6c936e80994acea2ec6ca`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 16 Aug 2023 01:10:12 GMT
ADD file:eeb766a3bb0461f0baa2425cfd43628994c064bd728f51f1b8df659a4bd2f489 in / 
# Wed, 16 Aug 2023 01:10:14 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 02:19:08 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 16 Aug 2023 02:19:11 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 16 Aug 2023 02:19:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 02:19:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 16 Aug 2023 02:19:49 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 16 Aug 2023 02:20:10 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 02:20:11 GMT
ENV COUCHDB_VERSION=3.3.2
# Wed, 16 Aug 2023 02:20:12 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 16 Aug 2023 02:20:44 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 16 Aug 2023 02:20:46 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 16 Aug 2023 02:20:46 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 16 Aug 2023 02:20:46 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 16 Aug 2023 02:20:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 16 Aug 2023 02:20:48 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 02:20:49 GMT
VOLUME [/opt/couchdb/data]
# Wed, 16 Aug 2023 02:20:49 GMT
EXPOSE 4369 5984 9100
# Wed, 16 Aug 2023 02:20:49 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:dacf4195c8a0403fd11459739bf9dc9be427261bf5e0bedb49e18d1498cf7c2e`  
		Last Modified: Wed, 16 Aug 2023 01:17:04 GMT  
		Size: 35.3 MB (35291067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e6a8655a620cffbe60c27dd03f9c5d03132e3fffd3e788526b63d70a3c6685`  
		Last Modified: Wed, 16 Aug 2023 02:21:45 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8a4468de45ced49ad8e3c084adfde3e9e39622bd4eefd7b50b2845c9f0748d`  
		Last Modified: Wed, 16 Aug 2023 02:21:45 GMT  
		Size: 6.0 MB (6044086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998ea43aefd6709362b0f13d999f80bbe87042afe3dc4d60e1d82a42a55017a0`  
		Last Modified: Wed, 16 Aug 2023 02:21:44 GMT  
		Size: 662.1 KB (662144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984bdece6eec3b2c06e59a0fc3ff6a3f4913dd41fda95c2a93ef7666c9faf49f`  
		Last Modified: Wed, 16 Aug 2023 02:21:44 GMT  
		Size: 294.4 KB (294359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289a2e380dbf7483fe7b0cb2a996ee515d9d0ad6782ced49cf64020a5331006c`  
		Last Modified: Wed, 16 Aug 2023 02:21:43 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ea07c066dd201b35d53a50df457fbf1aa89df808344455301d3b1d4157b30a`  
		Last Modified: Wed, 16 Aug 2023 02:21:50 GMT  
		Size: 53.7 MB (53662934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914b28fa3462815c14ab9660b2071c0f7e31f60935409831159e43a25a1b8f42`  
		Last Modified: Wed, 16 Aug 2023 02:21:41 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b653561e98b96ac3aaf3c9e0b5e4a86c1d2dda60e8f8463e9ea907b1c8b4f7a`  
		Last Modified: Wed, 16 Aug 2023 02:21:41 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16ed1d5bfe33233a937efc507eefb39df037724ea0e34f59328c1e8a7ee9f6a`  
		Last Modified: Wed, 16 Aug 2023 02:21:41 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe53b7a249ba7d07fdfbc4f2cf836d068d1b1e0d8d6af0594d6bca247c94736`  
		Last Modified: Wed, 16 Aug 2023 02:21:41 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; s390x

```console
$ docker pull couchdb@sha256:29e829b586b1cb6e650b0e13797721b362071a74370a5f6680669c847090f45a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.0 MB (86992619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:192ddd69ff7e41d2bdf0975625c068953c9226f56fe985a51b032813e5bb8c66`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 07 Sep 2023 00:44:33 GMT
ADD file:fb2f216acd6d0ecaf48e8d5dd7e3cdb5d1f51d414f2011ed318cb494f96d89ca in / 
# Thu, 07 Sep 2023 00:44:37 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:28:56 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 07 Sep 2023 01:28:58 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 07 Sep 2023 01:29:11 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:29:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Thu, 07 Sep 2023 01:29:17 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 07 Sep 2023 01:29:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:29:27 GMT
ENV COUCHDB_VERSION=3.3.2
# Thu, 07 Sep 2023 01:29:28 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 07 Sep 2023 01:29:56 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 07 Sep 2023 01:30:05 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 07 Sep 2023 01:30:05 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Thu, 07 Sep 2023 01:30:05 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Thu, 07 Sep 2023 01:30:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 07 Sep 2023 01:30:07 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 07 Sep 2023 01:30:07 GMT
VOLUME [/opt/couchdb/data]
# Thu, 07 Sep 2023 01:30:08 GMT
EXPOSE 4369 5984 9100
# Thu, 07 Sep 2023 01:30:09 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:c9501ad9402d64e6c612fa1bb94f16df51188e681dc1f28c603a6109f06f22d7`  
		Last Modified: Thu, 07 Sep 2023 00:50:10 GMT  
		Size: 29.7 MB (29652801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996ad4371fbc51ce08543507129d65ab8b90dd855e656f8eabd70335c57bb0a1`  
		Last Modified: Thu, 07 Sep 2023 01:30:26 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e0fe5808ef043ae040668477d7e9dfe710765ea40e3d011b82fa33031b7ea4`  
		Last Modified: Thu, 07 Sep 2023 01:30:25 GMT  
		Size: 5.1 MB (5110534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f126aebc8a50e39748585e27d5fd5a9836b6a93c873802d3d3403b156cac952`  
		Last Modified: Thu, 07 Sep 2023 01:30:25 GMT  
		Size: 573.0 KB (573029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f00d25b2e1271b6380742fbbeca5c10b9b084a78cfba7f031f12a3d00a87df5`  
		Last Modified: Thu, 07 Sep 2023 01:30:24 GMT  
		Size: 294.5 KB (294462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577394d2327382521d14f38714c2247fd0db46e1ab49b86cb2350c309835db81`  
		Last Modified: Thu, 07 Sep 2023 01:30:24 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4258fc35f99c32658815e5ea98c85edc9f278bcba6613030c57395fc75cae139`  
		Last Modified: Thu, 07 Sep 2023 01:30:28 GMT  
		Size: 51.4 MB (51354348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0bdcf38e015804f9400dd02e2614c14ea270ce30cfc9602fc0bf39c87dd1fb`  
		Last Modified: Thu, 07 Sep 2023 01:30:23 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67bc37b8d392d13a0a6a7312678435efade4fd7449ec2ed52945c52abe3b85d`  
		Last Modified: Thu, 07 Sep 2023 01:30:23 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3410bb24e7a70dfce7810cf4736b3f0e0a420444d7825a7d1a9a1309c56e7e`  
		Last Modified: Thu, 07 Sep 2023 01:30:23 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e526b2a03229b6f0cd56ffc8d6c5600b8eec7f407d56686697c3684634adbc52`  
		Last Modified: Thu, 07 Sep 2023 01:30:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1`

```console
$ docker pull couchdb@sha256:a34b5931ccc4a5ed16af0e01b38fdf536a1762b20f939dbee1593937474c0e70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:07810d9fd789371bb3b7a87b51e4471d4a9c687d6328c9f1fa1320f3c5f0e533
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.1 MB (80073609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:204fcdb2d34241e8c85371cc45dfe10c29b17bc6a5d7b9a73b0aec6f3fd55776`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:31 GMT
ADD file:d4315fd7ceb67a5501410e4392ad3fd73642d6e2490f3626ce20a29321fa3682 in / 
# Wed, 16 Aug 2023 01:00:32 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:55 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 16 Aug 2023 01:46:56 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 16 Aug 2023 01:47:05 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:47:09 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 16 Aug 2023 01:47:09 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 16 Aug 2023 01:47:17 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:47:17 GMT
ENV COUCHDB_VERSION=3.1.2
# Wed, 16 Aug 2023 01:47:17 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 16 Aug 2023 01:47:31 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 16 Aug 2023 01:47:31 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 16 Aug 2023 01:47:32 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 16 Aug 2023 01:47:32 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 16 Aug 2023 01:47:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 16 Aug 2023 01:47:32 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 01:47:32 GMT
VOLUME [/opt/couchdb/data]
# Wed, 16 Aug 2023 01:47:32 GMT
EXPOSE 4369 5984 9100
# Wed, 16 Aug 2023 01:47:33 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ddade83992f922bd9baa0e67dd5f7e8f518b6ed19c67e2ea076c92a8b38416c0`  
		Last Modified: Wed, 16 Aug 2023 01:05:53 GMT  
		Size: 27.2 MB (27187428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdb67f0bde13bfebd5a0c0957ca03e33e8fd6091372f61ea773900d51fa73b2`  
		Last Modified: Wed, 16 Aug 2023 01:48:51 GMT  
		Size: 3.4 KB (3417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6385c208f7c92df4b22509057f6a449d1ab2579284039131299430c05139541f`  
		Last Modified: Wed, 16 Aug 2023 01:48:50 GMT  
		Size: 6.7 MB (6704577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa5675fd0e6e871a478a47d4bc9a87a01facd68c1fb910b2f1d7a74489fd7fb`  
		Last Modified: Wed, 16 Aug 2023 01:48:49 GMT  
		Size: 1.3 MB (1259878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d18001037e081a3ed8f54e1de10912b457995d2b32c7353c3f2845c1f61e821`  
		Last Modified: Wed, 16 Aug 2023 01:48:49 GMT  
		Size: 294.6 KB (294572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3af0268f1ca6ca28d8e46fa9304b86cf098cd0721cac6f9d864c2d9946f7fa`  
		Last Modified: Wed, 16 Aug 2023 01:48:49 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8acd9e089dbf3eb0002648e711f0c9baf3c17c7f895557822f9a8211e6b5b278`  
		Last Modified: Wed, 16 Aug 2023 01:48:49 GMT  
		Size: 44.6 MB (44620140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65393823ffbf0fb3b0307f0cca845b0ca0a5fce5326d6c9041508d793eed1d5a`  
		Last Modified: Wed, 16 Aug 2023 01:48:44 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c11aa7b8461ab2b53354ea4ae3c90985e2ea0179c64bec5a3d6ddf600dc870a`  
		Last Modified: Wed, 16 Aug 2023 01:48:44 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c036acb8254b4adf3b1f07f4ab62df4111d8111febcb6a4cb7afe4b25991cded`  
		Last Modified: Wed, 16 Aug 2023 01:48:44 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866c0e27cfe3e680c1b7db5e26dc1e024601b223a200fe9dd22492a4461a108c`  
		Last Modified: Wed, 16 Aug 2023 01:48:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:0be9ef413ec69d41b069437b8885c7563aea3c2b915869f9649e825e13c7ccdc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75138213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:795656f601d47dde54aadce85f218763cbd25924912d412c98dfb6e22ed5996e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:25 GMT
ADD file:cc6c5417b68ddd7a05f4a3896e20ff80bbd9ae8951adb686823f4039db4eba9a in / 
# Tue, 15 Aug 2023 23:40:26 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:07:40 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 16 Aug 2023 01:07:40 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 16 Aug 2023 01:07:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:07:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 16 Aug 2023 01:07:52 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 16 Aug 2023 01:07:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:07:58 GMT
ENV COUCHDB_VERSION=3.1.2
# Wed, 16 Aug 2023 01:07:59 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 16 Aug 2023 01:08:11 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 16 Aug 2023 01:08:11 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 16 Aug 2023 01:08:11 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 16 Aug 2023 01:08:11 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 16 Aug 2023 01:08:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 16 Aug 2023 01:08:12 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 01:08:12 GMT
VOLUME [/opt/couchdb/data]
# Wed, 16 Aug 2023 01:08:12 GMT
EXPOSE 4369 5984 9100
# Wed, 16 Aug 2023 01:08:12 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:5b18dd3a8fc62fc571f4c7e2207d4072601fe59c0a6d3d739f4fddbff7f0dae3`  
		Last Modified: Tue, 15 Aug 2023 23:44:37 GMT  
		Size: 26.0 MB (25967768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa2eaff7ffcac23c7e7f43d656254fae8cd26f1a32d71f7094da4151e0acb5c`  
		Last Modified: Wed, 16 Aug 2023 01:09:08 GMT  
		Size: 3.4 KB (3437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d318ff6f28c4e31681ae006a971e3764e89587d7cd2d61bf1d94c687b840395f`  
		Last Modified: Wed, 16 Aug 2023 01:09:07 GMT  
		Size: 6.6 MB (6577627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5758ea29bc2ca0c5df4eb91c08975ea8fbdaaf99f8d8185f5dd7bb15aa6342`  
		Last Modified: Wed, 16 Aug 2023 01:09:07 GMT  
		Size: 1.2 MB (1164823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06785c3a618c2299d1c43c6166d218c293154f2b62388308489c543fb468fcc`  
		Last Modified: Wed, 16 Aug 2023 01:09:06 GMT  
		Size: 294.4 KB (294413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13db5751d0d30669960029c9dc9f4573eb2e498ba47ac3cd92ddd18c3d69f529`  
		Last Modified: Wed, 16 Aug 2023 01:09:06 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2d8b28c3773bf5ee838350826c5ac64584be54186987bc44818c7d9dbacc16`  
		Last Modified: Wed, 16 Aug 2023 01:09:08 GMT  
		Size: 41.1 MB (41126542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc059df8fa27f2fd0e76e73a0b57d115b58facd68cb8cc49eb0dd0d3c96451b9`  
		Last Modified: Wed, 16 Aug 2023 01:09:04 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a143b442aed69550094358e37c41a8b286b3fccbb0419d50344af0ccc584b4e`  
		Last Modified: Wed, 16 Aug 2023 01:09:04 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af3e620fbba87071b9849448da39963e51e1fa45d22c980b4186f19b63189b4`  
		Last Modified: Wed, 16 Aug 2023 01:09:04 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c8a19e4faf7dfad7e346443bfd88cbe85a3adb2f62eb3cbc8531cf73dff0343`  
		Last Modified: Wed, 16 Aug 2023 01:09:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1.2`

```console
$ docker pull couchdb@sha256:a34b5931ccc4a5ed16af0e01b38fdf536a1762b20f939dbee1593937474c0e70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1.2` - linux; amd64

```console
$ docker pull couchdb@sha256:07810d9fd789371bb3b7a87b51e4471d4a9c687d6328c9f1fa1320f3c5f0e533
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.1 MB (80073609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:204fcdb2d34241e8c85371cc45dfe10c29b17bc6a5d7b9a73b0aec6f3fd55776`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:31 GMT
ADD file:d4315fd7ceb67a5501410e4392ad3fd73642d6e2490f3626ce20a29321fa3682 in / 
# Wed, 16 Aug 2023 01:00:32 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:46:55 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 16 Aug 2023 01:46:56 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 16 Aug 2023 01:47:05 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:47:09 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 16 Aug 2023 01:47:09 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 16 Aug 2023 01:47:17 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:47:17 GMT
ENV COUCHDB_VERSION=3.1.2
# Wed, 16 Aug 2023 01:47:17 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 16 Aug 2023 01:47:31 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 16 Aug 2023 01:47:31 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 16 Aug 2023 01:47:32 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 16 Aug 2023 01:47:32 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 16 Aug 2023 01:47:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 16 Aug 2023 01:47:32 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 01:47:32 GMT
VOLUME [/opt/couchdb/data]
# Wed, 16 Aug 2023 01:47:32 GMT
EXPOSE 4369 5984 9100
# Wed, 16 Aug 2023 01:47:33 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ddade83992f922bd9baa0e67dd5f7e8f518b6ed19c67e2ea076c92a8b38416c0`  
		Last Modified: Wed, 16 Aug 2023 01:05:53 GMT  
		Size: 27.2 MB (27187428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdb67f0bde13bfebd5a0c0957ca03e33e8fd6091372f61ea773900d51fa73b2`  
		Last Modified: Wed, 16 Aug 2023 01:48:51 GMT  
		Size: 3.4 KB (3417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6385c208f7c92df4b22509057f6a449d1ab2579284039131299430c05139541f`  
		Last Modified: Wed, 16 Aug 2023 01:48:50 GMT  
		Size: 6.7 MB (6704577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa5675fd0e6e871a478a47d4bc9a87a01facd68c1fb910b2f1d7a74489fd7fb`  
		Last Modified: Wed, 16 Aug 2023 01:48:49 GMT  
		Size: 1.3 MB (1259878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d18001037e081a3ed8f54e1de10912b457995d2b32c7353c3f2845c1f61e821`  
		Last Modified: Wed, 16 Aug 2023 01:48:49 GMT  
		Size: 294.6 KB (294572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3af0268f1ca6ca28d8e46fa9304b86cf098cd0721cac6f9d864c2d9946f7fa`  
		Last Modified: Wed, 16 Aug 2023 01:48:49 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8acd9e089dbf3eb0002648e711f0c9baf3c17c7f895557822f9a8211e6b5b278`  
		Last Modified: Wed, 16 Aug 2023 01:48:49 GMT  
		Size: 44.6 MB (44620140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65393823ffbf0fb3b0307f0cca845b0ca0a5fce5326d6c9041508d793eed1d5a`  
		Last Modified: Wed, 16 Aug 2023 01:48:44 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c11aa7b8461ab2b53354ea4ae3c90985e2ea0179c64bec5a3d6ddf600dc870a`  
		Last Modified: Wed, 16 Aug 2023 01:48:44 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c036acb8254b4adf3b1f07f4ab62df4111d8111febcb6a4cb7afe4b25991cded`  
		Last Modified: Wed, 16 Aug 2023 01:48:44 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866c0e27cfe3e680c1b7db5e26dc1e024601b223a200fe9dd22492a4461a108c`  
		Last Modified: Wed, 16 Aug 2023 01:48:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:0be9ef413ec69d41b069437b8885c7563aea3c2b915869f9649e825e13c7ccdc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75138213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:795656f601d47dde54aadce85f218763cbd25924912d412c98dfb6e22ed5996e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:25 GMT
ADD file:cc6c5417b68ddd7a05f4a3896e20ff80bbd9ae8951adb686823f4039db4eba9a in / 
# Tue, 15 Aug 2023 23:40:26 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:07:40 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 16 Aug 2023 01:07:40 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 16 Aug 2023 01:07:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:07:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 16 Aug 2023 01:07:52 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 16 Aug 2023 01:07:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:07:58 GMT
ENV COUCHDB_VERSION=3.1.2
# Wed, 16 Aug 2023 01:07:59 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 16 Aug 2023 01:08:11 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 16 Aug 2023 01:08:11 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 16 Aug 2023 01:08:11 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 16 Aug 2023 01:08:11 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 16 Aug 2023 01:08:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 16 Aug 2023 01:08:12 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 01:08:12 GMT
VOLUME [/opt/couchdb/data]
# Wed, 16 Aug 2023 01:08:12 GMT
EXPOSE 4369 5984 9100
# Wed, 16 Aug 2023 01:08:12 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:5b18dd3a8fc62fc571f4c7e2207d4072601fe59c0a6d3d739f4fddbff7f0dae3`  
		Last Modified: Tue, 15 Aug 2023 23:44:37 GMT  
		Size: 26.0 MB (25967768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa2eaff7ffcac23c7e7f43d656254fae8cd26f1a32d71f7094da4151e0acb5c`  
		Last Modified: Wed, 16 Aug 2023 01:09:08 GMT  
		Size: 3.4 KB (3437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d318ff6f28c4e31681ae006a971e3764e89587d7cd2d61bf1d94c687b840395f`  
		Last Modified: Wed, 16 Aug 2023 01:09:07 GMT  
		Size: 6.6 MB (6577627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5758ea29bc2ca0c5df4eb91c08975ea8fbdaaf99f8d8185f5dd7bb15aa6342`  
		Last Modified: Wed, 16 Aug 2023 01:09:07 GMT  
		Size: 1.2 MB (1164823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06785c3a618c2299d1c43c6166d218c293154f2b62388308489c543fb468fcc`  
		Last Modified: Wed, 16 Aug 2023 01:09:06 GMT  
		Size: 294.4 KB (294413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13db5751d0d30669960029c9dc9f4573eb2e498ba47ac3cd92ddd18c3d69f529`  
		Last Modified: Wed, 16 Aug 2023 01:09:06 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2d8b28c3773bf5ee838350826c5ac64584be54186987bc44818c7d9dbacc16`  
		Last Modified: Wed, 16 Aug 2023 01:09:08 GMT  
		Size: 41.1 MB (41126542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc059df8fa27f2fd0e76e73a0b57d115b58facd68cb8cc49eb0dd0d3c96451b9`  
		Last Modified: Wed, 16 Aug 2023 01:09:04 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a143b442aed69550094358e37c41a8b286b3fccbb0419d50344af0ccc584b4e`  
		Last Modified: Wed, 16 Aug 2023 01:09:04 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af3e620fbba87071b9849448da39963e51e1fa45d22c980b4186f19b63189b4`  
		Last Modified: Wed, 16 Aug 2023 01:09:04 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c8a19e4faf7dfad7e346443bfd88cbe85a3adb2f62eb3cbc8531cf73dff0343`  
		Last Modified: Wed, 16 Aug 2023 01:09:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2`

```console
$ docker pull couchdb@sha256:c265e703fa388cd5519024caa7ba66e1758fb7329bad374a5514ccb8246ea97c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2` - linux; amd64

```console
$ docker pull couchdb@sha256:00148bbe9a3ca1456e2a1696d9c1fa29939c1473fe8e52845f3c2dbeed001298
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.7 MB (89741060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1724f2a1573494de2e3af92d238849fcb5c4274b20032184f32c524310bf8b37`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:45:54 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 16 Aug 2023 01:45:54 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 16 Aug 2023 01:46:01 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:46:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 16 Aug 2023 01:46:05 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 16 Aug 2023 01:46:11 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:46:35 GMT
ENV COUCHDB_VERSION=3.2.3
# Wed, 16 Aug 2023 01:46:35 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 16 Aug 2023 01:46:48 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 16 Aug 2023 01:46:49 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 16 Aug 2023 01:46:49 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 16 Aug 2023 01:46:49 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 16 Aug 2023 01:46:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 16 Aug 2023 01:46:50 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 01:46:50 GMT
VOLUME [/opt/couchdb/data]
# Wed, 16 Aug 2023 01:46:50 GMT
EXPOSE 4369 5984 9100
# Wed, 16 Aug 2023 01:46:50 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e683ea8132b62c891a7a7001a4607c52d59cec34fffc7d4c3bf1aa23dd1f8965`  
		Last Modified: Wed, 16 Aug 2023 01:48:14 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd02df917dc89d0c9f2f3b12495a7489bd0e56a9cc24b2293dbfe9d21e97516`  
		Last Modified: Wed, 16 Aug 2023 01:48:14 GMT  
		Size: 5.2 MB (5224576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27e9a0cc8fe852d5144ed084c43083b36f5f25d8c83db408340b31dce9682b3`  
		Last Modified: Wed, 16 Aug 2023 01:48:13 GMT  
		Size: 610.3 KB (610294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91d3a3133f57276711efc489279c7c15c935fe4b9ef5200d4575a884cc2278b`  
		Last Modified: Wed, 16 Aug 2023 01:48:13 GMT  
		Size: 294.5 KB (294462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90983cf50fdcc18557085830246996e58ee3b5a031955a058da283e12d7dce2f`  
		Last Modified: Wed, 16 Aug 2023 01:48:32 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5cf53ca9445a445bee9fb7c0858ebf698c34da9a5e3ad3fe966cf42e65d179`  
		Last Modified: Wed, 16 Aug 2023 01:48:35 GMT  
		Size: 52.2 MB (52186625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8084b322d86f1e26e31148670fb28b13ea705547d9c6f1e6a741c0486913bba`  
		Last Modified: Wed, 16 Aug 2023 01:48:30 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3d5a4ee2585647085163df2fb4977642c85e78921d9a29c27313952b86db93`  
		Last Modified: Wed, 16 Aug 2023 01:48:30 GMT  
		Size: 1.0 KB (1002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412b4d7ada39f23b03adead5e9fdfc7dac07c2d04ca31d971c4826883c88911f`  
		Last Modified: Wed, 16 Aug 2023 01:48:30 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974ab2cda28305a246e9c36a26a2db168c6a44560b87b8fc35b8cc2f0f671c27`  
		Last Modified: Wed, 16 Aug 2023 01:48:30 GMT  
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
$ docker pull couchdb@sha256:60f41f8b62ff4e0f0bd398e82db42d6ef054a11498a3b3d702157fb1ee8f3c7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchdb:3.2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:00148bbe9a3ca1456e2a1696d9c1fa29939c1473fe8e52845f3c2dbeed001298
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.7 MB (89741060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1724f2a1573494de2e3af92d238849fcb5c4274b20032184f32c524310bf8b37`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:45:54 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 16 Aug 2023 01:45:54 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 16 Aug 2023 01:46:01 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:46:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 16 Aug 2023 01:46:05 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 16 Aug 2023 01:46:11 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:46:35 GMT
ENV COUCHDB_VERSION=3.2.3
# Wed, 16 Aug 2023 01:46:35 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 16 Aug 2023 01:46:48 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 16 Aug 2023 01:46:49 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 16 Aug 2023 01:46:49 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 16 Aug 2023 01:46:49 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 16 Aug 2023 01:46:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 16 Aug 2023 01:46:50 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 01:46:50 GMT
VOLUME [/opt/couchdb/data]
# Wed, 16 Aug 2023 01:46:50 GMT
EXPOSE 4369 5984 9100
# Wed, 16 Aug 2023 01:46:50 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e683ea8132b62c891a7a7001a4607c52d59cec34fffc7d4c3bf1aa23dd1f8965`  
		Last Modified: Wed, 16 Aug 2023 01:48:14 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd02df917dc89d0c9f2f3b12495a7489bd0e56a9cc24b2293dbfe9d21e97516`  
		Last Modified: Wed, 16 Aug 2023 01:48:14 GMT  
		Size: 5.2 MB (5224576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27e9a0cc8fe852d5144ed084c43083b36f5f25d8c83db408340b31dce9682b3`  
		Last Modified: Wed, 16 Aug 2023 01:48:13 GMT  
		Size: 610.3 KB (610294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91d3a3133f57276711efc489279c7c15c935fe4b9ef5200d4575a884cc2278b`  
		Last Modified: Wed, 16 Aug 2023 01:48:13 GMT  
		Size: 294.5 KB (294462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90983cf50fdcc18557085830246996e58ee3b5a031955a058da283e12d7dce2f`  
		Last Modified: Wed, 16 Aug 2023 01:48:32 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5cf53ca9445a445bee9fb7c0858ebf698c34da9a5e3ad3fe966cf42e65d179`  
		Last Modified: Wed, 16 Aug 2023 01:48:35 GMT  
		Size: 52.2 MB (52186625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8084b322d86f1e26e31148670fb28b13ea705547d9c6f1e6a741c0486913bba`  
		Last Modified: Wed, 16 Aug 2023 01:48:30 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3d5a4ee2585647085163df2fb4977642c85e78921d9a29c27313952b86db93`  
		Last Modified: Wed, 16 Aug 2023 01:48:30 GMT  
		Size: 1.0 KB (1002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412b4d7ada39f23b03adead5e9fdfc7dac07c2d04ca31d971c4826883c88911f`  
		Last Modified: Wed, 16 Aug 2023 01:48:30 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974ab2cda28305a246e9c36a26a2db168c6a44560b87b8fc35b8cc2f0f671c27`  
		Last Modified: Wed, 16 Aug 2023 01:48:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.3`

```console
$ docker pull couchdb@sha256:6187c65b7c07941701ba71695b1102383887056019d421020c455a929e9df20e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `couchdb:3.3` - linux; amd64

```console
$ docker pull couchdb@sha256:1ec2426cf9d8628f6c7126fb477f51b8c536325289cd02ce93423aaebb274540
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90240695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ca978417950e1e879ab4ddb800644f67dbd2ce4e667da20f62cb3065bba3ef6`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:45:54 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 16 Aug 2023 01:45:54 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 16 Aug 2023 01:46:01 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:46:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 16 Aug 2023 01:46:05 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 16 Aug 2023 01:46:11 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:46:11 GMT
ENV COUCHDB_VERSION=3.3.2
# Wed, 16 Aug 2023 01:46:12 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 16 Aug 2023 01:46:26 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 16 Aug 2023 01:46:26 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 16 Aug 2023 01:46:26 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 16 Aug 2023 01:46:26 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 16 Aug 2023 01:46:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 16 Aug 2023 01:46:27 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 01:46:27 GMT
VOLUME [/opt/couchdb/data]
# Wed, 16 Aug 2023 01:46:27 GMT
EXPOSE 4369 5984 9100
# Wed, 16 Aug 2023 01:46:27 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e683ea8132b62c891a7a7001a4607c52d59cec34fffc7d4c3bf1aa23dd1f8965`  
		Last Modified: Wed, 16 Aug 2023 01:48:14 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd02df917dc89d0c9f2f3b12495a7489bd0e56a9cc24b2293dbfe9d21e97516`  
		Last Modified: Wed, 16 Aug 2023 01:48:14 GMT  
		Size: 5.2 MB (5224576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27e9a0cc8fe852d5144ed084c43083b36f5f25d8c83db408340b31dce9682b3`  
		Last Modified: Wed, 16 Aug 2023 01:48:13 GMT  
		Size: 610.3 KB (610294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91d3a3133f57276711efc489279c7c15c935fe4b9ef5200d4575a884cc2278b`  
		Last Modified: Wed, 16 Aug 2023 01:48:13 GMT  
		Size: 294.5 KB (294462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777caeb656baab6032799b4a60709899a93185ed9c41616fb1d55eb35330da2d`  
		Last Modified: Wed, 16 Aug 2023 01:48:12 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b7d6bbbb71932c5cd4a76f304203e9b46721051d9f9d66bf14767e2245c782`  
		Last Modified: Wed, 16 Aug 2023 01:48:16 GMT  
		Size: 52.7 MB (52686268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ba7d950ec4c78e5f5f1a13c0f11fb294498877976e64b55b5cd1153a4e834d`  
		Last Modified: Wed, 16 Aug 2023 01:48:10 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5e496fb52a8112cf321600bf11ba4269aac657a3e33896481640e379ffc00f`  
		Last Modified: Wed, 16 Aug 2023 01:48:11 GMT  
		Size: 997.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9eec9879e73cae7da79e5eb515359d0f3d64a4ecf49554fc895830759aeb04`  
		Last Modified: Wed, 16 Aug 2023 01:48:11 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32fcbbd11bd218e1902debe81797e81a97a2ec4d352fee88ea4d6ca440127ed`  
		Last Modified: Wed, 16 Aug 2023 01:48:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:30bfee6095c98d4127df9c620886e25c170779d5713ad95fab161d49c76a7717
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88684226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77e27a374b34255c7dce27560b0ad4e0805df34a91fc50eba889ea000cc85961`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:06:55 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 16 Aug 2023 01:06:56 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 16 Aug 2023 01:07:02 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:07:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 16 Aug 2023 01:07:05 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 16 Aug 2023 01:07:09 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:07:09 GMT
ENV COUCHDB_VERSION=3.3.2
# Wed, 16 Aug 2023 01:07:10 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 16 Aug 2023 01:07:22 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 16 Aug 2023 01:07:22 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 16 Aug 2023 01:07:22 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 16 Aug 2023 01:07:22 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 16 Aug 2023 01:07:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 16 Aug 2023 01:07:23 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 01:07:23 GMT
VOLUME [/opt/couchdb/data]
# Wed, 16 Aug 2023 01:07:23 GMT
EXPOSE 4369 5984 9100
# Wed, 16 Aug 2023 01:07:23 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ff9c650b66afcfcf0aecf606a24b4f6267031943f5cb2a9bee414c9b0f89ff`  
		Last Modified: Wed, 16 Aug 2023 01:08:50 GMT  
		Size: 3.4 KB (3436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3110b3b5e035aeab66963dbd48c79553935329f1f627cf3ff4fba44e3b3081`  
		Last Modified: Wed, 16 Aug 2023 01:08:49 GMT  
		Size: 5.2 MB (5209580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0ad12d938d91082a0c04662667c6e63c489ca6b935a55600c3cacd6dfcf6e7`  
		Last Modified: Wed, 16 Aug 2023 01:08:49 GMT  
		Size: 566.3 KB (566309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dcae50ed7b69ad69869743da712f37f818c5a7d003326b5ec9c68cf4c72f7e1`  
		Last Modified: Wed, 16 Aug 2023 01:08:49 GMT  
		Size: 294.3 KB (294339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988571db89e062bd3cc3cc0078fdf2a53dbbbc812ecbc119a71eac500f13a16f`  
		Last Modified: Wed, 16 Aug 2023 01:08:48 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab992810bd02bd6e6909d87fe14dce599f8115a9fb5a7bda65679454f2df3cd8`  
		Last Modified: Wed, 16 Aug 2023 01:08:51 GMT  
		Size: 52.5 MB (52543735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2d794dbe81b85b837cf872688ea211ac7838258ef6d747164c7285fff00580`  
		Last Modified: Wed, 16 Aug 2023 01:08:47 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c31a9ad71eb77b1c29e0cd83b58631175ef07966d3237863d8cacc5d2da53b`  
		Last Modified: Wed, 16 Aug 2023 01:08:47 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0091c75d975b9376b4c8dc194ba8d46241b674cec5dae6d1111cd407f3494e2e`  
		Last Modified: Wed, 16 Aug 2023 01:08:47 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73f0fa03869f341cb2662fad33bf15697269bcb5d7181fee4c6d43032074d7d`  
		Last Modified: Wed, 16 Aug 2023 01:08:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3` - linux; ppc64le

```console
$ docker pull couchdb@sha256:8e06df720f4e07d7c1aceefc45eb9f61d7d7d61fb5e3de18c1083b2f63b95f3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.0 MB (95962013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7747f406a39fb87acae729b3f33ef6b5ce3045b048a6c936e80994acea2ec6ca`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 16 Aug 2023 01:10:12 GMT
ADD file:eeb766a3bb0461f0baa2425cfd43628994c064bd728f51f1b8df659a4bd2f489 in / 
# Wed, 16 Aug 2023 01:10:14 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 02:19:08 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 16 Aug 2023 02:19:11 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 16 Aug 2023 02:19:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 02:19:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 16 Aug 2023 02:19:49 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 16 Aug 2023 02:20:10 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 02:20:11 GMT
ENV COUCHDB_VERSION=3.3.2
# Wed, 16 Aug 2023 02:20:12 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 16 Aug 2023 02:20:44 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 16 Aug 2023 02:20:46 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 16 Aug 2023 02:20:46 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 16 Aug 2023 02:20:46 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 16 Aug 2023 02:20:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 16 Aug 2023 02:20:48 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 02:20:49 GMT
VOLUME [/opt/couchdb/data]
# Wed, 16 Aug 2023 02:20:49 GMT
EXPOSE 4369 5984 9100
# Wed, 16 Aug 2023 02:20:49 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:dacf4195c8a0403fd11459739bf9dc9be427261bf5e0bedb49e18d1498cf7c2e`  
		Last Modified: Wed, 16 Aug 2023 01:17:04 GMT  
		Size: 35.3 MB (35291067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e6a8655a620cffbe60c27dd03f9c5d03132e3fffd3e788526b63d70a3c6685`  
		Last Modified: Wed, 16 Aug 2023 02:21:45 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8a4468de45ced49ad8e3c084adfde3e9e39622bd4eefd7b50b2845c9f0748d`  
		Last Modified: Wed, 16 Aug 2023 02:21:45 GMT  
		Size: 6.0 MB (6044086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998ea43aefd6709362b0f13d999f80bbe87042afe3dc4d60e1d82a42a55017a0`  
		Last Modified: Wed, 16 Aug 2023 02:21:44 GMT  
		Size: 662.1 KB (662144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984bdece6eec3b2c06e59a0fc3ff6a3f4913dd41fda95c2a93ef7666c9faf49f`  
		Last Modified: Wed, 16 Aug 2023 02:21:44 GMT  
		Size: 294.4 KB (294359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289a2e380dbf7483fe7b0cb2a996ee515d9d0ad6782ced49cf64020a5331006c`  
		Last Modified: Wed, 16 Aug 2023 02:21:43 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ea07c066dd201b35d53a50df457fbf1aa89df808344455301d3b1d4157b30a`  
		Last Modified: Wed, 16 Aug 2023 02:21:50 GMT  
		Size: 53.7 MB (53662934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914b28fa3462815c14ab9660b2071c0f7e31f60935409831159e43a25a1b8f42`  
		Last Modified: Wed, 16 Aug 2023 02:21:41 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b653561e98b96ac3aaf3c9e0b5e4a86c1d2dda60e8f8463e9ea907b1c8b4f7a`  
		Last Modified: Wed, 16 Aug 2023 02:21:41 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16ed1d5bfe33233a937efc507eefb39df037724ea0e34f59328c1e8a7ee9f6a`  
		Last Modified: Wed, 16 Aug 2023 02:21:41 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe53b7a249ba7d07fdfbc4f2cf836d068d1b1e0d8d6af0594d6bca247c94736`  
		Last Modified: Wed, 16 Aug 2023 02:21:41 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3` - linux; s390x

```console
$ docker pull couchdb@sha256:29e829b586b1cb6e650b0e13797721b362071a74370a5f6680669c847090f45a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.0 MB (86992619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:192ddd69ff7e41d2bdf0975625c068953c9226f56fe985a51b032813e5bb8c66`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 07 Sep 2023 00:44:33 GMT
ADD file:fb2f216acd6d0ecaf48e8d5dd7e3cdb5d1f51d414f2011ed318cb494f96d89ca in / 
# Thu, 07 Sep 2023 00:44:37 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:28:56 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 07 Sep 2023 01:28:58 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 07 Sep 2023 01:29:11 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:29:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Thu, 07 Sep 2023 01:29:17 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 07 Sep 2023 01:29:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:29:27 GMT
ENV COUCHDB_VERSION=3.3.2
# Thu, 07 Sep 2023 01:29:28 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 07 Sep 2023 01:29:56 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 07 Sep 2023 01:30:05 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 07 Sep 2023 01:30:05 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Thu, 07 Sep 2023 01:30:05 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Thu, 07 Sep 2023 01:30:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 07 Sep 2023 01:30:07 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 07 Sep 2023 01:30:07 GMT
VOLUME [/opt/couchdb/data]
# Thu, 07 Sep 2023 01:30:08 GMT
EXPOSE 4369 5984 9100
# Thu, 07 Sep 2023 01:30:09 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:c9501ad9402d64e6c612fa1bb94f16df51188e681dc1f28c603a6109f06f22d7`  
		Last Modified: Thu, 07 Sep 2023 00:50:10 GMT  
		Size: 29.7 MB (29652801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996ad4371fbc51ce08543507129d65ab8b90dd855e656f8eabd70335c57bb0a1`  
		Last Modified: Thu, 07 Sep 2023 01:30:26 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e0fe5808ef043ae040668477d7e9dfe710765ea40e3d011b82fa33031b7ea4`  
		Last Modified: Thu, 07 Sep 2023 01:30:25 GMT  
		Size: 5.1 MB (5110534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f126aebc8a50e39748585e27d5fd5a9836b6a93c873802d3d3403b156cac952`  
		Last Modified: Thu, 07 Sep 2023 01:30:25 GMT  
		Size: 573.0 KB (573029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f00d25b2e1271b6380742fbbeca5c10b9b084a78cfba7f031f12a3d00a87df5`  
		Last Modified: Thu, 07 Sep 2023 01:30:24 GMT  
		Size: 294.5 KB (294462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577394d2327382521d14f38714c2247fd0db46e1ab49b86cb2350c309835db81`  
		Last Modified: Thu, 07 Sep 2023 01:30:24 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4258fc35f99c32658815e5ea98c85edc9f278bcba6613030c57395fc75cae139`  
		Last Modified: Thu, 07 Sep 2023 01:30:28 GMT  
		Size: 51.4 MB (51354348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0bdcf38e015804f9400dd02e2614c14ea270ce30cfc9602fc0bf39c87dd1fb`  
		Last Modified: Thu, 07 Sep 2023 01:30:23 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67bc37b8d392d13a0a6a7312678435efade4fd7449ec2ed52945c52abe3b85d`  
		Last Modified: Thu, 07 Sep 2023 01:30:23 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3410bb24e7a70dfce7810cf4736b3f0e0a420444d7825a7d1a9a1309c56e7e`  
		Last Modified: Thu, 07 Sep 2023 01:30:23 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e526b2a03229b6f0cd56ffc8d6c5600b8eec7f407d56686697c3684634adbc52`  
		Last Modified: Thu, 07 Sep 2023 01:30:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.3.2`

```console
$ docker pull couchdb@sha256:6187c65b7c07941701ba71695b1102383887056019d421020c455a929e9df20e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `couchdb:3.3.2` - linux; amd64

```console
$ docker pull couchdb@sha256:1ec2426cf9d8628f6c7126fb477f51b8c536325289cd02ce93423aaebb274540
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90240695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ca978417950e1e879ab4ddb800644f67dbd2ce4e667da20f62cb3065bba3ef6`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:45:54 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 16 Aug 2023 01:45:54 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 16 Aug 2023 01:46:01 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:46:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 16 Aug 2023 01:46:05 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 16 Aug 2023 01:46:11 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:46:11 GMT
ENV COUCHDB_VERSION=3.3.2
# Wed, 16 Aug 2023 01:46:12 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 16 Aug 2023 01:46:26 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 16 Aug 2023 01:46:26 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 16 Aug 2023 01:46:26 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 16 Aug 2023 01:46:26 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 16 Aug 2023 01:46:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 16 Aug 2023 01:46:27 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 01:46:27 GMT
VOLUME [/opt/couchdb/data]
# Wed, 16 Aug 2023 01:46:27 GMT
EXPOSE 4369 5984 9100
# Wed, 16 Aug 2023 01:46:27 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e683ea8132b62c891a7a7001a4607c52d59cec34fffc7d4c3bf1aa23dd1f8965`  
		Last Modified: Wed, 16 Aug 2023 01:48:14 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd02df917dc89d0c9f2f3b12495a7489bd0e56a9cc24b2293dbfe9d21e97516`  
		Last Modified: Wed, 16 Aug 2023 01:48:14 GMT  
		Size: 5.2 MB (5224576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27e9a0cc8fe852d5144ed084c43083b36f5f25d8c83db408340b31dce9682b3`  
		Last Modified: Wed, 16 Aug 2023 01:48:13 GMT  
		Size: 610.3 KB (610294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91d3a3133f57276711efc489279c7c15c935fe4b9ef5200d4575a884cc2278b`  
		Last Modified: Wed, 16 Aug 2023 01:48:13 GMT  
		Size: 294.5 KB (294462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777caeb656baab6032799b4a60709899a93185ed9c41616fb1d55eb35330da2d`  
		Last Modified: Wed, 16 Aug 2023 01:48:12 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b7d6bbbb71932c5cd4a76f304203e9b46721051d9f9d66bf14767e2245c782`  
		Last Modified: Wed, 16 Aug 2023 01:48:16 GMT  
		Size: 52.7 MB (52686268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ba7d950ec4c78e5f5f1a13c0f11fb294498877976e64b55b5cd1153a4e834d`  
		Last Modified: Wed, 16 Aug 2023 01:48:10 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5e496fb52a8112cf321600bf11ba4269aac657a3e33896481640e379ffc00f`  
		Last Modified: Wed, 16 Aug 2023 01:48:11 GMT  
		Size: 997.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9eec9879e73cae7da79e5eb515359d0f3d64a4ecf49554fc895830759aeb04`  
		Last Modified: Wed, 16 Aug 2023 01:48:11 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32fcbbd11bd218e1902debe81797e81a97a2ec4d352fee88ea4d6ca440127ed`  
		Last Modified: Wed, 16 Aug 2023 01:48:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:30bfee6095c98d4127df9c620886e25c170779d5713ad95fab161d49c76a7717
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88684226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77e27a374b34255c7dce27560b0ad4e0805df34a91fc50eba889ea000cc85961`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:06:55 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 16 Aug 2023 01:06:56 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 16 Aug 2023 01:07:02 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:07:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 16 Aug 2023 01:07:05 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 16 Aug 2023 01:07:09 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:07:09 GMT
ENV COUCHDB_VERSION=3.3.2
# Wed, 16 Aug 2023 01:07:10 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 16 Aug 2023 01:07:22 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 16 Aug 2023 01:07:22 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 16 Aug 2023 01:07:22 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 16 Aug 2023 01:07:22 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 16 Aug 2023 01:07:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 16 Aug 2023 01:07:23 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 01:07:23 GMT
VOLUME [/opt/couchdb/data]
# Wed, 16 Aug 2023 01:07:23 GMT
EXPOSE 4369 5984 9100
# Wed, 16 Aug 2023 01:07:23 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ff9c650b66afcfcf0aecf606a24b4f6267031943f5cb2a9bee414c9b0f89ff`  
		Last Modified: Wed, 16 Aug 2023 01:08:50 GMT  
		Size: 3.4 KB (3436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3110b3b5e035aeab66963dbd48c79553935329f1f627cf3ff4fba44e3b3081`  
		Last Modified: Wed, 16 Aug 2023 01:08:49 GMT  
		Size: 5.2 MB (5209580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0ad12d938d91082a0c04662667c6e63c489ca6b935a55600c3cacd6dfcf6e7`  
		Last Modified: Wed, 16 Aug 2023 01:08:49 GMT  
		Size: 566.3 KB (566309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dcae50ed7b69ad69869743da712f37f818c5a7d003326b5ec9c68cf4c72f7e1`  
		Last Modified: Wed, 16 Aug 2023 01:08:49 GMT  
		Size: 294.3 KB (294339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988571db89e062bd3cc3cc0078fdf2a53dbbbc812ecbc119a71eac500f13a16f`  
		Last Modified: Wed, 16 Aug 2023 01:08:48 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab992810bd02bd6e6909d87fe14dce599f8115a9fb5a7bda65679454f2df3cd8`  
		Last Modified: Wed, 16 Aug 2023 01:08:51 GMT  
		Size: 52.5 MB (52543735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2d794dbe81b85b837cf872688ea211ac7838258ef6d747164c7285fff00580`  
		Last Modified: Wed, 16 Aug 2023 01:08:47 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c31a9ad71eb77b1c29e0cd83b58631175ef07966d3237863d8cacc5d2da53b`  
		Last Modified: Wed, 16 Aug 2023 01:08:47 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0091c75d975b9376b4c8dc194ba8d46241b674cec5dae6d1111cd407f3494e2e`  
		Last Modified: Wed, 16 Aug 2023 01:08:47 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73f0fa03869f341cb2662fad33bf15697269bcb5d7181fee4c6d43032074d7d`  
		Last Modified: Wed, 16 Aug 2023 01:08:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3.2` - linux; ppc64le

```console
$ docker pull couchdb@sha256:8e06df720f4e07d7c1aceefc45eb9f61d7d7d61fb5e3de18c1083b2f63b95f3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.0 MB (95962013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7747f406a39fb87acae729b3f33ef6b5ce3045b048a6c936e80994acea2ec6ca`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 16 Aug 2023 01:10:12 GMT
ADD file:eeb766a3bb0461f0baa2425cfd43628994c064bd728f51f1b8df659a4bd2f489 in / 
# Wed, 16 Aug 2023 01:10:14 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 02:19:08 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 16 Aug 2023 02:19:11 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 16 Aug 2023 02:19:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 02:19:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 16 Aug 2023 02:19:49 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 16 Aug 2023 02:20:10 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 02:20:11 GMT
ENV COUCHDB_VERSION=3.3.2
# Wed, 16 Aug 2023 02:20:12 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 16 Aug 2023 02:20:44 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 16 Aug 2023 02:20:46 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 16 Aug 2023 02:20:46 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 16 Aug 2023 02:20:46 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 16 Aug 2023 02:20:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 16 Aug 2023 02:20:48 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 02:20:49 GMT
VOLUME [/opt/couchdb/data]
# Wed, 16 Aug 2023 02:20:49 GMT
EXPOSE 4369 5984 9100
# Wed, 16 Aug 2023 02:20:49 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:dacf4195c8a0403fd11459739bf9dc9be427261bf5e0bedb49e18d1498cf7c2e`  
		Last Modified: Wed, 16 Aug 2023 01:17:04 GMT  
		Size: 35.3 MB (35291067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e6a8655a620cffbe60c27dd03f9c5d03132e3fffd3e788526b63d70a3c6685`  
		Last Modified: Wed, 16 Aug 2023 02:21:45 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8a4468de45ced49ad8e3c084adfde3e9e39622bd4eefd7b50b2845c9f0748d`  
		Last Modified: Wed, 16 Aug 2023 02:21:45 GMT  
		Size: 6.0 MB (6044086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998ea43aefd6709362b0f13d999f80bbe87042afe3dc4d60e1d82a42a55017a0`  
		Last Modified: Wed, 16 Aug 2023 02:21:44 GMT  
		Size: 662.1 KB (662144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984bdece6eec3b2c06e59a0fc3ff6a3f4913dd41fda95c2a93ef7666c9faf49f`  
		Last Modified: Wed, 16 Aug 2023 02:21:44 GMT  
		Size: 294.4 KB (294359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289a2e380dbf7483fe7b0cb2a996ee515d9d0ad6782ced49cf64020a5331006c`  
		Last Modified: Wed, 16 Aug 2023 02:21:43 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ea07c066dd201b35d53a50df457fbf1aa89df808344455301d3b1d4157b30a`  
		Last Modified: Wed, 16 Aug 2023 02:21:50 GMT  
		Size: 53.7 MB (53662934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914b28fa3462815c14ab9660b2071c0f7e31f60935409831159e43a25a1b8f42`  
		Last Modified: Wed, 16 Aug 2023 02:21:41 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b653561e98b96ac3aaf3c9e0b5e4a86c1d2dda60e8f8463e9ea907b1c8b4f7a`  
		Last Modified: Wed, 16 Aug 2023 02:21:41 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16ed1d5bfe33233a937efc507eefb39df037724ea0e34f59328c1e8a7ee9f6a`  
		Last Modified: Wed, 16 Aug 2023 02:21:41 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe53b7a249ba7d07fdfbc4f2cf836d068d1b1e0d8d6af0594d6bca247c94736`  
		Last Modified: Wed, 16 Aug 2023 02:21:41 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3.2` - linux; s390x

```console
$ docker pull couchdb@sha256:29e829b586b1cb6e650b0e13797721b362071a74370a5f6680669c847090f45a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.0 MB (86992619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:192ddd69ff7e41d2bdf0975625c068953c9226f56fe985a51b032813e5bb8c66`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 07 Sep 2023 00:44:33 GMT
ADD file:fb2f216acd6d0ecaf48e8d5dd7e3cdb5d1f51d414f2011ed318cb494f96d89ca in / 
# Thu, 07 Sep 2023 00:44:37 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:28:56 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 07 Sep 2023 01:28:58 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 07 Sep 2023 01:29:11 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:29:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Thu, 07 Sep 2023 01:29:17 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 07 Sep 2023 01:29:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:29:27 GMT
ENV COUCHDB_VERSION=3.3.2
# Thu, 07 Sep 2023 01:29:28 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 07 Sep 2023 01:29:56 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 07 Sep 2023 01:30:05 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 07 Sep 2023 01:30:05 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Thu, 07 Sep 2023 01:30:05 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Thu, 07 Sep 2023 01:30:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 07 Sep 2023 01:30:07 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 07 Sep 2023 01:30:07 GMT
VOLUME [/opt/couchdb/data]
# Thu, 07 Sep 2023 01:30:08 GMT
EXPOSE 4369 5984 9100
# Thu, 07 Sep 2023 01:30:09 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:c9501ad9402d64e6c612fa1bb94f16df51188e681dc1f28c603a6109f06f22d7`  
		Last Modified: Thu, 07 Sep 2023 00:50:10 GMT  
		Size: 29.7 MB (29652801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996ad4371fbc51ce08543507129d65ab8b90dd855e656f8eabd70335c57bb0a1`  
		Last Modified: Thu, 07 Sep 2023 01:30:26 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e0fe5808ef043ae040668477d7e9dfe710765ea40e3d011b82fa33031b7ea4`  
		Last Modified: Thu, 07 Sep 2023 01:30:25 GMT  
		Size: 5.1 MB (5110534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f126aebc8a50e39748585e27d5fd5a9836b6a93c873802d3d3403b156cac952`  
		Last Modified: Thu, 07 Sep 2023 01:30:25 GMT  
		Size: 573.0 KB (573029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f00d25b2e1271b6380742fbbeca5c10b9b084a78cfba7f031f12a3d00a87df5`  
		Last Modified: Thu, 07 Sep 2023 01:30:24 GMT  
		Size: 294.5 KB (294462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577394d2327382521d14f38714c2247fd0db46e1ab49b86cb2350c309835db81`  
		Last Modified: Thu, 07 Sep 2023 01:30:24 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4258fc35f99c32658815e5ea98c85edc9f278bcba6613030c57395fc75cae139`  
		Last Modified: Thu, 07 Sep 2023 01:30:28 GMT  
		Size: 51.4 MB (51354348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0bdcf38e015804f9400dd02e2614c14ea270ce30cfc9602fc0bf39c87dd1fb`  
		Last Modified: Thu, 07 Sep 2023 01:30:23 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67bc37b8d392d13a0a6a7312678435efade4fd7449ec2ed52945c52abe3b85d`  
		Last Modified: Thu, 07 Sep 2023 01:30:23 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3410bb24e7a70dfce7810cf4736b3f0e0a420444d7825a7d1a9a1309c56e7e`  
		Last Modified: Thu, 07 Sep 2023 01:30:23 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e526b2a03229b6f0cd56ffc8d6c5600b8eec7f407d56686697c3684634adbc52`  
		Last Modified: Thu, 07 Sep 2023 01:30:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:latest`

```console
$ docker pull couchdb@sha256:6187c65b7c07941701ba71695b1102383887056019d421020c455a929e9df20e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:1ec2426cf9d8628f6c7126fb477f51b8c536325289cd02ce93423aaebb274540
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90240695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ca978417950e1e879ab4ddb800644f67dbd2ce4e667da20f62cb3065bba3ef6`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:45:54 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 16 Aug 2023 01:45:54 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 16 Aug 2023 01:46:01 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:46:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 16 Aug 2023 01:46:05 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 16 Aug 2023 01:46:11 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:46:11 GMT
ENV COUCHDB_VERSION=3.3.2
# Wed, 16 Aug 2023 01:46:12 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 16 Aug 2023 01:46:26 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 16 Aug 2023 01:46:26 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 16 Aug 2023 01:46:26 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 16 Aug 2023 01:46:26 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 16 Aug 2023 01:46:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 16 Aug 2023 01:46:27 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 01:46:27 GMT
VOLUME [/opt/couchdb/data]
# Wed, 16 Aug 2023 01:46:27 GMT
EXPOSE 4369 5984 9100
# Wed, 16 Aug 2023 01:46:27 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e683ea8132b62c891a7a7001a4607c52d59cec34fffc7d4c3bf1aa23dd1f8965`  
		Last Modified: Wed, 16 Aug 2023 01:48:14 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd02df917dc89d0c9f2f3b12495a7489bd0e56a9cc24b2293dbfe9d21e97516`  
		Last Modified: Wed, 16 Aug 2023 01:48:14 GMT  
		Size: 5.2 MB (5224576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27e9a0cc8fe852d5144ed084c43083b36f5f25d8c83db408340b31dce9682b3`  
		Last Modified: Wed, 16 Aug 2023 01:48:13 GMT  
		Size: 610.3 KB (610294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91d3a3133f57276711efc489279c7c15c935fe4b9ef5200d4575a884cc2278b`  
		Last Modified: Wed, 16 Aug 2023 01:48:13 GMT  
		Size: 294.5 KB (294462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777caeb656baab6032799b4a60709899a93185ed9c41616fb1d55eb35330da2d`  
		Last Modified: Wed, 16 Aug 2023 01:48:12 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b7d6bbbb71932c5cd4a76f304203e9b46721051d9f9d66bf14767e2245c782`  
		Last Modified: Wed, 16 Aug 2023 01:48:16 GMT  
		Size: 52.7 MB (52686268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ba7d950ec4c78e5f5f1a13c0f11fb294498877976e64b55b5cd1153a4e834d`  
		Last Modified: Wed, 16 Aug 2023 01:48:10 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5e496fb52a8112cf321600bf11ba4269aac657a3e33896481640e379ffc00f`  
		Last Modified: Wed, 16 Aug 2023 01:48:11 GMT  
		Size: 997.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9eec9879e73cae7da79e5eb515359d0f3d64a4ecf49554fc895830759aeb04`  
		Last Modified: Wed, 16 Aug 2023 01:48:11 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32fcbbd11bd218e1902debe81797e81a97a2ec4d352fee88ea4d6ca440127ed`  
		Last Modified: Wed, 16 Aug 2023 01:48:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:30bfee6095c98d4127df9c620886e25c170779d5713ad95fab161d49c76a7717
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88684226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77e27a374b34255c7dce27560b0ad4e0805df34a91fc50eba889ea000cc85961`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:06:55 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 16 Aug 2023 01:06:56 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 16 Aug 2023 01:07:02 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:07:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 16 Aug 2023 01:07:05 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 16 Aug 2023 01:07:09 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:07:09 GMT
ENV COUCHDB_VERSION=3.3.2
# Wed, 16 Aug 2023 01:07:10 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 16 Aug 2023 01:07:22 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 16 Aug 2023 01:07:22 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 16 Aug 2023 01:07:22 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 16 Aug 2023 01:07:22 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 16 Aug 2023 01:07:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 16 Aug 2023 01:07:23 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 01:07:23 GMT
VOLUME [/opt/couchdb/data]
# Wed, 16 Aug 2023 01:07:23 GMT
EXPOSE 4369 5984 9100
# Wed, 16 Aug 2023 01:07:23 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ff9c650b66afcfcf0aecf606a24b4f6267031943f5cb2a9bee414c9b0f89ff`  
		Last Modified: Wed, 16 Aug 2023 01:08:50 GMT  
		Size: 3.4 KB (3436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3110b3b5e035aeab66963dbd48c79553935329f1f627cf3ff4fba44e3b3081`  
		Last Modified: Wed, 16 Aug 2023 01:08:49 GMT  
		Size: 5.2 MB (5209580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0ad12d938d91082a0c04662667c6e63c489ca6b935a55600c3cacd6dfcf6e7`  
		Last Modified: Wed, 16 Aug 2023 01:08:49 GMT  
		Size: 566.3 KB (566309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dcae50ed7b69ad69869743da712f37f818c5a7d003326b5ec9c68cf4c72f7e1`  
		Last Modified: Wed, 16 Aug 2023 01:08:49 GMT  
		Size: 294.3 KB (294339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988571db89e062bd3cc3cc0078fdf2a53dbbbc812ecbc119a71eac500f13a16f`  
		Last Modified: Wed, 16 Aug 2023 01:08:48 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab992810bd02bd6e6909d87fe14dce599f8115a9fb5a7bda65679454f2df3cd8`  
		Last Modified: Wed, 16 Aug 2023 01:08:51 GMT  
		Size: 52.5 MB (52543735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2d794dbe81b85b837cf872688ea211ac7838258ef6d747164c7285fff00580`  
		Last Modified: Wed, 16 Aug 2023 01:08:47 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c31a9ad71eb77b1c29e0cd83b58631175ef07966d3237863d8cacc5d2da53b`  
		Last Modified: Wed, 16 Aug 2023 01:08:47 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0091c75d975b9376b4c8dc194ba8d46241b674cec5dae6d1111cd407f3494e2e`  
		Last Modified: Wed, 16 Aug 2023 01:08:47 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73f0fa03869f341cb2662fad33bf15697269bcb5d7181fee4c6d43032074d7d`  
		Last Modified: Wed, 16 Aug 2023 01:08:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; ppc64le

```console
$ docker pull couchdb@sha256:8e06df720f4e07d7c1aceefc45eb9f61d7d7d61fb5e3de18c1083b2f63b95f3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.0 MB (95962013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7747f406a39fb87acae729b3f33ef6b5ce3045b048a6c936e80994acea2ec6ca`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 16 Aug 2023 01:10:12 GMT
ADD file:eeb766a3bb0461f0baa2425cfd43628994c064bd728f51f1b8df659a4bd2f489 in / 
# Wed, 16 Aug 2023 01:10:14 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 02:19:08 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 16 Aug 2023 02:19:11 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 16 Aug 2023 02:19:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 02:19:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 16 Aug 2023 02:19:49 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 16 Aug 2023 02:20:10 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 02:20:11 GMT
ENV COUCHDB_VERSION=3.3.2
# Wed, 16 Aug 2023 02:20:12 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 16 Aug 2023 02:20:44 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 16 Aug 2023 02:20:46 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 16 Aug 2023 02:20:46 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 16 Aug 2023 02:20:46 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 16 Aug 2023 02:20:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 16 Aug 2023 02:20:48 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 02:20:49 GMT
VOLUME [/opt/couchdb/data]
# Wed, 16 Aug 2023 02:20:49 GMT
EXPOSE 4369 5984 9100
# Wed, 16 Aug 2023 02:20:49 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:dacf4195c8a0403fd11459739bf9dc9be427261bf5e0bedb49e18d1498cf7c2e`  
		Last Modified: Wed, 16 Aug 2023 01:17:04 GMT  
		Size: 35.3 MB (35291067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e6a8655a620cffbe60c27dd03f9c5d03132e3fffd3e788526b63d70a3c6685`  
		Last Modified: Wed, 16 Aug 2023 02:21:45 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8a4468de45ced49ad8e3c084adfde3e9e39622bd4eefd7b50b2845c9f0748d`  
		Last Modified: Wed, 16 Aug 2023 02:21:45 GMT  
		Size: 6.0 MB (6044086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998ea43aefd6709362b0f13d999f80bbe87042afe3dc4d60e1d82a42a55017a0`  
		Last Modified: Wed, 16 Aug 2023 02:21:44 GMT  
		Size: 662.1 KB (662144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984bdece6eec3b2c06e59a0fc3ff6a3f4913dd41fda95c2a93ef7666c9faf49f`  
		Last Modified: Wed, 16 Aug 2023 02:21:44 GMT  
		Size: 294.4 KB (294359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289a2e380dbf7483fe7b0cb2a996ee515d9d0ad6782ced49cf64020a5331006c`  
		Last Modified: Wed, 16 Aug 2023 02:21:43 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ea07c066dd201b35d53a50df457fbf1aa89df808344455301d3b1d4157b30a`  
		Last Modified: Wed, 16 Aug 2023 02:21:50 GMT  
		Size: 53.7 MB (53662934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914b28fa3462815c14ab9660b2071c0f7e31f60935409831159e43a25a1b8f42`  
		Last Modified: Wed, 16 Aug 2023 02:21:41 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b653561e98b96ac3aaf3c9e0b5e4a86c1d2dda60e8f8463e9ea907b1c8b4f7a`  
		Last Modified: Wed, 16 Aug 2023 02:21:41 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16ed1d5bfe33233a937efc507eefb39df037724ea0e34f59328c1e8a7ee9f6a`  
		Last Modified: Wed, 16 Aug 2023 02:21:41 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe53b7a249ba7d07fdfbc4f2cf836d068d1b1e0d8d6af0594d6bca247c94736`  
		Last Modified: Wed, 16 Aug 2023 02:21:41 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; s390x

```console
$ docker pull couchdb@sha256:29e829b586b1cb6e650b0e13797721b362071a74370a5f6680669c847090f45a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.0 MB (86992619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:192ddd69ff7e41d2bdf0975625c068953c9226f56fe985a51b032813e5bb8c66`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 07 Sep 2023 00:44:33 GMT
ADD file:fb2f216acd6d0ecaf48e8d5dd7e3cdb5d1f51d414f2011ed318cb494f96d89ca in / 
# Thu, 07 Sep 2023 00:44:37 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:28:56 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 07 Sep 2023 01:28:58 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 07 Sep 2023 01:29:11 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:29:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Thu, 07 Sep 2023 01:29:17 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 07 Sep 2023 01:29:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:29:27 GMT
ENV COUCHDB_VERSION=3.3.2
# Thu, 07 Sep 2023 01:29:28 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 07 Sep 2023 01:29:56 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 07 Sep 2023 01:30:05 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 07 Sep 2023 01:30:05 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Thu, 07 Sep 2023 01:30:05 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Thu, 07 Sep 2023 01:30:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 07 Sep 2023 01:30:07 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 07 Sep 2023 01:30:07 GMT
VOLUME [/opt/couchdb/data]
# Thu, 07 Sep 2023 01:30:08 GMT
EXPOSE 4369 5984 9100
# Thu, 07 Sep 2023 01:30:09 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:c9501ad9402d64e6c612fa1bb94f16df51188e681dc1f28c603a6109f06f22d7`  
		Last Modified: Thu, 07 Sep 2023 00:50:10 GMT  
		Size: 29.7 MB (29652801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996ad4371fbc51ce08543507129d65ab8b90dd855e656f8eabd70335c57bb0a1`  
		Last Modified: Thu, 07 Sep 2023 01:30:26 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e0fe5808ef043ae040668477d7e9dfe710765ea40e3d011b82fa33031b7ea4`  
		Last Modified: Thu, 07 Sep 2023 01:30:25 GMT  
		Size: 5.1 MB (5110534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f126aebc8a50e39748585e27d5fd5a9836b6a93c873802d3d3403b156cac952`  
		Last Modified: Thu, 07 Sep 2023 01:30:25 GMT  
		Size: 573.0 KB (573029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f00d25b2e1271b6380742fbbeca5c10b9b084a78cfba7f031f12a3d00a87df5`  
		Last Modified: Thu, 07 Sep 2023 01:30:24 GMT  
		Size: 294.5 KB (294462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577394d2327382521d14f38714c2247fd0db46e1ab49b86cb2350c309835db81`  
		Last Modified: Thu, 07 Sep 2023 01:30:24 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4258fc35f99c32658815e5ea98c85edc9f278bcba6613030c57395fc75cae139`  
		Last Modified: Thu, 07 Sep 2023 01:30:28 GMT  
		Size: 51.4 MB (51354348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0bdcf38e015804f9400dd02e2614c14ea270ce30cfc9602fc0bf39c87dd1fb`  
		Last Modified: Thu, 07 Sep 2023 01:30:23 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67bc37b8d392d13a0a6a7312678435efade4fd7449ec2ed52945c52abe3b85d`  
		Last Modified: Thu, 07 Sep 2023 01:30:23 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3410bb24e7a70dfce7810cf4736b3f0e0a420444d7825a7d1a9a1309c56e7e`  
		Last Modified: Thu, 07 Sep 2023 01:30:23 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e526b2a03229b6f0cd56ffc8d6c5600b8eec7f407d56686697c3684634adbc52`  
		Last Modified: Thu, 07 Sep 2023 01:30:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
