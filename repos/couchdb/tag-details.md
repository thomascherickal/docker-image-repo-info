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
$ docker pull couchdb@sha256:8cf71a3a657d18dc0358402a2ea414f310cc2d4d7b12da5204f431c06c1d1c0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2` - linux; amd64

```console
$ docker pull couchdb@sha256:6deabbe84258c2151a91a3a82e6d127b2bcce1bb6b8659be675ca4005c795acc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.6 MB (84590179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5b72c4b3a9488f8358040dab8d2a1945460a6a17f63aa229e34e6831fe43f53`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:29 GMT
ADD file:20e7ad6bec617357895302b08431eb3430cce3113bdf0a8ff9827115f858d313 in / 
# Thu, 27 Jul 2023 23:25:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:54:43 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 28 Jul 2023 00:54:43 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 28 Jul 2023 00:54:53 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:54:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Fri, 28 Jul 2023 00:54:57 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Fri, 28 Jul 2023 00:55:04 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:55:24 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Fri, 28 Jul 2023 00:55:24 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Fri, 28 Jul 2023 00:55:43 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 28 Jul 2023 00:55:43 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Fri, 28 Jul 2023 00:55:43 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 28 Jul 2023 00:55:43 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Fri, 28 Jul 2023 00:55:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 00:55:44 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 00:55:44 GMT
VOLUME [/opt/couchdb/data]
# Fri, 28 Jul 2023 00:55:44 GMT
EXPOSE 4369 5984 9100
# Fri, 28 Jul 2023 00:55:44 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:3240fe174df9a5a4923c4b52f1d887dd1ad1a9ee69245c1fb867f399167584dd`  
		Last Modified: Thu, 27 Jul 2023 23:30:49 GMT  
		Size: 27.2 MB (27187431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d89b65f2dc832c2f7c348d9f12cf4b9e110e543efc4813b9f870c494429957`  
		Last Modified: Fri, 28 Jul 2023 00:56:38 GMT  
		Size: 3.4 KB (3416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef28276cebf24c8afba60bbb3445613b21460493b508d02d292c0fdd8b18f44`  
		Last Modified: Fri, 28 Jul 2023 00:56:37 GMT  
		Size: 6.7 MB (6704542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c905d0380fb2306d3e35170fbbc2bc64a4128012ea5e12393ed06dff6c5ce8b6`  
		Last Modified: Fri, 28 Jul 2023 00:56:36 GMT  
		Size: 1.3 MB (1259891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7672fd27b19b3a699dcc283d34f31cc9ef507fb4b8905d4d8ab9528e4ffbf8e3`  
		Last Modified: Fri, 28 Jul 2023 00:56:36 GMT  
		Size: 294.6 KB (294631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc9781684c058f6264128d586906d723e7969eb84e485a50c109c9df1973a30`  
		Last Modified: Fri, 28 Jul 2023 00:56:50 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9869b39f486c4ca6de8c713784e3c26bd689c63fb1c2417b420234c072a4e12e`  
		Last Modified: Fri, 28 Jul 2023 00:56:54 GMT  
		Size: 49.1 MB (49136664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840995d1ded1168d5abac83569f50653b98a44cb3bc3f81f02bdf77708ddef05`  
		Last Modified: Fri, 28 Jul 2023 00:56:48 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3f31d9c327854d02f8a037f4c6af150724e0f819fa2a2583856c6affbe5fc6`  
		Last Modified: Fri, 28 Jul 2023 00:56:48 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7955f1dacbb3649aba741a5cb06aa8ecf9f8e906d4cc0c41255e803b54803dc6`  
		Last Modified: Fri, 28 Jul 2023 00:56:48 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51fdd11a7c5ae8e5a94524653edad7bf72a6b28465d450065fe16a236c989446`  
		Last Modified: Fri, 28 Jul 2023 00:56:48 GMT  
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
$ docker pull couchdb@sha256:8cf71a3a657d18dc0358402a2ea414f310cc2d4d7b12da5204f431c06c1d1c0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:6deabbe84258c2151a91a3a82e6d127b2bcce1bb6b8659be675ca4005c795acc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.6 MB (84590179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5b72c4b3a9488f8358040dab8d2a1945460a6a17f63aa229e34e6831fe43f53`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:29 GMT
ADD file:20e7ad6bec617357895302b08431eb3430cce3113bdf0a8ff9827115f858d313 in / 
# Thu, 27 Jul 2023 23:25:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:54:43 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 28 Jul 2023 00:54:43 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 28 Jul 2023 00:54:53 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:54:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Fri, 28 Jul 2023 00:54:57 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Fri, 28 Jul 2023 00:55:04 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:55:24 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Fri, 28 Jul 2023 00:55:24 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Fri, 28 Jul 2023 00:55:43 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 28 Jul 2023 00:55:43 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Fri, 28 Jul 2023 00:55:43 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 28 Jul 2023 00:55:43 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Fri, 28 Jul 2023 00:55:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 00:55:44 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 00:55:44 GMT
VOLUME [/opt/couchdb/data]
# Fri, 28 Jul 2023 00:55:44 GMT
EXPOSE 4369 5984 9100
# Fri, 28 Jul 2023 00:55:44 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:3240fe174df9a5a4923c4b52f1d887dd1ad1a9ee69245c1fb867f399167584dd`  
		Last Modified: Thu, 27 Jul 2023 23:30:49 GMT  
		Size: 27.2 MB (27187431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d89b65f2dc832c2f7c348d9f12cf4b9e110e543efc4813b9f870c494429957`  
		Last Modified: Fri, 28 Jul 2023 00:56:38 GMT  
		Size: 3.4 KB (3416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef28276cebf24c8afba60bbb3445613b21460493b508d02d292c0fdd8b18f44`  
		Last Modified: Fri, 28 Jul 2023 00:56:37 GMT  
		Size: 6.7 MB (6704542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c905d0380fb2306d3e35170fbbc2bc64a4128012ea5e12393ed06dff6c5ce8b6`  
		Last Modified: Fri, 28 Jul 2023 00:56:36 GMT  
		Size: 1.3 MB (1259891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7672fd27b19b3a699dcc283d34f31cc9ef507fb4b8905d4d8ab9528e4ffbf8e3`  
		Last Modified: Fri, 28 Jul 2023 00:56:36 GMT  
		Size: 294.6 KB (294631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc9781684c058f6264128d586906d723e7969eb84e485a50c109c9df1973a30`  
		Last Modified: Fri, 28 Jul 2023 00:56:50 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9869b39f486c4ca6de8c713784e3c26bd689c63fb1c2417b420234c072a4e12e`  
		Last Modified: Fri, 28 Jul 2023 00:56:54 GMT  
		Size: 49.1 MB (49136664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840995d1ded1168d5abac83569f50653b98a44cb3bc3f81f02bdf77708ddef05`  
		Last Modified: Fri, 28 Jul 2023 00:56:48 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3f31d9c327854d02f8a037f4c6af150724e0f819fa2a2583856c6affbe5fc6`  
		Last Modified: Fri, 28 Jul 2023 00:56:48 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7955f1dacbb3649aba741a5cb06aa8ecf9f8e906d4cc0c41255e803b54803dc6`  
		Last Modified: Fri, 28 Jul 2023 00:56:48 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51fdd11a7c5ae8e5a94524653edad7bf72a6b28465d450065fe16a236c989446`  
		Last Modified: Fri, 28 Jul 2023 00:56:48 GMT  
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
$ docker pull couchdb@sha256:8cf71a3a657d18dc0358402a2ea414f310cc2d4d7b12da5204f431c06c1d1c0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:6deabbe84258c2151a91a3a82e6d127b2bcce1bb6b8659be675ca4005c795acc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.6 MB (84590179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5b72c4b3a9488f8358040dab8d2a1945460a6a17f63aa229e34e6831fe43f53`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:29 GMT
ADD file:20e7ad6bec617357895302b08431eb3430cce3113bdf0a8ff9827115f858d313 in / 
# Thu, 27 Jul 2023 23:25:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:54:43 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 28 Jul 2023 00:54:43 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 28 Jul 2023 00:54:53 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:54:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Fri, 28 Jul 2023 00:54:57 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Fri, 28 Jul 2023 00:55:04 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:55:24 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Fri, 28 Jul 2023 00:55:24 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Fri, 28 Jul 2023 00:55:43 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 28 Jul 2023 00:55:43 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Fri, 28 Jul 2023 00:55:43 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 28 Jul 2023 00:55:43 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Fri, 28 Jul 2023 00:55:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 00:55:44 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 00:55:44 GMT
VOLUME [/opt/couchdb/data]
# Fri, 28 Jul 2023 00:55:44 GMT
EXPOSE 4369 5984 9100
# Fri, 28 Jul 2023 00:55:44 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:3240fe174df9a5a4923c4b52f1d887dd1ad1a9ee69245c1fb867f399167584dd`  
		Last Modified: Thu, 27 Jul 2023 23:30:49 GMT  
		Size: 27.2 MB (27187431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d89b65f2dc832c2f7c348d9f12cf4b9e110e543efc4813b9f870c494429957`  
		Last Modified: Fri, 28 Jul 2023 00:56:38 GMT  
		Size: 3.4 KB (3416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef28276cebf24c8afba60bbb3445613b21460493b508d02d292c0fdd8b18f44`  
		Last Modified: Fri, 28 Jul 2023 00:56:37 GMT  
		Size: 6.7 MB (6704542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c905d0380fb2306d3e35170fbbc2bc64a4128012ea5e12393ed06dff6c5ce8b6`  
		Last Modified: Fri, 28 Jul 2023 00:56:36 GMT  
		Size: 1.3 MB (1259891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7672fd27b19b3a699dcc283d34f31cc9ef507fb4b8905d4d8ab9528e4ffbf8e3`  
		Last Modified: Fri, 28 Jul 2023 00:56:36 GMT  
		Size: 294.6 KB (294631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc9781684c058f6264128d586906d723e7969eb84e485a50c109c9df1973a30`  
		Last Modified: Fri, 28 Jul 2023 00:56:50 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9869b39f486c4ca6de8c713784e3c26bd689c63fb1c2417b420234c072a4e12e`  
		Last Modified: Fri, 28 Jul 2023 00:56:54 GMT  
		Size: 49.1 MB (49136664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840995d1ded1168d5abac83569f50653b98a44cb3bc3f81f02bdf77708ddef05`  
		Last Modified: Fri, 28 Jul 2023 00:56:48 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3f31d9c327854d02f8a037f4c6af150724e0f819fa2a2583856c6affbe5fc6`  
		Last Modified: Fri, 28 Jul 2023 00:56:48 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7955f1dacbb3649aba741a5cb06aa8ecf9f8e906d4cc0c41255e803b54803dc6`  
		Last Modified: Fri, 28 Jul 2023 00:56:48 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51fdd11a7c5ae8e5a94524653edad7bf72a6b28465d450065fe16a236c989446`  
		Last Modified: Fri, 28 Jul 2023 00:56:48 GMT  
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
$ docker pull couchdb@sha256:2e70d30a980adbf21d302cc6327d4cb14b4bcadc4788b6b7a9f7f9d3c0dc4a18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `couchdb:3` - linux; amd64

```console
$ docker pull couchdb@sha256:227198eb13b4d8e48ab02a69862ac03b68e44b2e879441399c96c3e130ed8cac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90240323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d827434098752cb94ff077a95fef98532ff66a71643aa133e760eeeda419ecb`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:53:51 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 28 Jul 2023 00:53:52 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 28 Jul 2023 00:54:00 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:54:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Fri, 28 Jul 2023 00:54:03 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Fri, 28 Jul 2023 00:54:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:54:08 GMT
ENV COUCHDB_VERSION=3.3.2
# Fri, 28 Jul 2023 00:54:08 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Fri, 28 Jul 2023 00:54:21 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 28 Jul 2023 00:54:22 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 28 Jul 2023 00:54:22 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Fri, 28 Jul 2023 00:54:22 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Fri, 28 Jul 2023 00:54:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 00:54:22 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 00:54:23 GMT
VOLUME [/opt/couchdb/data]
# Fri, 28 Jul 2023 00:54:23 GMT
EXPOSE 4369 5984 9100
# Fri, 28 Jul 2023 00:54:23 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c404450a25c52aaf36ad6cf2df7bf83eb65d98bca7cb78649b4a22fbe62aba`  
		Last Modified: Fri, 28 Jul 2023 00:56:02 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815e16992934da47a606ee48c95eebfce4c426068c7b046352ca614ce1161a10`  
		Last Modified: Fri, 28 Jul 2023 00:56:00 GMT  
		Size: 5.2 MB (5224480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4e80f87d5f0ac56fd4616490a14b6299e1b71054316e29e79922dabfe4cc77`  
		Last Modified: Fri, 28 Jul 2023 00:56:00 GMT  
		Size: 610.3 KB (610275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dcb668df53bd84b62cfbd8b5ca4fa69e26041fdd9a7e919993f81fa1de5dfaf`  
		Last Modified: Fri, 28 Jul 2023 00:56:00 GMT  
		Size: 294.4 KB (294410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519c2591a1a074436d27db4d303d302c79f5317fa1873cbdbf6a711863c6ef2c`  
		Last Modified: Fri, 28 Jul 2023 00:56:00 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc7cbd8bea6ee19dbafe441e0b78a2a7fe1c01a4e83f2d8518c09fcb2a4b57a`  
		Last Modified: Fri, 28 Jul 2023 00:56:03 GMT  
		Size: 52.7 MB (52686137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40fe90e4dff94e302b5f98efe1337955d9a56d04f64eaa8cd4642552a30dbeca`  
		Last Modified: Fri, 28 Jul 2023 00:55:58 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0572f1b6b33e5a9a305c54b7ac1ba36188faa7a53e3461c213bfa0f17eb9b4`  
		Last Modified: Fri, 28 Jul 2023 00:55:58 GMT  
		Size: 998.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520ff0c4c1c630b2c9838ee8eb05a11d541dfe16c5ac442c1db62fd8cb592fd2`  
		Last Modified: Fri, 28 Jul 2023 00:55:58 GMT  
		Size: 2.2 KB (2232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053c53a8228db1b37a14d63d5945d500959e69ab4832bfbe9d335a1bd314cb69`  
		Last Modified: Fri, 28 Jul 2023 00:55:58 GMT  
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
$ docker pull couchdb@sha256:195e387b9e77db7faf72f3138d8e494d67869deb38acb0d1dc5deae048f10c22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.0 MB (95962218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2b1b56534f75b9f1bbfbf2b5af66f6aed83154e252a6a25a6b6178032fa36f5`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 27 Jul 2023 23:23:41 GMT
ADD file:bc63550bad6e6b1e46c01c4911ac409a0a01e632b56a9a846fa2d7c86d8bb292 in / 
# Thu, 27 Jul 2023 23:23:43 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:44:19 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 28 Jul 2023 03:44:20 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 28 Jul 2023 03:44:43 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:44:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Fri, 28 Jul 2023 03:44:52 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Fri, 28 Jul 2023 03:45:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:45:08 GMT
ENV COUCHDB_VERSION=3.3.2
# Fri, 28 Jul 2023 03:45:11 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Fri, 28 Jul 2023 03:45:42 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 28 Jul 2023 03:45:44 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 28 Jul 2023 03:45:45 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Fri, 28 Jul 2023 03:45:45 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Fri, 28 Jul 2023 03:45:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 03:45:47 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 03:45:47 GMT
VOLUME [/opt/couchdb/data]
# Fri, 28 Jul 2023 03:45:48 GMT
EXPOSE 4369 5984 9100
# Fri, 28 Jul 2023 03:45:48 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:90fff1cd317dd6511bdf25cbc4f6797ea09a5bc0657b6e1d88772d885bed1da0`  
		Last Modified: Thu, 27 Jul 2023 23:30:33 GMT  
		Size: 35.3 MB (35291031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89881e295647078d9c302e443081459979a2cd3b1161a78a449001074720911`  
		Last Modified: Fri, 28 Jul 2023 03:46:39 GMT  
		Size: 3.4 KB (3416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44e1763c279db8dfa52f1640c68fa14adfa41f5a055addc6f0a7b9959585354`  
		Last Modified: Fri, 28 Jul 2023 03:46:38 GMT  
		Size: 6.0 MB (6044154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b95b80c92cb8cda5a88e018d853eff3eb94b9df3651a91fe4238fb4cf0dc0ef`  
		Last Modified: Fri, 28 Jul 2023 03:46:37 GMT  
		Size: 662.2 KB (662169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a478ddd7fcbd6eff286a6cc7dfe93f5ee5d3de16ccfc19e827e0b4fd82249e0b`  
		Last Modified: Fri, 28 Jul 2023 03:46:36 GMT  
		Size: 294.4 KB (294375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93724178719de15b26283a933ff2f41443ff52b2b11b6191b5b484501ad51c9b`  
		Last Modified: Fri, 28 Jul 2023 03:46:36 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45eeb8574d1906c43163ebcd0459cf5a3d8298a7a9fec7d2a16f9e6cc052b121`  
		Last Modified: Fri, 28 Jul 2023 03:46:44 GMT  
		Size: 53.7 MB (53663059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b1aa1f11ad7febca6e0e6a1d29121fbba6dd3a4abbe795f1d7184015e0caae`  
		Last Modified: Fri, 28 Jul 2023 03:46:34 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b3094563d60c9c847de9ae3119c4afc8edd6877d73a4308b4dc314eed18e4e`  
		Last Modified: Fri, 28 Jul 2023 03:46:34 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a76163dedbf2715457e9f61f4d785a3ad85110c6911e164bea2196d513e05835`  
		Last Modified: Fri, 28 Jul 2023 03:46:34 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b593398a60565eddef5653aa64a341cc80bcd14d839d4ae79cb54818f3c6ae6`  
		Last Modified: Fri, 28 Jul 2023 03:46:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; s390x

```console
$ docker pull couchdb@sha256:33428ddbe21a0084cda8c47c8ebaaa5a66eb0ae7e4f366b80e2f05ba6ada7c3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.0 MB (86993375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48f7780fb5b3a990520d94f48715586ec65d5eb17f2e62c441e3d171dfc320c5`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 15 Aug 2023 23:43:03 GMT
ADD file:9f523948b128cb562e74300061cc823a8b18f2ba392c765d4f7bd48804ec847c in / 
# Tue, 15 Aug 2023 23:43:06 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:49:06 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 16 Aug 2023 00:49:06 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 16 Aug 2023 00:49:13 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:49:17 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 16 Aug 2023 00:49:17 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 16 Aug 2023 00:49:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:49:22 GMT
ENV COUCHDB_VERSION=3.3.2
# Wed, 16 Aug 2023 00:49:23 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 16 Aug 2023 00:49:40 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 16 Aug 2023 00:49:43 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 16 Aug 2023 00:49:43 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 16 Aug 2023 00:49:43 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 16 Aug 2023 00:49:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 16 Aug 2023 00:49:44 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 00:49:45 GMT
VOLUME [/opt/couchdb/data]
# Wed, 16 Aug 2023 00:49:45 GMT
EXPOSE 4369 5984 9100
# Wed, 16 Aug 2023 00:49:45 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ea73d3d24162398a0ce0ad0034fa886c08f7b61653af0aa26b657c243f5ca5e5`  
		Last Modified: Tue, 15 Aug 2023 23:48:23 GMT  
		Size: 29.7 MB (29652979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b1faff094a041d01082c78deb5da534f05e3d3d0686bfa2cd5a9a8ece79a97`  
		Last Modified: Wed, 16 Aug 2023 00:50:05 GMT  
		Size: 3.4 KB (3431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6314a0b2e1bd86c6568bbb6db18dad199d3bc186280337b26bbb8af0b8406ca8`  
		Last Modified: Wed, 16 Aug 2023 00:50:04 GMT  
		Size: 5.1 MB (5110421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f7beb5eece62dfdfb39a1c1199f16e7087fe9df34dbba62a1e03ca1741df23`  
		Last Modified: Wed, 16 Aug 2023 00:50:03 GMT  
		Size: 573.0 KB (573029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dafb7efbd34871996ff03411966d95d782cc394a50d1be188bb012192d4d3af6`  
		Last Modified: Wed, 16 Aug 2023 00:50:03 GMT  
		Size: 294.4 KB (294416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e67fac25c2c11026fbf4ea20a7c5ea83526f989cd2fb05ecacd3610b64e07bf1`  
		Last Modified: Wed, 16 Aug 2023 00:50:03 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f402af39549fc7ba6410cc03e4e52fc4847374fa2797f20e881a619e761516`  
		Last Modified: Wed, 16 Aug 2023 00:50:06 GMT  
		Size: 51.4 MB (51355091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f0159d193e1bb47a98e14ba0c2fcc40ad391628ad75ab188759ea6b0c00968`  
		Last Modified: Wed, 16 Aug 2023 00:50:01 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4230fd636176641cd4af35d595ae9cf80d7ef5a25c34ab0475b7c7b07d3c24`  
		Last Modified: Wed, 16 Aug 2023 00:50:01 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fca6a6f87daa3628a3eeed609a716f5003135c33a47ec311ee6b7297f42e37`  
		Last Modified: Wed, 16 Aug 2023 00:50:01 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2447151f072539d94483f755d16bbdfb9a7d3c14654148d30064c8835ce59ef7`  
		Last Modified: Wed, 16 Aug 2023 00:50:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1`

```console
$ docker pull couchdb@sha256:e0fb61078f61f0584481adc5fea351ff93e172d6606a2aabdae86c8d13a9404a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:6d3320fa0a2ff4ea9e6b006a632579cfa20b3166aba1646aa768c2f22714e8a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.1 MB (80074627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ead0a95f6afc924f3982ae788b88458f47a2739c915e0209ae7922d1fe723ca1`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:29 GMT
ADD file:20e7ad6bec617357895302b08431eb3430cce3113bdf0a8ff9827115f858d313 in / 
# Thu, 27 Jul 2023 23:25:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:54:43 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 28 Jul 2023 00:54:43 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 28 Jul 2023 00:54:53 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:54:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Fri, 28 Jul 2023 00:54:57 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Fri, 28 Jul 2023 00:55:04 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:55:04 GMT
ENV COUCHDB_VERSION=3.1.2
# Fri, 28 Jul 2023 00:55:05 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Fri, 28 Jul 2023 00:55:18 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 28 Jul 2023 00:55:18 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 28 Jul 2023 00:55:19 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 28 Jul 2023 00:55:19 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Fri, 28 Jul 2023 00:55:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 00:55:19 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 00:55:19 GMT
VOLUME [/opt/couchdb/data]
# Fri, 28 Jul 2023 00:55:19 GMT
EXPOSE 4369 5984 9100
# Fri, 28 Jul 2023 00:55:19 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:3240fe174df9a5a4923c4b52f1d887dd1ad1a9ee69245c1fb867f399167584dd`  
		Last Modified: Thu, 27 Jul 2023 23:30:49 GMT  
		Size: 27.2 MB (27187431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d89b65f2dc832c2f7c348d9f12cf4b9e110e543efc4813b9f870c494429957`  
		Last Modified: Fri, 28 Jul 2023 00:56:38 GMT  
		Size: 3.4 KB (3416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef28276cebf24c8afba60bbb3445613b21460493b508d02d292c0fdd8b18f44`  
		Last Modified: Fri, 28 Jul 2023 00:56:37 GMT  
		Size: 6.7 MB (6704542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c905d0380fb2306d3e35170fbbc2bc64a4128012ea5e12393ed06dff6c5ce8b6`  
		Last Modified: Fri, 28 Jul 2023 00:56:36 GMT  
		Size: 1.3 MB (1259891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7672fd27b19b3a699dcc283d34f31cc9ef507fb4b8905d4d8ab9528e4ffbf8e3`  
		Last Modified: Fri, 28 Jul 2023 00:56:36 GMT  
		Size: 294.6 KB (294631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a60738e02b1b10e1918577229022c10aee9b81972200f20fbf1767ec9f4f43`  
		Last Modified: Fri, 28 Jul 2023 00:56:36 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b1eb9b5bcba498cae5a10dc7483e01f52ab00c327077d57da73bf9db4df6806`  
		Last Modified: Fri, 28 Jul 2023 00:56:38 GMT  
		Size: 44.6 MB (44621118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882f1dbfe924668195838b85a49ef8fbde9d86b22257234434d782637ecd2bcd`  
		Last Modified: Fri, 28 Jul 2023 00:56:34 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:986e9c436a7f1cf8a979637771ff0e2cde3502dccdda06806fc8068b2035eb57`  
		Last Modified: Fri, 28 Jul 2023 00:56:34 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ee7e2e9225a67265f1588a3cea2e4f2196093bf0ed09adab2e6b890913cc24`  
		Last Modified: Fri, 28 Jul 2023 00:56:34 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ae0c5a95ec5fb85130d31b1ac170ece67e422788039912f1d9b1085e2138eb`  
		Last Modified: Fri, 28 Jul 2023 00:56:34 GMT  
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
$ docker pull couchdb@sha256:e0fb61078f61f0584481adc5fea351ff93e172d6606a2aabdae86c8d13a9404a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1.2` - linux; amd64

```console
$ docker pull couchdb@sha256:6d3320fa0a2ff4ea9e6b006a632579cfa20b3166aba1646aa768c2f22714e8a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.1 MB (80074627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ead0a95f6afc924f3982ae788b88458f47a2739c915e0209ae7922d1fe723ca1`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:29 GMT
ADD file:20e7ad6bec617357895302b08431eb3430cce3113bdf0a8ff9827115f858d313 in / 
# Thu, 27 Jul 2023 23:25:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:54:43 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 28 Jul 2023 00:54:43 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 28 Jul 2023 00:54:53 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:54:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Fri, 28 Jul 2023 00:54:57 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Fri, 28 Jul 2023 00:55:04 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:55:04 GMT
ENV COUCHDB_VERSION=3.1.2
# Fri, 28 Jul 2023 00:55:05 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Fri, 28 Jul 2023 00:55:18 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 28 Jul 2023 00:55:18 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 28 Jul 2023 00:55:19 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 28 Jul 2023 00:55:19 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Fri, 28 Jul 2023 00:55:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 00:55:19 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 00:55:19 GMT
VOLUME [/opt/couchdb/data]
# Fri, 28 Jul 2023 00:55:19 GMT
EXPOSE 4369 5984 9100
# Fri, 28 Jul 2023 00:55:19 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:3240fe174df9a5a4923c4b52f1d887dd1ad1a9ee69245c1fb867f399167584dd`  
		Last Modified: Thu, 27 Jul 2023 23:30:49 GMT  
		Size: 27.2 MB (27187431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d89b65f2dc832c2f7c348d9f12cf4b9e110e543efc4813b9f870c494429957`  
		Last Modified: Fri, 28 Jul 2023 00:56:38 GMT  
		Size: 3.4 KB (3416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef28276cebf24c8afba60bbb3445613b21460493b508d02d292c0fdd8b18f44`  
		Last Modified: Fri, 28 Jul 2023 00:56:37 GMT  
		Size: 6.7 MB (6704542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c905d0380fb2306d3e35170fbbc2bc64a4128012ea5e12393ed06dff6c5ce8b6`  
		Last Modified: Fri, 28 Jul 2023 00:56:36 GMT  
		Size: 1.3 MB (1259891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7672fd27b19b3a699dcc283d34f31cc9ef507fb4b8905d4d8ab9528e4ffbf8e3`  
		Last Modified: Fri, 28 Jul 2023 00:56:36 GMT  
		Size: 294.6 KB (294631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a60738e02b1b10e1918577229022c10aee9b81972200f20fbf1767ec9f4f43`  
		Last Modified: Fri, 28 Jul 2023 00:56:36 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b1eb9b5bcba498cae5a10dc7483e01f52ab00c327077d57da73bf9db4df6806`  
		Last Modified: Fri, 28 Jul 2023 00:56:38 GMT  
		Size: 44.6 MB (44621118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882f1dbfe924668195838b85a49ef8fbde9d86b22257234434d782637ecd2bcd`  
		Last Modified: Fri, 28 Jul 2023 00:56:34 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:986e9c436a7f1cf8a979637771ff0e2cde3502dccdda06806fc8068b2035eb57`  
		Last Modified: Fri, 28 Jul 2023 00:56:34 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ee7e2e9225a67265f1588a3cea2e4f2196093bf0ed09adab2e6b890913cc24`  
		Last Modified: Fri, 28 Jul 2023 00:56:34 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ae0c5a95ec5fb85130d31b1ac170ece67e422788039912f1d9b1085e2138eb`  
		Last Modified: Fri, 28 Jul 2023 00:56:34 GMT  
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
$ docker pull couchdb@sha256:34e176ad511efe713c43c58c2aab962c2fc4811cbfc303d893eb7175c60c1c30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2` - linux; amd64

```console
$ docker pull couchdb@sha256:8d7483a7fd7da6a84fdc44099771efbe3d5d5430b545e1726a92f34c3d25e8fa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.7 MB (89740721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67ff1f0f1b2be8b4a2243fd4c8a2a3a034e4226f0fb521ea9a038f5ee8ac7299`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:53:51 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 28 Jul 2023 00:53:52 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 28 Jul 2023 00:54:00 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:54:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Fri, 28 Jul 2023 00:54:03 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Fri, 28 Jul 2023 00:54:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:54:26 GMT
ENV COUCHDB_VERSION=3.2.3
# Fri, 28 Jul 2023 00:54:26 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Fri, 28 Jul 2023 00:54:38 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 28 Jul 2023 00:54:39 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 28 Jul 2023 00:54:39 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Fri, 28 Jul 2023 00:54:39 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Fri, 28 Jul 2023 00:54:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 00:54:39 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 00:54:40 GMT
VOLUME [/opt/couchdb/data]
# Fri, 28 Jul 2023 00:54:40 GMT
EXPOSE 4369 5984 9100
# Fri, 28 Jul 2023 00:54:40 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c404450a25c52aaf36ad6cf2df7bf83eb65d98bca7cb78649b4a22fbe62aba`  
		Last Modified: Fri, 28 Jul 2023 00:56:02 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815e16992934da47a606ee48c95eebfce4c426068c7b046352ca614ce1161a10`  
		Last Modified: Fri, 28 Jul 2023 00:56:00 GMT  
		Size: 5.2 MB (5224480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4e80f87d5f0ac56fd4616490a14b6299e1b71054316e29e79922dabfe4cc77`  
		Last Modified: Fri, 28 Jul 2023 00:56:00 GMT  
		Size: 610.3 KB (610275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dcb668df53bd84b62cfbd8b5ca4fa69e26041fdd9a7e919993f81fa1de5dfaf`  
		Last Modified: Fri, 28 Jul 2023 00:56:00 GMT  
		Size: 294.4 KB (294410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692a2c8068b693b18caf9eeb950329bc0ae0c12b3d71915d6d57f5ba24ff568f`  
		Last Modified: Fri, 28 Jul 2023 00:56:21 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4c51160478bd0b149db84b0a56afc74ac4487a6933e71abfedb930da0b97f33`  
		Last Modified: Fri, 28 Jul 2023 00:56:24 GMT  
		Size: 52.2 MB (52186536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5295ff357554364e67230615e4a45658795749ef72dd64da65872ffd8b2c81a`  
		Last Modified: Fri, 28 Jul 2023 00:56:19 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ea65d0e2775c623a813f0e00990615f643c375dd029103cb4c4e0661610459`  
		Last Modified: Fri, 28 Jul 2023 00:56:19 GMT  
		Size: 998.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c134731a8b6b3db7d4bd899d93d90e6d0a9f00f1391d50290c7b37e4ead15e9e`  
		Last Modified: Fri, 28 Jul 2023 00:56:19 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d24eeed9a8e1d9cfd216e63108877e2c5f2d2892a592e75c9e63e32aec4ff5`  
		Last Modified: Fri, 28 Jul 2023 00:56:19 GMT  
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
$ docker pull couchdb@sha256:0861effa71efdd75f0e46835e72a6b2726f30f6f9e733e0229c35cd6c1d2ba3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchdb:3.2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:8d7483a7fd7da6a84fdc44099771efbe3d5d5430b545e1726a92f34c3d25e8fa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.7 MB (89740721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67ff1f0f1b2be8b4a2243fd4c8a2a3a034e4226f0fb521ea9a038f5ee8ac7299`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:53:51 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 28 Jul 2023 00:53:52 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 28 Jul 2023 00:54:00 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:54:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Fri, 28 Jul 2023 00:54:03 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Fri, 28 Jul 2023 00:54:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:54:26 GMT
ENV COUCHDB_VERSION=3.2.3
# Fri, 28 Jul 2023 00:54:26 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Fri, 28 Jul 2023 00:54:38 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 28 Jul 2023 00:54:39 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 28 Jul 2023 00:54:39 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Fri, 28 Jul 2023 00:54:39 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Fri, 28 Jul 2023 00:54:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 00:54:39 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 00:54:40 GMT
VOLUME [/opt/couchdb/data]
# Fri, 28 Jul 2023 00:54:40 GMT
EXPOSE 4369 5984 9100
# Fri, 28 Jul 2023 00:54:40 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c404450a25c52aaf36ad6cf2df7bf83eb65d98bca7cb78649b4a22fbe62aba`  
		Last Modified: Fri, 28 Jul 2023 00:56:02 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815e16992934da47a606ee48c95eebfce4c426068c7b046352ca614ce1161a10`  
		Last Modified: Fri, 28 Jul 2023 00:56:00 GMT  
		Size: 5.2 MB (5224480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4e80f87d5f0ac56fd4616490a14b6299e1b71054316e29e79922dabfe4cc77`  
		Last Modified: Fri, 28 Jul 2023 00:56:00 GMT  
		Size: 610.3 KB (610275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dcb668df53bd84b62cfbd8b5ca4fa69e26041fdd9a7e919993f81fa1de5dfaf`  
		Last Modified: Fri, 28 Jul 2023 00:56:00 GMT  
		Size: 294.4 KB (294410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692a2c8068b693b18caf9eeb950329bc0ae0c12b3d71915d6d57f5ba24ff568f`  
		Last Modified: Fri, 28 Jul 2023 00:56:21 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4c51160478bd0b149db84b0a56afc74ac4487a6933e71abfedb930da0b97f33`  
		Last Modified: Fri, 28 Jul 2023 00:56:24 GMT  
		Size: 52.2 MB (52186536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5295ff357554364e67230615e4a45658795749ef72dd64da65872ffd8b2c81a`  
		Last Modified: Fri, 28 Jul 2023 00:56:19 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ea65d0e2775c623a813f0e00990615f643c375dd029103cb4c4e0661610459`  
		Last Modified: Fri, 28 Jul 2023 00:56:19 GMT  
		Size: 998.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c134731a8b6b3db7d4bd899d93d90e6d0a9f00f1391d50290c7b37e4ead15e9e`  
		Last Modified: Fri, 28 Jul 2023 00:56:19 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d24eeed9a8e1d9cfd216e63108877e2c5f2d2892a592e75c9e63e32aec4ff5`  
		Last Modified: Fri, 28 Jul 2023 00:56:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.3`

```console
$ docker pull couchdb@sha256:2e70d30a980adbf21d302cc6327d4cb14b4bcadc4788b6b7a9f7f9d3c0dc4a18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `couchdb:3.3` - linux; amd64

```console
$ docker pull couchdb@sha256:227198eb13b4d8e48ab02a69862ac03b68e44b2e879441399c96c3e130ed8cac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90240323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d827434098752cb94ff077a95fef98532ff66a71643aa133e760eeeda419ecb`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:53:51 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 28 Jul 2023 00:53:52 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 28 Jul 2023 00:54:00 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:54:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Fri, 28 Jul 2023 00:54:03 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Fri, 28 Jul 2023 00:54:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:54:08 GMT
ENV COUCHDB_VERSION=3.3.2
# Fri, 28 Jul 2023 00:54:08 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Fri, 28 Jul 2023 00:54:21 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 28 Jul 2023 00:54:22 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 28 Jul 2023 00:54:22 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Fri, 28 Jul 2023 00:54:22 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Fri, 28 Jul 2023 00:54:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 00:54:22 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 00:54:23 GMT
VOLUME [/opt/couchdb/data]
# Fri, 28 Jul 2023 00:54:23 GMT
EXPOSE 4369 5984 9100
# Fri, 28 Jul 2023 00:54:23 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c404450a25c52aaf36ad6cf2df7bf83eb65d98bca7cb78649b4a22fbe62aba`  
		Last Modified: Fri, 28 Jul 2023 00:56:02 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815e16992934da47a606ee48c95eebfce4c426068c7b046352ca614ce1161a10`  
		Last Modified: Fri, 28 Jul 2023 00:56:00 GMT  
		Size: 5.2 MB (5224480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4e80f87d5f0ac56fd4616490a14b6299e1b71054316e29e79922dabfe4cc77`  
		Last Modified: Fri, 28 Jul 2023 00:56:00 GMT  
		Size: 610.3 KB (610275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dcb668df53bd84b62cfbd8b5ca4fa69e26041fdd9a7e919993f81fa1de5dfaf`  
		Last Modified: Fri, 28 Jul 2023 00:56:00 GMT  
		Size: 294.4 KB (294410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519c2591a1a074436d27db4d303d302c79f5317fa1873cbdbf6a711863c6ef2c`  
		Last Modified: Fri, 28 Jul 2023 00:56:00 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc7cbd8bea6ee19dbafe441e0b78a2a7fe1c01a4e83f2d8518c09fcb2a4b57a`  
		Last Modified: Fri, 28 Jul 2023 00:56:03 GMT  
		Size: 52.7 MB (52686137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40fe90e4dff94e302b5f98efe1337955d9a56d04f64eaa8cd4642552a30dbeca`  
		Last Modified: Fri, 28 Jul 2023 00:55:58 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0572f1b6b33e5a9a305c54b7ac1ba36188faa7a53e3461c213bfa0f17eb9b4`  
		Last Modified: Fri, 28 Jul 2023 00:55:58 GMT  
		Size: 998.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520ff0c4c1c630b2c9838ee8eb05a11d541dfe16c5ac442c1db62fd8cb592fd2`  
		Last Modified: Fri, 28 Jul 2023 00:55:58 GMT  
		Size: 2.2 KB (2232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053c53a8228db1b37a14d63d5945d500959e69ab4832bfbe9d335a1bd314cb69`  
		Last Modified: Fri, 28 Jul 2023 00:55:58 GMT  
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
$ docker pull couchdb@sha256:195e387b9e77db7faf72f3138d8e494d67869deb38acb0d1dc5deae048f10c22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.0 MB (95962218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2b1b56534f75b9f1bbfbf2b5af66f6aed83154e252a6a25a6b6178032fa36f5`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 27 Jul 2023 23:23:41 GMT
ADD file:bc63550bad6e6b1e46c01c4911ac409a0a01e632b56a9a846fa2d7c86d8bb292 in / 
# Thu, 27 Jul 2023 23:23:43 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:44:19 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 28 Jul 2023 03:44:20 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 28 Jul 2023 03:44:43 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:44:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Fri, 28 Jul 2023 03:44:52 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Fri, 28 Jul 2023 03:45:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:45:08 GMT
ENV COUCHDB_VERSION=3.3.2
# Fri, 28 Jul 2023 03:45:11 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Fri, 28 Jul 2023 03:45:42 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 28 Jul 2023 03:45:44 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 28 Jul 2023 03:45:45 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Fri, 28 Jul 2023 03:45:45 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Fri, 28 Jul 2023 03:45:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 03:45:47 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 03:45:47 GMT
VOLUME [/opt/couchdb/data]
# Fri, 28 Jul 2023 03:45:48 GMT
EXPOSE 4369 5984 9100
# Fri, 28 Jul 2023 03:45:48 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:90fff1cd317dd6511bdf25cbc4f6797ea09a5bc0657b6e1d88772d885bed1da0`  
		Last Modified: Thu, 27 Jul 2023 23:30:33 GMT  
		Size: 35.3 MB (35291031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89881e295647078d9c302e443081459979a2cd3b1161a78a449001074720911`  
		Last Modified: Fri, 28 Jul 2023 03:46:39 GMT  
		Size: 3.4 KB (3416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44e1763c279db8dfa52f1640c68fa14adfa41f5a055addc6f0a7b9959585354`  
		Last Modified: Fri, 28 Jul 2023 03:46:38 GMT  
		Size: 6.0 MB (6044154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b95b80c92cb8cda5a88e018d853eff3eb94b9df3651a91fe4238fb4cf0dc0ef`  
		Last Modified: Fri, 28 Jul 2023 03:46:37 GMT  
		Size: 662.2 KB (662169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a478ddd7fcbd6eff286a6cc7dfe93f5ee5d3de16ccfc19e827e0b4fd82249e0b`  
		Last Modified: Fri, 28 Jul 2023 03:46:36 GMT  
		Size: 294.4 KB (294375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93724178719de15b26283a933ff2f41443ff52b2b11b6191b5b484501ad51c9b`  
		Last Modified: Fri, 28 Jul 2023 03:46:36 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45eeb8574d1906c43163ebcd0459cf5a3d8298a7a9fec7d2a16f9e6cc052b121`  
		Last Modified: Fri, 28 Jul 2023 03:46:44 GMT  
		Size: 53.7 MB (53663059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b1aa1f11ad7febca6e0e6a1d29121fbba6dd3a4abbe795f1d7184015e0caae`  
		Last Modified: Fri, 28 Jul 2023 03:46:34 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b3094563d60c9c847de9ae3119c4afc8edd6877d73a4308b4dc314eed18e4e`  
		Last Modified: Fri, 28 Jul 2023 03:46:34 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a76163dedbf2715457e9f61f4d785a3ad85110c6911e164bea2196d513e05835`  
		Last Modified: Fri, 28 Jul 2023 03:46:34 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b593398a60565eddef5653aa64a341cc80bcd14d839d4ae79cb54818f3c6ae6`  
		Last Modified: Fri, 28 Jul 2023 03:46:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3` - linux; s390x

```console
$ docker pull couchdb@sha256:33428ddbe21a0084cda8c47c8ebaaa5a66eb0ae7e4f366b80e2f05ba6ada7c3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.0 MB (86993375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48f7780fb5b3a990520d94f48715586ec65d5eb17f2e62c441e3d171dfc320c5`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 15 Aug 2023 23:43:03 GMT
ADD file:9f523948b128cb562e74300061cc823a8b18f2ba392c765d4f7bd48804ec847c in / 
# Tue, 15 Aug 2023 23:43:06 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:49:06 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 16 Aug 2023 00:49:06 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 16 Aug 2023 00:49:13 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:49:17 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 16 Aug 2023 00:49:17 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 16 Aug 2023 00:49:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:49:22 GMT
ENV COUCHDB_VERSION=3.3.2
# Wed, 16 Aug 2023 00:49:23 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 16 Aug 2023 00:49:40 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 16 Aug 2023 00:49:43 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 16 Aug 2023 00:49:43 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 16 Aug 2023 00:49:43 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 16 Aug 2023 00:49:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 16 Aug 2023 00:49:44 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 00:49:45 GMT
VOLUME [/opt/couchdb/data]
# Wed, 16 Aug 2023 00:49:45 GMT
EXPOSE 4369 5984 9100
# Wed, 16 Aug 2023 00:49:45 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ea73d3d24162398a0ce0ad0034fa886c08f7b61653af0aa26b657c243f5ca5e5`  
		Last Modified: Tue, 15 Aug 2023 23:48:23 GMT  
		Size: 29.7 MB (29652979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b1faff094a041d01082c78deb5da534f05e3d3d0686bfa2cd5a9a8ece79a97`  
		Last Modified: Wed, 16 Aug 2023 00:50:05 GMT  
		Size: 3.4 KB (3431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6314a0b2e1bd86c6568bbb6db18dad199d3bc186280337b26bbb8af0b8406ca8`  
		Last Modified: Wed, 16 Aug 2023 00:50:04 GMT  
		Size: 5.1 MB (5110421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f7beb5eece62dfdfb39a1c1199f16e7087fe9df34dbba62a1e03ca1741df23`  
		Last Modified: Wed, 16 Aug 2023 00:50:03 GMT  
		Size: 573.0 KB (573029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dafb7efbd34871996ff03411966d95d782cc394a50d1be188bb012192d4d3af6`  
		Last Modified: Wed, 16 Aug 2023 00:50:03 GMT  
		Size: 294.4 KB (294416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e67fac25c2c11026fbf4ea20a7c5ea83526f989cd2fb05ecacd3610b64e07bf1`  
		Last Modified: Wed, 16 Aug 2023 00:50:03 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f402af39549fc7ba6410cc03e4e52fc4847374fa2797f20e881a619e761516`  
		Last Modified: Wed, 16 Aug 2023 00:50:06 GMT  
		Size: 51.4 MB (51355091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f0159d193e1bb47a98e14ba0c2fcc40ad391628ad75ab188759ea6b0c00968`  
		Last Modified: Wed, 16 Aug 2023 00:50:01 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4230fd636176641cd4af35d595ae9cf80d7ef5a25c34ab0475b7c7b07d3c24`  
		Last Modified: Wed, 16 Aug 2023 00:50:01 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fca6a6f87daa3628a3eeed609a716f5003135c33a47ec311ee6b7297f42e37`  
		Last Modified: Wed, 16 Aug 2023 00:50:01 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2447151f072539d94483f755d16bbdfb9a7d3c14654148d30064c8835ce59ef7`  
		Last Modified: Wed, 16 Aug 2023 00:50:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.3.2`

```console
$ docker pull couchdb@sha256:2e70d30a980adbf21d302cc6327d4cb14b4bcadc4788b6b7a9f7f9d3c0dc4a18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `couchdb:3.3.2` - linux; amd64

```console
$ docker pull couchdb@sha256:227198eb13b4d8e48ab02a69862ac03b68e44b2e879441399c96c3e130ed8cac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90240323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d827434098752cb94ff077a95fef98532ff66a71643aa133e760eeeda419ecb`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:53:51 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 28 Jul 2023 00:53:52 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 28 Jul 2023 00:54:00 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:54:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Fri, 28 Jul 2023 00:54:03 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Fri, 28 Jul 2023 00:54:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:54:08 GMT
ENV COUCHDB_VERSION=3.3.2
# Fri, 28 Jul 2023 00:54:08 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Fri, 28 Jul 2023 00:54:21 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 28 Jul 2023 00:54:22 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 28 Jul 2023 00:54:22 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Fri, 28 Jul 2023 00:54:22 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Fri, 28 Jul 2023 00:54:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 00:54:22 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 00:54:23 GMT
VOLUME [/opt/couchdb/data]
# Fri, 28 Jul 2023 00:54:23 GMT
EXPOSE 4369 5984 9100
# Fri, 28 Jul 2023 00:54:23 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c404450a25c52aaf36ad6cf2df7bf83eb65d98bca7cb78649b4a22fbe62aba`  
		Last Modified: Fri, 28 Jul 2023 00:56:02 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815e16992934da47a606ee48c95eebfce4c426068c7b046352ca614ce1161a10`  
		Last Modified: Fri, 28 Jul 2023 00:56:00 GMT  
		Size: 5.2 MB (5224480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4e80f87d5f0ac56fd4616490a14b6299e1b71054316e29e79922dabfe4cc77`  
		Last Modified: Fri, 28 Jul 2023 00:56:00 GMT  
		Size: 610.3 KB (610275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dcb668df53bd84b62cfbd8b5ca4fa69e26041fdd9a7e919993f81fa1de5dfaf`  
		Last Modified: Fri, 28 Jul 2023 00:56:00 GMT  
		Size: 294.4 KB (294410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519c2591a1a074436d27db4d303d302c79f5317fa1873cbdbf6a711863c6ef2c`  
		Last Modified: Fri, 28 Jul 2023 00:56:00 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc7cbd8bea6ee19dbafe441e0b78a2a7fe1c01a4e83f2d8518c09fcb2a4b57a`  
		Last Modified: Fri, 28 Jul 2023 00:56:03 GMT  
		Size: 52.7 MB (52686137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40fe90e4dff94e302b5f98efe1337955d9a56d04f64eaa8cd4642552a30dbeca`  
		Last Modified: Fri, 28 Jul 2023 00:55:58 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0572f1b6b33e5a9a305c54b7ac1ba36188faa7a53e3461c213bfa0f17eb9b4`  
		Last Modified: Fri, 28 Jul 2023 00:55:58 GMT  
		Size: 998.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520ff0c4c1c630b2c9838ee8eb05a11d541dfe16c5ac442c1db62fd8cb592fd2`  
		Last Modified: Fri, 28 Jul 2023 00:55:58 GMT  
		Size: 2.2 KB (2232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053c53a8228db1b37a14d63d5945d500959e69ab4832bfbe9d335a1bd314cb69`  
		Last Modified: Fri, 28 Jul 2023 00:55:58 GMT  
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
$ docker pull couchdb@sha256:195e387b9e77db7faf72f3138d8e494d67869deb38acb0d1dc5deae048f10c22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.0 MB (95962218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2b1b56534f75b9f1bbfbf2b5af66f6aed83154e252a6a25a6b6178032fa36f5`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 27 Jul 2023 23:23:41 GMT
ADD file:bc63550bad6e6b1e46c01c4911ac409a0a01e632b56a9a846fa2d7c86d8bb292 in / 
# Thu, 27 Jul 2023 23:23:43 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:44:19 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 28 Jul 2023 03:44:20 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 28 Jul 2023 03:44:43 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:44:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Fri, 28 Jul 2023 03:44:52 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Fri, 28 Jul 2023 03:45:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:45:08 GMT
ENV COUCHDB_VERSION=3.3.2
# Fri, 28 Jul 2023 03:45:11 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Fri, 28 Jul 2023 03:45:42 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 28 Jul 2023 03:45:44 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 28 Jul 2023 03:45:45 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Fri, 28 Jul 2023 03:45:45 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Fri, 28 Jul 2023 03:45:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 03:45:47 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 03:45:47 GMT
VOLUME [/opt/couchdb/data]
# Fri, 28 Jul 2023 03:45:48 GMT
EXPOSE 4369 5984 9100
# Fri, 28 Jul 2023 03:45:48 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:90fff1cd317dd6511bdf25cbc4f6797ea09a5bc0657b6e1d88772d885bed1da0`  
		Last Modified: Thu, 27 Jul 2023 23:30:33 GMT  
		Size: 35.3 MB (35291031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89881e295647078d9c302e443081459979a2cd3b1161a78a449001074720911`  
		Last Modified: Fri, 28 Jul 2023 03:46:39 GMT  
		Size: 3.4 KB (3416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44e1763c279db8dfa52f1640c68fa14adfa41f5a055addc6f0a7b9959585354`  
		Last Modified: Fri, 28 Jul 2023 03:46:38 GMT  
		Size: 6.0 MB (6044154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b95b80c92cb8cda5a88e018d853eff3eb94b9df3651a91fe4238fb4cf0dc0ef`  
		Last Modified: Fri, 28 Jul 2023 03:46:37 GMT  
		Size: 662.2 KB (662169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a478ddd7fcbd6eff286a6cc7dfe93f5ee5d3de16ccfc19e827e0b4fd82249e0b`  
		Last Modified: Fri, 28 Jul 2023 03:46:36 GMT  
		Size: 294.4 KB (294375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93724178719de15b26283a933ff2f41443ff52b2b11b6191b5b484501ad51c9b`  
		Last Modified: Fri, 28 Jul 2023 03:46:36 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45eeb8574d1906c43163ebcd0459cf5a3d8298a7a9fec7d2a16f9e6cc052b121`  
		Last Modified: Fri, 28 Jul 2023 03:46:44 GMT  
		Size: 53.7 MB (53663059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b1aa1f11ad7febca6e0e6a1d29121fbba6dd3a4abbe795f1d7184015e0caae`  
		Last Modified: Fri, 28 Jul 2023 03:46:34 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b3094563d60c9c847de9ae3119c4afc8edd6877d73a4308b4dc314eed18e4e`  
		Last Modified: Fri, 28 Jul 2023 03:46:34 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a76163dedbf2715457e9f61f4d785a3ad85110c6911e164bea2196d513e05835`  
		Last Modified: Fri, 28 Jul 2023 03:46:34 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b593398a60565eddef5653aa64a341cc80bcd14d839d4ae79cb54818f3c6ae6`  
		Last Modified: Fri, 28 Jul 2023 03:46:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3.2` - linux; s390x

```console
$ docker pull couchdb@sha256:33428ddbe21a0084cda8c47c8ebaaa5a66eb0ae7e4f366b80e2f05ba6ada7c3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.0 MB (86993375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48f7780fb5b3a990520d94f48715586ec65d5eb17f2e62c441e3d171dfc320c5`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 15 Aug 2023 23:43:03 GMT
ADD file:9f523948b128cb562e74300061cc823a8b18f2ba392c765d4f7bd48804ec847c in / 
# Tue, 15 Aug 2023 23:43:06 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:49:06 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 16 Aug 2023 00:49:06 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 16 Aug 2023 00:49:13 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:49:17 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 16 Aug 2023 00:49:17 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 16 Aug 2023 00:49:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:49:22 GMT
ENV COUCHDB_VERSION=3.3.2
# Wed, 16 Aug 2023 00:49:23 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 16 Aug 2023 00:49:40 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 16 Aug 2023 00:49:43 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 16 Aug 2023 00:49:43 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 16 Aug 2023 00:49:43 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 16 Aug 2023 00:49:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 16 Aug 2023 00:49:44 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 00:49:45 GMT
VOLUME [/opt/couchdb/data]
# Wed, 16 Aug 2023 00:49:45 GMT
EXPOSE 4369 5984 9100
# Wed, 16 Aug 2023 00:49:45 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ea73d3d24162398a0ce0ad0034fa886c08f7b61653af0aa26b657c243f5ca5e5`  
		Last Modified: Tue, 15 Aug 2023 23:48:23 GMT  
		Size: 29.7 MB (29652979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b1faff094a041d01082c78deb5da534f05e3d3d0686bfa2cd5a9a8ece79a97`  
		Last Modified: Wed, 16 Aug 2023 00:50:05 GMT  
		Size: 3.4 KB (3431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6314a0b2e1bd86c6568bbb6db18dad199d3bc186280337b26bbb8af0b8406ca8`  
		Last Modified: Wed, 16 Aug 2023 00:50:04 GMT  
		Size: 5.1 MB (5110421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f7beb5eece62dfdfb39a1c1199f16e7087fe9df34dbba62a1e03ca1741df23`  
		Last Modified: Wed, 16 Aug 2023 00:50:03 GMT  
		Size: 573.0 KB (573029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dafb7efbd34871996ff03411966d95d782cc394a50d1be188bb012192d4d3af6`  
		Last Modified: Wed, 16 Aug 2023 00:50:03 GMT  
		Size: 294.4 KB (294416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e67fac25c2c11026fbf4ea20a7c5ea83526f989cd2fb05ecacd3610b64e07bf1`  
		Last Modified: Wed, 16 Aug 2023 00:50:03 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f402af39549fc7ba6410cc03e4e52fc4847374fa2797f20e881a619e761516`  
		Last Modified: Wed, 16 Aug 2023 00:50:06 GMT  
		Size: 51.4 MB (51355091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f0159d193e1bb47a98e14ba0c2fcc40ad391628ad75ab188759ea6b0c00968`  
		Last Modified: Wed, 16 Aug 2023 00:50:01 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4230fd636176641cd4af35d595ae9cf80d7ef5a25c34ab0475b7c7b07d3c24`  
		Last Modified: Wed, 16 Aug 2023 00:50:01 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fca6a6f87daa3628a3eeed609a716f5003135c33a47ec311ee6b7297f42e37`  
		Last Modified: Wed, 16 Aug 2023 00:50:01 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2447151f072539d94483f755d16bbdfb9a7d3c14654148d30064c8835ce59ef7`  
		Last Modified: Wed, 16 Aug 2023 00:50:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:latest`

```console
$ docker pull couchdb@sha256:2e70d30a980adbf21d302cc6327d4cb14b4bcadc4788b6b7a9f7f9d3c0dc4a18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:227198eb13b4d8e48ab02a69862ac03b68e44b2e879441399c96c3e130ed8cac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90240323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d827434098752cb94ff077a95fef98532ff66a71643aa133e760eeeda419ecb`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:07 GMT
ADD file:3d726bf0abbc08d6dda026cc406cdfb529deb60071641d164de28fcd62d1c1c0 in / 
# Thu, 27 Jul 2023 23:25:07 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:53:51 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 28 Jul 2023 00:53:52 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 28 Jul 2023 00:54:00 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:54:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Fri, 28 Jul 2023 00:54:03 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Fri, 28 Jul 2023 00:54:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:54:08 GMT
ENV COUCHDB_VERSION=3.3.2
# Fri, 28 Jul 2023 00:54:08 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Fri, 28 Jul 2023 00:54:21 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 28 Jul 2023 00:54:22 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 28 Jul 2023 00:54:22 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Fri, 28 Jul 2023 00:54:22 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Fri, 28 Jul 2023 00:54:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 00:54:22 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 00:54:23 GMT
VOLUME [/opt/couchdb/data]
# Fri, 28 Jul 2023 00:54:23 GMT
EXPOSE 4369 5984 9100
# Fri, 28 Jul 2023 00:54:23 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:1d5252f66ea9b661aceca1027b3d7ca259a50608261a25b51148119ecf086932`  
		Last Modified: Thu, 27 Jul 2023 23:30:08 GMT  
		Size: 31.4 MB (31417602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c404450a25c52aaf36ad6cf2df7bf83eb65d98bca7cb78649b4a22fbe62aba`  
		Last Modified: Fri, 28 Jul 2023 00:56:02 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815e16992934da47a606ee48c95eebfce4c426068c7b046352ca614ce1161a10`  
		Last Modified: Fri, 28 Jul 2023 00:56:00 GMT  
		Size: 5.2 MB (5224480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4e80f87d5f0ac56fd4616490a14b6299e1b71054316e29e79922dabfe4cc77`  
		Last Modified: Fri, 28 Jul 2023 00:56:00 GMT  
		Size: 610.3 KB (610275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dcb668df53bd84b62cfbd8b5ca4fa69e26041fdd9a7e919993f81fa1de5dfaf`  
		Last Modified: Fri, 28 Jul 2023 00:56:00 GMT  
		Size: 294.4 KB (294410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519c2591a1a074436d27db4d303d302c79f5317fa1873cbdbf6a711863c6ef2c`  
		Last Modified: Fri, 28 Jul 2023 00:56:00 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc7cbd8bea6ee19dbafe441e0b78a2a7fe1c01a4e83f2d8518c09fcb2a4b57a`  
		Last Modified: Fri, 28 Jul 2023 00:56:03 GMT  
		Size: 52.7 MB (52686137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40fe90e4dff94e302b5f98efe1337955d9a56d04f64eaa8cd4642552a30dbeca`  
		Last Modified: Fri, 28 Jul 2023 00:55:58 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0572f1b6b33e5a9a305c54b7ac1ba36188faa7a53e3461c213bfa0f17eb9b4`  
		Last Modified: Fri, 28 Jul 2023 00:55:58 GMT  
		Size: 998.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520ff0c4c1c630b2c9838ee8eb05a11d541dfe16c5ac442c1db62fd8cb592fd2`  
		Last Modified: Fri, 28 Jul 2023 00:55:58 GMT  
		Size: 2.2 KB (2232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053c53a8228db1b37a14d63d5945d500959e69ab4832bfbe9d335a1bd314cb69`  
		Last Modified: Fri, 28 Jul 2023 00:55:58 GMT  
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
$ docker pull couchdb@sha256:195e387b9e77db7faf72f3138d8e494d67869deb38acb0d1dc5deae048f10c22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.0 MB (95962218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2b1b56534f75b9f1bbfbf2b5af66f6aed83154e252a6a25a6b6178032fa36f5`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 27 Jul 2023 23:23:41 GMT
ADD file:bc63550bad6e6b1e46c01c4911ac409a0a01e632b56a9a846fa2d7c86d8bb292 in / 
# Thu, 27 Jul 2023 23:23:43 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:44:19 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 28 Jul 2023 03:44:20 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 28 Jul 2023 03:44:43 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:44:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Fri, 28 Jul 2023 03:44:52 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Fri, 28 Jul 2023 03:45:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:45:08 GMT
ENV COUCHDB_VERSION=3.3.2
# Fri, 28 Jul 2023 03:45:11 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Fri, 28 Jul 2023 03:45:42 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 28 Jul 2023 03:45:44 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 28 Jul 2023 03:45:45 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Fri, 28 Jul 2023 03:45:45 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Fri, 28 Jul 2023 03:45:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 03:45:47 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 28 Jul 2023 03:45:47 GMT
VOLUME [/opt/couchdb/data]
# Fri, 28 Jul 2023 03:45:48 GMT
EXPOSE 4369 5984 9100
# Fri, 28 Jul 2023 03:45:48 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:90fff1cd317dd6511bdf25cbc4f6797ea09a5bc0657b6e1d88772d885bed1da0`  
		Last Modified: Thu, 27 Jul 2023 23:30:33 GMT  
		Size: 35.3 MB (35291031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89881e295647078d9c302e443081459979a2cd3b1161a78a449001074720911`  
		Last Modified: Fri, 28 Jul 2023 03:46:39 GMT  
		Size: 3.4 KB (3416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44e1763c279db8dfa52f1640c68fa14adfa41f5a055addc6f0a7b9959585354`  
		Last Modified: Fri, 28 Jul 2023 03:46:38 GMT  
		Size: 6.0 MB (6044154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b95b80c92cb8cda5a88e018d853eff3eb94b9df3651a91fe4238fb4cf0dc0ef`  
		Last Modified: Fri, 28 Jul 2023 03:46:37 GMT  
		Size: 662.2 KB (662169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a478ddd7fcbd6eff286a6cc7dfe93f5ee5d3de16ccfc19e827e0b4fd82249e0b`  
		Last Modified: Fri, 28 Jul 2023 03:46:36 GMT  
		Size: 294.4 KB (294375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93724178719de15b26283a933ff2f41443ff52b2b11b6191b5b484501ad51c9b`  
		Last Modified: Fri, 28 Jul 2023 03:46:36 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45eeb8574d1906c43163ebcd0459cf5a3d8298a7a9fec7d2a16f9e6cc052b121`  
		Last Modified: Fri, 28 Jul 2023 03:46:44 GMT  
		Size: 53.7 MB (53663059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b1aa1f11ad7febca6e0e6a1d29121fbba6dd3a4abbe795f1d7184015e0caae`  
		Last Modified: Fri, 28 Jul 2023 03:46:34 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b3094563d60c9c847de9ae3119c4afc8edd6877d73a4308b4dc314eed18e4e`  
		Last Modified: Fri, 28 Jul 2023 03:46:34 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a76163dedbf2715457e9f61f4d785a3ad85110c6911e164bea2196d513e05835`  
		Last Modified: Fri, 28 Jul 2023 03:46:34 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b593398a60565eddef5653aa64a341cc80bcd14d839d4ae79cb54818f3c6ae6`  
		Last Modified: Fri, 28 Jul 2023 03:46:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; s390x

```console
$ docker pull couchdb@sha256:33428ddbe21a0084cda8c47c8ebaaa5a66eb0ae7e4f366b80e2f05ba6ada7c3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.0 MB (86993375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48f7780fb5b3a990520d94f48715586ec65d5eb17f2e62c441e3d171dfc320c5`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 15 Aug 2023 23:43:03 GMT
ADD file:9f523948b128cb562e74300061cc823a8b18f2ba392c765d4f7bd48804ec847c in / 
# Tue, 15 Aug 2023 23:43:06 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:49:06 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 16 Aug 2023 00:49:06 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 16 Aug 2023 00:49:13 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:49:17 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 16 Aug 2023 00:49:17 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 16 Aug 2023 00:49:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:49:22 GMT
ENV COUCHDB_VERSION=3.3.2
# Wed, 16 Aug 2023 00:49:23 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 16 Aug 2023 00:49:40 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 16 Aug 2023 00:49:43 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 16 Aug 2023 00:49:43 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 16 Aug 2023 00:49:43 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 16 Aug 2023 00:49:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 16 Aug 2023 00:49:44 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 16 Aug 2023 00:49:45 GMT
VOLUME [/opt/couchdb/data]
# Wed, 16 Aug 2023 00:49:45 GMT
EXPOSE 4369 5984 9100
# Wed, 16 Aug 2023 00:49:45 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ea73d3d24162398a0ce0ad0034fa886c08f7b61653af0aa26b657c243f5ca5e5`  
		Last Modified: Tue, 15 Aug 2023 23:48:23 GMT  
		Size: 29.7 MB (29652979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b1faff094a041d01082c78deb5da534f05e3d3d0686bfa2cd5a9a8ece79a97`  
		Last Modified: Wed, 16 Aug 2023 00:50:05 GMT  
		Size: 3.4 KB (3431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6314a0b2e1bd86c6568bbb6db18dad199d3bc186280337b26bbb8af0b8406ca8`  
		Last Modified: Wed, 16 Aug 2023 00:50:04 GMT  
		Size: 5.1 MB (5110421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f7beb5eece62dfdfb39a1c1199f16e7087fe9df34dbba62a1e03ca1741df23`  
		Last Modified: Wed, 16 Aug 2023 00:50:03 GMT  
		Size: 573.0 KB (573029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dafb7efbd34871996ff03411966d95d782cc394a50d1be188bb012192d4d3af6`  
		Last Modified: Wed, 16 Aug 2023 00:50:03 GMT  
		Size: 294.4 KB (294416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e67fac25c2c11026fbf4ea20a7c5ea83526f989cd2fb05ecacd3610b64e07bf1`  
		Last Modified: Wed, 16 Aug 2023 00:50:03 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f402af39549fc7ba6410cc03e4e52fc4847374fa2797f20e881a619e761516`  
		Last Modified: Wed, 16 Aug 2023 00:50:06 GMT  
		Size: 51.4 MB (51355091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f0159d193e1bb47a98e14ba0c2fcc40ad391628ad75ab188759ea6b0c00968`  
		Last Modified: Wed, 16 Aug 2023 00:50:01 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4230fd636176641cd4af35d595ae9cf80d7ef5a25c34ab0475b7c7b07d3c24`  
		Last Modified: Wed, 16 Aug 2023 00:50:01 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73fca6a6f87daa3628a3eeed609a716f5003135c33a47ec311ee6b7297f42e37`  
		Last Modified: Wed, 16 Aug 2023 00:50:01 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2447151f072539d94483f755d16bbdfb9a7d3c14654148d30064c8835ce59ef7`  
		Last Modified: Wed, 16 Aug 2023 00:50:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
