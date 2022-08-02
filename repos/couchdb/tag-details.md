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
$ docker pull couchdb@sha256:fad4eb816cb14e2684b6ec0366b3bb8384e20561261df6c9d45d107d87f98ed2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2` - linux; amd64

```console
$ docker pull couchdb@sha256:3bb0696de18181a314d62f839ea7c5c171096ecbc1a1e27b80f2b05b76f15b04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84525272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f506dab4438ee77e886d87a02592506c31a5461cf43a757ddbd1b1e6589ef42d`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:32 GMT
ADD file:7f2320197e75c5169402827ce0c47d93629331875d76b9f0ddd389244747eccd in / 
# Tue, 12 Jul 2022 01:20:33 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 15:11:29 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 12 Jul 2022 15:11:29 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 12 Jul 2022 15:11:37 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 15:11:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 12 Jul 2022 15:11:42 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 12 Jul 2022 15:11:48 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 15:12:09 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 12 Jul 2022 15:12:09 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 12 Jul 2022 15:12:27 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 12 Jul 2022 15:12:28 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 12 Jul 2022 15:12:28 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 12 Jul 2022 15:12:28 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 12 Jul 2022 15:12:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 12 Jul 2022 15:12:29 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 12 Jul 2022 15:12:29 GMT
VOLUME [/opt/couchdb/data]
# Tue, 12 Jul 2022 15:12:29 GMT
EXPOSE 4369 5984 9100
# Tue, 12 Jul 2022 15:12:29 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ac2fb615420c18b61e0693f2569a3d38e3b9b58456b691bac44405e08389a591`  
		Last Modified: Tue, 12 Jul 2022 01:25:22 GMT  
		Size: 27.1 MB (27139850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8becf7841f9b4fb0b27c166b71ef7d2741114614403eeb9c12d76d5647cae7e7`  
		Last Modified: Tue, 12 Jul 2022 15:13:12 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c78710523089d618d3574d13c79d021dc0478f564fce416cb5db663a496ec05c`  
		Last Modified: Tue, 12 Jul 2022 15:13:11 GMT  
		Size: 6.7 MB (6698711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa21e100b4bbd01bbab03cb7e787a9dd2b1e65d0f92df57c9d8c0685d405cff`  
		Last Modified: Tue, 12 Jul 2022 15:13:10 GMT  
		Size: 1.3 MB (1258350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b4ccdfd36dda5d56b807c6291ff4347b139e9497b95553516b96b8e5ddb967`  
		Last Modified: Tue, 12 Jul 2022 15:13:10 GMT  
		Size: 293.0 KB (293047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7b69d9f2860f30ec08d7a3983923da54649458d4a93caf0df85b894cc8ab5f`  
		Last Modified: Tue, 12 Jul 2022 15:13:27 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0257ebbc0499963bf32d6c4fbb9b15f8fad5728e313613dbdd93fb90f37799`  
		Last Modified: Tue, 12 Jul 2022 15:13:30 GMT  
		Size: 49.1 MB (49128299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af73f2471978da1b4d0a3ece709f1028f3f41a64640ce647a82674df0e1f0b1`  
		Last Modified: Tue, 12 Jul 2022 15:13:24 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d71d7c5f725ee7905e9ad4ad5020cb5e309a11b843c15947660bd75520332fc`  
		Last Modified: Tue, 12 Jul 2022 15:13:24 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd719fa4db791965d1780d47553236439de3130240ec11d50967f6820a89c0ff`  
		Last Modified: Tue, 12 Jul 2022 15:13:24 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77e146f980443700da1a7250f5527e5bfe2f76936c4f6df41f1fa3ce025b718`  
		Last Modified: Tue, 12 Jul 2022 15:13:24 GMT  
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
$ docker pull couchdb@sha256:fad4eb816cb14e2684b6ec0366b3bb8384e20561261df6c9d45d107d87f98ed2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:3bb0696de18181a314d62f839ea7c5c171096ecbc1a1e27b80f2b05b76f15b04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84525272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f506dab4438ee77e886d87a02592506c31a5461cf43a757ddbd1b1e6589ef42d`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:32 GMT
ADD file:7f2320197e75c5169402827ce0c47d93629331875d76b9f0ddd389244747eccd in / 
# Tue, 12 Jul 2022 01:20:33 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 15:11:29 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 12 Jul 2022 15:11:29 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 12 Jul 2022 15:11:37 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 15:11:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 12 Jul 2022 15:11:42 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 12 Jul 2022 15:11:48 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 15:12:09 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 12 Jul 2022 15:12:09 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 12 Jul 2022 15:12:27 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 12 Jul 2022 15:12:28 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 12 Jul 2022 15:12:28 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 12 Jul 2022 15:12:28 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 12 Jul 2022 15:12:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 12 Jul 2022 15:12:29 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 12 Jul 2022 15:12:29 GMT
VOLUME [/opt/couchdb/data]
# Tue, 12 Jul 2022 15:12:29 GMT
EXPOSE 4369 5984 9100
# Tue, 12 Jul 2022 15:12:29 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ac2fb615420c18b61e0693f2569a3d38e3b9b58456b691bac44405e08389a591`  
		Last Modified: Tue, 12 Jul 2022 01:25:22 GMT  
		Size: 27.1 MB (27139850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8becf7841f9b4fb0b27c166b71ef7d2741114614403eeb9c12d76d5647cae7e7`  
		Last Modified: Tue, 12 Jul 2022 15:13:12 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c78710523089d618d3574d13c79d021dc0478f564fce416cb5db663a496ec05c`  
		Last Modified: Tue, 12 Jul 2022 15:13:11 GMT  
		Size: 6.7 MB (6698711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa21e100b4bbd01bbab03cb7e787a9dd2b1e65d0f92df57c9d8c0685d405cff`  
		Last Modified: Tue, 12 Jul 2022 15:13:10 GMT  
		Size: 1.3 MB (1258350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b4ccdfd36dda5d56b807c6291ff4347b139e9497b95553516b96b8e5ddb967`  
		Last Modified: Tue, 12 Jul 2022 15:13:10 GMT  
		Size: 293.0 KB (293047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7b69d9f2860f30ec08d7a3983923da54649458d4a93caf0df85b894cc8ab5f`  
		Last Modified: Tue, 12 Jul 2022 15:13:27 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0257ebbc0499963bf32d6c4fbb9b15f8fad5728e313613dbdd93fb90f37799`  
		Last Modified: Tue, 12 Jul 2022 15:13:30 GMT  
		Size: 49.1 MB (49128299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af73f2471978da1b4d0a3ece709f1028f3f41a64640ce647a82674df0e1f0b1`  
		Last Modified: Tue, 12 Jul 2022 15:13:24 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d71d7c5f725ee7905e9ad4ad5020cb5e309a11b843c15947660bd75520332fc`  
		Last Modified: Tue, 12 Jul 2022 15:13:24 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd719fa4db791965d1780d47553236439de3130240ec11d50967f6820a89c0ff`  
		Last Modified: Tue, 12 Jul 2022 15:13:24 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77e146f980443700da1a7250f5527e5bfe2f76936c4f6df41f1fa3ce025b718`  
		Last Modified: Tue, 12 Jul 2022 15:13:24 GMT  
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
$ docker pull couchdb@sha256:fad4eb816cb14e2684b6ec0366b3bb8384e20561261df6c9d45d107d87f98ed2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:3bb0696de18181a314d62f839ea7c5c171096ecbc1a1e27b80f2b05b76f15b04
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84525272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f506dab4438ee77e886d87a02592506c31a5461cf43a757ddbd1b1e6589ef42d`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:32 GMT
ADD file:7f2320197e75c5169402827ce0c47d93629331875d76b9f0ddd389244747eccd in / 
# Tue, 12 Jul 2022 01:20:33 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 15:11:29 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 12 Jul 2022 15:11:29 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 12 Jul 2022 15:11:37 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 15:11:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 12 Jul 2022 15:11:42 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 12 Jul 2022 15:11:48 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 15:12:09 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 12 Jul 2022 15:12:09 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 12 Jul 2022 15:12:27 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 12 Jul 2022 15:12:28 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 12 Jul 2022 15:12:28 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 12 Jul 2022 15:12:28 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 12 Jul 2022 15:12:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 12 Jul 2022 15:12:29 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 12 Jul 2022 15:12:29 GMT
VOLUME [/opt/couchdb/data]
# Tue, 12 Jul 2022 15:12:29 GMT
EXPOSE 4369 5984 9100
# Tue, 12 Jul 2022 15:12:29 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ac2fb615420c18b61e0693f2569a3d38e3b9b58456b691bac44405e08389a591`  
		Last Modified: Tue, 12 Jul 2022 01:25:22 GMT  
		Size: 27.1 MB (27139850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8becf7841f9b4fb0b27c166b71ef7d2741114614403eeb9c12d76d5647cae7e7`  
		Last Modified: Tue, 12 Jul 2022 15:13:12 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c78710523089d618d3574d13c79d021dc0478f564fce416cb5db663a496ec05c`  
		Last Modified: Tue, 12 Jul 2022 15:13:11 GMT  
		Size: 6.7 MB (6698711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa21e100b4bbd01bbab03cb7e787a9dd2b1e65d0f92df57c9d8c0685d405cff`  
		Last Modified: Tue, 12 Jul 2022 15:13:10 GMT  
		Size: 1.3 MB (1258350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b4ccdfd36dda5d56b807c6291ff4347b139e9497b95553516b96b8e5ddb967`  
		Last Modified: Tue, 12 Jul 2022 15:13:10 GMT  
		Size: 293.0 KB (293047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7b69d9f2860f30ec08d7a3983923da54649458d4a93caf0df85b894cc8ab5f`  
		Last Modified: Tue, 12 Jul 2022 15:13:27 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0257ebbc0499963bf32d6c4fbb9b15f8fad5728e313613dbdd93fb90f37799`  
		Last Modified: Tue, 12 Jul 2022 15:13:30 GMT  
		Size: 49.1 MB (49128299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3af73f2471978da1b4d0a3ece709f1028f3f41a64640ce647a82674df0e1f0b1`  
		Last Modified: Tue, 12 Jul 2022 15:13:24 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d71d7c5f725ee7905e9ad4ad5020cb5e309a11b843c15947660bd75520332fc`  
		Last Modified: Tue, 12 Jul 2022 15:13:24 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd719fa4db791965d1780d47553236439de3130240ec11d50967f6820a89c0ff`  
		Last Modified: Tue, 12 Jul 2022 15:13:24 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77e146f980443700da1a7250f5527e5bfe2f76936c4f6df41f1fa3ce025b718`  
		Last Modified: Tue, 12 Jul 2022 15:13:24 GMT  
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
$ docker pull couchdb@sha256:900ab11dd00c495fadd6aab160bbe0e2ad6a0029fe6a446beade8f6d1c503bbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3` - linux; amd64

```console
$ docker pull couchdb@sha256:12c59b7f8b202476487c670ba7a042b3a654cd91302335df1bfdff0197f92968
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87486230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:123f61a8e1f1ba63410c4e25acc53842ac2dbc34783eca4c59c101ec8541d6c0`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 15:10:48 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 12 Jul 2022 15:10:49 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 12 Jul 2022 15:10:56 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 15:11:00 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 12 Jul 2022 15:11:00 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 12 Jul 2022 15:11:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 15:11:06 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 12 Jul 2022 15:11:06 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 12 Jul 2022 15:11:20 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 12 Jul 2022 15:11:20 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 12 Jul 2022 15:11:20 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 12 Jul 2022 15:11:20 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 12 Jul 2022 15:11:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 12 Jul 2022 15:11:21 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 12 Jul 2022 15:11:21 GMT
VOLUME [/opt/couchdb/data]
# Tue, 12 Jul 2022 15:11:21 GMT
EXPOSE 4369 5984 9100
# Tue, 12 Jul 2022 15:11:21 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d6a8817335d9ffafa3f1017d6269bc446e119f240d553955ac4475c653286d3`  
		Last Modified: Tue, 12 Jul 2022 15:12:50 GMT  
		Size: 3.4 KB (3407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4c965b93ac974aa2c3fca509df0f936eeb579e157f28d6f4ab4d7085d05bdb`  
		Last Modified: Tue, 12 Jul 2022 15:12:49 GMT  
		Size: 5.2 MB (5224212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f213905bb36e848a27f9500bb1c48db584215e7263b497eddf4e93ae8de65458`  
		Last Modified: Tue, 12 Jul 2022 15:12:48 GMT  
		Size: 1.6 MB (1553262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed71cb8fd2ac6869ae41ba5895eba4bbeb89a3fba0949a707f9fe5cbe8f37fb`  
		Last Modified: Tue, 12 Jul 2022 15:12:48 GMT  
		Size: 295.6 KB (295583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5daea30650232dc1b123cb8425895747c91e406b3069bd16b7051b2df7f20b`  
		Last Modified: Tue, 12 Jul 2022 15:12:48 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1700f3de25a27003b3a6963022efbde7da7b557bd9d624a8251536cd1ce4d290`  
		Last Modified: Tue, 12 Jul 2022 15:12:51 GMT  
		Size: 49.0 MB (49039434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42db9a2185d560547609a16f7877805b1e086668898691f419e880f829108d5e`  
		Last Modified: Tue, 12 Jul 2022 15:12:46 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a24ba52538ad79ca5b97acbdd9a15944e280e3d97ccb10d606bd88d95b2cb1`  
		Last Modified: Tue, 12 Jul 2022 15:12:46 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c8ceb181745bf7b63863ac93e4a934578b9e9daa6ca47b74461bfd142b5cb4`  
		Last Modified: Tue, 12 Jul 2022 15:12:46 GMT  
		Size: 2.2 KB (2180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0694a648fdfcd1507041befc7582c472d2f25d8eb2c4d29c906d59dc2dd3089`  
		Last Modified: Tue, 12 Jul 2022 15:12:46 GMT  
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
$ docker pull couchdb@sha256:5343ac5a52c8a7f12318d9cdf2a04e347872dce8c1fdc87985a789f300bc4bf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:07ece78330fb63801e90d0864de1cb3f374b48c17ac0ef785e59120c9a30dbe3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80009987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39fcedb3bb5c4af7cbd84b0bb420f328945cbe2408efe349117ce86feb7a63ec`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:32 GMT
ADD file:7f2320197e75c5169402827ce0c47d93629331875d76b9f0ddd389244747eccd in / 
# Tue, 12 Jul 2022 01:20:33 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 15:11:29 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 12 Jul 2022 15:11:29 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 12 Jul 2022 15:11:37 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 15:11:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 12 Jul 2022 15:11:42 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 12 Jul 2022 15:11:48 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 15:11:48 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 12 Jul 2022 15:11:49 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 12 Jul 2022 15:12:02 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 12 Jul 2022 15:12:03 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 12 Jul 2022 15:12:03 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 12 Jul 2022 15:12:03 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 12 Jul 2022 15:12:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 12 Jul 2022 15:12:04 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 12 Jul 2022 15:12:04 GMT
VOLUME [/opt/couchdb/data]
# Tue, 12 Jul 2022 15:12:04 GMT
EXPOSE 4369 5984 9100
# Tue, 12 Jul 2022 15:12:04 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ac2fb615420c18b61e0693f2569a3d38e3b9b58456b691bac44405e08389a591`  
		Last Modified: Tue, 12 Jul 2022 01:25:22 GMT  
		Size: 27.1 MB (27139850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8becf7841f9b4fb0b27c166b71ef7d2741114614403eeb9c12d76d5647cae7e7`  
		Last Modified: Tue, 12 Jul 2022 15:13:12 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c78710523089d618d3574d13c79d021dc0478f564fce416cb5db663a496ec05c`  
		Last Modified: Tue, 12 Jul 2022 15:13:11 GMT  
		Size: 6.7 MB (6698711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa21e100b4bbd01bbab03cb7e787a9dd2b1e65d0f92df57c9d8c0685d405cff`  
		Last Modified: Tue, 12 Jul 2022 15:13:10 GMT  
		Size: 1.3 MB (1258350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b4ccdfd36dda5d56b807c6291ff4347b139e9497b95553516b96b8e5ddb967`  
		Last Modified: Tue, 12 Jul 2022 15:13:10 GMT  
		Size: 293.0 KB (293047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de05cfdfd2b5b68e7633c383d0560ea54a9c30a59fc44a357320ce849f896985`  
		Last Modified: Tue, 12 Jul 2022 15:13:10 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8def3570b3dafe69c9f9d91dddf86d956e0570f350563ac6f96a825b356478a5`  
		Last Modified: Tue, 12 Jul 2022 15:13:14 GMT  
		Size: 44.6 MB (44613014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f803aed236a0aa3a93ae8bf2ec2c0ee378781b177bb9ef9632681bee7dc31da`  
		Last Modified: Tue, 12 Jul 2022 15:13:07 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04984698254197e3853fe017953fd7c6cefdf31a08d625be3708ab809d329f8`  
		Last Modified: Tue, 12 Jul 2022 15:13:07 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfab52dd5b8042a629f832668c41058af4cef632d9473b7db09253bcf1b9bea`  
		Last Modified: Tue, 12 Jul 2022 15:13:07 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69d3a6dac27b8125d4aca3d553198eb72425ec9cff8c780898d5b80db6a3305`  
		Last Modified: Tue, 12 Jul 2022 15:13:07 GMT  
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
$ docker pull couchdb@sha256:5343ac5a52c8a7f12318d9cdf2a04e347872dce8c1fdc87985a789f300bc4bf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1.2` - linux; amd64

```console
$ docker pull couchdb@sha256:07ece78330fb63801e90d0864de1cb3f374b48c17ac0ef785e59120c9a30dbe3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80009987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39fcedb3bb5c4af7cbd84b0bb420f328945cbe2408efe349117ce86feb7a63ec`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:32 GMT
ADD file:7f2320197e75c5169402827ce0c47d93629331875d76b9f0ddd389244747eccd in / 
# Tue, 12 Jul 2022 01:20:33 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 15:11:29 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 12 Jul 2022 15:11:29 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 12 Jul 2022 15:11:37 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 15:11:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 12 Jul 2022 15:11:42 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 12 Jul 2022 15:11:48 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 15:11:48 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 12 Jul 2022 15:11:49 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 12 Jul 2022 15:12:02 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 12 Jul 2022 15:12:03 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 12 Jul 2022 15:12:03 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 12 Jul 2022 15:12:03 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 12 Jul 2022 15:12:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 12 Jul 2022 15:12:04 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 12 Jul 2022 15:12:04 GMT
VOLUME [/opt/couchdb/data]
# Tue, 12 Jul 2022 15:12:04 GMT
EXPOSE 4369 5984 9100
# Tue, 12 Jul 2022 15:12:04 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ac2fb615420c18b61e0693f2569a3d38e3b9b58456b691bac44405e08389a591`  
		Last Modified: Tue, 12 Jul 2022 01:25:22 GMT  
		Size: 27.1 MB (27139850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8becf7841f9b4fb0b27c166b71ef7d2741114614403eeb9c12d76d5647cae7e7`  
		Last Modified: Tue, 12 Jul 2022 15:13:12 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c78710523089d618d3574d13c79d021dc0478f564fce416cb5db663a496ec05c`  
		Last Modified: Tue, 12 Jul 2022 15:13:11 GMT  
		Size: 6.7 MB (6698711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa21e100b4bbd01bbab03cb7e787a9dd2b1e65d0f92df57c9d8c0685d405cff`  
		Last Modified: Tue, 12 Jul 2022 15:13:10 GMT  
		Size: 1.3 MB (1258350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b4ccdfd36dda5d56b807c6291ff4347b139e9497b95553516b96b8e5ddb967`  
		Last Modified: Tue, 12 Jul 2022 15:13:10 GMT  
		Size: 293.0 KB (293047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de05cfdfd2b5b68e7633c383d0560ea54a9c30a59fc44a357320ce849f896985`  
		Last Modified: Tue, 12 Jul 2022 15:13:10 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8def3570b3dafe69c9f9d91dddf86d956e0570f350563ac6f96a825b356478a5`  
		Last Modified: Tue, 12 Jul 2022 15:13:14 GMT  
		Size: 44.6 MB (44613014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f803aed236a0aa3a93ae8bf2ec2c0ee378781b177bb9ef9632681bee7dc31da`  
		Last Modified: Tue, 12 Jul 2022 15:13:07 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04984698254197e3853fe017953fd7c6cefdf31a08d625be3708ab809d329f8`  
		Last Modified: Tue, 12 Jul 2022 15:13:07 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfab52dd5b8042a629f832668c41058af4cef632d9473b7db09253bcf1b9bea`  
		Last Modified: Tue, 12 Jul 2022 15:13:07 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69d3a6dac27b8125d4aca3d553198eb72425ec9cff8c780898d5b80db6a3305`  
		Last Modified: Tue, 12 Jul 2022 15:13:07 GMT  
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
$ docker pull couchdb@sha256:900ab11dd00c495fadd6aab160bbe0e2ad6a0029fe6a446beade8f6d1c503bbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2` - linux; amd64

```console
$ docker pull couchdb@sha256:12c59b7f8b202476487c670ba7a042b3a654cd91302335df1bfdff0197f92968
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87486230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:123f61a8e1f1ba63410c4e25acc53842ac2dbc34783eca4c59c101ec8541d6c0`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 15:10:48 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 12 Jul 2022 15:10:49 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 12 Jul 2022 15:10:56 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 15:11:00 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 12 Jul 2022 15:11:00 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 12 Jul 2022 15:11:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 15:11:06 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 12 Jul 2022 15:11:06 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 12 Jul 2022 15:11:20 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 12 Jul 2022 15:11:20 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 12 Jul 2022 15:11:20 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 12 Jul 2022 15:11:20 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 12 Jul 2022 15:11:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 12 Jul 2022 15:11:21 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 12 Jul 2022 15:11:21 GMT
VOLUME [/opt/couchdb/data]
# Tue, 12 Jul 2022 15:11:21 GMT
EXPOSE 4369 5984 9100
# Tue, 12 Jul 2022 15:11:21 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d6a8817335d9ffafa3f1017d6269bc446e119f240d553955ac4475c653286d3`  
		Last Modified: Tue, 12 Jul 2022 15:12:50 GMT  
		Size: 3.4 KB (3407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4c965b93ac974aa2c3fca509df0f936eeb579e157f28d6f4ab4d7085d05bdb`  
		Last Modified: Tue, 12 Jul 2022 15:12:49 GMT  
		Size: 5.2 MB (5224212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f213905bb36e848a27f9500bb1c48db584215e7263b497eddf4e93ae8de65458`  
		Last Modified: Tue, 12 Jul 2022 15:12:48 GMT  
		Size: 1.6 MB (1553262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed71cb8fd2ac6869ae41ba5895eba4bbeb89a3fba0949a707f9fe5cbe8f37fb`  
		Last Modified: Tue, 12 Jul 2022 15:12:48 GMT  
		Size: 295.6 KB (295583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5daea30650232dc1b123cb8425895747c91e406b3069bd16b7051b2df7f20b`  
		Last Modified: Tue, 12 Jul 2022 15:12:48 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1700f3de25a27003b3a6963022efbde7da7b557bd9d624a8251536cd1ce4d290`  
		Last Modified: Tue, 12 Jul 2022 15:12:51 GMT  
		Size: 49.0 MB (49039434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42db9a2185d560547609a16f7877805b1e086668898691f419e880f829108d5e`  
		Last Modified: Tue, 12 Jul 2022 15:12:46 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a24ba52538ad79ca5b97acbdd9a15944e280e3d97ccb10d606bd88d95b2cb1`  
		Last Modified: Tue, 12 Jul 2022 15:12:46 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c8ceb181745bf7b63863ac93e4a934578b9e9daa6ca47b74461bfd142b5cb4`  
		Last Modified: Tue, 12 Jul 2022 15:12:46 GMT  
		Size: 2.2 KB (2180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0694a648fdfcd1507041befc7582c472d2f25d8eb2c4d29c906d59dc2dd3089`  
		Last Modified: Tue, 12 Jul 2022 15:12:46 GMT  
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
$ docker pull couchdb@sha256:900ab11dd00c495fadd6aab160bbe0e2ad6a0029fe6a446beade8f6d1c503bbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2.2` - linux; amd64

```console
$ docker pull couchdb@sha256:12c59b7f8b202476487c670ba7a042b3a654cd91302335df1bfdff0197f92968
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87486230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:123f61a8e1f1ba63410c4e25acc53842ac2dbc34783eca4c59c101ec8541d6c0`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 15:10:48 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 12 Jul 2022 15:10:49 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 12 Jul 2022 15:10:56 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 15:11:00 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 12 Jul 2022 15:11:00 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 12 Jul 2022 15:11:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 15:11:06 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 12 Jul 2022 15:11:06 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 12 Jul 2022 15:11:20 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 12 Jul 2022 15:11:20 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 12 Jul 2022 15:11:20 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 12 Jul 2022 15:11:20 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 12 Jul 2022 15:11:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 12 Jul 2022 15:11:21 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 12 Jul 2022 15:11:21 GMT
VOLUME [/opt/couchdb/data]
# Tue, 12 Jul 2022 15:11:21 GMT
EXPOSE 4369 5984 9100
# Tue, 12 Jul 2022 15:11:21 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d6a8817335d9ffafa3f1017d6269bc446e119f240d553955ac4475c653286d3`  
		Last Modified: Tue, 12 Jul 2022 15:12:50 GMT  
		Size: 3.4 KB (3407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4c965b93ac974aa2c3fca509df0f936eeb579e157f28d6f4ab4d7085d05bdb`  
		Last Modified: Tue, 12 Jul 2022 15:12:49 GMT  
		Size: 5.2 MB (5224212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f213905bb36e848a27f9500bb1c48db584215e7263b497eddf4e93ae8de65458`  
		Last Modified: Tue, 12 Jul 2022 15:12:48 GMT  
		Size: 1.6 MB (1553262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed71cb8fd2ac6869ae41ba5895eba4bbeb89a3fba0949a707f9fe5cbe8f37fb`  
		Last Modified: Tue, 12 Jul 2022 15:12:48 GMT  
		Size: 295.6 KB (295583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5daea30650232dc1b123cb8425895747c91e406b3069bd16b7051b2df7f20b`  
		Last Modified: Tue, 12 Jul 2022 15:12:48 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1700f3de25a27003b3a6963022efbde7da7b557bd9d624a8251536cd1ce4d290`  
		Last Modified: Tue, 12 Jul 2022 15:12:51 GMT  
		Size: 49.0 MB (49039434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42db9a2185d560547609a16f7877805b1e086668898691f419e880f829108d5e`  
		Last Modified: Tue, 12 Jul 2022 15:12:46 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a24ba52538ad79ca5b97acbdd9a15944e280e3d97ccb10d606bd88d95b2cb1`  
		Last Modified: Tue, 12 Jul 2022 15:12:46 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c8ceb181745bf7b63863ac93e4a934578b9e9daa6ca47b74461bfd142b5cb4`  
		Last Modified: Tue, 12 Jul 2022 15:12:46 GMT  
		Size: 2.2 KB (2180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0694a648fdfcd1507041befc7582c472d2f25d8eb2c4d29c906d59dc2dd3089`  
		Last Modified: Tue, 12 Jul 2022 15:12:46 GMT  
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
$ docker pull couchdb@sha256:900ab11dd00c495fadd6aab160bbe0e2ad6a0029fe6a446beade8f6d1c503bbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:12c59b7f8b202476487c670ba7a042b3a654cd91302335df1bfdff0197f92968
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87486230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:123f61a8e1f1ba63410c4e25acc53842ac2dbc34783eca4c59c101ec8541d6c0`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 12 Jul 2022 01:20:10 GMT
ADD file:d978f6d3025a06f5142a0c13c98bf12fbd47cdf9162ed31fbc05c86983b0a679 in / 
# Tue, 12 Jul 2022 01:20:10 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 15:10:48 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 12 Jul 2022 15:10:49 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 12 Jul 2022 15:10:56 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 15:11:00 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 12 Jul 2022 15:11:00 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 12 Jul 2022 15:11:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 15:11:06 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 12 Jul 2022 15:11:06 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 12 Jul 2022 15:11:20 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 12 Jul 2022 15:11:20 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 12 Jul 2022 15:11:20 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 12 Jul 2022 15:11:20 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 12 Jul 2022 15:11:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 12 Jul 2022 15:11:21 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 12 Jul 2022 15:11:21 GMT
VOLUME [/opt/couchdb/data]
# Tue, 12 Jul 2022 15:11:21 GMT
EXPOSE 4369 5984 9100
# Tue, 12 Jul 2022 15:11:21 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:461246efe0a75316d99afdbf348f7063b57b0caeee8daab775f1f08152ea36f4`  
		Last Modified: Tue, 12 Jul 2022 01:24:34 GMT  
		Size: 31.4 MB (31366610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d6a8817335d9ffafa3f1017d6269bc446e119f240d553955ac4475c653286d3`  
		Last Modified: Tue, 12 Jul 2022 15:12:50 GMT  
		Size: 3.4 KB (3407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4c965b93ac974aa2c3fca509df0f936eeb579e157f28d6f4ab4d7085d05bdb`  
		Last Modified: Tue, 12 Jul 2022 15:12:49 GMT  
		Size: 5.2 MB (5224212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f213905bb36e848a27f9500bb1c48db584215e7263b497eddf4e93ae8de65458`  
		Last Modified: Tue, 12 Jul 2022 15:12:48 GMT  
		Size: 1.6 MB (1553262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed71cb8fd2ac6869ae41ba5895eba4bbeb89a3fba0949a707f9fe5cbe8f37fb`  
		Last Modified: Tue, 12 Jul 2022 15:12:48 GMT  
		Size: 295.6 KB (295583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5daea30650232dc1b123cb8425895747c91e406b3069bd16b7051b2df7f20b`  
		Last Modified: Tue, 12 Jul 2022 15:12:48 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1700f3de25a27003b3a6963022efbde7da7b557bd9d624a8251536cd1ce4d290`  
		Last Modified: Tue, 12 Jul 2022 15:12:51 GMT  
		Size: 49.0 MB (49039434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42db9a2185d560547609a16f7877805b1e086668898691f419e880f829108d5e`  
		Last Modified: Tue, 12 Jul 2022 15:12:46 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a24ba52538ad79ca5b97acbdd9a15944e280e3d97ccb10d606bd88d95b2cb1`  
		Last Modified: Tue, 12 Jul 2022 15:12:46 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11c8ceb181745bf7b63863ac93e4a934578b9e9daa6ca47b74461bfd142b5cb4`  
		Last Modified: Tue, 12 Jul 2022 15:12:46 GMT  
		Size: 2.2 KB (2180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0694a648fdfcd1507041befc7582c472d2f25d8eb2c4d29c906d59dc2dd3089`  
		Last Modified: Tue, 12 Jul 2022 15:12:46 GMT  
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
