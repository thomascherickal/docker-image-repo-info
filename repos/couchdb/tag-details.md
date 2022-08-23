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
$ docker pull couchdb@sha256:379cc480ca8018dda6747a0dd84be3789b95a8a18ed219011ccb18e3ea0d0f00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2` - linux; amd64

```console
$ docker pull couchdb@sha256:13d018f1ed6e86c82a3b436b3256de29ff3087be2b3de00f6433db8522b40ac0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84523967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9038854c2182537bc8710d1982035a1750713c0c2810c33d2ad204c9fe5bd9b`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:10 GMT
ADD file:baca493d7744d12304f6d9c7b6ec0800453a0ba02cbf4005ec35c7b921adf0c4 in / 
# Tue, 23 Aug 2022 00:21:10 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:00:22 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 23 Aug 2022 01:00:23 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 23 Aug 2022 01:00:30 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:00:34 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 23 Aug 2022 01:00:34 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 23 Aug 2022 01:00:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:01:02 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 23 Aug 2022 01:01:03 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 23 Aug 2022 01:01:21 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 23 Aug 2022 01:01:21 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 23 Aug 2022 01:01:22 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 23 Aug 2022 01:01:22 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 23 Aug 2022 01:01:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 23 Aug 2022 01:01:22 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 23 Aug 2022 01:01:22 GMT
VOLUME [/opt/couchdb/data]
# Tue, 23 Aug 2022 01:01:23 GMT
EXPOSE 4369 5984 9100
# Tue, 23 Aug 2022 01:01:23 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:2238450926aa858e592e60bb5d68dd26eeab8a984eee45505ca89d2022e3b450`  
		Last Modified: Tue, 23 Aug 2022 00:25:43 GMT  
		Size: 27.1 MB (27138330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6084fa4d86e93366006f55826b94420b2f1e20e2091002b49c7ff36846bf51`  
		Last Modified: Tue, 23 Aug 2022 01:02:05 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1737606016d2a4df0846b77ccddfa4c2127ebd871472500aa3ae8dfd5e106bee`  
		Last Modified: Tue, 23 Aug 2022 01:02:04 GMT  
		Size: 6.7 MB (6698697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b674fd6baeb95da8cedb1b0eca5cc8e9d202a017dd85db0b0b5018cd5db686de`  
		Last Modified: Tue, 23 Aug 2022 01:02:03 GMT  
		Size: 1.3 MB (1258376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4eae5c4b34e7fc4f9287c166a1a3396cf39291938b60589fb2c41c2a2689f5`  
		Last Modified: Tue, 23 Aug 2022 01:02:03 GMT  
		Size: 293.0 KB (292997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751c6601a972ebbc68b9cb1a515bbd917ec52a98b412275dc9d61c90c0e6da77`  
		Last Modified: Tue, 23 Aug 2022 01:02:18 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840c9409c12d107d03d4252f199abfdb0dce68e2e94f9733704306a668294ba5`  
		Last Modified: Tue, 23 Aug 2022 01:02:22 GMT  
		Size: 49.1 MB (49128549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd987d9abb06923f49472c0af68f593df154a9dc22cd7bac5fdaffc6c63fb00`  
		Last Modified: Tue, 23 Aug 2022 01:02:16 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8b958f5957b88f8c8cd22ec9e725ccf6f8f1b72112bad1068e0a2c35aefc9d`  
		Last Modified: Tue, 23 Aug 2022 01:02:16 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790293a8baa732b1d7da51f61fc02fb31f9d3c5e115f37747526ca5bc45787a8`  
		Last Modified: Tue, 23 Aug 2022 01:02:16 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51d087410abead77d42c585db1cbb1cf0a19c06718660e091d7d3bfec989ea1`  
		Last Modified: Tue, 23 Aug 2022 01:02:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:4d27419ac8548d5697a69904409954b075eff3c85f130b61dc24734fd0b02da1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72533193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:279fccb83aaef6ba53144c947958807e2351eb025796431109aac874500def7a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 02 Aug 2022 00:41:03 GMT
ADD file:d973e057fdca9166fb9f39e73d7d5d4ca8ac2af6a55813580bf14a13cef4c159 in / 
# Tue, 02 Aug 2022 00:41:04 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:54:02 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 02 Aug 2022 01:54:03 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 02 Aug 2022 01:54:11 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:54:14 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 02 Aug 2022 01:54:15 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 02 Aug 2022 01:54:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:55:03 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 02 Aug 2022 01:55:04 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 02 Aug 2022 01:55:22 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 02 Aug 2022 01:55:23 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 02 Aug 2022 01:55:24 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 02 Aug 2022 01:55:25 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 02 Aug 2022 01:55:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 02 Aug 2022 01:55:26 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 02 Aug 2022 01:55:27 GMT
VOLUME [/opt/couchdb/data]
# Tue, 02 Aug 2022 01:55:28 GMT
EXPOSE 4369 5984 9100
# Tue, 02 Aug 2022 01:55:29 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6d588874b4737b02fc84169cf7d3d1d70f20c7f5dbd1ddfe27de4aff25e23314`  
		Last Modified: Tue, 02 Aug 2022 00:46:56 GMT  
		Size: 25.9 MB (25914363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffbb2e29bd8913eeb0828eb30855bd8099016bbccb4656f7a85247aff324e02`  
		Last Modified: Tue, 02 Aug 2022 01:56:25 GMT  
		Size: 3.3 KB (3321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:192633bb64010e741a13bef0a4f95d38e465792d3a07eac67e0d4b6f66c33390`  
		Last Modified: Tue, 02 Aug 2022 01:56:24 GMT  
		Size: 6.6 MB (6557119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9daf7a28b3a5155810d9966f34c4a4c0331f957d4458341c8e3683e074b5e376`  
		Last Modified: Tue, 02 Aug 2022 01:56:24 GMT  
		Size: 951.2 KB (951168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ee939b6b94519e887f775efeeb8e38f7c6753a794a56656ca795a354437b8e`  
		Last Modified: Tue, 02 Aug 2022 01:56:23 GMT  
		Size: 80.0 KB (79958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b37c305cd45c9aef4b1a597fc55fa8d3fa7e4f9897fa193afd26353b0cb078`  
		Last Modified: Tue, 02 Aug 2022 01:56:40 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457dc458bba7846a4079f786880799c5f68a2fd7d81ae7624bb5173592aba1ea`  
		Last Modified: Tue, 02 Aug 2022 01:56:42 GMT  
		Size: 39.0 MB (39023658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ba602d04fc89ca241f7f72d4089adde2e712789f5cb20abdc08e0b3631f3ef`  
		Last Modified: Tue, 02 Aug 2022 01:56:38 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd028aa13d7ec3c819b6f22e8e4abba06c33d9114c0ab5aea6477dd04611ded`  
		Last Modified: Tue, 02 Aug 2022 01:56:38 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbccfa07785ac255a6a516db7d50c754ca2a142980319abb5e4825d021e9677`  
		Last Modified: Tue, 02 Aug 2022 01:56:38 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a882295cd756e516c322046d3077da8fb85a77e71fcc9babb9d16f54b81e3c`  
		Last Modified: Tue, 02 Aug 2022 01:56:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3`

```console
$ docker pull couchdb@sha256:379cc480ca8018dda6747a0dd84be3789b95a8a18ed219011ccb18e3ea0d0f00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:13d018f1ed6e86c82a3b436b3256de29ff3087be2b3de00f6433db8522b40ac0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84523967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9038854c2182537bc8710d1982035a1750713c0c2810c33d2ad204c9fe5bd9b`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:10 GMT
ADD file:baca493d7744d12304f6d9c7b6ec0800453a0ba02cbf4005ec35c7b921adf0c4 in / 
# Tue, 23 Aug 2022 00:21:10 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:00:22 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 23 Aug 2022 01:00:23 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 23 Aug 2022 01:00:30 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:00:34 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 23 Aug 2022 01:00:34 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 23 Aug 2022 01:00:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:01:02 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 23 Aug 2022 01:01:03 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 23 Aug 2022 01:01:21 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 23 Aug 2022 01:01:21 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 23 Aug 2022 01:01:22 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 23 Aug 2022 01:01:22 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 23 Aug 2022 01:01:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 23 Aug 2022 01:01:22 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 23 Aug 2022 01:01:22 GMT
VOLUME [/opt/couchdb/data]
# Tue, 23 Aug 2022 01:01:23 GMT
EXPOSE 4369 5984 9100
# Tue, 23 Aug 2022 01:01:23 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:2238450926aa858e592e60bb5d68dd26eeab8a984eee45505ca89d2022e3b450`  
		Last Modified: Tue, 23 Aug 2022 00:25:43 GMT  
		Size: 27.1 MB (27138330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6084fa4d86e93366006f55826b94420b2f1e20e2091002b49c7ff36846bf51`  
		Last Modified: Tue, 23 Aug 2022 01:02:05 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1737606016d2a4df0846b77ccddfa4c2127ebd871472500aa3ae8dfd5e106bee`  
		Last Modified: Tue, 23 Aug 2022 01:02:04 GMT  
		Size: 6.7 MB (6698697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b674fd6baeb95da8cedb1b0eca5cc8e9d202a017dd85db0b0b5018cd5db686de`  
		Last Modified: Tue, 23 Aug 2022 01:02:03 GMT  
		Size: 1.3 MB (1258376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4eae5c4b34e7fc4f9287c166a1a3396cf39291938b60589fb2c41c2a2689f5`  
		Last Modified: Tue, 23 Aug 2022 01:02:03 GMT  
		Size: 293.0 KB (292997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751c6601a972ebbc68b9cb1a515bbd917ec52a98b412275dc9d61c90c0e6da77`  
		Last Modified: Tue, 23 Aug 2022 01:02:18 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840c9409c12d107d03d4252f199abfdb0dce68e2e94f9733704306a668294ba5`  
		Last Modified: Tue, 23 Aug 2022 01:02:22 GMT  
		Size: 49.1 MB (49128549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd987d9abb06923f49472c0af68f593df154a9dc22cd7bac5fdaffc6c63fb00`  
		Last Modified: Tue, 23 Aug 2022 01:02:16 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8b958f5957b88f8c8cd22ec9e725ccf6f8f1b72112bad1068e0a2c35aefc9d`  
		Last Modified: Tue, 23 Aug 2022 01:02:16 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790293a8baa732b1d7da51f61fc02fb31f9d3c5e115f37747526ca5bc45787a8`  
		Last Modified: Tue, 23 Aug 2022 01:02:16 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51d087410abead77d42c585db1cbb1cf0a19c06718660e091d7d3bfec989ea1`  
		Last Modified: Tue, 23 Aug 2022 01:02:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:4d27419ac8548d5697a69904409954b075eff3c85f130b61dc24734fd0b02da1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72533193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:279fccb83aaef6ba53144c947958807e2351eb025796431109aac874500def7a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 02 Aug 2022 00:41:03 GMT
ADD file:d973e057fdca9166fb9f39e73d7d5d4ca8ac2af6a55813580bf14a13cef4c159 in / 
# Tue, 02 Aug 2022 00:41:04 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:54:02 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 02 Aug 2022 01:54:03 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 02 Aug 2022 01:54:11 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:54:14 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 02 Aug 2022 01:54:15 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 02 Aug 2022 01:54:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:55:03 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 02 Aug 2022 01:55:04 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 02 Aug 2022 01:55:22 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 02 Aug 2022 01:55:23 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 02 Aug 2022 01:55:24 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 02 Aug 2022 01:55:25 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 02 Aug 2022 01:55:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 02 Aug 2022 01:55:26 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 02 Aug 2022 01:55:27 GMT
VOLUME [/opt/couchdb/data]
# Tue, 02 Aug 2022 01:55:28 GMT
EXPOSE 4369 5984 9100
# Tue, 02 Aug 2022 01:55:29 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6d588874b4737b02fc84169cf7d3d1d70f20c7f5dbd1ddfe27de4aff25e23314`  
		Last Modified: Tue, 02 Aug 2022 00:46:56 GMT  
		Size: 25.9 MB (25914363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffbb2e29bd8913eeb0828eb30855bd8099016bbccb4656f7a85247aff324e02`  
		Last Modified: Tue, 02 Aug 2022 01:56:25 GMT  
		Size: 3.3 KB (3321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:192633bb64010e741a13bef0a4f95d38e465792d3a07eac67e0d4b6f66c33390`  
		Last Modified: Tue, 02 Aug 2022 01:56:24 GMT  
		Size: 6.6 MB (6557119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9daf7a28b3a5155810d9966f34c4a4c0331f957d4458341c8e3683e074b5e376`  
		Last Modified: Tue, 02 Aug 2022 01:56:24 GMT  
		Size: 951.2 KB (951168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ee939b6b94519e887f775efeeb8e38f7c6753a794a56656ca795a354437b8e`  
		Last Modified: Tue, 02 Aug 2022 01:56:23 GMT  
		Size: 80.0 KB (79958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b37c305cd45c9aef4b1a597fc55fa8d3fa7e4f9897fa193afd26353b0cb078`  
		Last Modified: Tue, 02 Aug 2022 01:56:40 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457dc458bba7846a4079f786880799c5f68a2fd7d81ae7624bb5173592aba1ea`  
		Last Modified: Tue, 02 Aug 2022 01:56:42 GMT  
		Size: 39.0 MB (39023658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ba602d04fc89ca241f7f72d4089adde2e712789f5cb20abdc08e0b3631f3ef`  
		Last Modified: Tue, 02 Aug 2022 01:56:38 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd028aa13d7ec3c819b6f22e8e4abba06c33d9114c0ab5aea6477dd04611ded`  
		Last Modified: Tue, 02 Aug 2022 01:56:38 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbccfa07785ac255a6a516db7d50c754ca2a142980319abb5e4825d021e9677`  
		Last Modified: Tue, 02 Aug 2022 01:56:38 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a882295cd756e516c322046d3077da8fb85a77e71fcc9babb9d16f54b81e3c`  
		Last Modified: Tue, 02 Aug 2022 01:56:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3.1`

```console
$ docker pull couchdb@sha256:379cc480ca8018dda6747a0dd84be3789b95a8a18ed219011ccb18e3ea0d0f00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:13d018f1ed6e86c82a3b436b3256de29ff3087be2b3de00f6433db8522b40ac0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84523967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9038854c2182537bc8710d1982035a1750713c0c2810c33d2ad204c9fe5bd9b`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:10 GMT
ADD file:baca493d7744d12304f6d9c7b6ec0800453a0ba02cbf4005ec35c7b921adf0c4 in / 
# Tue, 23 Aug 2022 00:21:10 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:00:22 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 23 Aug 2022 01:00:23 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 23 Aug 2022 01:00:30 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:00:34 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 23 Aug 2022 01:00:34 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 23 Aug 2022 01:00:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:01:02 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 23 Aug 2022 01:01:03 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 23 Aug 2022 01:01:21 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 23 Aug 2022 01:01:21 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 23 Aug 2022 01:01:22 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 23 Aug 2022 01:01:22 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 23 Aug 2022 01:01:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 23 Aug 2022 01:01:22 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 23 Aug 2022 01:01:22 GMT
VOLUME [/opt/couchdb/data]
# Tue, 23 Aug 2022 01:01:23 GMT
EXPOSE 4369 5984 9100
# Tue, 23 Aug 2022 01:01:23 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:2238450926aa858e592e60bb5d68dd26eeab8a984eee45505ca89d2022e3b450`  
		Last Modified: Tue, 23 Aug 2022 00:25:43 GMT  
		Size: 27.1 MB (27138330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6084fa4d86e93366006f55826b94420b2f1e20e2091002b49c7ff36846bf51`  
		Last Modified: Tue, 23 Aug 2022 01:02:05 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1737606016d2a4df0846b77ccddfa4c2127ebd871472500aa3ae8dfd5e106bee`  
		Last Modified: Tue, 23 Aug 2022 01:02:04 GMT  
		Size: 6.7 MB (6698697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b674fd6baeb95da8cedb1b0eca5cc8e9d202a017dd85db0b0b5018cd5db686de`  
		Last Modified: Tue, 23 Aug 2022 01:02:03 GMT  
		Size: 1.3 MB (1258376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4eae5c4b34e7fc4f9287c166a1a3396cf39291938b60589fb2c41c2a2689f5`  
		Last Modified: Tue, 23 Aug 2022 01:02:03 GMT  
		Size: 293.0 KB (292997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751c6601a972ebbc68b9cb1a515bbd917ec52a98b412275dc9d61c90c0e6da77`  
		Last Modified: Tue, 23 Aug 2022 01:02:18 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840c9409c12d107d03d4252f199abfdb0dce68e2e94f9733704306a668294ba5`  
		Last Modified: Tue, 23 Aug 2022 01:02:22 GMT  
		Size: 49.1 MB (49128549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd987d9abb06923f49472c0af68f593df154a9dc22cd7bac5fdaffc6c63fb00`  
		Last Modified: Tue, 23 Aug 2022 01:02:16 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8b958f5957b88f8c8cd22ec9e725ccf6f8f1b72112bad1068e0a2c35aefc9d`  
		Last Modified: Tue, 23 Aug 2022 01:02:16 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790293a8baa732b1d7da51f61fc02fb31f9d3c5e115f37747526ca5bc45787a8`  
		Last Modified: Tue, 23 Aug 2022 01:02:16 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51d087410abead77d42c585db1cbb1cf0a19c06718660e091d7d3bfec989ea1`  
		Last Modified: Tue, 23 Aug 2022 01:02:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:4d27419ac8548d5697a69904409954b075eff3c85f130b61dc24734fd0b02da1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72533193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:279fccb83aaef6ba53144c947958807e2351eb025796431109aac874500def7a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 02 Aug 2022 00:41:03 GMT
ADD file:d973e057fdca9166fb9f39e73d7d5d4ca8ac2af6a55813580bf14a13cef4c159 in / 
# Tue, 02 Aug 2022 00:41:04 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:54:02 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 02 Aug 2022 01:54:03 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 02 Aug 2022 01:54:11 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:54:14 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 02 Aug 2022 01:54:15 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 02 Aug 2022 01:54:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:55:03 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 02 Aug 2022 01:55:04 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 02 Aug 2022 01:55:22 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 02 Aug 2022 01:55:23 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 02 Aug 2022 01:55:24 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 02 Aug 2022 01:55:25 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 02 Aug 2022 01:55:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 02 Aug 2022 01:55:26 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 02 Aug 2022 01:55:27 GMT
VOLUME [/opt/couchdb/data]
# Tue, 02 Aug 2022 01:55:28 GMT
EXPOSE 4369 5984 9100
# Tue, 02 Aug 2022 01:55:29 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6d588874b4737b02fc84169cf7d3d1d70f20c7f5dbd1ddfe27de4aff25e23314`  
		Last Modified: Tue, 02 Aug 2022 00:46:56 GMT  
		Size: 25.9 MB (25914363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffbb2e29bd8913eeb0828eb30855bd8099016bbccb4656f7a85247aff324e02`  
		Last Modified: Tue, 02 Aug 2022 01:56:25 GMT  
		Size: 3.3 KB (3321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:192633bb64010e741a13bef0a4f95d38e465792d3a07eac67e0d4b6f66c33390`  
		Last Modified: Tue, 02 Aug 2022 01:56:24 GMT  
		Size: 6.6 MB (6557119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9daf7a28b3a5155810d9966f34c4a4c0331f957d4458341c8e3683e074b5e376`  
		Last Modified: Tue, 02 Aug 2022 01:56:24 GMT  
		Size: 951.2 KB (951168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ee939b6b94519e887f775efeeb8e38f7c6753a794a56656ca795a354437b8e`  
		Last Modified: Tue, 02 Aug 2022 01:56:23 GMT  
		Size: 80.0 KB (79958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19b37c305cd45c9aef4b1a597fc55fa8d3fa7e4f9897fa193afd26353b0cb078`  
		Last Modified: Tue, 02 Aug 2022 01:56:40 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457dc458bba7846a4079f786880799c5f68a2fd7d81ae7624bb5173592aba1ea`  
		Last Modified: Tue, 02 Aug 2022 01:56:42 GMT  
		Size: 39.0 MB (39023658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ba602d04fc89ca241f7f72d4089adde2e712789f5cb20abdc08e0b3631f3ef`  
		Last Modified: Tue, 02 Aug 2022 01:56:38 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd028aa13d7ec3c819b6f22e8e4abba06c33d9114c0ab5aea6477dd04611ded`  
		Last Modified: Tue, 02 Aug 2022 01:56:38 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbccfa07785ac255a6a516db7d50c754ca2a142980319abb5e4825d021e9677`  
		Last Modified: Tue, 02 Aug 2022 01:56:38 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a882295cd756e516c322046d3077da8fb85a77e71fcc9babb9d16f54b81e3c`  
		Last Modified: Tue, 02 Aug 2022 01:56:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3`

```console
$ docker pull couchdb@sha256:fd7a739e37deab2c10119a81886ff8c626f9e1de6e786ed60b31ca9c30450035
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3` - linux; amd64

```console
$ docker pull couchdb@sha256:28124b34f4148ed792f9bf2c71207cc3ea9bb7e76546d67daffb19234952df81
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87503932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0396728d49f5ac43a68e07bf8b23d34cdbcec06f4aa08229ce8b509f9f465c64`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:59:42 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 23 Aug 2022 00:59:42 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 23 Aug 2022 00:59:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:59:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 23 Aug 2022 00:59:53 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 23 Aug 2022 00:59:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:59:59 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 23 Aug 2022 00:59:59 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 23 Aug 2022 01:00:13 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 23 Aug 2022 01:00:13 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 23 Aug 2022 01:00:13 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 23 Aug 2022 01:00:14 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 23 Aug 2022 01:00:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 23 Aug 2022 01:00:14 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 23 Aug 2022 01:00:14 GMT
VOLUME [/opt/couchdb/data]
# Tue, 23 Aug 2022 01:00:14 GMT
EXPOSE 4369 5984 9100
# Tue, 23 Aug 2022 01:00:15 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1836a36860638007d7b2592171befa5754532a9d47de8f0e775fad866c82393e`  
		Last Modified: Tue, 23 Aug 2022 01:01:43 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e2e2b5b7b5034043633af72843d3b8666f8ccc0c2aeae43af0afe8e9fdb2c8`  
		Last Modified: Tue, 23 Aug 2022 01:01:43 GMT  
		Size: 5.2 MB (5224227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c99ac86ee0acd5521ed2df4dce63d77342c2a96acff9b2af72b76e5893f62f`  
		Last Modified: Tue, 23 Aug 2022 01:01:42 GMT  
		Size: 1.6 MB (1553304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8979b473c30718ae0cbb8a38a2e402f873ad242554184f7beabb593d4451bfc0`  
		Last Modified: Tue, 23 Aug 2022 01:01:41 GMT  
		Size: 295.6 KB (295581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510ed5a8f7236ce7e23d8bb548f076632c0b48a3e1e8430e0e262ef6647f7ebc`  
		Last Modified: Tue, 23 Aug 2022 01:01:41 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e968620046651f8bd94db8256d249f0684ba2a454fb63d1c109ca1b45920ae`  
		Last Modified: Tue, 23 Aug 2022 01:01:45 GMT  
		Size: 49.0 MB (49042191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8920bb938feadb5c2b98dd12c72f655b1e47b736dd024cf1098c3f1acb2e645`  
		Last Modified: Tue, 23 Aug 2022 01:01:39 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a6954a2f0617948efb306d9b1a5b784d64a0beff38481b6828d069ca696e18`  
		Last Modified: Tue, 23 Aug 2022 01:01:39 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41292b445e0d087758fc8486322576d3605d68a540ca3fb3243dbc84ab1d4dda`  
		Last Modified: Tue, 23 Aug 2022 01:01:39 GMT  
		Size: 2.2 KB (2185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eaa46afbe00ace5c0c20bfc3c7912cde4600f9e8f942d5149e988d0473464fc`  
		Last Modified: Tue, 23 Aug 2022 01:01:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:2cc537fd46496d460ec408ea389dd4cc27c180608e89c59761c4682d6dac0cbd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.6 MB (85622605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faece9a6aa805f3e9d71e0136a8c7add2db196a28de98b26dc652d2eb88bf4ee`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:38 GMT
ADD file:6039adfbca55ed34a719c37672c664e3524130a0e2a3b8663629b8120b81b790 in / 
# Tue, 02 Aug 2022 00:40:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:53:11 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 02 Aug 2022 01:53:11 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 02 Aug 2022 01:53:19 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:53:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 02 Aug 2022 01:53:23 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 02 Aug 2022 01:53:29 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:53:29 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 02 Aug 2022 01:53:30 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 02 Aug 2022 01:53:44 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 02 Aug 2022 01:53:45 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 02 Aug 2022 01:53:46 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 02 Aug 2022 01:53:47 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 02 Aug 2022 01:53:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 02 Aug 2022 01:53:48 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 02 Aug 2022 01:53:49 GMT
VOLUME [/opt/couchdb/data]
# Tue, 02 Aug 2022 01:53:50 GMT
EXPOSE 4369 5984 9100
# Tue, 02 Aug 2022 01:53:51 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:a9fe95647e78b5516c7e2327355b6996e2ea295cd76ae242cbfe87f016b4e760`  
		Last Modified: Tue, 02 Aug 2022 00:46:05 GMT  
		Size: 30.1 MB (30054304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f36ebccf7ea0ca6c4e42a56d3e761f51620dde7809ff4cd6c9c47f4d92dda45`  
		Last Modified: Tue, 02 Aug 2022 01:56:00 GMT  
		Size: 3.3 KB (3320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57988538f1066bad59a075d99704fbc2ed80b7f279168e98ae1ac061cddb0e54`  
		Last Modified: Tue, 02 Aug 2022 01:55:59 GMT  
		Size: 5.2 MB (5207882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d6f84207bfc6da3f978a06e64089cd163b0b7cfce56aa03f050fffcf6aa1fa`  
		Last Modified: Tue, 02 Aug 2022 01:55:59 GMT  
		Size: 1.2 MB (1221114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f79004f600a1443f5dd0ab501f8d2726ae96d9790d635ef946c8ab58fc7639`  
		Last Modified: Tue, 02 Aug 2022 01:55:58 GMT  
		Size: 79.2 KB (79204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea246a4776bb764303aebd0c230598840bac0a3067bf67395be8aa1d4a9796c0`  
		Last Modified: Tue, 02 Aug 2022 01:55:58 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afec05def1afee67aa528ce2ecc14afe3dd947292160af59436483a6eb8307d8`  
		Last Modified: Tue, 02 Aug 2022 01:56:02 GMT  
		Size: 49.1 MB (49053054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f205452c1f21b508f3eff3ca454e831b24598073851b7c10ad77092021c63b80`  
		Last Modified: Tue, 02 Aug 2022 01:55:56 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb0d06feb8b8d747a8a616d3dbdb4dbff7f3d1c07726fc7fabbd0d857588a65`  
		Last Modified: Tue, 02 Aug 2022 01:55:56 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833640fe1553f0d57940524d810c11944b07d0171e7979f091beca62d8c235a2`  
		Last Modified: Tue, 02 Aug 2022 01:55:56 GMT  
		Size: 2.2 KB (2184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c60df208533e1fc53978ad88b63060ba603756eef0b46beaa35572ff7fc1aa2`  
		Last Modified: Tue, 02 Aug 2022 01:55:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; ppc64le

```console
$ docker pull couchdb@sha256:1e403730c20e44b3297dc2ca59567dc4f7f8608ea517c016cf6b814fa428f6f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93209223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9532ba1899566dfcf8498c068f3eca6b79c8afa3fae5d939c52255a7ae9d96b4`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 02 Aug 2022 01:17:30 GMT
ADD file:3a95a896d463569ce82199957052b3467123a4bd3385a0a4e397cf08402a99c3 in / 
# Tue, 02 Aug 2022 01:17:32 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:45:51 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 02 Aug 2022 01:45:52 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 02 Aug 2022 01:46:07 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:46:13 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 02 Aug 2022 01:46:14 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 02 Aug 2022 01:46:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:46:24 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 02 Aug 2022 01:46:25 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 02 Aug 2022 01:46:47 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 02 Aug 2022 01:46:48 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 02 Aug 2022 01:46:49 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 02 Aug 2022 01:46:49 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 02 Aug 2022 01:46:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 02 Aug 2022 01:46:50 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 02 Aug 2022 01:46:51 GMT
VOLUME [/opt/couchdb/data]
# Tue, 02 Aug 2022 01:46:51 GMT
EXPOSE 4369 5984 9100
# Tue, 02 Aug 2022 01:46:51 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:5241cd116d6e6e2d62f3d8c2245b74daca9f6cc154eaccd738feb41984c74714`  
		Last Modified: Tue, 02 Aug 2022 01:24:39 GMT  
		Size: 35.3 MB (35272771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd616d47d2a8f573397f07010fd143095697a31e5f728cac1c1b7269738c47a`  
		Last Modified: Tue, 02 Aug 2022 01:47:19 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1a77f89868067efb94d63fe88604742503d85f515b25f7ab84711a016d3e4f`  
		Last Modified: Tue, 02 Aug 2022 01:47:19 GMT  
		Size: 6.0 MB (6043687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f741e9865e3fdcb0bd227a5993c271ef87a11ea1804cdbbdd3814773c085fd4`  
		Last Modified: Tue, 02 Aug 2022 01:47:17 GMT  
		Size: 1.5 MB (1509129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a56ea83b77070cf87034a857804e0e5dc6e22a75e16d352364a0c6f2cf81cd`  
		Last Modified: Tue, 02 Aug 2022 01:47:17 GMT  
		Size: 295.5 KB (295465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe12fc56262eb1a9961df421373e9e93f9755a2e423207066c543f023b488f7`  
		Last Modified: Tue, 02 Aug 2022 01:47:17 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51cf6274a3105c304db4a54d429807a6d97294428538c809f791158d3a610942`  
		Last Modified: Tue, 02 Aug 2022 01:47:24 GMT  
		Size: 50.1 MB (50081019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48855ad409841498cce766b60da4e1cd5f59a6da57e69031b5cb1e70944c7e06`  
		Last Modified: Tue, 02 Aug 2022 01:47:14 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d93f33d896f43831a247689b5fe6b3c85972c92c57c27a55ae2ca50fd89216c`  
		Last Modified: Tue, 02 Aug 2022 01:47:15 GMT  
		Size: 768.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2efe54a8f4ae1598aa0cad697c24d96e9bd6701de850e533e452cb0ddc5df62`  
		Last Modified: Tue, 02 Aug 2022 01:47:15 GMT  
		Size: 2.2 KB (2188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fa6fb130ed09e3914ae920a1e5cd0affdd896fa22de827e2b222afb58a04e4`  
		Last Modified: Tue, 02 Aug 2022 01:47:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1`

```console
$ docker pull couchdb@sha256:6e74fd6d7f1858b1005d80798f9db4d85f544c9721a0e341bbef7aa379642438
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:ac1928bc048a788609af6eff591800b3699bfae238d9bbb8c1ccbc0dc4549f82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80007797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1b76c6938dc5cc74f8600648e21f969681a99fe38f773c009fe21020e35d9a0`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:10 GMT
ADD file:baca493d7744d12304f6d9c7b6ec0800453a0ba02cbf4005ec35c7b921adf0c4 in / 
# Tue, 23 Aug 2022 00:21:10 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:00:22 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 23 Aug 2022 01:00:23 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 23 Aug 2022 01:00:30 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:00:34 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 23 Aug 2022 01:00:34 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 23 Aug 2022 01:00:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:00:41 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 23 Aug 2022 01:00:41 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 23 Aug 2022 01:00:55 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 23 Aug 2022 01:00:55 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 23 Aug 2022 01:00:55 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 23 Aug 2022 01:00:55 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 23 Aug 2022 01:00:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 23 Aug 2022 01:00:56 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 23 Aug 2022 01:00:56 GMT
VOLUME [/opt/couchdb/data]
# Tue, 23 Aug 2022 01:00:56 GMT
EXPOSE 4369 5984 9100
# Tue, 23 Aug 2022 01:00:56 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:2238450926aa858e592e60bb5d68dd26eeab8a984eee45505ca89d2022e3b450`  
		Last Modified: Tue, 23 Aug 2022 00:25:43 GMT  
		Size: 27.1 MB (27138330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6084fa4d86e93366006f55826b94420b2f1e20e2091002b49c7ff36846bf51`  
		Last Modified: Tue, 23 Aug 2022 01:02:05 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1737606016d2a4df0846b77ccddfa4c2127ebd871472500aa3ae8dfd5e106bee`  
		Last Modified: Tue, 23 Aug 2022 01:02:04 GMT  
		Size: 6.7 MB (6698697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b674fd6baeb95da8cedb1b0eca5cc8e9d202a017dd85db0b0b5018cd5db686de`  
		Last Modified: Tue, 23 Aug 2022 01:02:03 GMT  
		Size: 1.3 MB (1258376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4eae5c4b34e7fc4f9287c166a1a3396cf39291938b60589fb2c41c2a2689f5`  
		Last Modified: Tue, 23 Aug 2022 01:02:03 GMT  
		Size: 293.0 KB (292997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77632105ca22f652ef3d63e33b26ff1e36790ec0b02e3342597b90d4799f040`  
		Last Modified: Tue, 23 Aug 2022 01:02:02 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dad725ab9e6a3ba9502491f26af9b845cfc79c33b5f8473cea59ae1e80d6624`  
		Last Modified: Tue, 23 Aug 2022 01:02:05 GMT  
		Size: 44.6 MB (44612383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53645a91576006b5d14ec1cbff7cdd2b0b26af9ae2d78334b534621cb8880fbd`  
		Last Modified: Tue, 23 Aug 2022 01:02:00 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6d6954df5ef6586f14c99e7f6f81eaac9d35c01fe36f119036b5af779bb6b7`  
		Last Modified: Tue, 23 Aug 2022 01:02:00 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062905c89617104a732efd46df6237c6236e6a76639da396eb0610ebdba9af6d`  
		Last Modified: Tue, 23 Aug 2022 01:02:00 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3d0c25e7b5f1251abafa7fd376b419f9dc6e33718a7bd3e189ae4508924b7d`  
		Last Modified: Tue, 23 Aug 2022 01:02:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:f2a4273e1c132ca7d51a766e8924507ecb2fa433447ad227a94b9ebd735b1bb2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74622170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5a97102b89f803528279a50487b76e5cf67c9db39b6e50eaaa512ca9c876c9c`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 02 Aug 2022 00:41:03 GMT
ADD file:d973e057fdca9166fb9f39e73d7d5d4ca8ac2af6a55813580bf14a13cef4c159 in / 
# Tue, 02 Aug 2022 00:41:04 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:54:02 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 02 Aug 2022 01:54:03 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 02 Aug 2022 01:54:11 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:54:14 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 02 Aug 2022 01:54:15 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 02 Aug 2022 01:54:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:54:23 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 02 Aug 2022 01:54:24 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 02 Aug 2022 01:54:42 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 02 Aug 2022 01:54:43 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 02 Aug 2022 01:54:44 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 02 Aug 2022 01:54:45 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 02 Aug 2022 01:54:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 02 Aug 2022 01:54:46 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 02 Aug 2022 01:54:47 GMT
VOLUME [/opt/couchdb/data]
# Tue, 02 Aug 2022 01:54:48 GMT
EXPOSE 4369 5984 9100
# Tue, 02 Aug 2022 01:54:49 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6d588874b4737b02fc84169cf7d3d1d70f20c7f5dbd1ddfe27de4aff25e23314`  
		Last Modified: Tue, 02 Aug 2022 00:46:56 GMT  
		Size: 25.9 MB (25914363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffbb2e29bd8913eeb0828eb30855bd8099016bbccb4656f7a85247aff324e02`  
		Last Modified: Tue, 02 Aug 2022 01:56:25 GMT  
		Size: 3.3 KB (3321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:192633bb64010e741a13bef0a4f95d38e465792d3a07eac67e0d4b6f66c33390`  
		Last Modified: Tue, 02 Aug 2022 01:56:24 GMT  
		Size: 6.6 MB (6557119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9daf7a28b3a5155810d9966f34c4a4c0331f957d4458341c8e3683e074b5e376`  
		Last Modified: Tue, 02 Aug 2022 01:56:24 GMT  
		Size: 951.2 KB (951168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ee939b6b94519e887f775efeeb8e38f7c6753a794a56656ca795a354437b8e`  
		Last Modified: Tue, 02 Aug 2022 01:56:23 GMT  
		Size: 80.0 KB (79958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c1e56d17f55a93521148990b2f560a6401fc7bd06faec0f376e4a453cac903`  
		Last Modified: Tue, 02 Aug 2022 01:56:23 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f09ea26de4b63303321d6c9ea720b4e8116a8cdc261bc1dd0060fc58d7ebd3c`  
		Last Modified: Tue, 02 Aug 2022 01:56:26 GMT  
		Size: 41.1 MB (41112637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9354706eff555a86dfa9987feb6ca7ce1176d000dab12847b18f8349666d2d`  
		Last Modified: Tue, 02 Aug 2022 01:56:21 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a84a0c3df2496088046a0d00a1ef05a3c452627e37d79a60db80c6499c634cf`  
		Last Modified: Tue, 02 Aug 2022 01:56:21 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6541aa9f62e6abcfcca9b7d5155e5f035aef4d612c0aad572e69ee1ad006956a`  
		Last Modified: Tue, 02 Aug 2022 01:56:21 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7e0309716beca4eb00c072e238149bb9236708376e0b9b80ae104c047b960f`  
		Last Modified: Tue, 02 Aug 2022 01:56:21 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1.2`

```console
$ docker pull couchdb@sha256:6e74fd6d7f1858b1005d80798f9db4d85f544c9721a0e341bbef7aa379642438
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1.2` - linux; amd64

```console
$ docker pull couchdb@sha256:ac1928bc048a788609af6eff591800b3699bfae238d9bbb8c1ccbc0dc4549f82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80007797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1b76c6938dc5cc74f8600648e21f969681a99fe38f773c009fe21020e35d9a0`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:10 GMT
ADD file:baca493d7744d12304f6d9c7b6ec0800453a0ba02cbf4005ec35c7b921adf0c4 in / 
# Tue, 23 Aug 2022 00:21:10 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:00:22 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 23 Aug 2022 01:00:23 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 23 Aug 2022 01:00:30 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:00:34 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 23 Aug 2022 01:00:34 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 23 Aug 2022 01:00:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:00:41 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 23 Aug 2022 01:00:41 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 23 Aug 2022 01:00:55 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 23 Aug 2022 01:00:55 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 23 Aug 2022 01:00:55 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 23 Aug 2022 01:00:55 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 23 Aug 2022 01:00:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 23 Aug 2022 01:00:56 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 23 Aug 2022 01:00:56 GMT
VOLUME [/opt/couchdb/data]
# Tue, 23 Aug 2022 01:00:56 GMT
EXPOSE 4369 5984 9100
# Tue, 23 Aug 2022 01:00:56 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:2238450926aa858e592e60bb5d68dd26eeab8a984eee45505ca89d2022e3b450`  
		Last Modified: Tue, 23 Aug 2022 00:25:43 GMT  
		Size: 27.1 MB (27138330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6084fa4d86e93366006f55826b94420b2f1e20e2091002b49c7ff36846bf51`  
		Last Modified: Tue, 23 Aug 2022 01:02:05 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1737606016d2a4df0846b77ccddfa4c2127ebd871472500aa3ae8dfd5e106bee`  
		Last Modified: Tue, 23 Aug 2022 01:02:04 GMT  
		Size: 6.7 MB (6698697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b674fd6baeb95da8cedb1b0eca5cc8e9d202a017dd85db0b0b5018cd5db686de`  
		Last Modified: Tue, 23 Aug 2022 01:02:03 GMT  
		Size: 1.3 MB (1258376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4eae5c4b34e7fc4f9287c166a1a3396cf39291938b60589fb2c41c2a2689f5`  
		Last Modified: Tue, 23 Aug 2022 01:02:03 GMT  
		Size: 293.0 KB (292997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77632105ca22f652ef3d63e33b26ff1e36790ec0b02e3342597b90d4799f040`  
		Last Modified: Tue, 23 Aug 2022 01:02:02 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dad725ab9e6a3ba9502491f26af9b845cfc79c33b5f8473cea59ae1e80d6624`  
		Last Modified: Tue, 23 Aug 2022 01:02:05 GMT  
		Size: 44.6 MB (44612383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53645a91576006b5d14ec1cbff7cdd2b0b26af9ae2d78334b534621cb8880fbd`  
		Last Modified: Tue, 23 Aug 2022 01:02:00 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6d6954df5ef6586f14c99e7f6f81eaac9d35c01fe36f119036b5af779bb6b7`  
		Last Modified: Tue, 23 Aug 2022 01:02:00 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062905c89617104a732efd46df6237c6236e6a76639da396eb0610ebdba9af6d`  
		Last Modified: Tue, 23 Aug 2022 01:02:00 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3d0c25e7b5f1251abafa7fd376b419f9dc6e33718a7bd3e189ae4508924b7d`  
		Last Modified: Tue, 23 Aug 2022 01:02:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:f2a4273e1c132ca7d51a766e8924507ecb2fa433447ad227a94b9ebd735b1bb2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74622170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5a97102b89f803528279a50487b76e5cf67c9db39b6e50eaaa512ca9c876c9c`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 02 Aug 2022 00:41:03 GMT
ADD file:d973e057fdca9166fb9f39e73d7d5d4ca8ac2af6a55813580bf14a13cef4c159 in / 
# Tue, 02 Aug 2022 00:41:04 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:54:02 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 02 Aug 2022 01:54:03 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 02 Aug 2022 01:54:11 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:54:14 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 02 Aug 2022 01:54:15 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 02 Aug 2022 01:54:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:54:23 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 02 Aug 2022 01:54:24 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 02 Aug 2022 01:54:42 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 02 Aug 2022 01:54:43 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 02 Aug 2022 01:54:44 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 02 Aug 2022 01:54:45 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 02 Aug 2022 01:54:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 02 Aug 2022 01:54:46 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 02 Aug 2022 01:54:47 GMT
VOLUME [/opt/couchdb/data]
# Tue, 02 Aug 2022 01:54:48 GMT
EXPOSE 4369 5984 9100
# Tue, 02 Aug 2022 01:54:49 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6d588874b4737b02fc84169cf7d3d1d70f20c7f5dbd1ddfe27de4aff25e23314`  
		Last Modified: Tue, 02 Aug 2022 00:46:56 GMT  
		Size: 25.9 MB (25914363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffbb2e29bd8913eeb0828eb30855bd8099016bbccb4656f7a85247aff324e02`  
		Last Modified: Tue, 02 Aug 2022 01:56:25 GMT  
		Size: 3.3 KB (3321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:192633bb64010e741a13bef0a4f95d38e465792d3a07eac67e0d4b6f66c33390`  
		Last Modified: Tue, 02 Aug 2022 01:56:24 GMT  
		Size: 6.6 MB (6557119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9daf7a28b3a5155810d9966f34c4a4c0331f957d4458341c8e3683e074b5e376`  
		Last Modified: Tue, 02 Aug 2022 01:56:24 GMT  
		Size: 951.2 KB (951168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ee939b6b94519e887f775efeeb8e38f7c6753a794a56656ca795a354437b8e`  
		Last Modified: Tue, 02 Aug 2022 01:56:23 GMT  
		Size: 80.0 KB (79958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c1e56d17f55a93521148990b2f560a6401fc7bd06faec0f376e4a453cac903`  
		Last Modified: Tue, 02 Aug 2022 01:56:23 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f09ea26de4b63303321d6c9ea720b4e8116a8cdc261bc1dd0060fc58d7ebd3c`  
		Last Modified: Tue, 02 Aug 2022 01:56:26 GMT  
		Size: 41.1 MB (41112637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9354706eff555a86dfa9987feb6ca7ce1176d000dab12847b18f8349666d2d`  
		Last Modified: Tue, 02 Aug 2022 01:56:21 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a84a0c3df2496088046a0d00a1ef05a3c452627e37d79a60db80c6499c634cf`  
		Last Modified: Tue, 02 Aug 2022 01:56:21 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6541aa9f62e6abcfcca9b7d5155e5f035aef4d612c0aad572e69ee1ad006956a`  
		Last Modified: Tue, 02 Aug 2022 01:56:21 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7e0309716beca4eb00c072e238149bb9236708376e0b9b80ae104c047b960f`  
		Last Modified: Tue, 02 Aug 2022 01:56:21 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2`

```console
$ docker pull couchdb@sha256:fd7a739e37deab2c10119a81886ff8c626f9e1de6e786ed60b31ca9c30450035
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2` - linux; amd64

```console
$ docker pull couchdb@sha256:28124b34f4148ed792f9bf2c71207cc3ea9bb7e76546d67daffb19234952df81
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87503932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0396728d49f5ac43a68e07bf8b23d34cdbcec06f4aa08229ce8b509f9f465c64`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:59:42 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 23 Aug 2022 00:59:42 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 23 Aug 2022 00:59:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:59:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 23 Aug 2022 00:59:53 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 23 Aug 2022 00:59:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:59:59 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 23 Aug 2022 00:59:59 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 23 Aug 2022 01:00:13 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 23 Aug 2022 01:00:13 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 23 Aug 2022 01:00:13 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 23 Aug 2022 01:00:14 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 23 Aug 2022 01:00:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 23 Aug 2022 01:00:14 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 23 Aug 2022 01:00:14 GMT
VOLUME [/opt/couchdb/data]
# Tue, 23 Aug 2022 01:00:14 GMT
EXPOSE 4369 5984 9100
# Tue, 23 Aug 2022 01:00:15 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1836a36860638007d7b2592171befa5754532a9d47de8f0e775fad866c82393e`  
		Last Modified: Tue, 23 Aug 2022 01:01:43 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e2e2b5b7b5034043633af72843d3b8666f8ccc0c2aeae43af0afe8e9fdb2c8`  
		Last Modified: Tue, 23 Aug 2022 01:01:43 GMT  
		Size: 5.2 MB (5224227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c99ac86ee0acd5521ed2df4dce63d77342c2a96acff9b2af72b76e5893f62f`  
		Last Modified: Tue, 23 Aug 2022 01:01:42 GMT  
		Size: 1.6 MB (1553304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8979b473c30718ae0cbb8a38a2e402f873ad242554184f7beabb593d4451bfc0`  
		Last Modified: Tue, 23 Aug 2022 01:01:41 GMT  
		Size: 295.6 KB (295581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510ed5a8f7236ce7e23d8bb548f076632c0b48a3e1e8430e0e262ef6647f7ebc`  
		Last Modified: Tue, 23 Aug 2022 01:01:41 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e968620046651f8bd94db8256d249f0684ba2a454fb63d1c109ca1b45920ae`  
		Last Modified: Tue, 23 Aug 2022 01:01:45 GMT  
		Size: 49.0 MB (49042191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8920bb938feadb5c2b98dd12c72f655b1e47b736dd024cf1098c3f1acb2e645`  
		Last Modified: Tue, 23 Aug 2022 01:01:39 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a6954a2f0617948efb306d9b1a5b784d64a0beff38481b6828d069ca696e18`  
		Last Modified: Tue, 23 Aug 2022 01:01:39 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41292b445e0d087758fc8486322576d3605d68a540ca3fb3243dbc84ab1d4dda`  
		Last Modified: Tue, 23 Aug 2022 01:01:39 GMT  
		Size: 2.2 KB (2185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eaa46afbe00ace5c0c20bfc3c7912cde4600f9e8f942d5149e988d0473464fc`  
		Last Modified: Tue, 23 Aug 2022 01:01:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:2cc537fd46496d460ec408ea389dd4cc27c180608e89c59761c4682d6dac0cbd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.6 MB (85622605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faece9a6aa805f3e9d71e0136a8c7add2db196a28de98b26dc652d2eb88bf4ee`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:38 GMT
ADD file:6039adfbca55ed34a719c37672c664e3524130a0e2a3b8663629b8120b81b790 in / 
# Tue, 02 Aug 2022 00:40:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:53:11 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 02 Aug 2022 01:53:11 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 02 Aug 2022 01:53:19 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:53:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 02 Aug 2022 01:53:23 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 02 Aug 2022 01:53:29 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:53:29 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 02 Aug 2022 01:53:30 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 02 Aug 2022 01:53:44 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 02 Aug 2022 01:53:45 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 02 Aug 2022 01:53:46 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 02 Aug 2022 01:53:47 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 02 Aug 2022 01:53:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 02 Aug 2022 01:53:48 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 02 Aug 2022 01:53:49 GMT
VOLUME [/opt/couchdb/data]
# Tue, 02 Aug 2022 01:53:50 GMT
EXPOSE 4369 5984 9100
# Tue, 02 Aug 2022 01:53:51 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:a9fe95647e78b5516c7e2327355b6996e2ea295cd76ae242cbfe87f016b4e760`  
		Last Modified: Tue, 02 Aug 2022 00:46:05 GMT  
		Size: 30.1 MB (30054304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f36ebccf7ea0ca6c4e42a56d3e761f51620dde7809ff4cd6c9c47f4d92dda45`  
		Last Modified: Tue, 02 Aug 2022 01:56:00 GMT  
		Size: 3.3 KB (3320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57988538f1066bad59a075d99704fbc2ed80b7f279168e98ae1ac061cddb0e54`  
		Last Modified: Tue, 02 Aug 2022 01:55:59 GMT  
		Size: 5.2 MB (5207882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d6f84207bfc6da3f978a06e64089cd163b0b7cfce56aa03f050fffcf6aa1fa`  
		Last Modified: Tue, 02 Aug 2022 01:55:59 GMT  
		Size: 1.2 MB (1221114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f79004f600a1443f5dd0ab501f8d2726ae96d9790d635ef946c8ab58fc7639`  
		Last Modified: Tue, 02 Aug 2022 01:55:58 GMT  
		Size: 79.2 KB (79204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea246a4776bb764303aebd0c230598840bac0a3067bf67395be8aa1d4a9796c0`  
		Last Modified: Tue, 02 Aug 2022 01:55:58 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afec05def1afee67aa528ce2ecc14afe3dd947292160af59436483a6eb8307d8`  
		Last Modified: Tue, 02 Aug 2022 01:56:02 GMT  
		Size: 49.1 MB (49053054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f205452c1f21b508f3eff3ca454e831b24598073851b7c10ad77092021c63b80`  
		Last Modified: Tue, 02 Aug 2022 01:55:56 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb0d06feb8b8d747a8a616d3dbdb4dbff7f3d1c07726fc7fabbd0d857588a65`  
		Last Modified: Tue, 02 Aug 2022 01:55:56 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833640fe1553f0d57940524d810c11944b07d0171e7979f091beca62d8c235a2`  
		Last Modified: Tue, 02 Aug 2022 01:55:56 GMT  
		Size: 2.2 KB (2184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c60df208533e1fc53978ad88b63060ba603756eef0b46beaa35572ff7fc1aa2`  
		Last Modified: Tue, 02 Aug 2022 01:55:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; ppc64le

```console
$ docker pull couchdb@sha256:1e403730c20e44b3297dc2ca59567dc4f7f8608ea517c016cf6b814fa428f6f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93209223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9532ba1899566dfcf8498c068f3eca6b79c8afa3fae5d939c52255a7ae9d96b4`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 02 Aug 2022 01:17:30 GMT
ADD file:3a95a896d463569ce82199957052b3467123a4bd3385a0a4e397cf08402a99c3 in / 
# Tue, 02 Aug 2022 01:17:32 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:45:51 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 02 Aug 2022 01:45:52 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 02 Aug 2022 01:46:07 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:46:13 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 02 Aug 2022 01:46:14 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 02 Aug 2022 01:46:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:46:24 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 02 Aug 2022 01:46:25 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 02 Aug 2022 01:46:47 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 02 Aug 2022 01:46:48 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 02 Aug 2022 01:46:49 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 02 Aug 2022 01:46:49 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 02 Aug 2022 01:46:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 02 Aug 2022 01:46:50 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 02 Aug 2022 01:46:51 GMT
VOLUME [/opt/couchdb/data]
# Tue, 02 Aug 2022 01:46:51 GMT
EXPOSE 4369 5984 9100
# Tue, 02 Aug 2022 01:46:51 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:5241cd116d6e6e2d62f3d8c2245b74daca9f6cc154eaccd738feb41984c74714`  
		Last Modified: Tue, 02 Aug 2022 01:24:39 GMT  
		Size: 35.3 MB (35272771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd616d47d2a8f573397f07010fd143095697a31e5f728cac1c1b7269738c47a`  
		Last Modified: Tue, 02 Aug 2022 01:47:19 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1a77f89868067efb94d63fe88604742503d85f515b25f7ab84711a016d3e4f`  
		Last Modified: Tue, 02 Aug 2022 01:47:19 GMT  
		Size: 6.0 MB (6043687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f741e9865e3fdcb0bd227a5993c271ef87a11ea1804cdbbdd3814773c085fd4`  
		Last Modified: Tue, 02 Aug 2022 01:47:17 GMT  
		Size: 1.5 MB (1509129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a56ea83b77070cf87034a857804e0e5dc6e22a75e16d352364a0c6f2cf81cd`  
		Last Modified: Tue, 02 Aug 2022 01:47:17 GMT  
		Size: 295.5 KB (295465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe12fc56262eb1a9961df421373e9e93f9755a2e423207066c543f023b488f7`  
		Last Modified: Tue, 02 Aug 2022 01:47:17 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51cf6274a3105c304db4a54d429807a6d97294428538c809f791158d3a610942`  
		Last Modified: Tue, 02 Aug 2022 01:47:24 GMT  
		Size: 50.1 MB (50081019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48855ad409841498cce766b60da4e1cd5f59a6da57e69031b5cb1e70944c7e06`  
		Last Modified: Tue, 02 Aug 2022 01:47:14 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d93f33d896f43831a247689b5fe6b3c85972c92c57c27a55ae2ca50fd89216c`  
		Last Modified: Tue, 02 Aug 2022 01:47:15 GMT  
		Size: 768.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2efe54a8f4ae1598aa0cad697c24d96e9bd6701de850e533e452cb0ddc5df62`  
		Last Modified: Tue, 02 Aug 2022 01:47:15 GMT  
		Size: 2.2 KB (2188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fa6fb130ed09e3914ae920a1e5cd0affdd896fa22de827e2b222afb58a04e4`  
		Last Modified: Tue, 02 Aug 2022 01:47:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2.2`

```console
$ docker pull couchdb@sha256:fd7a739e37deab2c10119a81886ff8c626f9e1de6e786ed60b31ca9c30450035
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2.2` - linux; amd64

```console
$ docker pull couchdb@sha256:28124b34f4148ed792f9bf2c71207cc3ea9bb7e76546d67daffb19234952df81
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87503932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0396728d49f5ac43a68e07bf8b23d34cdbcec06f4aa08229ce8b509f9f465c64`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:59:42 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 23 Aug 2022 00:59:42 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 23 Aug 2022 00:59:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:59:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 23 Aug 2022 00:59:53 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 23 Aug 2022 00:59:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:59:59 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 23 Aug 2022 00:59:59 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 23 Aug 2022 01:00:13 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 23 Aug 2022 01:00:13 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 23 Aug 2022 01:00:13 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 23 Aug 2022 01:00:14 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 23 Aug 2022 01:00:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 23 Aug 2022 01:00:14 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 23 Aug 2022 01:00:14 GMT
VOLUME [/opt/couchdb/data]
# Tue, 23 Aug 2022 01:00:14 GMT
EXPOSE 4369 5984 9100
# Tue, 23 Aug 2022 01:00:15 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1836a36860638007d7b2592171befa5754532a9d47de8f0e775fad866c82393e`  
		Last Modified: Tue, 23 Aug 2022 01:01:43 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e2e2b5b7b5034043633af72843d3b8666f8ccc0c2aeae43af0afe8e9fdb2c8`  
		Last Modified: Tue, 23 Aug 2022 01:01:43 GMT  
		Size: 5.2 MB (5224227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c99ac86ee0acd5521ed2df4dce63d77342c2a96acff9b2af72b76e5893f62f`  
		Last Modified: Tue, 23 Aug 2022 01:01:42 GMT  
		Size: 1.6 MB (1553304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8979b473c30718ae0cbb8a38a2e402f873ad242554184f7beabb593d4451bfc0`  
		Last Modified: Tue, 23 Aug 2022 01:01:41 GMT  
		Size: 295.6 KB (295581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510ed5a8f7236ce7e23d8bb548f076632c0b48a3e1e8430e0e262ef6647f7ebc`  
		Last Modified: Tue, 23 Aug 2022 01:01:41 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e968620046651f8bd94db8256d249f0684ba2a454fb63d1c109ca1b45920ae`  
		Last Modified: Tue, 23 Aug 2022 01:01:45 GMT  
		Size: 49.0 MB (49042191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8920bb938feadb5c2b98dd12c72f655b1e47b736dd024cf1098c3f1acb2e645`  
		Last Modified: Tue, 23 Aug 2022 01:01:39 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a6954a2f0617948efb306d9b1a5b784d64a0beff38481b6828d069ca696e18`  
		Last Modified: Tue, 23 Aug 2022 01:01:39 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41292b445e0d087758fc8486322576d3605d68a540ca3fb3243dbc84ab1d4dda`  
		Last Modified: Tue, 23 Aug 2022 01:01:39 GMT  
		Size: 2.2 KB (2185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eaa46afbe00ace5c0c20bfc3c7912cde4600f9e8f942d5149e988d0473464fc`  
		Last Modified: Tue, 23 Aug 2022 01:01:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:2cc537fd46496d460ec408ea389dd4cc27c180608e89c59761c4682d6dac0cbd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.6 MB (85622605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faece9a6aa805f3e9d71e0136a8c7add2db196a28de98b26dc652d2eb88bf4ee`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:38 GMT
ADD file:6039adfbca55ed34a719c37672c664e3524130a0e2a3b8663629b8120b81b790 in / 
# Tue, 02 Aug 2022 00:40:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:53:11 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 02 Aug 2022 01:53:11 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 02 Aug 2022 01:53:19 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:53:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 02 Aug 2022 01:53:23 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 02 Aug 2022 01:53:29 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:53:29 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 02 Aug 2022 01:53:30 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 02 Aug 2022 01:53:44 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 02 Aug 2022 01:53:45 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 02 Aug 2022 01:53:46 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 02 Aug 2022 01:53:47 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 02 Aug 2022 01:53:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 02 Aug 2022 01:53:48 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 02 Aug 2022 01:53:49 GMT
VOLUME [/opt/couchdb/data]
# Tue, 02 Aug 2022 01:53:50 GMT
EXPOSE 4369 5984 9100
# Tue, 02 Aug 2022 01:53:51 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:a9fe95647e78b5516c7e2327355b6996e2ea295cd76ae242cbfe87f016b4e760`  
		Last Modified: Tue, 02 Aug 2022 00:46:05 GMT  
		Size: 30.1 MB (30054304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f36ebccf7ea0ca6c4e42a56d3e761f51620dde7809ff4cd6c9c47f4d92dda45`  
		Last Modified: Tue, 02 Aug 2022 01:56:00 GMT  
		Size: 3.3 KB (3320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57988538f1066bad59a075d99704fbc2ed80b7f279168e98ae1ac061cddb0e54`  
		Last Modified: Tue, 02 Aug 2022 01:55:59 GMT  
		Size: 5.2 MB (5207882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d6f84207bfc6da3f978a06e64089cd163b0b7cfce56aa03f050fffcf6aa1fa`  
		Last Modified: Tue, 02 Aug 2022 01:55:59 GMT  
		Size: 1.2 MB (1221114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f79004f600a1443f5dd0ab501f8d2726ae96d9790d635ef946c8ab58fc7639`  
		Last Modified: Tue, 02 Aug 2022 01:55:58 GMT  
		Size: 79.2 KB (79204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea246a4776bb764303aebd0c230598840bac0a3067bf67395be8aa1d4a9796c0`  
		Last Modified: Tue, 02 Aug 2022 01:55:58 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afec05def1afee67aa528ce2ecc14afe3dd947292160af59436483a6eb8307d8`  
		Last Modified: Tue, 02 Aug 2022 01:56:02 GMT  
		Size: 49.1 MB (49053054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f205452c1f21b508f3eff3ca454e831b24598073851b7c10ad77092021c63b80`  
		Last Modified: Tue, 02 Aug 2022 01:55:56 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb0d06feb8b8d747a8a616d3dbdb4dbff7f3d1c07726fc7fabbd0d857588a65`  
		Last Modified: Tue, 02 Aug 2022 01:55:56 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833640fe1553f0d57940524d810c11944b07d0171e7979f091beca62d8c235a2`  
		Last Modified: Tue, 02 Aug 2022 01:55:56 GMT  
		Size: 2.2 KB (2184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c60df208533e1fc53978ad88b63060ba603756eef0b46beaa35572ff7fc1aa2`  
		Last Modified: Tue, 02 Aug 2022 01:55:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2.2` - linux; ppc64le

```console
$ docker pull couchdb@sha256:1e403730c20e44b3297dc2ca59567dc4f7f8608ea517c016cf6b814fa428f6f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93209223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9532ba1899566dfcf8498c068f3eca6b79c8afa3fae5d939c52255a7ae9d96b4`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 02 Aug 2022 01:17:30 GMT
ADD file:3a95a896d463569ce82199957052b3467123a4bd3385a0a4e397cf08402a99c3 in / 
# Tue, 02 Aug 2022 01:17:32 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:45:51 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 02 Aug 2022 01:45:52 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 02 Aug 2022 01:46:07 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:46:13 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 02 Aug 2022 01:46:14 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 02 Aug 2022 01:46:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:46:24 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 02 Aug 2022 01:46:25 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 02 Aug 2022 01:46:47 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 02 Aug 2022 01:46:48 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 02 Aug 2022 01:46:49 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 02 Aug 2022 01:46:49 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 02 Aug 2022 01:46:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 02 Aug 2022 01:46:50 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 02 Aug 2022 01:46:51 GMT
VOLUME [/opt/couchdb/data]
# Tue, 02 Aug 2022 01:46:51 GMT
EXPOSE 4369 5984 9100
# Tue, 02 Aug 2022 01:46:51 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:5241cd116d6e6e2d62f3d8c2245b74daca9f6cc154eaccd738feb41984c74714`  
		Last Modified: Tue, 02 Aug 2022 01:24:39 GMT  
		Size: 35.3 MB (35272771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd616d47d2a8f573397f07010fd143095697a31e5f728cac1c1b7269738c47a`  
		Last Modified: Tue, 02 Aug 2022 01:47:19 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1a77f89868067efb94d63fe88604742503d85f515b25f7ab84711a016d3e4f`  
		Last Modified: Tue, 02 Aug 2022 01:47:19 GMT  
		Size: 6.0 MB (6043687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f741e9865e3fdcb0bd227a5993c271ef87a11ea1804cdbbdd3814773c085fd4`  
		Last Modified: Tue, 02 Aug 2022 01:47:17 GMT  
		Size: 1.5 MB (1509129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a56ea83b77070cf87034a857804e0e5dc6e22a75e16d352364a0c6f2cf81cd`  
		Last Modified: Tue, 02 Aug 2022 01:47:17 GMT  
		Size: 295.5 KB (295465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe12fc56262eb1a9961df421373e9e93f9755a2e423207066c543f023b488f7`  
		Last Modified: Tue, 02 Aug 2022 01:47:17 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51cf6274a3105c304db4a54d429807a6d97294428538c809f791158d3a610942`  
		Last Modified: Tue, 02 Aug 2022 01:47:24 GMT  
		Size: 50.1 MB (50081019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48855ad409841498cce766b60da4e1cd5f59a6da57e69031b5cb1e70944c7e06`  
		Last Modified: Tue, 02 Aug 2022 01:47:14 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d93f33d896f43831a247689b5fe6b3c85972c92c57c27a55ae2ca50fd89216c`  
		Last Modified: Tue, 02 Aug 2022 01:47:15 GMT  
		Size: 768.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2efe54a8f4ae1598aa0cad697c24d96e9bd6701de850e533e452cb0ddc5df62`  
		Last Modified: Tue, 02 Aug 2022 01:47:15 GMT  
		Size: 2.2 KB (2188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fa6fb130ed09e3914ae920a1e5cd0affdd896fa22de827e2b222afb58a04e4`  
		Last Modified: Tue, 02 Aug 2022 01:47:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:latest`

```console
$ docker pull couchdb@sha256:fd7a739e37deab2c10119a81886ff8c626f9e1de6e786ed60b31ca9c30450035
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:28124b34f4148ed792f9bf2c71207cc3ea9bb7e76546d67daffb19234952df81
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87503932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0396728d49f5ac43a68e07bf8b23d34cdbcec06f4aa08229ce8b509f9f465c64`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:59:42 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 23 Aug 2022 00:59:42 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 23 Aug 2022 00:59:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:59:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 23 Aug 2022 00:59:53 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 23 Aug 2022 00:59:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:59:59 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 23 Aug 2022 00:59:59 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 23 Aug 2022 01:00:13 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 23 Aug 2022 01:00:13 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 23 Aug 2022 01:00:13 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 23 Aug 2022 01:00:14 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 23 Aug 2022 01:00:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 23 Aug 2022 01:00:14 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 23 Aug 2022 01:00:14 GMT
VOLUME [/opt/couchdb/data]
# Tue, 23 Aug 2022 01:00:14 GMT
EXPOSE 4369 5984 9100
# Tue, 23 Aug 2022 01:00:15 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1836a36860638007d7b2592171befa5754532a9d47de8f0e775fad866c82393e`  
		Last Modified: Tue, 23 Aug 2022 01:01:43 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e2e2b5b7b5034043633af72843d3b8666f8ccc0c2aeae43af0afe8e9fdb2c8`  
		Last Modified: Tue, 23 Aug 2022 01:01:43 GMT  
		Size: 5.2 MB (5224227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c99ac86ee0acd5521ed2df4dce63d77342c2a96acff9b2af72b76e5893f62f`  
		Last Modified: Tue, 23 Aug 2022 01:01:42 GMT  
		Size: 1.6 MB (1553304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8979b473c30718ae0cbb8a38a2e402f873ad242554184f7beabb593d4451bfc0`  
		Last Modified: Tue, 23 Aug 2022 01:01:41 GMT  
		Size: 295.6 KB (295581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510ed5a8f7236ce7e23d8bb548f076632c0b48a3e1e8430e0e262ef6647f7ebc`  
		Last Modified: Tue, 23 Aug 2022 01:01:41 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e968620046651f8bd94db8256d249f0684ba2a454fb63d1c109ca1b45920ae`  
		Last Modified: Tue, 23 Aug 2022 01:01:45 GMT  
		Size: 49.0 MB (49042191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8920bb938feadb5c2b98dd12c72f655b1e47b736dd024cf1098c3f1acb2e645`  
		Last Modified: Tue, 23 Aug 2022 01:01:39 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a6954a2f0617948efb306d9b1a5b784d64a0beff38481b6828d069ca696e18`  
		Last Modified: Tue, 23 Aug 2022 01:01:39 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41292b445e0d087758fc8486322576d3605d68a540ca3fb3243dbc84ab1d4dda`  
		Last Modified: Tue, 23 Aug 2022 01:01:39 GMT  
		Size: 2.2 KB (2185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eaa46afbe00ace5c0c20bfc3c7912cde4600f9e8f942d5149e988d0473464fc`  
		Last Modified: Tue, 23 Aug 2022 01:01:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:2cc537fd46496d460ec408ea389dd4cc27c180608e89c59761c4682d6dac0cbd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.6 MB (85622605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faece9a6aa805f3e9d71e0136a8c7add2db196a28de98b26dc652d2eb88bf4ee`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:38 GMT
ADD file:6039adfbca55ed34a719c37672c664e3524130a0e2a3b8663629b8120b81b790 in / 
# Tue, 02 Aug 2022 00:40:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:53:11 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 02 Aug 2022 01:53:11 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 02 Aug 2022 01:53:19 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:53:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 02 Aug 2022 01:53:23 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 02 Aug 2022 01:53:29 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:53:29 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 02 Aug 2022 01:53:30 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 02 Aug 2022 01:53:44 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 02 Aug 2022 01:53:45 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 02 Aug 2022 01:53:46 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 02 Aug 2022 01:53:47 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 02 Aug 2022 01:53:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 02 Aug 2022 01:53:48 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 02 Aug 2022 01:53:49 GMT
VOLUME [/opt/couchdb/data]
# Tue, 02 Aug 2022 01:53:50 GMT
EXPOSE 4369 5984 9100
# Tue, 02 Aug 2022 01:53:51 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:a9fe95647e78b5516c7e2327355b6996e2ea295cd76ae242cbfe87f016b4e760`  
		Last Modified: Tue, 02 Aug 2022 00:46:05 GMT  
		Size: 30.1 MB (30054304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f36ebccf7ea0ca6c4e42a56d3e761f51620dde7809ff4cd6c9c47f4d92dda45`  
		Last Modified: Tue, 02 Aug 2022 01:56:00 GMT  
		Size: 3.3 KB (3320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57988538f1066bad59a075d99704fbc2ed80b7f279168e98ae1ac061cddb0e54`  
		Last Modified: Tue, 02 Aug 2022 01:55:59 GMT  
		Size: 5.2 MB (5207882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d6f84207bfc6da3f978a06e64089cd163b0b7cfce56aa03f050fffcf6aa1fa`  
		Last Modified: Tue, 02 Aug 2022 01:55:59 GMT  
		Size: 1.2 MB (1221114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f79004f600a1443f5dd0ab501f8d2726ae96d9790d635ef946c8ab58fc7639`  
		Last Modified: Tue, 02 Aug 2022 01:55:58 GMT  
		Size: 79.2 KB (79204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea246a4776bb764303aebd0c230598840bac0a3067bf67395be8aa1d4a9796c0`  
		Last Modified: Tue, 02 Aug 2022 01:55:58 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afec05def1afee67aa528ce2ecc14afe3dd947292160af59436483a6eb8307d8`  
		Last Modified: Tue, 02 Aug 2022 01:56:02 GMT  
		Size: 49.1 MB (49053054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f205452c1f21b508f3eff3ca454e831b24598073851b7c10ad77092021c63b80`  
		Last Modified: Tue, 02 Aug 2022 01:55:56 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb0d06feb8b8d747a8a616d3dbdb4dbff7f3d1c07726fc7fabbd0d857588a65`  
		Last Modified: Tue, 02 Aug 2022 01:55:56 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833640fe1553f0d57940524d810c11944b07d0171e7979f091beca62d8c235a2`  
		Last Modified: Tue, 02 Aug 2022 01:55:56 GMT  
		Size: 2.2 KB (2184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c60df208533e1fc53978ad88b63060ba603756eef0b46beaa35572ff7fc1aa2`  
		Last Modified: Tue, 02 Aug 2022 01:55:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; ppc64le

```console
$ docker pull couchdb@sha256:1e403730c20e44b3297dc2ca59567dc4f7f8608ea517c016cf6b814fa428f6f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93209223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9532ba1899566dfcf8498c068f3eca6b79c8afa3fae5d939c52255a7ae9d96b4`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 02 Aug 2022 01:17:30 GMT
ADD file:3a95a896d463569ce82199957052b3467123a4bd3385a0a4e397cf08402a99c3 in / 
# Tue, 02 Aug 2022 01:17:32 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:45:51 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 02 Aug 2022 01:45:52 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 02 Aug 2022 01:46:07 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:46:13 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 02 Aug 2022 01:46:14 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 02 Aug 2022 01:46:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:46:24 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 02 Aug 2022 01:46:25 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 02 Aug 2022 01:46:47 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 02 Aug 2022 01:46:48 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 02 Aug 2022 01:46:49 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 02 Aug 2022 01:46:49 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 02 Aug 2022 01:46:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 02 Aug 2022 01:46:50 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 02 Aug 2022 01:46:51 GMT
VOLUME [/opt/couchdb/data]
# Tue, 02 Aug 2022 01:46:51 GMT
EXPOSE 4369 5984 9100
# Tue, 02 Aug 2022 01:46:51 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:5241cd116d6e6e2d62f3d8c2245b74daca9f6cc154eaccd738feb41984c74714`  
		Last Modified: Tue, 02 Aug 2022 01:24:39 GMT  
		Size: 35.3 MB (35272771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd616d47d2a8f573397f07010fd143095697a31e5f728cac1c1b7269738c47a`  
		Last Modified: Tue, 02 Aug 2022 01:47:19 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1a77f89868067efb94d63fe88604742503d85f515b25f7ab84711a016d3e4f`  
		Last Modified: Tue, 02 Aug 2022 01:47:19 GMT  
		Size: 6.0 MB (6043687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f741e9865e3fdcb0bd227a5993c271ef87a11ea1804cdbbdd3814773c085fd4`  
		Last Modified: Tue, 02 Aug 2022 01:47:17 GMT  
		Size: 1.5 MB (1509129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a56ea83b77070cf87034a857804e0e5dc6e22a75e16d352364a0c6f2cf81cd`  
		Last Modified: Tue, 02 Aug 2022 01:47:17 GMT  
		Size: 295.5 KB (295465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe12fc56262eb1a9961df421373e9e93f9755a2e423207066c543f023b488f7`  
		Last Modified: Tue, 02 Aug 2022 01:47:17 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51cf6274a3105c304db4a54d429807a6d97294428538c809f791158d3a610942`  
		Last Modified: Tue, 02 Aug 2022 01:47:24 GMT  
		Size: 50.1 MB (50081019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48855ad409841498cce766b60da4e1cd5f59a6da57e69031b5cb1e70944c7e06`  
		Last Modified: Tue, 02 Aug 2022 01:47:14 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d93f33d896f43831a247689b5fe6b3c85972c92c57c27a55ae2ca50fd89216c`  
		Last Modified: Tue, 02 Aug 2022 01:47:15 GMT  
		Size: 768.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2efe54a8f4ae1598aa0cad697c24d96e9bd6701de850e533e452cb0ddc5df62`  
		Last Modified: Tue, 02 Aug 2022 01:47:15 GMT  
		Size: 2.2 KB (2188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fa6fb130ed09e3914ae920a1e5cd0affdd896fa22de827e2b222afb58a04e4`  
		Last Modified: Tue, 02 Aug 2022 01:47:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
