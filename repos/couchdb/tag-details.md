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
$ docker pull couchdb@sha256:9c1857225762323a36c3460a048d19000dcb0ec3900ea657a81c79172ba3059f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2` - linux; amd64

```console
$ docker pull couchdb@sha256:6bfa0c63118cc551231a6c9f66888efe9994eff949c5cdf93c09a0140be77fc1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84529402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb2695394336cc3c0b33abf96483195d65b99ce6f3297899655bd2ecf038fc13`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 04 Oct 2022 23:27:01 GMT
ADD file:706105a4a2ea63ba10911afb5998d321ff745f9bcedd2e2e8efcf33f5dad584b in / 
# Tue, 04 Oct 2022 23:27:01 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:54:14 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 05 Oct 2022 01:54:15 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 05 Oct 2022 01:54:25 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:54:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 05 Oct 2022 01:54:30 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 05 Oct 2022 01:54:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:55:02 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 05 Oct 2022 01:55:03 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 05 Oct 2022 01:55:23 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Oct 2022 01:55:24 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 05 Oct 2022 01:55:24 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 05 Oct 2022 01:55:24 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 05 Oct 2022 01:55:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 01:55:25 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 01:55:25 GMT
VOLUME [/opt/couchdb/data]
# Wed, 05 Oct 2022 01:55:25 GMT
EXPOSE 4369 5984 9100
# Wed, 05 Oct 2022 01:55:25 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:f6e04ba6531065d60cd73d6509ec153307f5cc6f95e72ca47745d37aef6380a7`  
		Last Modified: Tue, 04 Oct 2022 23:31:38 GMT  
		Size: 27.1 MB (27138043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec87ba537290953e899b660193e5bb7f3878854413a2dfb4845bae815f2dbf7`  
		Last Modified: Wed, 05 Oct 2022 01:56:10 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b53637f2aa395282433b4bec0cb705eb8ff5b56f564c6ca9c6325ab47bc0874`  
		Last Modified: Wed, 05 Oct 2022 01:56:09 GMT  
		Size: 6.7 MB (6698608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfe7771eede499889c711fe9577563e4fc035d8be22a96485abec7736baa8c8`  
		Last Modified: Wed, 05 Oct 2022 01:56:08 GMT  
		Size: 1.3 MB (1258320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd61eff79af60ac4fdd43efe778148bc679cab9c6451d8da10055cb64646d25`  
		Last Modified: Wed, 05 Oct 2022 01:56:08 GMT  
		Size: 293.1 KB (293055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5f76fc240cdc66635f05cff5f3c124051443a27af50078e5bd496a0ae7ba73`  
		Last Modified: Wed, 05 Oct 2022 01:56:23 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189b747aebaca39179cbabc925e8ba8dd71ec37d4fd79f642d5f29a9ecbc4a2b`  
		Last Modified: Wed, 05 Oct 2022 01:56:27 GMT  
		Size: 49.1 MB (49134356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f404d48d2eb6da68bf8943dc98d738e84f5552bcae60de6dc77205b5607a54`  
		Last Modified: Wed, 05 Oct 2022 01:56:20 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a812e3f5839156fd725135efbe606c5842f10069e24b33b17652b81dde8c243`  
		Last Modified: Wed, 05 Oct 2022 01:56:21 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3f99aea20b6247cd46ffaca4ecd3dc88abfeb920c4a6b9f3f3f7e43f945857`  
		Last Modified: Wed, 05 Oct 2022 01:56:20 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0d8746d2a396b502f7556c7272d84b2290857618924b2262e71d4dc128bea2`  
		Last Modified: Wed, 05 Oct 2022 01:56:21 GMT  
		Size: 121.0 B  
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
$ docker pull couchdb@sha256:9c1857225762323a36c3460a048d19000dcb0ec3900ea657a81c79172ba3059f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:6bfa0c63118cc551231a6c9f66888efe9994eff949c5cdf93c09a0140be77fc1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84529402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb2695394336cc3c0b33abf96483195d65b99ce6f3297899655bd2ecf038fc13`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 04 Oct 2022 23:27:01 GMT
ADD file:706105a4a2ea63ba10911afb5998d321ff745f9bcedd2e2e8efcf33f5dad584b in / 
# Tue, 04 Oct 2022 23:27:01 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:54:14 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 05 Oct 2022 01:54:15 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 05 Oct 2022 01:54:25 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:54:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 05 Oct 2022 01:54:30 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 05 Oct 2022 01:54:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:55:02 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 05 Oct 2022 01:55:03 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 05 Oct 2022 01:55:23 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Oct 2022 01:55:24 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 05 Oct 2022 01:55:24 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 05 Oct 2022 01:55:24 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 05 Oct 2022 01:55:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 01:55:25 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 01:55:25 GMT
VOLUME [/opt/couchdb/data]
# Wed, 05 Oct 2022 01:55:25 GMT
EXPOSE 4369 5984 9100
# Wed, 05 Oct 2022 01:55:25 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:f6e04ba6531065d60cd73d6509ec153307f5cc6f95e72ca47745d37aef6380a7`  
		Last Modified: Tue, 04 Oct 2022 23:31:38 GMT  
		Size: 27.1 MB (27138043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec87ba537290953e899b660193e5bb7f3878854413a2dfb4845bae815f2dbf7`  
		Last Modified: Wed, 05 Oct 2022 01:56:10 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b53637f2aa395282433b4bec0cb705eb8ff5b56f564c6ca9c6325ab47bc0874`  
		Last Modified: Wed, 05 Oct 2022 01:56:09 GMT  
		Size: 6.7 MB (6698608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfe7771eede499889c711fe9577563e4fc035d8be22a96485abec7736baa8c8`  
		Last Modified: Wed, 05 Oct 2022 01:56:08 GMT  
		Size: 1.3 MB (1258320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd61eff79af60ac4fdd43efe778148bc679cab9c6451d8da10055cb64646d25`  
		Last Modified: Wed, 05 Oct 2022 01:56:08 GMT  
		Size: 293.1 KB (293055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5f76fc240cdc66635f05cff5f3c124051443a27af50078e5bd496a0ae7ba73`  
		Last Modified: Wed, 05 Oct 2022 01:56:23 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189b747aebaca39179cbabc925e8ba8dd71ec37d4fd79f642d5f29a9ecbc4a2b`  
		Last Modified: Wed, 05 Oct 2022 01:56:27 GMT  
		Size: 49.1 MB (49134356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f404d48d2eb6da68bf8943dc98d738e84f5552bcae60de6dc77205b5607a54`  
		Last Modified: Wed, 05 Oct 2022 01:56:20 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a812e3f5839156fd725135efbe606c5842f10069e24b33b17652b81dde8c243`  
		Last Modified: Wed, 05 Oct 2022 01:56:21 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3f99aea20b6247cd46ffaca4ecd3dc88abfeb920c4a6b9f3f3f7e43f945857`  
		Last Modified: Wed, 05 Oct 2022 01:56:20 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0d8746d2a396b502f7556c7272d84b2290857618924b2262e71d4dc128bea2`  
		Last Modified: Wed, 05 Oct 2022 01:56:21 GMT  
		Size: 121.0 B  
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
$ docker pull couchdb@sha256:9c1857225762323a36c3460a048d19000dcb0ec3900ea657a81c79172ba3059f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:6bfa0c63118cc551231a6c9f66888efe9994eff949c5cdf93c09a0140be77fc1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84529402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb2695394336cc3c0b33abf96483195d65b99ce6f3297899655bd2ecf038fc13`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 04 Oct 2022 23:27:01 GMT
ADD file:706105a4a2ea63ba10911afb5998d321ff745f9bcedd2e2e8efcf33f5dad584b in / 
# Tue, 04 Oct 2022 23:27:01 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:54:14 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 05 Oct 2022 01:54:15 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 05 Oct 2022 01:54:25 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:54:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 05 Oct 2022 01:54:30 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 05 Oct 2022 01:54:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:55:02 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 05 Oct 2022 01:55:03 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 05 Oct 2022 01:55:23 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Oct 2022 01:55:24 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 05 Oct 2022 01:55:24 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 05 Oct 2022 01:55:24 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 05 Oct 2022 01:55:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 01:55:25 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 01:55:25 GMT
VOLUME [/opt/couchdb/data]
# Wed, 05 Oct 2022 01:55:25 GMT
EXPOSE 4369 5984 9100
# Wed, 05 Oct 2022 01:55:25 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:f6e04ba6531065d60cd73d6509ec153307f5cc6f95e72ca47745d37aef6380a7`  
		Last Modified: Tue, 04 Oct 2022 23:31:38 GMT  
		Size: 27.1 MB (27138043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec87ba537290953e899b660193e5bb7f3878854413a2dfb4845bae815f2dbf7`  
		Last Modified: Wed, 05 Oct 2022 01:56:10 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b53637f2aa395282433b4bec0cb705eb8ff5b56f564c6ca9c6325ab47bc0874`  
		Last Modified: Wed, 05 Oct 2022 01:56:09 GMT  
		Size: 6.7 MB (6698608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfe7771eede499889c711fe9577563e4fc035d8be22a96485abec7736baa8c8`  
		Last Modified: Wed, 05 Oct 2022 01:56:08 GMT  
		Size: 1.3 MB (1258320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd61eff79af60ac4fdd43efe778148bc679cab9c6451d8da10055cb64646d25`  
		Last Modified: Wed, 05 Oct 2022 01:56:08 GMT  
		Size: 293.1 KB (293055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5f76fc240cdc66635f05cff5f3c124051443a27af50078e5bd496a0ae7ba73`  
		Last Modified: Wed, 05 Oct 2022 01:56:23 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189b747aebaca39179cbabc925e8ba8dd71ec37d4fd79f642d5f29a9ecbc4a2b`  
		Last Modified: Wed, 05 Oct 2022 01:56:27 GMT  
		Size: 49.1 MB (49134356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f404d48d2eb6da68bf8943dc98d738e84f5552bcae60de6dc77205b5607a54`  
		Last Modified: Wed, 05 Oct 2022 01:56:20 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a812e3f5839156fd725135efbe606c5842f10069e24b33b17652b81dde8c243`  
		Last Modified: Wed, 05 Oct 2022 01:56:21 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3f99aea20b6247cd46ffaca4ecd3dc88abfeb920c4a6b9f3f3f7e43f945857`  
		Last Modified: Wed, 05 Oct 2022 01:56:20 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf0d8746d2a396b502f7556c7272d84b2290857618924b2262e71d4dc128bea2`  
		Last Modified: Wed, 05 Oct 2022 01:56:21 GMT  
		Size: 121.0 B  
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
$ docker pull couchdb@sha256:5c9cf1d98ed100ef2bfdae5572ec4fd521dcc779850c89f83ea9082f86834fa8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3` - linux; amd64

```console
$ docker pull couchdb@sha256:c976642fe0bfed70d8481293702fb32f3fcfdac0950f239f069c45daf356be80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87546176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:994fdcd357aad6beca4304e782ea3a7229ecba3e960b971af51f441d5239efa6`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:53:34 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 05 Oct 2022 01:53:34 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 05 Oct 2022 01:53:42 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:53:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 05 Oct 2022 01:53:46 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 05 Oct 2022 01:53:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:53:52 GMT
ENV COUCHDB_VERSION=3.2.2
# Wed, 05 Oct 2022 01:53:53 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 05 Oct 2022 01:54:06 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Oct 2022 01:54:06 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 05 Oct 2022 01:54:06 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 05 Oct 2022 01:54:07 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 05 Oct 2022 01:54:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 01:54:07 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 01:54:07 GMT
VOLUME [/opt/couchdb/data]
# Wed, 05 Oct 2022 01:54:07 GMT
EXPOSE 4369 5984 9100
# Wed, 05 Oct 2022 01:54:08 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50830c09adfb39841093b2852fab7bea49db61e68b181aa91f648c74e4fc3e0b`  
		Last Modified: Wed, 05 Oct 2022 01:55:48 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c824d0a873bcb23ad01abb767d707f3b6f081cb277e8c122922cf47a303ff355`  
		Last Modified: Wed, 05 Oct 2022 01:55:47 GMT  
		Size: 5.2 MB (5224222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133338a2a25751a2cd2f69feab9b8f6df2ba1b6de10397de86f03bc729671988`  
		Last Modified: Wed, 05 Oct 2022 01:55:47 GMT  
		Size: 1.6 MB (1553266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161d047ac6b618b63098da64cfe365c125d4f1c4fc18d6d0b37766316b72fa5a`  
		Last Modified: Wed, 05 Oct 2022 01:55:46 GMT  
		Size: 295.6 KB (295590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b72fa5f875f42c5673b59fc12f6c245e49d4f7bd00feb59be64338f8f1c1dde`  
		Last Modified: Wed, 05 Oct 2022 01:55:46 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3091ee36bd0f70205d0e31b10bbc8e7b208bc234f6cc6f3cc3f0783949ac4b2a`  
		Last Modified: Wed, 05 Oct 2022 01:55:49 GMT  
		Size: 49.0 MB (49045858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122333888771cf497009bb9f5b7ea36ab9f42124c802dd3cf7a288063965b0d1`  
		Last Modified: Wed, 05 Oct 2022 01:55:44 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d4e15d74c555d6cda273d6a13afd6916c978a8e719f392f84b1db3428b35f0`  
		Last Modified: Wed, 05 Oct 2022 01:55:44 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f295483f6e8ed514ad1436fee874f7dc7bc996719cab0933ba483af2464386e`  
		Last Modified: Wed, 05 Oct 2022 01:55:44 GMT  
		Size: 2.2 KB (2185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57950f766fe983d4ac0415aa1846954b52f66e8fd0abf3db9a77c7b829f523c2`  
		Last Modified: Wed, 05 Oct 2022 01:55:44 GMT  
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
$ docker pull couchdb@sha256:573d9f033093c79429f5843b2a1845aa5b5c8701a3d8cefa3bf152f2f1bce088
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93234836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a5a5850a83bb2bf101cfa7b9bb0103dcd391c3ab793dfc9e5f8b95a52a137e1`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 25 Oct 2022 03:13:50 GMT
ADD file:1f622759c37363caaa6e6b14831ec9369303345c096f3a018eba66a620b08d26 in / 
# Tue, 25 Oct 2022 03:13:52 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:06:51 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 25 Oct 2022 06:06:53 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 25 Oct 2022 06:07:06 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:07:14 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 25 Oct 2022 06:07:14 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 25 Oct 2022 06:07:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:07:25 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 25 Oct 2022 06:07:26 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 25 Oct 2022 06:07:47 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 25 Oct 2022 06:07:49 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 25 Oct 2022 06:07:49 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 25 Oct 2022 06:07:49 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 25 Oct 2022 06:07:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 25 Oct 2022 06:07:51 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 25 Oct 2022 06:07:51 GMT
VOLUME [/opt/couchdb/data]
# Tue, 25 Oct 2022 06:07:51 GMT
EXPOSE 4369 5984 9100
# Tue, 25 Oct 2022 06:07:51 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6d95b62526dd55d76e7ec2bd4015a327b5bb37161f2ffe8bc2bb08d34a677716`  
		Last Modified: Tue, 25 Oct 2022 03:19:31 GMT  
		Size: 35.3 MB (35290086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff951905b209915c9a1df313fb16760244fac7d51fb589c9f6916ce989182da9`  
		Last Modified: Tue, 25 Oct 2022 06:08:19 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712443240476010b6c006ffa2d932751e6a255ccf2bd596dd1cbcc186e0fb5e`  
		Last Modified: Tue, 25 Oct 2022 06:08:18 GMT  
		Size: 6.0 MB (6045421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f46f597f71b51e9ffcdfe3f8cf65b3491a0ebfa511eb59f6e3ff451da97250`  
		Last Modified: Tue, 25 Oct 2022 06:08:17 GMT  
		Size: 1.5 MB (1509798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267bfa28563276da0d4ed400b10397b96bda9f17d00515d9d055228fbfe9fbd4`  
		Last Modified: Tue, 25 Oct 2022 06:08:17 GMT  
		Size: 296.1 KB (296141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07bf29c43588bb1a85d84ad57b455a4deabff4dd3e3f08943c1856fbb833c10`  
		Last Modified: Tue, 25 Oct 2022 06:08:17 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60206143ed7547d03f4b565c8a75579fee7d7f413101d112a407be39258a70b1`  
		Last Modified: Tue, 25 Oct 2022 06:08:24 GMT  
		Size: 50.1 MB (50086243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fbc205c67ebc790386455cf628f98ef1efd3d8e904116ebcb13960e8f60824`  
		Last Modified: Tue, 25 Oct 2022 06:08:15 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef686fe48f6ff7d5d868d3cd987b968a42d57e6aa75fe77fee0e915ebcffa789`  
		Last Modified: Tue, 25 Oct 2022 06:08:14 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62513520123c4ad12dd19aa946930c527f1ed47cf745829a9e3edcc51f36cbe`  
		Last Modified: Tue, 25 Oct 2022 06:08:14 GMT  
		Size: 2.2 KB (2188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5a1f67b4e79b0ebb1f15b26357f97af2973fc445cb7a1f41c9460ce5821d26`  
		Last Modified: Tue, 25 Oct 2022 06:08:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1`

```console
$ docker pull couchdb@sha256:831f42b61874b9bd5456e8622166f2d1e48b10f7765f8f3b8ccb66cdbae893de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:15609f891bb0ed4f6de7d11c1a98c79f2853f6de9c19d4f7e06d42d5a17d5176
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80012333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8888ba1d853302d491c8a60072926ec8247c1b7862d03ac25f6b22b1223a1798`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 04 Oct 2022 23:27:01 GMT
ADD file:706105a4a2ea63ba10911afb5998d321ff745f9bcedd2e2e8efcf33f5dad584b in / 
# Tue, 04 Oct 2022 23:27:01 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:54:14 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 05 Oct 2022 01:54:15 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 05 Oct 2022 01:54:25 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:54:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 05 Oct 2022 01:54:30 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 05 Oct 2022 01:54:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:54:37 GMT
ENV COUCHDB_VERSION=3.1.2
# Wed, 05 Oct 2022 01:54:38 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 05 Oct 2022 01:54:52 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Oct 2022 01:54:53 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 05 Oct 2022 01:54:53 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 05 Oct 2022 01:54:53 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 05 Oct 2022 01:54:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 01:54:54 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 01:54:54 GMT
VOLUME [/opt/couchdb/data]
# Wed, 05 Oct 2022 01:54:54 GMT
EXPOSE 4369 5984 9100
# Wed, 05 Oct 2022 01:54:54 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:f6e04ba6531065d60cd73d6509ec153307f5cc6f95e72ca47745d37aef6380a7`  
		Last Modified: Tue, 04 Oct 2022 23:31:38 GMT  
		Size: 27.1 MB (27138043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec87ba537290953e899b660193e5bb7f3878854413a2dfb4845bae815f2dbf7`  
		Last Modified: Wed, 05 Oct 2022 01:56:10 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b53637f2aa395282433b4bec0cb705eb8ff5b56f564c6ca9c6325ab47bc0874`  
		Last Modified: Wed, 05 Oct 2022 01:56:09 GMT  
		Size: 6.7 MB (6698608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfe7771eede499889c711fe9577563e4fc035d8be22a96485abec7736baa8c8`  
		Last Modified: Wed, 05 Oct 2022 01:56:08 GMT  
		Size: 1.3 MB (1258320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd61eff79af60ac4fdd43efe778148bc679cab9c6451d8da10055cb64646d25`  
		Last Modified: Wed, 05 Oct 2022 01:56:08 GMT  
		Size: 293.1 KB (293055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf2434bf12d16c23376086e5d672fef9fbf805c698ce76799acdd548609c4a0`  
		Last Modified: Wed, 05 Oct 2022 01:56:08 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649966bbf588d3d9b99a775bdb8852a4788fab5d5992dd08c50afd31ac8ea152`  
		Last Modified: Wed, 05 Oct 2022 01:56:10 GMT  
		Size: 44.6 MB (44617299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da212b8578d97d290894dd4ebdf54f781a4796f7904ce4abcbdc42f192acd621`  
		Last Modified: Wed, 05 Oct 2022 01:56:05 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e9c1267dd05667e858fd996aa85bb035fdc47f222d8a54c9b1d0c9837c9c1a`  
		Last Modified: Wed, 05 Oct 2022 01:56:05 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423db0aa4e277f15b985f531a7ae8b4874ba8e223aa4d17029d6ee9620d23cf1`  
		Last Modified: Wed, 05 Oct 2022 01:56:05 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5b95744f6902108ecec623a6f2cbfab6eb669799ee90d4a6a8d37d7daa8734`  
		Last Modified: Wed, 05 Oct 2022 01:56:05 GMT  
		Size: 121.0 B  
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
$ docker pull couchdb@sha256:831f42b61874b9bd5456e8622166f2d1e48b10f7765f8f3b8ccb66cdbae893de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1.2` - linux; amd64

```console
$ docker pull couchdb@sha256:15609f891bb0ed4f6de7d11c1a98c79f2853f6de9c19d4f7e06d42d5a17d5176
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80012333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8888ba1d853302d491c8a60072926ec8247c1b7862d03ac25f6b22b1223a1798`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 04 Oct 2022 23:27:01 GMT
ADD file:706105a4a2ea63ba10911afb5998d321ff745f9bcedd2e2e8efcf33f5dad584b in / 
# Tue, 04 Oct 2022 23:27:01 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:54:14 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 05 Oct 2022 01:54:15 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 05 Oct 2022 01:54:25 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:54:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 05 Oct 2022 01:54:30 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 05 Oct 2022 01:54:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:54:37 GMT
ENV COUCHDB_VERSION=3.1.2
# Wed, 05 Oct 2022 01:54:38 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 05 Oct 2022 01:54:52 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Oct 2022 01:54:53 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 05 Oct 2022 01:54:53 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 05 Oct 2022 01:54:53 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 05 Oct 2022 01:54:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 01:54:54 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 01:54:54 GMT
VOLUME [/opt/couchdb/data]
# Wed, 05 Oct 2022 01:54:54 GMT
EXPOSE 4369 5984 9100
# Wed, 05 Oct 2022 01:54:54 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:f6e04ba6531065d60cd73d6509ec153307f5cc6f95e72ca47745d37aef6380a7`  
		Last Modified: Tue, 04 Oct 2022 23:31:38 GMT  
		Size: 27.1 MB (27138043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec87ba537290953e899b660193e5bb7f3878854413a2dfb4845bae815f2dbf7`  
		Last Modified: Wed, 05 Oct 2022 01:56:10 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b53637f2aa395282433b4bec0cb705eb8ff5b56f564c6ca9c6325ab47bc0874`  
		Last Modified: Wed, 05 Oct 2022 01:56:09 GMT  
		Size: 6.7 MB (6698608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfe7771eede499889c711fe9577563e4fc035d8be22a96485abec7736baa8c8`  
		Last Modified: Wed, 05 Oct 2022 01:56:08 GMT  
		Size: 1.3 MB (1258320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd61eff79af60ac4fdd43efe778148bc679cab9c6451d8da10055cb64646d25`  
		Last Modified: Wed, 05 Oct 2022 01:56:08 GMT  
		Size: 293.1 KB (293055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf2434bf12d16c23376086e5d672fef9fbf805c698ce76799acdd548609c4a0`  
		Last Modified: Wed, 05 Oct 2022 01:56:08 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649966bbf588d3d9b99a775bdb8852a4788fab5d5992dd08c50afd31ac8ea152`  
		Last Modified: Wed, 05 Oct 2022 01:56:10 GMT  
		Size: 44.6 MB (44617299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da212b8578d97d290894dd4ebdf54f781a4796f7904ce4abcbdc42f192acd621`  
		Last Modified: Wed, 05 Oct 2022 01:56:05 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e9c1267dd05667e858fd996aa85bb035fdc47f222d8a54c9b1d0c9837c9c1a`  
		Last Modified: Wed, 05 Oct 2022 01:56:05 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423db0aa4e277f15b985f531a7ae8b4874ba8e223aa4d17029d6ee9620d23cf1`  
		Last Modified: Wed, 05 Oct 2022 01:56:05 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5b95744f6902108ecec623a6f2cbfab6eb669799ee90d4a6a8d37d7daa8734`  
		Last Modified: Wed, 05 Oct 2022 01:56:05 GMT  
		Size: 121.0 B  
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
$ docker pull couchdb@sha256:5c9cf1d98ed100ef2bfdae5572ec4fd521dcc779850c89f83ea9082f86834fa8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2` - linux; amd64

```console
$ docker pull couchdb@sha256:c976642fe0bfed70d8481293702fb32f3fcfdac0950f239f069c45daf356be80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87546176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:994fdcd357aad6beca4304e782ea3a7229ecba3e960b971af51f441d5239efa6`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:53:34 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 05 Oct 2022 01:53:34 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 05 Oct 2022 01:53:42 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:53:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 05 Oct 2022 01:53:46 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 05 Oct 2022 01:53:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:53:52 GMT
ENV COUCHDB_VERSION=3.2.2
# Wed, 05 Oct 2022 01:53:53 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 05 Oct 2022 01:54:06 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Oct 2022 01:54:06 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 05 Oct 2022 01:54:06 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 05 Oct 2022 01:54:07 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 05 Oct 2022 01:54:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 01:54:07 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 01:54:07 GMT
VOLUME [/opt/couchdb/data]
# Wed, 05 Oct 2022 01:54:07 GMT
EXPOSE 4369 5984 9100
# Wed, 05 Oct 2022 01:54:08 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50830c09adfb39841093b2852fab7bea49db61e68b181aa91f648c74e4fc3e0b`  
		Last Modified: Wed, 05 Oct 2022 01:55:48 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c824d0a873bcb23ad01abb767d707f3b6f081cb277e8c122922cf47a303ff355`  
		Last Modified: Wed, 05 Oct 2022 01:55:47 GMT  
		Size: 5.2 MB (5224222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133338a2a25751a2cd2f69feab9b8f6df2ba1b6de10397de86f03bc729671988`  
		Last Modified: Wed, 05 Oct 2022 01:55:47 GMT  
		Size: 1.6 MB (1553266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161d047ac6b618b63098da64cfe365c125d4f1c4fc18d6d0b37766316b72fa5a`  
		Last Modified: Wed, 05 Oct 2022 01:55:46 GMT  
		Size: 295.6 KB (295590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b72fa5f875f42c5673b59fc12f6c245e49d4f7bd00feb59be64338f8f1c1dde`  
		Last Modified: Wed, 05 Oct 2022 01:55:46 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3091ee36bd0f70205d0e31b10bbc8e7b208bc234f6cc6f3cc3f0783949ac4b2a`  
		Last Modified: Wed, 05 Oct 2022 01:55:49 GMT  
		Size: 49.0 MB (49045858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122333888771cf497009bb9f5b7ea36ab9f42124c802dd3cf7a288063965b0d1`  
		Last Modified: Wed, 05 Oct 2022 01:55:44 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d4e15d74c555d6cda273d6a13afd6916c978a8e719f392f84b1db3428b35f0`  
		Last Modified: Wed, 05 Oct 2022 01:55:44 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f295483f6e8ed514ad1436fee874f7dc7bc996719cab0933ba483af2464386e`  
		Last Modified: Wed, 05 Oct 2022 01:55:44 GMT  
		Size: 2.2 KB (2185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57950f766fe983d4ac0415aa1846954b52f66e8fd0abf3db9a77c7b829f523c2`  
		Last Modified: Wed, 05 Oct 2022 01:55:44 GMT  
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
$ docker pull couchdb@sha256:573d9f033093c79429f5843b2a1845aa5b5c8701a3d8cefa3bf152f2f1bce088
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93234836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a5a5850a83bb2bf101cfa7b9bb0103dcd391c3ab793dfc9e5f8b95a52a137e1`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 25 Oct 2022 03:13:50 GMT
ADD file:1f622759c37363caaa6e6b14831ec9369303345c096f3a018eba66a620b08d26 in / 
# Tue, 25 Oct 2022 03:13:52 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:06:51 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 25 Oct 2022 06:06:53 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 25 Oct 2022 06:07:06 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:07:14 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 25 Oct 2022 06:07:14 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 25 Oct 2022 06:07:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:07:25 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 25 Oct 2022 06:07:26 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 25 Oct 2022 06:07:47 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 25 Oct 2022 06:07:49 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 25 Oct 2022 06:07:49 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 25 Oct 2022 06:07:49 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 25 Oct 2022 06:07:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 25 Oct 2022 06:07:51 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 25 Oct 2022 06:07:51 GMT
VOLUME [/opt/couchdb/data]
# Tue, 25 Oct 2022 06:07:51 GMT
EXPOSE 4369 5984 9100
# Tue, 25 Oct 2022 06:07:51 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6d95b62526dd55d76e7ec2bd4015a327b5bb37161f2ffe8bc2bb08d34a677716`  
		Last Modified: Tue, 25 Oct 2022 03:19:31 GMT  
		Size: 35.3 MB (35290086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff951905b209915c9a1df313fb16760244fac7d51fb589c9f6916ce989182da9`  
		Last Modified: Tue, 25 Oct 2022 06:08:19 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712443240476010b6c006ffa2d932751e6a255ccf2bd596dd1cbcc186e0fb5e`  
		Last Modified: Tue, 25 Oct 2022 06:08:18 GMT  
		Size: 6.0 MB (6045421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f46f597f71b51e9ffcdfe3f8cf65b3491a0ebfa511eb59f6e3ff451da97250`  
		Last Modified: Tue, 25 Oct 2022 06:08:17 GMT  
		Size: 1.5 MB (1509798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267bfa28563276da0d4ed400b10397b96bda9f17d00515d9d055228fbfe9fbd4`  
		Last Modified: Tue, 25 Oct 2022 06:08:17 GMT  
		Size: 296.1 KB (296141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07bf29c43588bb1a85d84ad57b455a4deabff4dd3e3f08943c1856fbb833c10`  
		Last Modified: Tue, 25 Oct 2022 06:08:17 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60206143ed7547d03f4b565c8a75579fee7d7f413101d112a407be39258a70b1`  
		Last Modified: Tue, 25 Oct 2022 06:08:24 GMT  
		Size: 50.1 MB (50086243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fbc205c67ebc790386455cf628f98ef1efd3d8e904116ebcb13960e8f60824`  
		Last Modified: Tue, 25 Oct 2022 06:08:15 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef686fe48f6ff7d5d868d3cd987b968a42d57e6aa75fe77fee0e915ebcffa789`  
		Last Modified: Tue, 25 Oct 2022 06:08:14 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62513520123c4ad12dd19aa946930c527f1ed47cf745829a9e3edcc51f36cbe`  
		Last Modified: Tue, 25 Oct 2022 06:08:14 GMT  
		Size: 2.2 KB (2188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5a1f67b4e79b0ebb1f15b26357f97af2973fc445cb7a1f41c9460ce5821d26`  
		Last Modified: Tue, 25 Oct 2022 06:08:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2.2`

```console
$ docker pull couchdb@sha256:5c9cf1d98ed100ef2bfdae5572ec4fd521dcc779850c89f83ea9082f86834fa8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2.2` - linux; amd64

```console
$ docker pull couchdb@sha256:c976642fe0bfed70d8481293702fb32f3fcfdac0950f239f069c45daf356be80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87546176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:994fdcd357aad6beca4304e782ea3a7229ecba3e960b971af51f441d5239efa6`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:53:34 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 05 Oct 2022 01:53:34 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 05 Oct 2022 01:53:42 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:53:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 05 Oct 2022 01:53:46 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 05 Oct 2022 01:53:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:53:52 GMT
ENV COUCHDB_VERSION=3.2.2
# Wed, 05 Oct 2022 01:53:53 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 05 Oct 2022 01:54:06 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Oct 2022 01:54:06 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 05 Oct 2022 01:54:06 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 05 Oct 2022 01:54:07 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 05 Oct 2022 01:54:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 01:54:07 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 01:54:07 GMT
VOLUME [/opt/couchdb/data]
# Wed, 05 Oct 2022 01:54:07 GMT
EXPOSE 4369 5984 9100
# Wed, 05 Oct 2022 01:54:08 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50830c09adfb39841093b2852fab7bea49db61e68b181aa91f648c74e4fc3e0b`  
		Last Modified: Wed, 05 Oct 2022 01:55:48 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c824d0a873bcb23ad01abb767d707f3b6f081cb277e8c122922cf47a303ff355`  
		Last Modified: Wed, 05 Oct 2022 01:55:47 GMT  
		Size: 5.2 MB (5224222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133338a2a25751a2cd2f69feab9b8f6df2ba1b6de10397de86f03bc729671988`  
		Last Modified: Wed, 05 Oct 2022 01:55:47 GMT  
		Size: 1.6 MB (1553266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161d047ac6b618b63098da64cfe365c125d4f1c4fc18d6d0b37766316b72fa5a`  
		Last Modified: Wed, 05 Oct 2022 01:55:46 GMT  
		Size: 295.6 KB (295590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b72fa5f875f42c5673b59fc12f6c245e49d4f7bd00feb59be64338f8f1c1dde`  
		Last Modified: Wed, 05 Oct 2022 01:55:46 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3091ee36bd0f70205d0e31b10bbc8e7b208bc234f6cc6f3cc3f0783949ac4b2a`  
		Last Modified: Wed, 05 Oct 2022 01:55:49 GMT  
		Size: 49.0 MB (49045858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122333888771cf497009bb9f5b7ea36ab9f42124c802dd3cf7a288063965b0d1`  
		Last Modified: Wed, 05 Oct 2022 01:55:44 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d4e15d74c555d6cda273d6a13afd6916c978a8e719f392f84b1db3428b35f0`  
		Last Modified: Wed, 05 Oct 2022 01:55:44 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f295483f6e8ed514ad1436fee874f7dc7bc996719cab0933ba483af2464386e`  
		Last Modified: Wed, 05 Oct 2022 01:55:44 GMT  
		Size: 2.2 KB (2185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57950f766fe983d4ac0415aa1846954b52f66e8fd0abf3db9a77c7b829f523c2`  
		Last Modified: Wed, 05 Oct 2022 01:55:44 GMT  
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
$ docker pull couchdb@sha256:573d9f033093c79429f5843b2a1845aa5b5c8701a3d8cefa3bf152f2f1bce088
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93234836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a5a5850a83bb2bf101cfa7b9bb0103dcd391c3ab793dfc9e5f8b95a52a137e1`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 25 Oct 2022 03:13:50 GMT
ADD file:1f622759c37363caaa6e6b14831ec9369303345c096f3a018eba66a620b08d26 in / 
# Tue, 25 Oct 2022 03:13:52 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:06:51 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 25 Oct 2022 06:06:53 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 25 Oct 2022 06:07:06 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:07:14 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 25 Oct 2022 06:07:14 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 25 Oct 2022 06:07:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:07:25 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 25 Oct 2022 06:07:26 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 25 Oct 2022 06:07:47 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 25 Oct 2022 06:07:49 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 25 Oct 2022 06:07:49 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 25 Oct 2022 06:07:49 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 25 Oct 2022 06:07:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 25 Oct 2022 06:07:51 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 25 Oct 2022 06:07:51 GMT
VOLUME [/opt/couchdb/data]
# Tue, 25 Oct 2022 06:07:51 GMT
EXPOSE 4369 5984 9100
# Tue, 25 Oct 2022 06:07:51 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6d95b62526dd55d76e7ec2bd4015a327b5bb37161f2ffe8bc2bb08d34a677716`  
		Last Modified: Tue, 25 Oct 2022 03:19:31 GMT  
		Size: 35.3 MB (35290086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff951905b209915c9a1df313fb16760244fac7d51fb589c9f6916ce989182da9`  
		Last Modified: Tue, 25 Oct 2022 06:08:19 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712443240476010b6c006ffa2d932751e6a255ccf2bd596dd1cbcc186e0fb5e`  
		Last Modified: Tue, 25 Oct 2022 06:08:18 GMT  
		Size: 6.0 MB (6045421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f46f597f71b51e9ffcdfe3f8cf65b3491a0ebfa511eb59f6e3ff451da97250`  
		Last Modified: Tue, 25 Oct 2022 06:08:17 GMT  
		Size: 1.5 MB (1509798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267bfa28563276da0d4ed400b10397b96bda9f17d00515d9d055228fbfe9fbd4`  
		Last Modified: Tue, 25 Oct 2022 06:08:17 GMT  
		Size: 296.1 KB (296141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07bf29c43588bb1a85d84ad57b455a4deabff4dd3e3f08943c1856fbb833c10`  
		Last Modified: Tue, 25 Oct 2022 06:08:17 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60206143ed7547d03f4b565c8a75579fee7d7f413101d112a407be39258a70b1`  
		Last Modified: Tue, 25 Oct 2022 06:08:24 GMT  
		Size: 50.1 MB (50086243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fbc205c67ebc790386455cf628f98ef1efd3d8e904116ebcb13960e8f60824`  
		Last Modified: Tue, 25 Oct 2022 06:08:15 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef686fe48f6ff7d5d868d3cd987b968a42d57e6aa75fe77fee0e915ebcffa789`  
		Last Modified: Tue, 25 Oct 2022 06:08:14 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62513520123c4ad12dd19aa946930c527f1ed47cf745829a9e3edcc51f36cbe`  
		Last Modified: Tue, 25 Oct 2022 06:08:14 GMT  
		Size: 2.2 KB (2188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5a1f67b4e79b0ebb1f15b26357f97af2973fc445cb7a1f41c9460ce5821d26`  
		Last Modified: Tue, 25 Oct 2022 06:08:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:latest`

```console
$ docker pull couchdb@sha256:5c9cf1d98ed100ef2bfdae5572ec4fd521dcc779850c89f83ea9082f86834fa8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:c976642fe0bfed70d8481293702fb32f3fcfdac0950f239f069c45daf356be80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87546176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:994fdcd357aad6beca4304e782ea3a7229ecba3e960b971af51f441d5239efa6`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:53:34 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 05 Oct 2022 01:53:34 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 05 Oct 2022 01:53:42 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:53:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 05 Oct 2022 01:53:46 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 05 Oct 2022 01:53:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:53:52 GMT
ENV COUCHDB_VERSION=3.2.2
# Wed, 05 Oct 2022 01:53:53 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 05 Oct 2022 01:54:06 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Oct 2022 01:54:06 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 05 Oct 2022 01:54:06 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 05 Oct 2022 01:54:07 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 05 Oct 2022 01:54:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 01:54:07 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 01:54:07 GMT
VOLUME [/opt/couchdb/data]
# Wed, 05 Oct 2022 01:54:07 GMT
EXPOSE 4369 5984 9100
# Wed, 05 Oct 2022 01:54:08 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50830c09adfb39841093b2852fab7bea49db61e68b181aa91f648c74e4fc3e0b`  
		Last Modified: Wed, 05 Oct 2022 01:55:48 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c824d0a873bcb23ad01abb767d707f3b6f081cb277e8c122922cf47a303ff355`  
		Last Modified: Wed, 05 Oct 2022 01:55:47 GMT  
		Size: 5.2 MB (5224222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133338a2a25751a2cd2f69feab9b8f6df2ba1b6de10397de86f03bc729671988`  
		Last Modified: Wed, 05 Oct 2022 01:55:47 GMT  
		Size: 1.6 MB (1553266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161d047ac6b618b63098da64cfe365c125d4f1c4fc18d6d0b37766316b72fa5a`  
		Last Modified: Wed, 05 Oct 2022 01:55:46 GMT  
		Size: 295.6 KB (295590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b72fa5f875f42c5673b59fc12f6c245e49d4f7bd00feb59be64338f8f1c1dde`  
		Last Modified: Wed, 05 Oct 2022 01:55:46 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3091ee36bd0f70205d0e31b10bbc8e7b208bc234f6cc6f3cc3f0783949ac4b2a`  
		Last Modified: Wed, 05 Oct 2022 01:55:49 GMT  
		Size: 49.0 MB (49045858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122333888771cf497009bb9f5b7ea36ab9f42124c802dd3cf7a288063965b0d1`  
		Last Modified: Wed, 05 Oct 2022 01:55:44 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d4e15d74c555d6cda273d6a13afd6916c978a8e719f392f84b1db3428b35f0`  
		Last Modified: Wed, 05 Oct 2022 01:55:44 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f295483f6e8ed514ad1436fee874f7dc7bc996719cab0933ba483af2464386e`  
		Last Modified: Wed, 05 Oct 2022 01:55:44 GMT  
		Size: 2.2 KB (2185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57950f766fe983d4ac0415aa1846954b52f66e8fd0abf3db9a77c7b829f523c2`  
		Last Modified: Wed, 05 Oct 2022 01:55:44 GMT  
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
$ docker pull couchdb@sha256:573d9f033093c79429f5843b2a1845aa5b5c8701a3d8cefa3bf152f2f1bce088
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93234836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a5a5850a83bb2bf101cfa7b9bb0103dcd391c3ab793dfc9e5f8b95a52a137e1`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 25 Oct 2022 03:13:50 GMT
ADD file:1f622759c37363caaa6e6b14831ec9369303345c096f3a018eba66a620b08d26 in / 
# Tue, 25 Oct 2022 03:13:52 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:06:51 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 25 Oct 2022 06:06:53 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 25 Oct 2022 06:07:06 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:07:14 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 25 Oct 2022 06:07:14 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 25 Oct 2022 06:07:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:07:25 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 25 Oct 2022 06:07:26 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 25 Oct 2022 06:07:47 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 25 Oct 2022 06:07:49 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 25 Oct 2022 06:07:49 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 25 Oct 2022 06:07:49 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 25 Oct 2022 06:07:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 25 Oct 2022 06:07:51 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 25 Oct 2022 06:07:51 GMT
VOLUME [/opt/couchdb/data]
# Tue, 25 Oct 2022 06:07:51 GMT
EXPOSE 4369 5984 9100
# Tue, 25 Oct 2022 06:07:51 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6d95b62526dd55d76e7ec2bd4015a327b5bb37161f2ffe8bc2bb08d34a677716`  
		Last Modified: Tue, 25 Oct 2022 03:19:31 GMT  
		Size: 35.3 MB (35290086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff951905b209915c9a1df313fb16760244fac7d51fb589c9f6916ce989182da9`  
		Last Modified: Tue, 25 Oct 2022 06:08:19 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b712443240476010b6c006ffa2d932751e6a255ccf2bd596dd1cbcc186e0fb5e`  
		Last Modified: Tue, 25 Oct 2022 06:08:18 GMT  
		Size: 6.0 MB (6045421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f46f597f71b51e9ffcdfe3f8cf65b3491a0ebfa511eb59f6e3ff451da97250`  
		Last Modified: Tue, 25 Oct 2022 06:08:17 GMT  
		Size: 1.5 MB (1509798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267bfa28563276da0d4ed400b10397b96bda9f17d00515d9d055228fbfe9fbd4`  
		Last Modified: Tue, 25 Oct 2022 06:08:17 GMT  
		Size: 296.1 KB (296141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07bf29c43588bb1a85d84ad57b455a4deabff4dd3e3f08943c1856fbb833c10`  
		Last Modified: Tue, 25 Oct 2022 06:08:17 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60206143ed7547d03f4b565c8a75579fee7d7f413101d112a407be39258a70b1`  
		Last Modified: Tue, 25 Oct 2022 06:08:24 GMT  
		Size: 50.1 MB (50086243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fbc205c67ebc790386455cf628f98ef1efd3d8e904116ebcb13960e8f60824`  
		Last Modified: Tue, 25 Oct 2022 06:08:15 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef686fe48f6ff7d5d868d3cd987b968a42d57e6aa75fe77fee0e915ebcffa789`  
		Last Modified: Tue, 25 Oct 2022 06:08:14 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62513520123c4ad12dd19aa946930c527f1ed47cf745829a9e3edcc51f36cbe`  
		Last Modified: Tue, 25 Oct 2022 06:08:14 GMT  
		Size: 2.2 KB (2188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5a1f67b4e79b0ebb1f15b26357f97af2973fc445cb7a1f41c9460ce5821d26`  
		Last Modified: Tue, 25 Oct 2022 06:08:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
