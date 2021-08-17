<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `couchdb`

-	[`couchdb:2`](#couchdb2)
-	[`couchdb:2.3`](#couchdb23)
-	[`couchdb:2.3.1`](#couchdb231)
-	[`couchdb:3`](#couchdb3)
-	[`couchdb:3.1`](#couchdb31)
-	[`couchdb:3.1.1`](#couchdb311)
-	[`couchdb:latest`](#couchdblatest)

## `couchdb:2`

```console
$ docker pull couchdb@sha256:094d7d3c88e561eaf0cd77ffaf7823030f2c0a4a1ea41c892b99be9e3d74f2ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2` - linux; amd64

```console
$ docker pull couchdb@sha256:e37a61155424c9392f840e18e7d791fa58c6af19396a85f4475c13a8c4f4621c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84508904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e385abfd92be3d6f88eefbf7fd40e19acc9d30377c011bfe3ea4c3e4fcfa034e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:38:17 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 17 Aug 2021 09:38:18 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 17 Aug 2021 09:38:39 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:38:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 17 Aug 2021 09:38:45 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 17 Aug 2021 09:38:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:39:18 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 17 Aug 2021 09:39:20 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 17 Aug 2021 09:39:45 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 17 Aug 2021 09:39:46 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 17 Aug 2021 09:39:47 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 17 Aug 2021 09:39:47 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 17 Aug 2021 09:39:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 17 Aug 2021 09:39:49 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 09:39:49 GMT
VOLUME [/opt/couchdb/data]
# Tue, 17 Aug 2021 09:39:49 GMT
EXPOSE 4369 5984 9100
# Tue, 17 Aug 2021 09:39:50 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f42f4d38cbf31bed3f27b58346190ea29ee14cec152ad44f07ef55175d9c055`  
		Last Modified: Tue, 17 Aug 2021 09:40:15 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b8216568b0598794cab6ed82a1c24c039865819e4ac0cdf2b871a943ac813b`  
		Last Modified: Tue, 17 Aug 2021 09:40:15 GMT  
		Size: 6.7 MB (6690783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eed64046c4dd433adb7d77997f00edb049f5d6cbc3fc5ddf3d61527741be6db`  
		Last Modified: Tue, 17 Aug 2021 09:40:13 GMT  
		Size: 1.3 MB (1258341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cba51966f0872e9bd9dac956ed819756d7b3b7c6f039ab31be7c8c9e8baa1ce`  
		Last Modified: Tue, 17 Aug 2021 09:40:13 GMT  
		Size: 293.0 KB (292974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8202e5f9d59551d3c66f183f03417ee311966bb3d6c0b7d3c9798314232b8986`  
		Last Modified: Tue, 17 Aug 2021 09:40:38 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0dcecb097e2e6b7350c669da4db8e4e14b06405c8cb937540b669a1071c0350`  
		Last Modified: Tue, 17 Aug 2021 09:40:44 GMT  
		Size: 49.1 MB (49113803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff91ea03c5ea787f36358768f71a6a3a1b3914e9f22cb33681d2329d6f47030`  
		Last Modified: Tue, 17 Aug 2021 09:40:36 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17b674c40f8737133bb393c5ae9de618ae2584db47c95040cdd8076e72d5a41`  
		Last Modified: Tue, 17 Aug 2021 09:40:36 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0883416cf372ee9e76d8fb14f4340f56a1bdffdc86171c8cafdfc38a053e73c8`  
		Last Modified: Tue, 17 Aug 2021 09:40:36 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb1b38ac64d87240ac4c63d1698e0c4298a59aa6f6bf67b0407ca9da8c64de9`  
		Last Modified: Tue, 17 Aug 2021 09:40:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:c24f7a9b72f99f8de9dd9aafbbf91c2113d20bbef8e930e7f0aa099929454fba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72941030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62316d039132754d9d4443adc0abf22c1589b3ecafd4d8a81755bbd0b8964298`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 08:09:33 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 17 Aug 2021 08:09:33 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 17 Aug 2021 08:09:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 08:09:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 17 Aug 2021 08:09:45 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 17 Aug 2021 08:09:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 08:10:17 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 17 Aug 2021 08:10:17 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 17 Aug 2021 08:10:29 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 17 Aug 2021 08:10:30 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 17 Aug 2021 08:10:30 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 17 Aug 2021 08:10:30 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 17 Aug 2021 08:10:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 17 Aug 2021 08:10:31 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 08:10:31 GMT
VOLUME [/opt/couchdb/data]
# Tue, 17 Aug 2021 08:10:31 GMT
EXPOSE 4369 5984 9100
# Tue, 17 Aug 2021 08:10:32 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab787026ef6a8144c5eabbda8d5bdf43afc3c79eef1ada02802921541490d37`  
		Last Modified: Tue, 17 Aug 2021 08:11:00 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ebe0a9c5656679672b817a6a586b31d8a518f90b2f77b5e5a0d70841c93a47`  
		Last Modified: Tue, 17 Aug 2021 08:10:59 GMT  
		Size: 6.6 MB (6550146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67fe32ef3fc734dde11d93c43255cdc4631d4f400588f69dbd6fca417c452e7`  
		Last Modified: Tue, 17 Aug 2021 08:10:57 GMT  
		Size: 1.2 MB (1163423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a7736bc7346c11850cfda36cd6466ed5503f0bbaf145f42af99fbc8e23ee4c`  
		Last Modified: Tue, 17 Aug 2021 08:10:57 GMT  
		Size: 292.8 KB (292835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fe9e372cfe0caab24efa7e96eb98d339b54b9470b7f482cfdce79e15005191`  
		Last Modified: Tue, 17 Aug 2021 08:11:23 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26eeb178d4fdcdbf876869d68b8987595700e96b056699ed2a0e68687c7d3403`  
		Last Modified: Tue, 17 Aug 2021 08:11:26 GMT  
		Size: 39.0 MB (39012521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba0fab1910d9cfb77b99d702ad814df9dc27dadbe1cdf0a50247ba6e82b191c`  
		Last Modified: Tue, 17 Aug 2021 08:11:21 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35f1dd2b09826e38bed72be68349b4a00a5381a85505de247ed15381260afca`  
		Last Modified: Tue, 17 Aug 2021 08:11:21 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ac5b9c2f22264469e294a19641a7b391670cb42031b2339aa0771ef088696d`  
		Last Modified: Tue, 17 Aug 2021 08:11:21 GMT  
		Size: 2.1 KB (2055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75b315b30a0eacc36a44f10412cbc0c7ee42ffc59693b6627d7642ba6c5562b`  
		Last Modified: Tue, 17 Aug 2021 08:11:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3`

```console
$ docker pull couchdb@sha256:094d7d3c88e561eaf0cd77ffaf7823030f2c0a4a1ea41c892b99be9e3d74f2ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:e37a61155424c9392f840e18e7d791fa58c6af19396a85f4475c13a8c4f4621c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84508904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e385abfd92be3d6f88eefbf7fd40e19acc9d30377c011bfe3ea4c3e4fcfa034e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:38:17 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 17 Aug 2021 09:38:18 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 17 Aug 2021 09:38:39 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:38:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 17 Aug 2021 09:38:45 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 17 Aug 2021 09:38:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:39:18 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 17 Aug 2021 09:39:20 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 17 Aug 2021 09:39:45 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 17 Aug 2021 09:39:46 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 17 Aug 2021 09:39:47 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 17 Aug 2021 09:39:47 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 17 Aug 2021 09:39:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 17 Aug 2021 09:39:49 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 09:39:49 GMT
VOLUME [/opt/couchdb/data]
# Tue, 17 Aug 2021 09:39:49 GMT
EXPOSE 4369 5984 9100
# Tue, 17 Aug 2021 09:39:50 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f42f4d38cbf31bed3f27b58346190ea29ee14cec152ad44f07ef55175d9c055`  
		Last Modified: Tue, 17 Aug 2021 09:40:15 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b8216568b0598794cab6ed82a1c24c039865819e4ac0cdf2b871a943ac813b`  
		Last Modified: Tue, 17 Aug 2021 09:40:15 GMT  
		Size: 6.7 MB (6690783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eed64046c4dd433adb7d77997f00edb049f5d6cbc3fc5ddf3d61527741be6db`  
		Last Modified: Tue, 17 Aug 2021 09:40:13 GMT  
		Size: 1.3 MB (1258341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cba51966f0872e9bd9dac956ed819756d7b3b7c6f039ab31be7c8c9e8baa1ce`  
		Last Modified: Tue, 17 Aug 2021 09:40:13 GMT  
		Size: 293.0 KB (292974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8202e5f9d59551d3c66f183f03417ee311966bb3d6c0b7d3c9798314232b8986`  
		Last Modified: Tue, 17 Aug 2021 09:40:38 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0dcecb097e2e6b7350c669da4db8e4e14b06405c8cb937540b669a1071c0350`  
		Last Modified: Tue, 17 Aug 2021 09:40:44 GMT  
		Size: 49.1 MB (49113803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff91ea03c5ea787f36358768f71a6a3a1b3914e9f22cb33681d2329d6f47030`  
		Last Modified: Tue, 17 Aug 2021 09:40:36 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17b674c40f8737133bb393c5ae9de618ae2584db47c95040cdd8076e72d5a41`  
		Last Modified: Tue, 17 Aug 2021 09:40:36 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0883416cf372ee9e76d8fb14f4340f56a1bdffdc86171c8cafdfc38a053e73c8`  
		Last Modified: Tue, 17 Aug 2021 09:40:36 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb1b38ac64d87240ac4c63d1698e0c4298a59aa6f6bf67b0407ca9da8c64de9`  
		Last Modified: Tue, 17 Aug 2021 09:40:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:c24f7a9b72f99f8de9dd9aafbbf91c2113d20bbef8e930e7f0aa099929454fba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72941030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62316d039132754d9d4443adc0abf22c1589b3ecafd4d8a81755bbd0b8964298`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 08:09:33 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 17 Aug 2021 08:09:33 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 17 Aug 2021 08:09:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 08:09:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 17 Aug 2021 08:09:45 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 17 Aug 2021 08:09:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 08:10:17 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 17 Aug 2021 08:10:17 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 17 Aug 2021 08:10:29 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 17 Aug 2021 08:10:30 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 17 Aug 2021 08:10:30 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 17 Aug 2021 08:10:30 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 17 Aug 2021 08:10:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 17 Aug 2021 08:10:31 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 08:10:31 GMT
VOLUME [/opt/couchdb/data]
# Tue, 17 Aug 2021 08:10:31 GMT
EXPOSE 4369 5984 9100
# Tue, 17 Aug 2021 08:10:32 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab787026ef6a8144c5eabbda8d5bdf43afc3c79eef1ada02802921541490d37`  
		Last Modified: Tue, 17 Aug 2021 08:11:00 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ebe0a9c5656679672b817a6a586b31d8a518f90b2f77b5e5a0d70841c93a47`  
		Last Modified: Tue, 17 Aug 2021 08:10:59 GMT  
		Size: 6.6 MB (6550146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67fe32ef3fc734dde11d93c43255cdc4631d4f400588f69dbd6fca417c452e7`  
		Last Modified: Tue, 17 Aug 2021 08:10:57 GMT  
		Size: 1.2 MB (1163423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a7736bc7346c11850cfda36cd6466ed5503f0bbaf145f42af99fbc8e23ee4c`  
		Last Modified: Tue, 17 Aug 2021 08:10:57 GMT  
		Size: 292.8 KB (292835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fe9e372cfe0caab24efa7e96eb98d339b54b9470b7f482cfdce79e15005191`  
		Last Modified: Tue, 17 Aug 2021 08:11:23 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26eeb178d4fdcdbf876869d68b8987595700e96b056699ed2a0e68687c7d3403`  
		Last Modified: Tue, 17 Aug 2021 08:11:26 GMT  
		Size: 39.0 MB (39012521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba0fab1910d9cfb77b99d702ad814df9dc27dadbe1cdf0a50247ba6e82b191c`  
		Last Modified: Tue, 17 Aug 2021 08:11:21 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35f1dd2b09826e38bed72be68349b4a00a5381a85505de247ed15381260afca`  
		Last Modified: Tue, 17 Aug 2021 08:11:21 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ac5b9c2f22264469e294a19641a7b391670cb42031b2339aa0771ef088696d`  
		Last Modified: Tue, 17 Aug 2021 08:11:21 GMT  
		Size: 2.1 KB (2055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75b315b30a0eacc36a44f10412cbc0c7ee42ffc59693b6627d7642ba6c5562b`  
		Last Modified: Tue, 17 Aug 2021 08:11:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3.1`

```console
$ docker pull couchdb@sha256:094d7d3c88e561eaf0cd77ffaf7823030f2c0a4a1ea41c892b99be9e3d74f2ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:e37a61155424c9392f840e18e7d791fa58c6af19396a85f4475c13a8c4f4621c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84508904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e385abfd92be3d6f88eefbf7fd40e19acc9d30377c011bfe3ea4c3e4fcfa034e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:38:17 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 17 Aug 2021 09:38:18 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 17 Aug 2021 09:38:39 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:38:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 17 Aug 2021 09:38:45 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 17 Aug 2021 09:38:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:39:18 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 17 Aug 2021 09:39:20 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 17 Aug 2021 09:39:45 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 17 Aug 2021 09:39:46 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 17 Aug 2021 09:39:47 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 17 Aug 2021 09:39:47 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 17 Aug 2021 09:39:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 17 Aug 2021 09:39:49 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 09:39:49 GMT
VOLUME [/opt/couchdb/data]
# Tue, 17 Aug 2021 09:39:49 GMT
EXPOSE 4369 5984 9100
# Tue, 17 Aug 2021 09:39:50 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f42f4d38cbf31bed3f27b58346190ea29ee14cec152ad44f07ef55175d9c055`  
		Last Modified: Tue, 17 Aug 2021 09:40:15 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b8216568b0598794cab6ed82a1c24c039865819e4ac0cdf2b871a943ac813b`  
		Last Modified: Tue, 17 Aug 2021 09:40:15 GMT  
		Size: 6.7 MB (6690783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eed64046c4dd433adb7d77997f00edb049f5d6cbc3fc5ddf3d61527741be6db`  
		Last Modified: Tue, 17 Aug 2021 09:40:13 GMT  
		Size: 1.3 MB (1258341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cba51966f0872e9bd9dac956ed819756d7b3b7c6f039ab31be7c8c9e8baa1ce`  
		Last Modified: Tue, 17 Aug 2021 09:40:13 GMT  
		Size: 293.0 KB (292974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8202e5f9d59551d3c66f183f03417ee311966bb3d6c0b7d3c9798314232b8986`  
		Last Modified: Tue, 17 Aug 2021 09:40:38 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0dcecb097e2e6b7350c669da4db8e4e14b06405c8cb937540b669a1071c0350`  
		Last Modified: Tue, 17 Aug 2021 09:40:44 GMT  
		Size: 49.1 MB (49113803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff91ea03c5ea787f36358768f71a6a3a1b3914e9f22cb33681d2329d6f47030`  
		Last Modified: Tue, 17 Aug 2021 09:40:36 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a17b674c40f8737133bb393c5ae9de618ae2584db47c95040cdd8076e72d5a41`  
		Last Modified: Tue, 17 Aug 2021 09:40:36 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0883416cf372ee9e76d8fb14f4340f56a1bdffdc86171c8cafdfc38a053e73c8`  
		Last Modified: Tue, 17 Aug 2021 09:40:36 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb1b38ac64d87240ac4c63d1698e0c4298a59aa6f6bf67b0407ca9da8c64de9`  
		Last Modified: Tue, 17 Aug 2021 09:40:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:c24f7a9b72f99f8de9dd9aafbbf91c2113d20bbef8e930e7f0aa099929454fba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72941030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62316d039132754d9d4443adc0abf22c1589b3ecafd4d8a81755bbd0b8964298`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 08:09:33 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 17 Aug 2021 08:09:33 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 17 Aug 2021 08:09:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 08:09:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 17 Aug 2021 08:09:45 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 17 Aug 2021 08:09:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 08:10:17 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 17 Aug 2021 08:10:17 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 17 Aug 2021 08:10:29 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 17 Aug 2021 08:10:30 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 17 Aug 2021 08:10:30 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 17 Aug 2021 08:10:30 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 17 Aug 2021 08:10:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 17 Aug 2021 08:10:31 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 08:10:31 GMT
VOLUME [/opt/couchdb/data]
# Tue, 17 Aug 2021 08:10:31 GMT
EXPOSE 4369 5984 9100
# Tue, 17 Aug 2021 08:10:32 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab787026ef6a8144c5eabbda8d5bdf43afc3c79eef1ada02802921541490d37`  
		Last Modified: Tue, 17 Aug 2021 08:11:00 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ebe0a9c5656679672b817a6a586b31d8a518f90b2f77b5e5a0d70841c93a47`  
		Last Modified: Tue, 17 Aug 2021 08:10:59 GMT  
		Size: 6.6 MB (6550146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67fe32ef3fc734dde11d93c43255cdc4631d4f400588f69dbd6fca417c452e7`  
		Last Modified: Tue, 17 Aug 2021 08:10:57 GMT  
		Size: 1.2 MB (1163423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a7736bc7346c11850cfda36cd6466ed5503f0bbaf145f42af99fbc8e23ee4c`  
		Last Modified: Tue, 17 Aug 2021 08:10:57 GMT  
		Size: 292.8 KB (292835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fe9e372cfe0caab24efa7e96eb98d339b54b9470b7f482cfdce79e15005191`  
		Last Modified: Tue, 17 Aug 2021 08:11:23 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26eeb178d4fdcdbf876869d68b8987595700e96b056699ed2a0e68687c7d3403`  
		Last Modified: Tue, 17 Aug 2021 08:11:26 GMT  
		Size: 39.0 MB (39012521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba0fab1910d9cfb77b99d702ad814df9dc27dadbe1cdf0a50247ba6e82b191c`  
		Last Modified: Tue, 17 Aug 2021 08:11:21 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35f1dd2b09826e38bed72be68349b4a00a5381a85505de247ed15381260afca`  
		Last Modified: Tue, 17 Aug 2021 08:11:21 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ac5b9c2f22264469e294a19641a7b391670cb42031b2339aa0771ef088696d`  
		Last Modified: Tue, 17 Aug 2021 08:11:21 GMT  
		Size: 2.1 KB (2055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75b315b30a0eacc36a44f10412cbc0c7ee42ffc59693b6627d7642ba6c5562b`  
		Last Modified: Tue, 17 Aug 2021 08:11:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3`

```console
$ docker pull couchdb@sha256:2116065ff651d516bac7c3521229d142982487c55792944e02be93fc44d94bbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3` - linux; amd64

```console
$ docker pull couchdb@sha256:f842b081d584a9cebd2c7e9236cf83573dd709d8536f134c25748bd2db6f8f15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.8 MB (83771505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14502741b94c59331f032467a706322ac7a366d8803179a8a59a52ccafb41a96`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:38:17 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 17 Aug 2021 09:38:18 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 17 Aug 2021 09:38:39 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:38:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 17 Aug 2021 09:38:45 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 17 Aug 2021 09:38:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:38:52 GMT
ENV COUCHDB_VERSION=3.1.1
# Tue, 17 Aug 2021 09:38:53 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 17 Aug 2021 09:39:09 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 17 Aug 2021 09:39:10 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 17 Aug 2021 09:39:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 17 Aug 2021 09:39:11 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 17 Aug 2021 09:39:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 17 Aug 2021 09:39:13 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 09:39:13 GMT
VOLUME [/opt/couchdb/data]
# Tue, 17 Aug 2021 09:39:13 GMT
EXPOSE 4369 5984 9100
# Tue, 17 Aug 2021 09:39:13 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f42f4d38cbf31bed3f27b58346190ea29ee14cec152ad44f07ef55175d9c055`  
		Last Modified: Tue, 17 Aug 2021 09:40:15 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b8216568b0598794cab6ed82a1c24c039865819e4ac0cdf2b871a943ac813b`  
		Last Modified: Tue, 17 Aug 2021 09:40:15 GMT  
		Size: 6.7 MB (6690783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eed64046c4dd433adb7d77997f00edb049f5d6cbc3fc5ddf3d61527741be6db`  
		Last Modified: Tue, 17 Aug 2021 09:40:13 GMT  
		Size: 1.3 MB (1258341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cba51966f0872e9bd9dac956ed819756d7b3b7c6f039ab31be7c8c9e8baa1ce`  
		Last Modified: Tue, 17 Aug 2021 09:40:13 GMT  
		Size: 293.0 KB (292974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d65e3faec249f895849040e0b4aaf63cf54c47334b53be172b175e58814491`  
		Last Modified: Tue, 17 Aug 2021 09:40:12 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86d59f14c279a50719e39dfbe41a4f9faf00faf4a49d3dc7dd7e473013f8870`  
		Last Modified: Tue, 17 Aug 2021 09:40:18 GMT  
		Size: 48.4 MB (48376415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2b701d40adb5e7ed270dbd7ee811b24742e501179af04ad97e09590c3cca1`  
		Last Modified: Tue, 17 Aug 2021 09:40:10 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c6100ff07eaad02be6c5725c74f06ac475ec795b8abce0132ab4735b859cb0`  
		Last Modified: Tue, 17 Aug 2021 09:40:10 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fbd510ecd6db8e961e87596cf295bce60babe8836c36a8c9e7d975733c9521`  
		Last Modified: Tue, 17 Aug 2021 09:40:10 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90225c0f1a6a0dd6719927c561d22e407323fe15e377723415fe6fc58bbb2daa`  
		Last Modified: Tue, 17 Aug 2021 09:40:10 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:dd84e57fbd0faf425780658104d397b60e416045e79a1d9ad6875f94136db802
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.8 MB (78786772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e503901387235ad71719d6b858db23dfa2790c3feb5fe61cd18caf43eff221b0`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 08:09:33 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 17 Aug 2021 08:09:33 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 17 Aug 2021 08:09:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 08:09:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 17 Aug 2021 08:09:45 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 17 Aug 2021 08:09:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 08:09:51 GMT
ENV COUCHDB_VERSION=3.1.1
# Tue, 17 Aug 2021 08:09:52 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 17 Aug 2021 08:10:05 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 17 Aug 2021 08:10:05 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 17 Aug 2021 08:10:05 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 17 Aug 2021 08:10:05 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 17 Aug 2021 08:10:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 17 Aug 2021 08:10:06 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 08:10:06 GMT
VOLUME [/opt/couchdb/data]
# Tue, 17 Aug 2021 08:10:07 GMT
EXPOSE 4369 5984 9100
# Tue, 17 Aug 2021 08:10:07 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab787026ef6a8144c5eabbda8d5bdf43afc3c79eef1ada02802921541490d37`  
		Last Modified: Tue, 17 Aug 2021 08:11:00 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ebe0a9c5656679672b817a6a586b31d8a518f90b2f77b5e5a0d70841c93a47`  
		Last Modified: Tue, 17 Aug 2021 08:10:59 GMT  
		Size: 6.6 MB (6550146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67fe32ef3fc734dde11d93c43255cdc4631d4f400588f69dbd6fca417c452e7`  
		Last Modified: Tue, 17 Aug 2021 08:10:57 GMT  
		Size: 1.2 MB (1163423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a7736bc7346c11850cfda36cd6466ed5503f0bbaf145f42af99fbc8e23ee4c`  
		Last Modified: Tue, 17 Aug 2021 08:10:57 GMT  
		Size: 292.8 KB (292835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674f4f8ee188a1fc3881a8df04010762aea5571dbd6f6f94bde11b6d99fcd226`  
		Last Modified: Tue, 17 Aug 2021 08:10:57 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7357dc2ac83e096d9a5a8339d536e1f107fe6ec9aa137f55f22ca3dc5b50ce2d`  
		Last Modified: Tue, 17 Aug 2021 08:11:01 GMT  
		Size: 44.9 MB (44858259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd867e8dd88bd32c96ea29ef89ca9d1a96eb3f2cecce22f7ed0bf15e53a5d973`  
		Last Modified: Tue, 17 Aug 2021 08:10:55 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdee44909007a1881df438bf583366a0a50b63445592b3768da9eb3e9a02c66b`  
		Last Modified: Tue, 17 Aug 2021 08:10:55 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5af2b755a984a8b02e191a3d99bc10694845107932d5b1388e565f5ae05b54`  
		Last Modified: Tue, 17 Aug 2021 08:10:55 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40fbecafdba0dbcfe6591ece6bd85ddce50a962bbbdc03a262a86ff64dc5caea`  
		Last Modified: Tue, 17 Aug 2021 08:10:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1`

```console
$ docker pull couchdb@sha256:2116065ff651d516bac7c3521229d142982487c55792944e02be93fc44d94bbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:f842b081d584a9cebd2c7e9236cf83573dd709d8536f134c25748bd2db6f8f15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.8 MB (83771505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14502741b94c59331f032467a706322ac7a366d8803179a8a59a52ccafb41a96`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:38:17 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 17 Aug 2021 09:38:18 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 17 Aug 2021 09:38:39 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:38:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 17 Aug 2021 09:38:45 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 17 Aug 2021 09:38:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:38:52 GMT
ENV COUCHDB_VERSION=3.1.1
# Tue, 17 Aug 2021 09:38:53 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 17 Aug 2021 09:39:09 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 17 Aug 2021 09:39:10 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 17 Aug 2021 09:39:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 17 Aug 2021 09:39:11 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 17 Aug 2021 09:39:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 17 Aug 2021 09:39:13 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 09:39:13 GMT
VOLUME [/opt/couchdb/data]
# Tue, 17 Aug 2021 09:39:13 GMT
EXPOSE 4369 5984 9100
# Tue, 17 Aug 2021 09:39:13 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f42f4d38cbf31bed3f27b58346190ea29ee14cec152ad44f07ef55175d9c055`  
		Last Modified: Tue, 17 Aug 2021 09:40:15 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b8216568b0598794cab6ed82a1c24c039865819e4ac0cdf2b871a943ac813b`  
		Last Modified: Tue, 17 Aug 2021 09:40:15 GMT  
		Size: 6.7 MB (6690783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eed64046c4dd433adb7d77997f00edb049f5d6cbc3fc5ddf3d61527741be6db`  
		Last Modified: Tue, 17 Aug 2021 09:40:13 GMT  
		Size: 1.3 MB (1258341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cba51966f0872e9bd9dac956ed819756d7b3b7c6f039ab31be7c8c9e8baa1ce`  
		Last Modified: Tue, 17 Aug 2021 09:40:13 GMT  
		Size: 293.0 KB (292974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d65e3faec249f895849040e0b4aaf63cf54c47334b53be172b175e58814491`  
		Last Modified: Tue, 17 Aug 2021 09:40:12 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86d59f14c279a50719e39dfbe41a4f9faf00faf4a49d3dc7dd7e473013f8870`  
		Last Modified: Tue, 17 Aug 2021 09:40:18 GMT  
		Size: 48.4 MB (48376415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2b701d40adb5e7ed270dbd7ee811b24742e501179af04ad97e09590c3cca1`  
		Last Modified: Tue, 17 Aug 2021 09:40:10 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c6100ff07eaad02be6c5725c74f06ac475ec795b8abce0132ab4735b859cb0`  
		Last Modified: Tue, 17 Aug 2021 09:40:10 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fbd510ecd6db8e961e87596cf295bce60babe8836c36a8c9e7d975733c9521`  
		Last Modified: Tue, 17 Aug 2021 09:40:10 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90225c0f1a6a0dd6719927c561d22e407323fe15e377723415fe6fc58bbb2daa`  
		Last Modified: Tue, 17 Aug 2021 09:40:10 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:dd84e57fbd0faf425780658104d397b60e416045e79a1d9ad6875f94136db802
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.8 MB (78786772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e503901387235ad71719d6b858db23dfa2790c3feb5fe61cd18caf43eff221b0`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 08:09:33 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 17 Aug 2021 08:09:33 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 17 Aug 2021 08:09:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 08:09:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 17 Aug 2021 08:09:45 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 17 Aug 2021 08:09:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 08:09:51 GMT
ENV COUCHDB_VERSION=3.1.1
# Tue, 17 Aug 2021 08:09:52 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 17 Aug 2021 08:10:05 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 17 Aug 2021 08:10:05 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 17 Aug 2021 08:10:05 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 17 Aug 2021 08:10:05 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 17 Aug 2021 08:10:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 17 Aug 2021 08:10:06 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 08:10:06 GMT
VOLUME [/opt/couchdb/data]
# Tue, 17 Aug 2021 08:10:07 GMT
EXPOSE 4369 5984 9100
# Tue, 17 Aug 2021 08:10:07 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab787026ef6a8144c5eabbda8d5bdf43afc3c79eef1ada02802921541490d37`  
		Last Modified: Tue, 17 Aug 2021 08:11:00 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ebe0a9c5656679672b817a6a586b31d8a518f90b2f77b5e5a0d70841c93a47`  
		Last Modified: Tue, 17 Aug 2021 08:10:59 GMT  
		Size: 6.6 MB (6550146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67fe32ef3fc734dde11d93c43255cdc4631d4f400588f69dbd6fca417c452e7`  
		Last Modified: Tue, 17 Aug 2021 08:10:57 GMT  
		Size: 1.2 MB (1163423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a7736bc7346c11850cfda36cd6466ed5503f0bbaf145f42af99fbc8e23ee4c`  
		Last Modified: Tue, 17 Aug 2021 08:10:57 GMT  
		Size: 292.8 KB (292835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674f4f8ee188a1fc3881a8df04010762aea5571dbd6f6f94bde11b6d99fcd226`  
		Last Modified: Tue, 17 Aug 2021 08:10:57 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7357dc2ac83e096d9a5a8339d536e1f107fe6ec9aa137f55f22ca3dc5b50ce2d`  
		Last Modified: Tue, 17 Aug 2021 08:11:01 GMT  
		Size: 44.9 MB (44858259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd867e8dd88bd32c96ea29ef89ca9d1a96eb3f2cecce22f7ed0bf15e53a5d973`  
		Last Modified: Tue, 17 Aug 2021 08:10:55 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdee44909007a1881df438bf583366a0a50b63445592b3768da9eb3e9a02c66b`  
		Last Modified: Tue, 17 Aug 2021 08:10:55 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5af2b755a984a8b02e191a3d99bc10694845107932d5b1388e565f5ae05b54`  
		Last Modified: Tue, 17 Aug 2021 08:10:55 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40fbecafdba0dbcfe6591ece6bd85ddce50a962bbbdc03a262a86ff64dc5caea`  
		Last Modified: Tue, 17 Aug 2021 08:10:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1.1`

```console
$ docker pull couchdb@sha256:2116065ff651d516bac7c3521229d142982487c55792944e02be93fc44d94bbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1.1` - linux; amd64

```console
$ docker pull couchdb@sha256:f842b081d584a9cebd2c7e9236cf83573dd709d8536f134c25748bd2db6f8f15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.8 MB (83771505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14502741b94c59331f032467a706322ac7a366d8803179a8a59a52ccafb41a96`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:38:17 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 17 Aug 2021 09:38:18 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 17 Aug 2021 09:38:39 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:38:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 17 Aug 2021 09:38:45 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 17 Aug 2021 09:38:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:38:52 GMT
ENV COUCHDB_VERSION=3.1.1
# Tue, 17 Aug 2021 09:38:53 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 17 Aug 2021 09:39:09 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 17 Aug 2021 09:39:10 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 17 Aug 2021 09:39:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 17 Aug 2021 09:39:11 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 17 Aug 2021 09:39:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 17 Aug 2021 09:39:13 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 09:39:13 GMT
VOLUME [/opt/couchdb/data]
# Tue, 17 Aug 2021 09:39:13 GMT
EXPOSE 4369 5984 9100
# Tue, 17 Aug 2021 09:39:13 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f42f4d38cbf31bed3f27b58346190ea29ee14cec152ad44f07ef55175d9c055`  
		Last Modified: Tue, 17 Aug 2021 09:40:15 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b8216568b0598794cab6ed82a1c24c039865819e4ac0cdf2b871a943ac813b`  
		Last Modified: Tue, 17 Aug 2021 09:40:15 GMT  
		Size: 6.7 MB (6690783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eed64046c4dd433adb7d77997f00edb049f5d6cbc3fc5ddf3d61527741be6db`  
		Last Modified: Tue, 17 Aug 2021 09:40:13 GMT  
		Size: 1.3 MB (1258341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cba51966f0872e9bd9dac956ed819756d7b3b7c6f039ab31be7c8c9e8baa1ce`  
		Last Modified: Tue, 17 Aug 2021 09:40:13 GMT  
		Size: 293.0 KB (292974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d65e3faec249f895849040e0b4aaf63cf54c47334b53be172b175e58814491`  
		Last Modified: Tue, 17 Aug 2021 09:40:12 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86d59f14c279a50719e39dfbe41a4f9faf00faf4a49d3dc7dd7e473013f8870`  
		Last Modified: Tue, 17 Aug 2021 09:40:18 GMT  
		Size: 48.4 MB (48376415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2b701d40adb5e7ed270dbd7ee811b24742e501179af04ad97e09590c3cca1`  
		Last Modified: Tue, 17 Aug 2021 09:40:10 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c6100ff07eaad02be6c5725c74f06ac475ec795b8abce0132ab4735b859cb0`  
		Last Modified: Tue, 17 Aug 2021 09:40:10 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fbd510ecd6db8e961e87596cf295bce60babe8836c36a8c9e7d975733c9521`  
		Last Modified: Tue, 17 Aug 2021 09:40:10 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90225c0f1a6a0dd6719927c561d22e407323fe15e377723415fe6fc58bbb2daa`  
		Last Modified: Tue, 17 Aug 2021 09:40:10 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:dd84e57fbd0faf425780658104d397b60e416045e79a1d9ad6875f94136db802
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.8 MB (78786772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e503901387235ad71719d6b858db23dfa2790c3feb5fe61cd18caf43eff221b0`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 08:09:33 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 17 Aug 2021 08:09:33 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 17 Aug 2021 08:09:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 08:09:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 17 Aug 2021 08:09:45 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 17 Aug 2021 08:09:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 08:09:51 GMT
ENV COUCHDB_VERSION=3.1.1
# Tue, 17 Aug 2021 08:09:52 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 17 Aug 2021 08:10:05 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 17 Aug 2021 08:10:05 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 17 Aug 2021 08:10:05 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 17 Aug 2021 08:10:05 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 17 Aug 2021 08:10:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 17 Aug 2021 08:10:06 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 08:10:06 GMT
VOLUME [/opt/couchdb/data]
# Tue, 17 Aug 2021 08:10:07 GMT
EXPOSE 4369 5984 9100
# Tue, 17 Aug 2021 08:10:07 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab787026ef6a8144c5eabbda8d5bdf43afc3c79eef1ada02802921541490d37`  
		Last Modified: Tue, 17 Aug 2021 08:11:00 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ebe0a9c5656679672b817a6a586b31d8a518f90b2f77b5e5a0d70841c93a47`  
		Last Modified: Tue, 17 Aug 2021 08:10:59 GMT  
		Size: 6.6 MB (6550146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67fe32ef3fc734dde11d93c43255cdc4631d4f400588f69dbd6fca417c452e7`  
		Last Modified: Tue, 17 Aug 2021 08:10:57 GMT  
		Size: 1.2 MB (1163423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a7736bc7346c11850cfda36cd6466ed5503f0bbaf145f42af99fbc8e23ee4c`  
		Last Modified: Tue, 17 Aug 2021 08:10:57 GMT  
		Size: 292.8 KB (292835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674f4f8ee188a1fc3881a8df04010762aea5571dbd6f6f94bde11b6d99fcd226`  
		Last Modified: Tue, 17 Aug 2021 08:10:57 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7357dc2ac83e096d9a5a8339d536e1f107fe6ec9aa137f55f22ca3dc5b50ce2d`  
		Last Modified: Tue, 17 Aug 2021 08:11:01 GMT  
		Size: 44.9 MB (44858259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd867e8dd88bd32c96ea29ef89ca9d1a96eb3f2cecce22f7ed0bf15e53a5d973`  
		Last Modified: Tue, 17 Aug 2021 08:10:55 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdee44909007a1881df438bf583366a0a50b63445592b3768da9eb3e9a02c66b`  
		Last Modified: Tue, 17 Aug 2021 08:10:55 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5af2b755a984a8b02e191a3d99bc10694845107932d5b1388e565f5ae05b54`  
		Last Modified: Tue, 17 Aug 2021 08:10:55 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40fbecafdba0dbcfe6591ece6bd85ddce50a962bbbdc03a262a86ff64dc5caea`  
		Last Modified: Tue, 17 Aug 2021 08:10:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:latest`

```console
$ docker pull couchdb@sha256:2116065ff651d516bac7c3521229d142982487c55792944e02be93fc44d94bbc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:f842b081d584a9cebd2c7e9236cf83573dd709d8536f134c25748bd2db6f8f15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.8 MB (83771505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14502741b94c59331f032467a706322ac7a366d8803179a8a59a52ccafb41a96`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:38:17 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 17 Aug 2021 09:38:18 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 17 Aug 2021 09:38:39 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:38:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 17 Aug 2021 09:38:45 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 17 Aug 2021 09:38:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:38:52 GMT
ENV COUCHDB_VERSION=3.1.1
# Tue, 17 Aug 2021 09:38:53 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 17 Aug 2021 09:39:09 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 17 Aug 2021 09:39:10 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 17 Aug 2021 09:39:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 17 Aug 2021 09:39:11 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 17 Aug 2021 09:39:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 17 Aug 2021 09:39:13 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 09:39:13 GMT
VOLUME [/opt/couchdb/data]
# Tue, 17 Aug 2021 09:39:13 GMT
EXPOSE 4369 5984 9100
# Tue, 17 Aug 2021 09:39:13 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f42f4d38cbf31bed3f27b58346190ea29ee14cec152ad44f07ef55175d9c055`  
		Last Modified: Tue, 17 Aug 2021 09:40:15 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b8216568b0598794cab6ed82a1c24c039865819e4ac0cdf2b871a943ac813b`  
		Last Modified: Tue, 17 Aug 2021 09:40:15 GMT  
		Size: 6.7 MB (6690783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eed64046c4dd433adb7d77997f00edb049f5d6cbc3fc5ddf3d61527741be6db`  
		Last Modified: Tue, 17 Aug 2021 09:40:13 GMT  
		Size: 1.3 MB (1258341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cba51966f0872e9bd9dac956ed819756d7b3b7c6f039ab31be7c8c9e8baa1ce`  
		Last Modified: Tue, 17 Aug 2021 09:40:13 GMT  
		Size: 293.0 KB (292974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d65e3faec249f895849040e0b4aaf63cf54c47334b53be172b175e58814491`  
		Last Modified: Tue, 17 Aug 2021 09:40:12 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86d59f14c279a50719e39dfbe41a4f9faf00faf4a49d3dc7dd7e473013f8870`  
		Last Modified: Tue, 17 Aug 2021 09:40:18 GMT  
		Size: 48.4 MB (48376415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2b701d40adb5e7ed270dbd7ee811b24742e501179af04ad97e09590c3cca1`  
		Last Modified: Tue, 17 Aug 2021 09:40:10 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c6100ff07eaad02be6c5725c74f06ac475ec795b8abce0132ab4735b859cb0`  
		Last Modified: Tue, 17 Aug 2021 09:40:10 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fbd510ecd6db8e961e87596cf295bce60babe8836c36a8c9e7d975733c9521`  
		Last Modified: Tue, 17 Aug 2021 09:40:10 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90225c0f1a6a0dd6719927c561d22e407323fe15e377723415fe6fc58bbb2daa`  
		Last Modified: Tue, 17 Aug 2021 09:40:10 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:dd84e57fbd0faf425780658104d397b60e416045e79a1d9ad6875f94136db802
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.8 MB (78786772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e503901387235ad71719d6b858db23dfa2790c3feb5fe61cd18caf43eff221b0`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 08:09:33 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 17 Aug 2021 08:09:33 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 17 Aug 2021 08:09:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 08:09:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 17 Aug 2021 08:09:45 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 17 Aug 2021 08:09:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 08:09:51 GMT
ENV COUCHDB_VERSION=3.1.1
# Tue, 17 Aug 2021 08:09:52 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 17 Aug 2021 08:10:05 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 17 Aug 2021 08:10:05 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 17 Aug 2021 08:10:05 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 17 Aug 2021 08:10:05 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 17 Aug 2021 08:10:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 17 Aug 2021 08:10:06 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 08:10:06 GMT
VOLUME [/opt/couchdb/data]
# Tue, 17 Aug 2021 08:10:07 GMT
EXPOSE 4369 5984 9100
# Tue, 17 Aug 2021 08:10:07 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab787026ef6a8144c5eabbda8d5bdf43afc3c79eef1ada02802921541490d37`  
		Last Modified: Tue, 17 Aug 2021 08:11:00 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ebe0a9c5656679672b817a6a586b31d8a518f90b2f77b5e5a0d70841c93a47`  
		Last Modified: Tue, 17 Aug 2021 08:10:59 GMT  
		Size: 6.6 MB (6550146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67fe32ef3fc734dde11d93c43255cdc4631d4f400588f69dbd6fca417c452e7`  
		Last Modified: Tue, 17 Aug 2021 08:10:57 GMT  
		Size: 1.2 MB (1163423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a7736bc7346c11850cfda36cd6466ed5503f0bbaf145f42af99fbc8e23ee4c`  
		Last Modified: Tue, 17 Aug 2021 08:10:57 GMT  
		Size: 292.8 KB (292835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674f4f8ee188a1fc3881a8df04010762aea5571dbd6f6f94bde11b6d99fcd226`  
		Last Modified: Tue, 17 Aug 2021 08:10:57 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7357dc2ac83e096d9a5a8339d536e1f107fe6ec9aa137f55f22ca3dc5b50ce2d`  
		Last Modified: Tue, 17 Aug 2021 08:11:01 GMT  
		Size: 44.9 MB (44858259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd867e8dd88bd32c96ea29ef89ca9d1a96eb3f2cecce22f7ed0bf15e53a5d973`  
		Last Modified: Tue, 17 Aug 2021 08:10:55 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdee44909007a1881df438bf583366a0a50b63445592b3768da9eb3e9a02c66b`  
		Last Modified: Tue, 17 Aug 2021 08:10:55 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5af2b755a984a8b02e191a3d99bc10694845107932d5b1388e565f5ae05b54`  
		Last Modified: Tue, 17 Aug 2021 08:10:55 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40fbecafdba0dbcfe6591ece6bd85ddce50a962bbbdc03a262a86ff64dc5caea`  
		Last Modified: Tue, 17 Aug 2021 08:10:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
