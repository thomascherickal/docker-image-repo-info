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
-	[`couchdb:3.3`](#couchdb33)
-	[`couchdb:3.3.1`](#couchdb331)
-	[`couchdb:latest`](#couchdblatest)

## `couchdb:2`

```console
$ docker pull couchdb@sha256:120b6f2f5645dc188b888b87a57eb322edc67c9c54f53835faaa5aa3cf371f75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2` - linux; amd64

```console
$ docker pull couchdb@sha256:fc9d5c8b5add16d454c00eb141ec35eb14b47e4e767c2bd195f0d65b7a6a8964
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84537541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d408e3fa433f2afba8d7f76673d33861543bbcfffe66849d21fbf2669a73403f`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:48 GMT
ADD file:6c5da7126f75c404a5d182eb6345153d6ea45be11da8be63a1bd355011412847 in / 
# Thu, 09 Feb 2023 03:20:48 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:45:07 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 09 Feb 2023 09:45:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 09 Feb 2023 09:45:17 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:45:21 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 09 Feb 2023 09:45:21 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 09 Feb 2023 09:45:28 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:45:48 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Thu, 09 Feb 2023 09:45:48 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 09 Feb 2023 09:46:07 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 09 Feb 2023 09:46:08 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Thu, 09 Feb 2023 09:46:08 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 09 Feb 2023 09:46:08 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Thu, 09 Feb 2023 09:46:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 09 Feb 2023 09:46:09 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 09:46:09 GMT
VOLUME [/opt/couchdb/data]
# Thu, 09 Feb 2023 09:46:09 GMT
EXPOSE 4369 5984 9100
# Thu, 09 Feb 2023 09:46:09 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:29cd48154c03e9242f1ff4f9895cf886a344fb94c9b71029455e76e11214328f`  
		Last Modified: Thu, 09 Feb 2023 03:25:54 GMT  
		Size: 27.1 MB (27140531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac729d2a283867f9e363c476aa79fc9820f59ba1e95bea0b85214968147e4343`  
		Last Modified: Thu, 09 Feb 2023 09:47:01 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28f4a773fed044da74bbc78ef4eea06ad96191f6b41914ac5052eecf8654b10`  
		Last Modified: Thu, 09 Feb 2023 09:47:01 GMT  
		Size: 6.7 MB (6703802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ad8a46fddc13bf2f1c9bff7193c14445d15eee0c1ed52788850acaa452ce0f`  
		Last Modified: Thu, 09 Feb 2023 09:47:00 GMT  
		Size: 1.3 MB (1259581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e1a7a96866d8b941f299fe0fb0f6a21406565c8745747d9bfef3435bf00dd`  
		Last Modified: Thu, 09 Feb 2023 09:47:00 GMT  
		Size: 294.3 KB (294314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b2fcd76f6c6a65777c1aa7bd3f5a3cc77adc5b384c48473dd3840117a1bf30c`  
		Last Modified: Thu, 09 Feb 2023 09:47:13 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53e81d2db713da91217db52bdfd249f9eee03e3e820eb5f1c9761f228696833`  
		Last Modified: Thu, 09 Feb 2023 09:47:17 GMT  
		Size: 49.1 MB (49132298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97251e135cc9f24b1c3b07091fd0b70ad6030901efb0c075716be19e33a91f5e`  
		Last Modified: Thu, 09 Feb 2023 09:47:11 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18cbf75e3caffedc51a7b150058e69cb41c1011accd485dba3af6b8c3cf70987`  
		Last Modified: Thu, 09 Feb 2023 09:47:11 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d90d3d52fd1cf395d7252f2bbca42f9babf3504c08734a35f124a8ab2b44697`  
		Last Modified: Thu, 09 Feb 2023 09:47:11 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec71c1292d2a1be6aaf6ad7211469232287e0a1ab46471cddbb44f794b2826d6`  
		Last Modified: Thu, 09 Feb 2023 09:47:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:9282e4f1ea4b4f8e27fd49814b2cbebd4fa6991e6e56ea9950b83aef7e78067f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72995080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c59ba586564eb6b87da57dbf349987dcb930d64027b90237d9b2c95f2347c209`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:54 GMT
ADD file:cf6ecb1d6b034b0d4fc309542cb25fff0c997661b323f524ecc258ac323e43f6 in / 
# Sat, 04 Feb 2023 06:17:55 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:23:26 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 04 Feb 2023 17:23:27 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 04 Feb 2023 17:23:36 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:23:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Sat, 04 Feb 2023 17:23:40 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Sat, 04 Feb 2023 17:23:47 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:24:07 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Sat, 04 Feb 2023 17:24:07 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Sat, 04 Feb 2023 17:24:19 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 04 Feb 2023 17:24:19 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Sat, 04 Feb 2023 17:24:19 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 04 Feb 2023 17:24:19 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Sat, 04 Feb 2023 17:24:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 04 Feb 2023 17:24:20 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 17:24:20 GMT
VOLUME [/opt/couchdb/data]
# Sat, 04 Feb 2023 17:24:20 GMT
EXPOSE 4369 5984 9100
# Sat, 04 Feb 2023 17:24:20 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:bd2853c1424a5596deda2f31e1f82920613a03c667c3ff58cb461340b7bb89cd`  
		Last Modified: Sat, 04 Feb 2023 06:22:04 GMT  
		Size: 25.9 MB (25922631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8a62ccf8e59638b0517ad1d1a354034664d36052acdc1007393f79923b09ff`  
		Last Modified: Sat, 04 Feb 2023 17:25:14 GMT  
		Size: 3.4 KB (3433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da58a5e8b0f83e2f8c127ee36d5df953b1eedf83a1c940a26f1827bccae92e77`  
		Last Modified: Sat, 04 Feb 2023 17:25:13 GMT  
		Size: 6.6 MB (6577113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0820839b88a386cac47030ea3b6e170444ee4e3dca1128c5c05016c76be91741`  
		Last Modified: Sat, 04 Feb 2023 17:25:12 GMT  
		Size: 1.2 MB (1164509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4925ba84891a23ed965e55b8d715945da41150c876b369ef9766a6a1fd20d680`  
		Last Modified: Sat, 04 Feb 2023 17:25:12 GMT  
		Size: 294.1 KB (294119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e905ebd4da4dfbd63b50536c361b330eef2761195581953d38353b2fd0f10d4d`  
		Last Modified: Sat, 04 Feb 2023 17:25:25 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9d6261d0277e15acc577a7012f49fc547f0f81b9ae47cb7e248b772d31a690`  
		Last Modified: Sat, 04 Feb 2023 17:25:27 GMT  
		Size: 39.0 MB (39029670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8f435a537d8b78b67074bcc6078113636f6ca5b1264e9de943ca343952064f`  
		Last Modified: Sat, 04 Feb 2023 17:25:23 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4c6faa2d220d2b29393f87efbea4142e3790f241c14ab85203bc7279a3ccca`  
		Last Modified: Sat, 04 Feb 2023 17:25:23 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9087253588293d0619ab30747d5f6167edbdb9fe79471da1cf446b5c19123d98`  
		Last Modified: Sat, 04 Feb 2023 17:25:23 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7607af1258bacb8fc9046c8a33e169c0dc6225a45b260a83328299ed74222cf`  
		Last Modified: Sat, 04 Feb 2023 17:25:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3`

```console
$ docker pull couchdb@sha256:120b6f2f5645dc188b888b87a57eb322edc67c9c54f53835faaa5aa3cf371f75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:fc9d5c8b5add16d454c00eb141ec35eb14b47e4e767c2bd195f0d65b7a6a8964
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84537541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d408e3fa433f2afba8d7f76673d33861543bbcfffe66849d21fbf2669a73403f`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:48 GMT
ADD file:6c5da7126f75c404a5d182eb6345153d6ea45be11da8be63a1bd355011412847 in / 
# Thu, 09 Feb 2023 03:20:48 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:45:07 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 09 Feb 2023 09:45:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 09 Feb 2023 09:45:17 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:45:21 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 09 Feb 2023 09:45:21 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 09 Feb 2023 09:45:28 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:45:48 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Thu, 09 Feb 2023 09:45:48 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 09 Feb 2023 09:46:07 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 09 Feb 2023 09:46:08 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Thu, 09 Feb 2023 09:46:08 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 09 Feb 2023 09:46:08 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Thu, 09 Feb 2023 09:46:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 09 Feb 2023 09:46:09 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 09:46:09 GMT
VOLUME [/opt/couchdb/data]
# Thu, 09 Feb 2023 09:46:09 GMT
EXPOSE 4369 5984 9100
# Thu, 09 Feb 2023 09:46:09 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:29cd48154c03e9242f1ff4f9895cf886a344fb94c9b71029455e76e11214328f`  
		Last Modified: Thu, 09 Feb 2023 03:25:54 GMT  
		Size: 27.1 MB (27140531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac729d2a283867f9e363c476aa79fc9820f59ba1e95bea0b85214968147e4343`  
		Last Modified: Thu, 09 Feb 2023 09:47:01 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28f4a773fed044da74bbc78ef4eea06ad96191f6b41914ac5052eecf8654b10`  
		Last Modified: Thu, 09 Feb 2023 09:47:01 GMT  
		Size: 6.7 MB (6703802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ad8a46fddc13bf2f1c9bff7193c14445d15eee0c1ed52788850acaa452ce0f`  
		Last Modified: Thu, 09 Feb 2023 09:47:00 GMT  
		Size: 1.3 MB (1259581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e1a7a96866d8b941f299fe0fb0f6a21406565c8745747d9bfef3435bf00dd`  
		Last Modified: Thu, 09 Feb 2023 09:47:00 GMT  
		Size: 294.3 KB (294314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b2fcd76f6c6a65777c1aa7bd3f5a3cc77adc5b384c48473dd3840117a1bf30c`  
		Last Modified: Thu, 09 Feb 2023 09:47:13 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53e81d2db713da91217db52bdfd249f9eee03e3e820eb5f1c9761f228696833`  
		Last Modified: Thu, 09 Feb 2023 09:47:17 GMT  
		Size: 49.1 MB (49132298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97251e135cc9f24b1c3b07091fd0b70ad6030901efb0c075716be19e33a91f5e`  
		Last Modified: Thu, 09 Feb 2023 09:47:11 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18cbf75e3caffedc51a7b150058e69cb41c1011accd485dba3af6b8c3cf70987`  
		Last Modified: Thu, 09 Feb 2023 09:47:11 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d90d3d52fd1cf395d7252f2bbca42f9babf3504c08734a35f124a8ab2b44697`  
		Last Modified: Thu, 09 Feb 2023 09:47:11 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec71c1292d2a1be6aaf6ad7211469232287e0a1ab46471cddbb44f794b2826d6`  
		Last Modified: Thu, 09 Feb 2023 09:47:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:9282e4f1ea4b4f8e27fd49814b2cbebd4fa6991e6e56ea9950b83aef7e78067f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72995080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c59ba586564eb6b87da57dbf349987dcb930d64027b90237d9b2c95f2347c209`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:54 GMT
ADD file:cf6ecb1d6b034b0d4fc309542cb25fff0c997661b323f524ecc258ac323e43f6 in / 
# Sat, 04 Feb 2023 06:17:55 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:23:26 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 04 Feb 2023 17:23:27 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 04 Feb 2023 17:23:36 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:23:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Sat, 04 Feb 2023 17:23:40 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Sat, 04 Feb 2023 17:23:47 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:24:07 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Sat, 04 Feb 2023 17:24:07 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Sat, 04 Feb 2023 17:24:19 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 04 Feb 2023 17:24:19 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Sat, 04 Feb 2023 17:24:19 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 04 Feb 2023 17:24:19 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Sat, 04 Feb 2023 17:24:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 04 Feb 2023 17:24:20 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 17:24:20 GMT
VOLUME [/opt/couchdb/data]
# Sat, 04 Feb 2023 17:24:20 GMT
EXPOSE 4369 5984 9100
# Sat, 04 Feb 2023 17:24:20 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:bd2853c1424a5596deda2f31e1f82920613a03c667c3ff58cb461340b7bb89cd`  
		Last Modified: Sat, 04 Feb 2023 06:22:04 GMT  
		Size: 25.9 MB (25922631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8a62ccf8e59638b0517ad1d1a354034664d36052acdc1007393f79923b09ff`  
		Last Modified: Sat, 04 Feb 2023 17:25:14 GMT  
		Size: 3.4 KB (3433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da58a5e8b0f83e2f8c127ee36d5df953b1eedf83a1c940a26f1827bccae92e77`  
		Last Modified: Sat, 04 Feb 2023 17:25:13 GMT  
		Size: 6.6 MB (6577113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0820839b88a386cac47030ea3b6e170444ee4e3dca1128c5c05016c76be91741`  
		Last Modified: Sat, 04 Feb 2023 17:25:12 GMT  
		Size: 1.2 MB (1164509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4925ba84891a23ed965e55b8d715945da41150c876b369ef9766a6a1fd20d680`  
		Last Modified: Sat, 04 Feb 2023 17:25:12 GMT  
		Size: 294.1 KB (294119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e905ebd4da4dfbd63b50536c361b330eef2761195581953d38353b2fd0f10d4d`  
		Last Modified: Sat, 04 Feb 2023 17:25:25 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9d6261d0277e15acc577a7012f49fc547f0f81b9ae47cb7e248b772d31a690`  
		Last Modified: Sat, 04 Feb 2023 17:25:27 GMT  
		Size: 39.0 MB (39029670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8f435a537d8b78b67074bcc6078113636f6ca5b1264e9de943ca343952064f`  
		Last Modified: Sat, 04 Feb 2023 17:25:23 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4c6faa2d220d2b29393f87efbea4142e3790f241c14ab85203bc7279a3ccca`  
		Last Modified: Sat, 04 Feb 2023 17:25:23 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9087253588293d0619ab30747d5f6167edbdb9fe79471da1cf446b5c19123d98`  
		Last Modified: Sat, 04 Feb 2023 17:25:23 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7607af1258bacb8fc9046c8a33e169c0dc6225a45b260a83328299ed74222cf`  
		Last Modified: Sat, 04 Feb 2023 17:25:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3.1`

```console
$ docker pull couchdb@sha256:120b6f2f5645dc188b888b87a57eb322edc67c9c54f53835faaa5aa3cf371f75
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:fc9d5c8b5add16d454c00eb141ec35eb14b47e4e767c2bd195f0d65b7a6a8964
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84537541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d408e3fa433f2afba8d7f76673d33861543bbcfffe66849d21fbf2669a73403f`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:48 GMT
ADD file:6c5da7126f75c404a5d182eb6345153d6ea45be11da8be63a1bd355011412847 in / 
# Thu, 09 Feb 2023 03:20:48 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:45:07 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 09 Feb 2023 09:45:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 09 Feb 2023 09:45:17 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:45:21 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 09 Feb 2023 09:45:21 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 09 Feb 2023 09:45:28 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:45:48 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Thu, 09 Feb 2023 09:45:48 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 09 Feb 2023 09:46:07 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 09 Feb 2023 09:46:08 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Thu, 09 Feb 2023 09:46:08 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 09 Feb 2023 09:46:08 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Thu, 09 Feb 2023 09:46:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 09 Feb 2023 09:46:09 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 09:46:09 GMT
VOLUME [/opt/couchdb/data]
# Thu, 09 Feb 2023 09:46:09 GMT
EXPOSE 4369 5984 9100
# Thu, 09 Feb 2023 09:46:09 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:29cd48154c03e9242f1ff4f9895cf886a344fb94c9b71029455e76e11214328f`  
		Last Modified: Thu, 09 Feb 2023 03:25:54 GMT  
		Size: 27.1 MB (27140531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac729d2a283867f9e363c476aa79fc9820f59ba1e95bea0b85214968147e4343`  
		Last Modified: Thu, 09 Feb 2023 09:47:01 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28f4a773fed044da74bbc78ef4eea06ad96191f6b41914ac5052eecf8654b10`  
		Last Modified: Thu, 09 Feb 2023 09:47:01 GMT  
		Size: 6.7 MB (6703802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ad8a46fddc13bf2f1c9bff7193c14445d15eee0c1ed52788850acaa452ce0f`  
		Last Modified: Thu, 09 Feb 2023 09:47:00 GMT  
		Size: 1.3 MB (1259581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e1a7a96866d8b941f299fe0fb0f6a21406565c8745747d9bfef3435bf00dd`  
		Last Modified: Thu, 09 Feb 2023 09:47:00 GMT  
		Size: 294.3 KB (294314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b2fcd76f6c6a65777c1aa7bd3f5a3cc77adc5b384c48473dd3840117a1bf30c`  
		Last Modified: Thu, 09 Feb 2023 09:47:13 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53e81d2db713da91217db52bdfd249f9eee03e3e820eb5f1c9761f228696833`  
		Last Modified: Thu, 09 Feb 2023 09:47:17 GMT  
		Size: 49.1 MB (49132298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97251e135cc9f24b1c3b07091fd0b70ad6030901efb0c075716be19e33a91f5e`  
		Last Modified: Thu, 09 Feb 2023 09:47:11 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18cbf75e3caffedc51a7b150058e69cb41c1011accd485dba3af6b8c3cf70987`  
		Last Modified: Thu, 09 Feb 2023 09:47:11 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d90d3d52fd1cf395d7252f2bbca42f9babf3504c08734a35f124a8ab2b44697`  
		Last Modified: Thu, 09 Feb 2023 09:47:11 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec71c1292d2a1be6aaf6ad7211469232287e0a1ab46471cddbb44f794b2826d6`  
		Last Modified: Thu, 09 Feb 2023 09:47:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:9282e4f1ea4b4f8e27fd49814b2cbebd4fa6991e6e56ea9950b83aef7e78067f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72995080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c59ba586564eb6b87da57dbf349987dcb930d64027b90237d9b2c95f2347c209`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:54 GMT
ADD file:cf6ecb1d6b034b0d4fc309542cb25fff0c997661b323f524ecc258ac323e43f6 in / 
# Sat, 04 Feb 2023 06:17:55 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:23:26 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 04 Feb 2023 17:23:27 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 04 Feb 2023 17:23:36 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:23:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Sat, 04 Feb 2023 17:23:40 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Sat, 04 Feb 2023 17:23:47 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:24:07 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Sat, 04 Feb 2023 17:24:07 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Sat, 04 Feb 2023 17:24:19 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 04 Feb 2023 17:24:19 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Sat, 04 Feb 2023 17:24:19 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 04 Feb 2023 17:24:19 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Sat, 04 Feb 2023 17:24:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 04 Feb 2023 17:24:20 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 17:24:20 GMT
VOLUME [/opt/couchdb/data]
# Sat, 04 Feb 2023 17:24:20 GMT
EXPOSE 4369 5984 9100
# Sat, 04 Feb 2023 17:24:20 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:bd2853c1424a5596deda2f31e1f82920613a03c667c3ff58cb461340b7bb89cd`  
		Last Modified: Sat, 04 Feb 2023 06:22:04 GMT  
		Size: 25.9 MB (25922631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8a62ccf8e59638b0517ad1d1a354034664d36052acdc1007393f79923b09ff`  
		Last Modified: Sat, 04 Feb 2023 17:25:14 GMT  
		Size: 3.4 KB (3433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da58a5e8b0f83e2f8c127ee36d5df953b1eedf83a1c940a26f1827bccae92e77`  
		Last Modified: Sat, 04 Feb 2023 17:25:13 GMT  
		Size: 6.6 MB (6577113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0820839b88a386cac47030ea3b6e170444ee4e3dca1128c5c05016c76be91741`  
		Last Modified: Sat, 04 Feb 2023 17:25:12 GMT  
		Size: 1.2 MB (1164509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4925ba84891a23ed965e55b8d715945da41150c876b369ef9766a6a1fd20d680`  
		Last Modified: Sat, 04 Feb 2023 17:25:12 GMT  
		Size: 294.1 KB (294119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e905ebd4da4dfbd63b50536c361b330eef2761195581953d38353b2fd0f10d4d`  
		Last Modified: Sat, 04 Feb 2023 17:25:25 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9d6261d0277e15acc577a7012f49fc547f0f81b9ae47cb7e248b772d31a690`  
		Last Modified: Sat, 04 Feb 2023 17:25:27 GMT  
		Size: 39.0 MB (39029670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8f435a537d8b78b67074bcc6078113636f6ca5b1264e9de943ca343952064f`  
		Last Modified: Sat, 04 Feb 2023 17:25:23 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4c6faa2d220d2b29393f87efbea4142e3790f241c14ab85203bc7279a3ccca`  
		Last Modified: Sat, 04 Feb 2023 17:25:23 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9087253588293d0619ab30747d5f6167edbdb9fe79471da1cf446b5c19123d98`  
		Last Modified: Sat, 04 Feb 2023 17:25:23 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7607af1258bacb8fc9046c8a33e169c0dc6225a45b260a83328299ed74222cf`  
		Last Modified: Sat, 04 Feb 2023 17:25:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3`

```console
$ docker pull couchdb@sha256:f0934c58b043bd8734f4e51ea528c80b0e123877524d72fca72f82cca15cac42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3` - linux; amd64

```console
$ docker pull couchdb@sha256:c87c0b765c6cfe23561354f6b65c144d3a4a434c2fcc3c0387af6579ff3605d3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91168681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6d3263c547000f0245836d8529790dce4a86314f29bfebdc51087085c22d919`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:44:06 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 09 Feb 2023 09:44:07 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 09 Feb 2023 09:44:14 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:44:18 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 09 Feb 2023 09:44:18 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 09 Feb 2023 09:44:23 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:44:23 GMT
ENV COUCHDB_VERSION=3.3.1
# Thu, 09 Feb 2023 09:44:24 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 09 Feb 2023 09:44:37 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 09 Feb 2023 09:44:37 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 09 Feb 2023 09:44:38 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Thu, 09 Feb 2023 09:44:38 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Thu, 09 Feb 2023 09:44:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 09 Feb 2023 09:44:38 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 09:44:38 GMT
VOLUME [/opt/couchdb/data]
# Thu, 09 Feb 2023 09:44:39 GMT
EXPOSE 4369 5984 9100
# Thu, 09 Feb 2023 09:44:39 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2345cb2c67b59cd95add5b6be1729d91b01d262a2608a908cb694fe66abca041`  
		Last Modified: Thu, 09 Feb 2023 09:46:28 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b099decb39c6e5245f15055a881c64ac470fac937c698c3dbaee1d6bd6b4c1e1`  
		Last Modified: Thu, 09 Feb 2023 09:46:27 GMT  
		Size: 5.2 MB (5224297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fb61b503efee85952ba73c92cc7b7423655632230e1371d61cd5cabdb53890`  
		Last Modified: Thu, 09 Feb 2023 09:46:27 GMT  
		Size: 1.6 MB (1553314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e2e3947bc9363c6751cbf0ef33583a86e265aee42701a08f8fab8d2788b025`  
		Last Modified: Thu, 09 Feb 2023 09:46:26 GMT  
		Size: 295.6 KB (295585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1027b762cc1e59ed2e554a3270bdb420664faa7075e47505085c244f35869a21`  
		Last Modified: Thu, 09 Feb 2023 09:46:26 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644fbc84104dc655bdd2bb4be14754764d745b27b96f861ceb7d81cfd53cdcfb`  
		Last Modified: Thu, 09 Feb 2023 09:46:30 GMT  
		Size: 52.7 MB (52676291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c8ab0a8f425c2b4cb93bdd5bc4cb16a30133aecda1218d06747d42991106ec`  
		Last Modified: Thu, 09 Feb 2023 09:46:25 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3518f4c3e75c54acebad4f7c502275d0930edb50ccf69654e34bb221782db08a`  
		Last Modified: Thu, 09 Feb 2023 09:46:24 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7c6f882dacf6fc131f0726dd7a4c32cce4bec5b7286c69151f4e02539620ea`  
		Last Modified: Thu, 09 Feb 2023 09:46:24 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743e027ade58faf21563babcbb4f5644d0815d9698e0febf31720cd5b800a2f1`  
		Last Modified: Thu, 09 Feb 2023 09:46:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:f47214cda4815057ea91d1e9a4d91162e54a8ac989e95a7967188ed731a0715d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.5 MB (89524965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:087681dc3a72d1ede1dd62e5d9301d995f74db542b76733f7863f4c53b97ea50`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:22:37 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 04 Feb 2023 17:22:37 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 04 Feb 2023 17:22:44 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:22:47 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Sat, 04 Feb 2023 17:22:47 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Sat, 04 Feb 2023 17:22:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:22:51 GMT
ENV COUCHDB_VERSION=3.3.1
# Sat, 04 Feb 2023 17:22:52 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Sat, 04 Feb 2023 17:23:03 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 04 Feb 2023 17:23:03 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 04 Feb 2023 17:23:03 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Sat, 04 Feb 2023 17:23:04 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Sat, 04 Feb 2023 17:23:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 04 Feb 2023 17:23:04 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 17:23:04 GMT
VOLUME [/opt/couchdb/data]
# Sat, 04 Feb 2023 17:23:04 GMT
EXPOSE 4369 5984 9100
# Sat, 04 Feb 2023 17:23:04 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a68b903b215e1326a49d623b968ae9dffb9483f717208de255349c5d90e0c`  
		Last Modified: Sat, 04 Feb 2023 17:24:41 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0896f3d03f5fcf819d2ba488cd714b1f497268a29f42afbc7991c4272f316402`  
		Last Modified: Sat, 04 Feb 2023 17:24:40 GMT  
		Size: 5.2 MB (5209405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1fa2e4021b0341c215eb2ddd910807ff6966a6e4a9053184d0e4697ebe77ac`  
		Last Modified: Sat, 04 Feb 2023 17:24:39 GMT  
		Size: 1.4 MB (1435920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abaa6061145834dec5f9e2b45997678bac8395c13ad3a300ae32657eea68da65`  
		Last Modified: Sat, 04 Feb 2023 17:24:39 GMT  
		Size: 295.5 KB (295512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef10d1c6b240541aefba0be0f0917df8c6a278710eb1bfa84c0d0ad391795228`  
		Last Modified: Sat, 04 Feb 2023 17:24:39 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c0f32f0cf1ebdca383c1ca2c12f5ec375ff56a4a46707cc18a100b0af2fe94`  
		Last Modified: Sat, 04 Feb 2023 17:24:42 GMT  
		Size: 52.5 MB (52531937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05dfba68eff09a898e5e00541bdeb444f52c9719f2045d19379e969501b6e98c`  
		Last Modified: Sat, 04 Feb 2023 17:24:37 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1341ba060142c109d06e0afc78e4ea0e8d417deec8711f680597dd6099974dcf`  
		Last Modified: Sat, 04 Feb 2023 17:24:37 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d220bd1836270f8ee7590b9aa0747a028bc3d707b94febd2cd4c75f8e85db3`  
		Last Modified: Sat, 04 Feb 2023 17:24:37 GMT  
		Size: 2.2 KB (2185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde49c7224b4154ade30b287c54fc2d2a879480e08a742a12a5f36de68d3c282`  
		Last Modified: Sat, 04 Feb 2023 17:24:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; ppc64le

```console
$ docker pull couchdb@sha256:169c08ffd541c72b2a9615587f87774d4b8047b8a2baeea19668987253ed48fb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.7 MB (96660088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcda0be97c2bcc7cd1d4cca5ce768530b9e41fd99a7fb1a0c41e110153f32673`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Sat, 04 Feb 2023 12:25:55 GMT
ADD file:2c82cc89d7ac2efeaf54e7589e28644e3e8436d66f6909bf295a2b030116ac58 in / 
# Sat, 04 Feb 2023 12:25:58 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 12:51:10 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 04 Feb 2023 12:51:12 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 04 Feb 2023 12:51:30 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 12:51:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Sat, 04 Feb 2023 12:51:38 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Sat, 04 Feb 2023 12:51:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 12:51:50 GMT
ENV COUCHDB_VERSION=3.3.1
# Sat, 04 Feb 2023 12:51:51 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Sat, 04 Feb 2023 12:52:14 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 04 Feb 2023 12:52:16 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 04 Feb 2023 12:52:16 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Sat, 04 Feb 2023 12:52:17 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Sat, 04 Feb 2023 12:52:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 04 Feb 2023 12:52:18 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 12:52:19 GMT
VOLUME [/opt/couchdb/data]
# Sat, 04 Feb 2023 12:52:19 GMT
EXPOSE 4369 5984 9100
# Sat, 04 Feb 2023 12:52:19 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:0604364135762a6c4b3503dd7f0396a51396443bf6052b34b8df7f67679b42c0`  
		Last Modified: Sat, 04 Feb 2023 12:32:12 GMT  
		Size: 35.3 MB (35268795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0db1dae9c381949243f87d00a076dd8935eadd9dfbb4a26770b524da132c28`  
		Last Modified: Sat, 04 Feb 2023 12:53:30 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bb94746f03717925610786197b18595ba7711a5da5b2b691065b02f97414f8`  
		Last Modified: Sat, 04 Feb 2023 12:53:30 GMT  
		Size: 6.0 MB (6043885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffda288060566d345a0058dc1b6f9d096be2045f7d3513b4f20c3d02702e267a`  
		Last Modified: Sat, 04 Feb 2023 12:53:28 GMT  
		Size: 1.5 MB (1509213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29955520a52a30117d393a5c4ec1010873a9bdc7b3d20b207b28b405b0ff648c`  
		Last Modified: Sat, 04 Feb 2023 12:53:28 GMT  
		Size: 295.5 KB (295538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb000d7900471baa0e0264363864b8b3eeb4c04cdb58e634bd1269c20845e7c7`  
		Last Modified: Sat, 04 Feb 2023 12:53:28 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a4e664ddc338ba1e6a85ef75b34219f136dbde3d7b1185395835ad562bc6d7`  
		Last Modified: Sat, 04 Feb 2023 12:53:35 GMT  
		Size: 53.5 MB (53535280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b178a6f96077dd23d510229a7e4030f5fc16474f7cc3164854ac56e093b5715d`  
		Last Modified: Sat, 04 Feb 2023 12:53:26 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:952cec49825f14d1b7dda9a2abc0eaae519d7c0a986e8802df091983c330c6ea`  
		Last Modified: Sat, 04 Feb 2023 12:53:26 GMT  
		Size: 1.0 KB (1002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574106f414796bdfe45f81d686c17d256278791e951bb805d23a1864624cd20a`  
		Last Modified: Sat, 04 Feb 2023 12:53:26 GMT  
		Size: 2.2 KB (2183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0dbba1f74a1ce38b5ed919e7bafc5ddf118b6a9111ea35faa296c5a2c2fdb2`  
		Last Modified: Sat, 04 Feb 2023 12:53:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1`

```console
$ docker pull couchdb@sha256:e7763c0ab2fd169a88eac9bb0d91de2e9fa72b037cfd1c62bcc19e0cdf545db1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:b491c09a88cd31480bb207d1bfe2c77177056273b786de652f6892188acc3d45
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80024421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b058008662dab849e59e40101f657bc93e04281069c2b2480982bf5e801d0ba2`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:48 GMT
ADD file:6c5da7126f75c404a5d182eb6345153d6ea45be11da8be63a1bd355011412847 in / 
# Thu, 09 Feb 2023 03:20:48 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:45:07 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 09 Feb 2023 09:45:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 09 Feb 2023 09:45:17 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:45:21 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 09 Feb 2023 09:45:21 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 09 Feb 2023 09:45:28 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:45:28 GMT
ENV COUCHDB_VERSION=3.1.2
# Thu, 09 Feb 2023 09:45:28 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 09 Feb 2023 09:45:42 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 09 Feb 2023 09:45:43 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 09 Feb 2023 09:45:43 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 09 Feb 2023 09:45:43 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Thu, 09 Feb 2023 09:45:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 09 Feb 2023 09:45:44 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 09:45:44 GMT
VOLUME [/opt/couchdb/data]
# Thu, 09 Feb 2023 09:45:44 GMT
EXPOSE 4369 5984 9100
# Thu, 09 Feb 2023 09:45:44 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:29cd48154c03e9242f1ff4f9895cf886a344fb94c9b71029455e76e11214328f`  
		Last Modified: Thu, 09 Feb 2023 03:25:54 GMT  
		Size: 27.1 MB (27140531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac729d2a283867f9e363c476aa79fc9820f59ba1e95bea0b85214968147e4343`  
		Last Modified: Thu, 09 Feb 2023 09:47:01 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28f4a773fed044da74bbc78ef4eea06ad96191f6b41914ac5052eecf8654b10`  
		Last Modified: Thu, 09 Feb 2023 09:47:01 GMT  
		Size: 6.7 MB (6703802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ad8a46fddc13bf2f1c9bff7193c14445d15eee0c1ed52788850acaa452ce0f`  
		Last Modified: Thu, 09 Feb 2023 09:47:00 GMT  
		Size: 1.3 MB (1259581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e1a7a96866d8b941f299fe0fb0f6a21406565c8745747d9bfef3435bf00dd`  
		Last Modified: Thu, 09 Feb 2023 09:47:00 GMT  
		Size: 294.3 KB (294314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072336ac542ce2a9b4897d6753b8e99ffd4846efd3741dffaba18d208dcf0edd`  
		Last Modified: Thu, 09 Feb 2023 09:46:59 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068c24c7124881f09569f1dc321e8940a062d0beaf0ce7bf01aba9a5777a6dbb`  
		Last Modified: Thu, 09 Feb 2023 09:47:03 GMT  
		Size: 44.6 MB (44619176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cad6d3e1fd037ea7713f2a688f81e218c4b8c49b5e5ba90cb8902da6d6042d3`  
		Last Modified: Thu, 09 Feb 2023 09:46:58 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9726d29448d106e8d84c1c23fa5026a4bab837c5ffc7cbc5b443126ec4cbb35a`  
		Last Modified: Thu, 09 Feb 2023 09:46:58 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80be3967e8e35c2c7f5de00c56078632987439550d13c47c9b1a2c1309977fe4`  
		Last Modified: Thu, 09 Feb 2023 09:46:58 GMT  
		Size: 2.1 KB (2063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b19a6b6646f89688402c68f86a58d94a4158b70d789c15b060029f752529dd`  
		Last Modified: Thu, 09 Feb 2023 09:46:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:3ff203a23533bbe1be0d1de1e325145b6440d41080642107773a41c61b5d645f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75090028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b63de552fb94de512e2e8ba597f614bc9fd466ab0f15490d9dff62d1bd2ac5f`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:54 GMT
ADD file:cf6ecb1d6b034b0d4fc309542cb25fff0c997661b323f524ecc258ac323e43f6 in / 
# Sat, 04 Feb 2023 06:17:55 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:23:26 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 04 Feb 2023 17:23:27 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 04 Feb 2023 17:23:36 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:23:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Sat, 04 Feb 2023 17:23:40 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Sat, 04 Feb 2023 17:23:47 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:23:47 GMT
ENV COUCHDB_VERSION=3.1.2
# Sat, 04 Feb 2023 17:23:47 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Sat, 04 Feb 2023 17:23:59 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 04 Feb 2023 17:23:59 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 04 Feb 2023 17:23:59 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 04 Feb 2023 17:23:59 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Sat, 04 Feb 2023 17:24:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 04 Feb 2023 17:24:00 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 17:24:00 GMT
VOLUME [/opt/couchdb/data]
# Sat, 04 Feb 2023 17:24:00 GMT
EXPOSE 4369 5984 9100
# Sat, 04 Feb 2023 17:24:00 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:bd2853c1424a5596deda2f31e1f82920613a03c667c3ff58cb461340b7bb89cd`  
		Last Modified: Sat, 04 Feb 2023 06:22:04 GMT  
		Size: 25.9 MB (25922631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8a62ccf8e59638b0517ad1d1a354034664d36052acdc1007393f79923b09ff`  
		Last Modified: Sat, 04 Feb 2023 17:25:14 GMT  
		Size: 3.4 KB (3433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da58a5e8b0f83e2f8c127ee36d5df953b1eedf83a1c940a26f1827bccae92e77`  
		Last Modified: Sat, 04 Feb 2023 17:25:13 GMT  
		Size: 6.6 MB (6577113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0820839b88a386cac47030ea3b6e170444ee4e3dca1128c5c05016c76be91741`  
		Last Modified: Sat, 04 Feb 2023 17:25:12 GMT  
		Size: 1.2 MB (1164509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4925ba84891a23ed965e55b8d715945da41150c876b369ef9766a6a1fd20d680`  
		Last Modified: Sat, 04 Feb 2023 17:25:12 GMT  
		Size: 294.1 KB (294119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc866dd6a69a88035efbb1570112d63d0a2d06fdbe2089617d20cc1cdcf762f`  
		Last Modified: Sat, 04 Feb 2023 17:25:12 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a198bd30f329169d2b8c134e867826cb317453be5f512c3651eca7435966e166`  
		Last Modified: Sat, 04 Feb 2023 17:25:14 GMT  
		Size: 41.1 MB (41124623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc445dc55a2afe674b3771cab0a04c3de58501c53e61b21f73fc82654c2ba0a0`  
		Last Modified: Sat, 04 Feb 2023 17:25:10 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd2c87373fa3b018d6968ce6ec38657cf43aa5102524845b1f6adad45f0e007`  
		Last Modified: Sat, 04 Feb 2023 17:25:10 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926fc08fe492818385645f88849bfe4b51c19e776e2e0db4d292f76d0eda3111`  
		Last Modified: Sat, 04 Feb 2023 17:25:11 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51bf2d7b152387786231ee965618ab35e7674c89beae9ce8773f50af34788c6`  
		Last Modified: Sat, 04 Feb 2023 17:25:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1.2`

```console
$ docker pull couchdb@sha256:e7763c0ab2fd169a88eac9bb0d91de2e9fa72b037cfd1c62bcc19e0cdf545db1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1.2` - linux; amd64

```console
$ docker pull couchdb@sha256:b491c09a88cd31480bb207d1bfe2c77177056273b786de652f6892188acc3d45
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80024421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b058008662dab849e59e40101f657bc93e04281069c2b2480982bf5e801d0ba2`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:48 GMT
ADD file:6c5da7126f75c404a5d182eb6345153d6ea45be11da8be63a1bd355011412847 in / 
# Thu, 09 Feb 2023 03:20:48 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:45:07 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 09 Feb 2023 09:45:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 09 Feb 2023 09:45:17 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:45:21 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 09 Feb 2023 09:45:21 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 09 Feb 2023 09:45:28 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:45:28 GMT
ENV COUCHDB_VERSION=3.1.2
# Thu, 09 Feb 2023 09:45:28 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 09 Feb 2023 09:45:42 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 09 Feb 2023 09:45:43 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 09 Feb 2023 09:45:43 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 09 Feb 2023 09:45:43 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Thu, 09 Feb 2023 09:45:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 09 Feb 2023 09:45:44 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 09:45:44 GMT
VOLUME [/opt/couchdb/data]
# Thu, 09 Feb 2023 09:45:44 GMT
EXPOSE 4369 5984 9100
# Thu, 09 Feb 2023 09:45:44 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:29cd48154c03e9242f1ff4f9895cf886a344fb94c9b71029455e76e11214328f`  
		Last Modified: Thu, 09 Feb 2023 03:25:54 GMT  
		Size: 27.1 MB (27140531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac729d2a283867f9e363c476aa79fc9820f59ba1e95bea0b85214968147e4343`  
		Last Modified: Thu, 09 Feb 2023 09:47:01 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28f4a773fed044da74bbc78ef4eea06ad96191f6b41914ac5052eecf8654b10`  
		Last Modified: Thu, 09 Feb 2023 09:47:01 GMT  
		Size: 6.7 MB (6703802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ad8a46fddc13bf2f1c9bff7193c14445d15eee0c1ed52788850acaa452ce0f`  
		Last Modified: Thu, 09 Feb 2023 09:47:00 GMT  
		Size: 1.3 MB (1259581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e1a7a96866d8b941f299fe0fb0f6a21406565c8745747d9bfef3435bf00dd`  
		Last Modified: Thu, 09 Feb 2023 09:47:00 GMT  
		Size: 294.3 KB (294314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072336ac542ce2a9b4897d6753b8e99ffd4846efd3741dffaba18d208dcf0edd`  
		Last Modified: Thu, 09 Feb 2023 09:46:59 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068c24c7124881f09569f1dc321e8940a062d0beaf0ce7bf01aba9a5777a6dbb`  
		Last Modified: Thu, 09 Feb 2023 09:47:03 GMT  
		Size: 44.6 MB (44619176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cad6d3e1fd037ea7713f2a688f81e218c4b8c49b5e5ba90cb8902da6d6042d3`  
		Last Modified: Thu, 09 Feb 2023 09:46:58 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9726d29448d106e8d84c1c23fa5026a4bab837c5ffc7cbc5b443126ec4cbb35a`  
		Last Modified: Thu, 09 Feb 2023 09:46:58 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80be3967e8e35c2c7f5de00c56078632987439550d13c47c9b1a2c1309977fe4`  
		Last Modified: Thu, 09 Feb 2023 09:46:58 GMT  
		Size: 2.1 KB (2063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b19a6b6646f89688402c68f86a58d94a4158b70d789c15b060029f752529dd`  
		Last Modified: Thu, 09 Feb 2023 09:46:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:3ff203a23533bbe1be0d1de1e325145b6440d41080642107773a41c61b5d645f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75090028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b63de552fb94de512e2e8ba597f614bc9fd466ab0f15490d9dff62d1bd2ac5f`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:54 GMT
ADD file:cf6ecb1d6b034b0d4fc309542cb25fff0c997661b323f524ecc258ac323e43f6 in / 
# Sat, 04 Feb 2023 06:17:55 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:23:26 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 04 Feb 2023 17:23:27 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 04 Feb 2023 17:23:36 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:23:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Sat, 04 Feb 2023 17:23:40 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Sat, 04 Feb 2023 17:23:47 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:23:47 GMT
ENV COUCHDB_VERSION=3.1.2
# Sat, 04 Feb 2023 17:23:47 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Sat, 04 Feb 2023 17:23:59 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 04 Feb 2023 17:23:59 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 04 Feb 2023 17:23:59 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 04 Feb 2023 17:23:59 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Sat, 04 Feb 2023 17:24:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 04 Feb 2023 17:24:00 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 17:24:00 GMT
VOLUME [/opt/couchdb/data]
# Sat, 04 Feb 2023 17:24:00 GMT
EXPOSE 4369 5984 9100
# Sat, 04 Feb 2023 17:24:00 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:bd2853c1424a5596deda2f31e1f82920613a03c667c3ff58cb461340b7bb89cd`  
		Last Modified: Sat, 04 Feb 2023 06:22:04 GMT  
		Size: 25.9 MB (25922631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8a62ccf8e59638b0517ad1d1a354034664d36052acdc1007393f79923b09ff`  
		Last Modified: Sat, 04 Feb 2023 17:25:14 GMT  
		Size: 3.4 KB (3433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da58a5e8b0f83e2f8c127ee36d5df953b1eedf83a1c940a26f1827bccae92e77`  
		Last Modified: Sat, 04 Feb 2023 17:25:13 GMT  
		Size: 6.6 MB (6577113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0820839b88a386cac47030ea3b6e170444ee4e3dca1128c5c05016c76be91741`  
		Last Modified: Sat, 04 Feb 2023 17:25:12 GMT  
		Size: 1.2 MB (1164509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4925ba84891a23ed965e55b8d715945da41150c876b369ef9766a6a1fd20d680`  
		Last Modified: Sat, 04 Feb 2023 17:25:12 GMT  
		Size: 294.1 KB (294119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc866dd6a69a88035efbb1570112d63d0a2d06fdbe2089617d20cc1cdcf762f`  
		Last Modified: Sat, 04 Feb 2023 17:25:12 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a198bd30f329169d2b8c134e867826cb317453be5f512c3651eca7435966e166`  
		Last Modified: Sat, 04 Feb 2023 17:25:14 GMT  
		Size: 41.1 MB (41124623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc445dc55a2afe674b3771cab0a04c3de58501c53e61b21f73fc82654c2ba0a0`  
		Last Modified: Sat, 04 Feb 2023 17:25:10 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd2c87373fa3b018d6968ce6ec38657cf43aa5102524845b1f6adad45f0e007`  
		Last Modified: Sat, 04 Feb 2023 17:25:10 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926fc08fe492818385645f88849bfe4b51c19e776e2e0db4d292f76d0eda3111`  
		Last Modified: Sat, 04 Feb 2023 17:25:11 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51bf2d7b152387786231ee965618ab35e7674c89beae9ce8773f50af34788c6`  
		Last Modified: Sat, 04 Feb 2023 17:25:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2`

```console
$ docker pull couchdb@sha256:bfe4646d2ca88a2e37b8dd13b1e642956c492c25011922bf2c86f14f4e213ead
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2` - linux; amd64

```console
$ docker pull couchdb@sha256:a9374fca37b228787ce3748a45550976516962c023f432ef114101eb342f5f3f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87539585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:371f8a53e42a2204634e821304fa2ab05f3d41fcde8991f13d743ee98f8ff563`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:44:06 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 09 Feb 2023 09:44:07 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 09 Feb 2023 09:44:14 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:44:18 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 09 Feb 2023 09:44:18 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 09 Feb 2023 09:44:23 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:44:47 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Thu, 09 Feb 2023 09:44:48 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 09 Feb 2023 09:45:01 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 09 Feb 2023 09:45:01 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 09 Feb 2023 09:45:01 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 09 Feb 2023 09:45:01 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Thu, 09 Feb 2023 09:45:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 09 Feb 2023 09:45:02 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 09:45:02 GMT
VOLUME [/opt/couchdb/data]
# Thu, 09 Feb 2023 09:45:02 GMT
EXPOSE 4369 5984 9100
# Thu, 09 Feb 2023 09:45:02 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2345cb2c67b59cd95add5b6be1729d91b01d262a2608a908cb694fe66abca041`  
		Last Modified: Thu, 09 Feb 2023 09:46:28 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b099decb39c6e5245f15055a881c64ac470fac937c698c3dbaee1d6bd6b4c1e1`  
		Last Modified: Thu, 09 Feb 2023 09:46:27 GMT  
		Size: 5.2 MB (5224297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fb61b503efee85952ba73c92cc7b7423655632230e1371d61cd5cabdb53890`  
		Last Modified: Thu, 09 Feb 2023 09:46:27 GMT  
		Size: 1.6 MB (1553314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e2e3947bc9363c6751cbf0ef33583a86e265aee42701a08f8fab8d2788b025`  
		Last Modified: Thu, 09 Feb 2023 09:46:26 GMT  
		Size: 295.6 KB (295585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4acee21edbfbe6573a294eb80c60c7dc38ffea44c08eece87dff35a5f82a5a91`  
		Last Modified: Thu, 09 Feb 2023 09:46:45 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec20cd59ed4404a0cc5fee5a8298d3c23272153c91a25c9c82636cf07703bec`  
		Last Modified: Thu, 09 Feb 2023 09:46:49 GMT  
		Size: 49.0 MB (49047434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6523992e391a5cf83318f42929fcad83f55aa97374c345e78ba0974efe33d1`  
		Last Modified: Thu, 09 Feb 2023 09:46:43 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f586cd38adf3cb29bbabf94549a51e043f72a3a902a3336dd5b424bf4c9b87f`  
		Last Modified: Thu, 09 Feb 2023 09:46:44 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7236ac55d2997fb0df53b7077da07eee43f63639b85073f16a0e3bef0d9655`  
		Last Modified: Thu, 09 Feb 2023 09:46:44 GMT  
		Size: 2.2 KB (2188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83070691eba38139e0e34ad0552db91e38fa970e686d524f94c8f438ff3df247`  
		Last Modified: Thu, 09 Feb 2023 09:46:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:c7c768e9c2f304f8e178864b5343f178cc336073640f09bf33ce035fc236e776
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.1 MB (86059287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f9c7086fe0e67dee82316adc5e8fed58ac4c27872cfa9f5413dbd7dc967dc58`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:22:37 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 04 Feb 2023 17:22:37 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 04 Feb 2023 17:22:44 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:22:47 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Sat, 04 Feb 2023 17:22:47 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Sat, 04 Feb 2023 17:22:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:23:10 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Sat, 04 Feb 2023 17:23:11 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Sat, 04 Feb 2023 17:23:22 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 04 Feb 2023 17:23:22 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 04 Feb 2023 17:23:22 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 04 Feb 2023 17:23:22 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Sat, 04 Feb 2023 17:23:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 04 Feb 2023 17:23:23 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 17:23:23 GMT
VOLUME [/opt/couchdb/data]
# Sat, 04 Feb 2023 17:23:23 GMT
EXPOSE 4369 5984 9100
# Sat, 04 Feb 2023 17:23:23 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a68b903b215e1326a49d623b968ae9dffb9483f717208de255349c5d90e0c`  
		Last Modified: Sat, 04 Feb 2023 17:24:41 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0896f3d03f5fcf819d2ba488cd714b1f497268a29f42afbc7991c4272f316402`  
		Last Modified: Sat, 04 Feb 2023 17:24:40 GMT  
		Size: 5.2 MB (5209405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1fa2e4021b0341c215eb2ddd910807ff6966a6e4a9053184d0e4697ebe77ac`  
		Last Modified: Sat, 04 Feb 2023 17:24:39 GMT  
		Size: 1.4 MB (1435920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abaa6061145834dec5f9e2b45997678bac8395c13ad3a300ae32657eea68da65`  
		Last Modified: Sat, 04 Feb 2023 17:24:39 GMT  
		Size: 295.5 KB (295512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ff60dabccbec4f2ecf28bba2b4b5aebf60e241922eaee06fcead273c855a21`  
		Last Modified: Sat, 04 Feb 2023 17:24:58 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680f11db1350a8b880af0e7d610578aea45f51fe90fe7b73971cc57fa20a0ebe`  
		Last Modified: Sat, 04 Feb 2023 17:25:01 GMT  
		Size: 49.1 MB (49066492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6da41e4f05240420f62c306b0af301e2e9f0da8bcffe9c24f18afa63dcc5f5`  
		Last Modified: Sat, 04 Feb 2023 17:24:56 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a59c9a71565546ada1a9239f408594a72e7044d7cfb52f638114cf84e910f1`  
		Last Modified: Sat, 04 Feb 2023 17:24:56 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca2bc20c04484a74cecbcfacee7c1c0a9099d31f00c14df03e551aa7abda2be`  
		Last Modified: Sat, 04 Feb 2023 17:24:56 GMT  
		Size: 2.2 KB (2184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0802d476de4384bd56f0e06ab3ad0fb0d7f8df7e23dbbb4b092d2fb61cf1d4ab`  
		Last Modified: Sat, 04 Feb 2023 17:24:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; ppc64le

```console
$ docker pull couchdb@sha256:0a1831ce1ba3833784186968dc0198e9de4884616a3e3d01785759cbda93f662
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93211071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8659a551041dd94e4816058f52f1f62a909362325a09a8abef166d2e09b27520`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Sat, 04 Feb 2023 12:25:55 GMT
ADD file:2c82cc89d7ac2efeaf54e7589e28644e3e8436d66f6909bf295a2b030116ac58 in / 
# Sat, 04 Feb 2023 12:25:58 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 12:51:10 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 04 Feb 2023 12:51:12 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 04 Feb 2023 12:51:30 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 12:51:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Sat, 04 Feb 2023 12:51:38 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Sat, 04 Feb 2023 12:51:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 12:52:36 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Sat, 04 Feb 2023 12:52:37 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Sat, 04 Feb 2023 12:53:00 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 04 Feb 2023 12:53:02 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 04 Feb 2023 12:53:03 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 04 Feb 2023 12:53:03 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Sat, 04 Feb 2023 12:53:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 04 Feb 2023 12:53:05 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 12:53:05 GMT
VOLUME [/opt/couchdb/data]
# Sat, 04 Feb 2023 12:53:06 GMT
EXPOSE 4369 5984 9100
# Sat, 04 Feb 2023 12:53:07 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:0604364135762a6c4b3503dd7f0396a51396443bf6052b34b8df7f67679b42c0`  
		Last Modified: Sat, 04 Feb 2023 12:32:12 GMT  
		Size: 35.3 MB (35268795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0db1dae9c381949243f87d00a076dd8935eadd9dfbb4a26770b524da132c28`  
		Last Modified: Sat, 04 Feb 2023 12:53:30 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bb94746f03717925610786197b18595ba7711a5da5b2b691065b02f97414f8`  
		Last Modified: Sat, 04 Feb 2023 12:53:30 GMT  
		Size: 6.0 MB (6043885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffda288060566d345a0058dc1b6f9d096be2045f7d3513b4f20c3d02702e267a`  
		Last Modified: Sat, 04 Feb 2023 12:53:28 GMT  
		Size: 1.5 MB (1509213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29955520a52a30117d393a5c4ec1010873a9bdc7b3d20b207b28b405b0ff648c`  
		Last Modified: Sat, 04 Feb 2023 12:53:28 GMT  
		Size: 295.5 KB (295538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c6c094478af3456f9e296f86f9168abaad9ed22970ff3afda436e454b258fbd`  
		Last Modified: Sat, 04 Feb 2023 12:53:56 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3619811146b2fb6872b5e21bfce7b51476595f68962ce09e71beb5af7ba4e564`  
		Last Modified: Sat, 04 Feb 2023 12:54:03 GMT  
		Size: 50.1 MB (50086503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db09c0e44ebe0e99368e2259d49fd60a09a378c0f3db1db86cb73c5443a797e5`  
		Last Modified: Sat, 04 Feb 2023 12:53:54 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fce7736048f051ca62f270940d5b0dca17ba4eb7ab4da055bbf6a220aeca139`  
		Last Modified: Sat, 04 Feb 2023 12:53:54 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a5ce9a6f8375a170a8cb95fb41c417e27068b3319ffd3c6667ffc77fa842a82`  
		Last Modified: Sat, 04 Feb 2023 12:53:54 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec4b24d52b42b49d361cc6f394acce6691888cbe5e4c9d0090661ce6179e6d0a`  
		Last Modified: Sat, 04 Feb 2023 12:53:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2.2`

```console
$ docker pull couchdb@sha256:bfe4646d2ca88a2e37b8dd13b1e642956c492c25011922bf2c86f14f4e213ead
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2.2` - linux; amd64

```console
$ docker pull couchdb@sha256:a9374fca37b228787ce3748a45550976516962c023f432ef114101eb342f5f3f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87539585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:371f8a53e42a2204634e821304fa2ab05f3d41fcde8991f13d743ee98f8ff563`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:44:06 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 09 Feb 2023 09:44:07 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 09 Feb 2023 09:44:14 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:44:18 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 09 Feb 2023 09:44:18 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 09 Feb 2023 09:44:23 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:44:47 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Thu, 09 Feb 2023 09:44:48 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 09 Feb 2023 09:45:01 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 09 Feb 2023 09:45:01 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 09 Feb 2023 09:45:01 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 09 Feb 2023 09:45:01 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Thu, 09 Feb 2023 09:45:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 09 Feb 2023 09:45:02 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 09:45:02 GMT
VOLUME [/opt/couchdb/data]
# Thu, 09 Feb 2023 09:45:02 GMT
EXPOSE 4369 5984 9100
# Thu, 09 Feb 2023 09:45:02 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2345cb2c67b59cd95add5b6be1729d91b01d262a2608a908cb694fe66abca041`  
		Last Modified: Thu, 09 Feb 2023 09:46:28 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b099decb39c6e5245f15055a881c64ac470fac937c698c3dbaee1d6bd6b4c1e1`  
		Last Modified: Thu, 09 Feb 2023 09:46:27 GMT  
		Size: 5.2 MB (5224297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fb61b503efee85952ba73c92cc7b7423655632230e1371d61cd5cabdb53890`  
		Last Modified: Thu, 09 Feb 2023 09:46:27 GMT  
		Size: 1.6 MB (1553314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e2e3947bc9363c6751cbf0ef33583a86e265aee42701a08f8fab8d2788b025`  
		Last Modified: Thu, 09 Feb 2023 09:46:26 GMT  
		Size: 295.6 KB (295585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4acee21edbfbe6573a294eb80c60c7dc38ffea44c08eece87dff35a5f82a5a91`  
		Last Modified: Thu, 09 Feb 2023 09:46:45 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec20cd59ed4404a0cc5fee5a8298d3c23272153c91a25c9c82636cf07703bec`  
		Last Modified: Thu, 09 Feb 2023 09:46:49 GMT  
		Size: 49.0 MB (49047434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6523992e391a5cf83318f42929fcad83f55aa97374c345e78ba0974efe33d1`  
		Last Modified: Thu, 09 Feb 2023 09:46:43 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f586cd38adf3cb29bbabf94549a51e043f72a3a902a3336dd5b424bf4c9b87f`  
		Last Modified: Thu, 09 Feb 2023 09:46:44 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7236ac55d2997fb0df53b7077da07eee43f63639b85073f16a0e3bef0d9655`  
		Last Modified: Thu, 09 Feb 2023 09:46:44 GMT  
		Size: 2.2 KB (2188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83070691eba38139e0e34ad0552db91e38fa970e686d524f94c8f438ff3df247`  
		Last Modified: Thu, 09 Feb 2023 09:46:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:c7c768e9c2f304f8e178864b5343f178cc336073640f09bf33ce035fc236e776
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.1 MB (86059287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f9c7086fe0e67dee82316adc5e8fed58ac4c27872cfa9f5413dbd7dc967dc58`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:22:37 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 04 Feb 2023 17:22:37 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 04 Feb 2023 17:22:44 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:22:47 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Sat, 04 Feb 2023 17:22:47 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Sat, 04 Feb 2023 17:22:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:23:10 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Sat, 04 Feb 2023 17:23:11 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Sat, 04 Feb 2023 17:23:22 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 04 Feb 2023 17:23:22 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 04 Feb 2023 17:23:22 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 04 Feb 2023 17:23:22 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Sat, 04 Feb 2023 17:23:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 04 Feb 2023 17:23:23 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 17:23:23 GMT
VOLUME [/opt/couchdb/data]
# Sat, 04 Feb 2023 17:23:23 GMT
EXPOSE 4369 5984 9100
# Sat, 04 Feb 2023 17:23:23 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a68b903b215e1326a49d623b968ae9dffb9483f717208de255349c5d90e0c`  
		Last Modified: Sat, 04 Feb 2023 17:24:41 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0896f3d03f5fcf819d2ba488cd714b1f497268a29f42afbc7991c4272f316402`  
		Last Modified: Sat, 04 Feb 2023 17:24:40 GMT  
		Size: 5.2 MB (5209405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1fa2e4021b0341c215eb2ddd910807ff6966a6e4a9053184d0e4697ebe77ac`  
		Last Modified: Sat, 04 Feb 2023 17:24:39 GMT  
		Size: 1.4 MB (1435920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abaa6061145834dec5f9e2b45997678bac8395c13ad3a300ae32657eea68da65`  
		Last Modified: Sat, 04 Feb 2023 17:24:39 GMT  
		Size: 295.5 KB (295512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ff60dabccbec4f2ecf28bba2b4b5aebf60e241922eaee06fcead273c855a21`  
		Last Modified: Sat, 04 Feb 2023 17:24:58 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680f11db1350a8b880af0e7d610578aea45f51fe90fe7b73971cc57fa20a0ebe`  
		Last Modified: Sat, 04 Feb 2023 17:25:01 GMT  
		Size: 49.1 MB (49066492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6da41e4f05240420f62c306b0af301e2e9f0da8bcffe9c24f18afa63dcc5f5`  
		Last Modified: Sat, 04 Feb 2023 17:24:56 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a59c9a71565546ada1a9239f408594a72e7044d7cfb52f638114cf84e910f1`  
		Last Modified: Sat, 04 Feb 2023 17:24:56 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca2bc20c04484a74cecbcfacee7c1c0a9099d31f00c14df03e551aa7abda2be`  
		Last Modified: Sat, 04 Feb 2023 17:24:56 GMT  
		Size: 2.2 KB (2184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0802d476de4384bd56f0e06ab3ad0fb0d7f8df7e23dbbb4b092d2fb61cf1d4ab`  
		Last Modified: Sat, 04 Feb 2023 17:24:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2.2` - linux; ppc64le

```console
$ docker pull couchdb@sha256:0a1831ce1ba3833784186968dc0198e9de4884616a3e3d01785759cbda93f662
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93211071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8659a551041dd94e4816058f52f1f62a909362325a09a8abef166d2e09b27520`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Sat, 04 Feb 2023 12:25:55 GMT
ADD file:2c82cc89d7ac2efeaf54e7589e28644e3e8436d66f6909bf295a2b030116ac58 in / 
# Sat, 04 Feb 2023 12:25:58 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 12:51:10 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 04 Feb 2023 12:51:12 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 04 Feb 2023 12:51:30 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 12:51:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Sat, 04 Feb 2023 12:51:38 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Sat, 04 Feb 2023 12:51:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 12:52:36 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Sat, 04 Feb 2023 12:52:37 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Sat, 04 Feb 2023 12:53:00 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 04 Feb 2023 12:53:02 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 04 Feb 2023 12:53:03 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 04 Feb 2023 12:53:03 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Sat, 04 Feb 2023 12:53:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 04 Feb 2023 12:53:05 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 12:53:05 GMT
VOLUME [/opt/couchdb/data]
# Sat, 04 Feb 2023 12:53:06 GMT
EXPOSE 4369 5984 9100
# Sat, 04 Feb 2023 12:53:07 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:0604364135762a6c4b3503dd7f0396a51396443bf6052b34b8df7f67679b42c0`  
		Last Modified: Sat, 04 Feb 2023 12:32:12 GMT  
		Size: 35.3 MB (35268795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0db1dae9c381949243f87d00a076dd8935eadd9dfbb4a26770b524da132c28`  
		Last Modified: Sat, 04 Feb 2023 12:53:30 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bb94746f03717925610786197b18595ba7711a5da5b2b691065b02f97414f8`  
		Last Modified: Sat, 04 Feb 2023 12:53:30 GMT  
		Size: 6.0 MB (6043885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffda288060566d345a0058dc1b6f9d096be2045f7d3513b4f20c3d02702e267a`  
		Last Modified: Sat, 04 Feb 2023 12:53:28 GMT  
		Size: 1.5 MB (1509213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29955520a52a30117d393a5c4ec1010873a9bdc7b3d20b207b28b405b0ff648c`  
		Last Modified: Sat, 04 Feb 2023 12:53:28 GMT  
		Size: 295.5 KB (295538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c6c094478af3456f9e296f86f9168abaad9ed22970ff3afda436e454b258fbd`  
		Last Modified: Sat, 04 Feb 2023 12:53:56 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3619811146b2fb6872b5e21bfce7b51476595f68962ce09e71beb5af7ba4e564`  
		Last Modified: Sat, 04 Feb 2023 12:54:03 GMT  
		Size: 50.1 MB (50086503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db09c0e44ebe0e99368e2259d49fd60a09a378c0f3db1db86cb73c5443a797e5`  
		Last Modified: Sat, 04 Feb 2023 12:53:54 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fce7736048f051ca62f270940d5b0dca17ba4eb7ab4da055bbf6a220aeca139`  
		Last Modified: Sat, 04 Feb 2023 12:53:54 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a5ce9a6f8375a170a8cb95fb41c417e27068b3319ffd3c6667ffc77fa842a82`  
		Last Modified: Sat, 04 Feb 2023 12:53:54 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec4b24d52b42b49d361cc6f394acce6691888cbe5e4c9d0090661ce6179e6d0a`  
		Last Modified: Sat, 04 Feb 2023 12:53:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.3`

```console
$ docker pull couchdb@sha256:f0934c58b043bd8734f4e51ea528c80b0e123877524d72fca72f82cca15cac42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.3` - linux; amd64

```console
$ docker pull couchdb@sha256:c87c0b765c6cfe23561354f6b65c144d3a4a434c2fcc3c0387af6579ff3605d3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91168681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6d3263c547000f0245836d8529790dce4a86314f29bfebdc51087085c22d919`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:44:06 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 09 Feb 2023 09:44:07 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 09 Feb 2023 09:44:14 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:44:18 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 09 Feb 2023 09:44:18 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 09 Feb 2023 09:44:23 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:44:23 GMT
ENV COUCHDB_VERSION=3.3.1
# Thu, 09 Feb 2023 09:44:24 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 09 Feb 2023 09:44:37 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 09 Feb 2023 09:44:37 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 09 Feb 2023 09:44:38 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Thu, 09 Feb 2023 09:44:38 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Thu, 09 Feb 2023 09:44:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 09 Feb 2023 09:44:38 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 09:44:38 GMT
VOLUME [/opt/couchdb/data]
# Thu, 09 Feb 2023 09:44:39 GMT
EXPOSE 4369 5984 9100
# Thu, 09 Feb 2023 09:44:39 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2345cb2c67b59cd95add5b6be1729d91b01d262a2608a908cb694fe66abca041`  
		Last Modified: Thu, 09 Feb 2023 09:46:28 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b099decb39c6e5245f15055a881c64ac470fac937c698c3dbaee1d6bd6b4c1e1`  
		Last Modified: Thu, 09 Feb 2023 09:46:27 GMT  
		Size: 5.2 MB (5224297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fb61b503efee85952ba73c92cc7b7423655632230e1371d61cd5cabdb53890`  
		Last Modified: Thu, 09 Feb 2023 09:46:27 GMT  
		Size: 1.6 MB (1553314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e2e3947bc9363c6751cbf0ef33583a86e265aee42701a08f8fab8d2788b025`  
		Last Modified: Thu, 09 Feb 2023 09:46:26 GMT  
		Size: 295.6 KB (295585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1027b762cc1e59ed2e554a3270bdb420664faa7075e47505085c244f35869a21`  
		Last Modified: Thu, 09 Feb 2023 09:46:26 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644fbc84104dc655bdd2bb4be14754764d745b27b96f861ceb7d81cfd53cdcfb`  
		Last Modified: Thu, 09 Feb 2023 09:46:30 GMT  
		Size: 52.7 MB (52676291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c8ab0a8f425c2b4cb93bdd5bc4cb16a30133aecda1218d06747d42991106ec`  
		Last Modified: Thu, 09 Feb 2023 09:46:25 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3518f4c3e75c54acebad4f7c502275d0930edb50ccf69654e34bb221782db08a`  
		Last Modified: Thu, 09 Feb 2023 09:46:24 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7c6f882dacf6fc131f0726dd7a4c32cce4bec5b7286c69151f4e02539620ea`  
		Last Modified: Thu, 09 Feb 2023 09:46:24 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743e027ade58faf21563babcbb4f5644d0815d9698e0febf31720cd5b800a2f1`  
		Last Modified: Thu, 09 Feb 2023 09:46:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:f47214cda4815057ea91d1e9a4d91162e54a8ac989e95a7967188ed731a0715d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.5 MB (89524965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:087681dc3a72d1ede1dd62e5d9301d995f74db542b76733f7863f4c53b97ea50`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:22:37 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 04 Feb 2023 17:22:37 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 04 Feb 2023 17:22:44 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:22:47 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Sat, 04 Feb 2023 17:22:47 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Sat, 04 Feb 2023 17:22:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:22:51 GMT
ENV COUCHDB_VERSION=3.3.1
# Sat, 04 Feb 2023 17:22:52 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Sat, 04 Feb 2023 17:23:03 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 04 Feb 2023 17:23:03 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 04 Feb 2023 17:23:03 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Sat, 04 Feb 2023 17:23:04 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Sat, 04 Feb 2023 17:23:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 04 Feb 2023 17:23:04 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 17:23:04 GMT
VOLUME [/opt/couchdb/data]
# Sat, 04 Feb 2023 17:23:04 GMT
EXPOSE 4369 5984 9100
# Sat, 04 Feb 2023 17:23:04 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a68b903b215e1326a49d623b968ae9dffb9483f717208de255349c5d90e0c`  
		Last Modified: Sat, 04 Feb 2023 17:24:41 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0896f3d03f5fcf819d2ba488cd714b1f497268a29f42afbc7991c4272f316402`  
		Last Modified: Sat, 04 Feb 2023 17:24:40 GMT  
		Size: 5.2 MB (5209405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1fa2e4021b0341c215eb2ddd910807ff6966a6e4a9053184d0e4697ebe77ac`  
		Last Modified: Sat, 04 Feb 2023 17:24:39 GMT  
		Size: 1.4 MB (1435920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abaa6061145834dec5f9e2b45997678bac8395c13ad3a300ae32657eea68da65`  
		Last Modified: Sat, 04 Feb 2023 17:24:39 GMT  
		Size: 295.5 KB (295512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef10d1c6b240541aefba0be0f0917df8c6a278710eb1bfa84c0d0ad391795228`  
		Last Modified: Sat, 04 Feb 2023 17:24:39 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c0f32f0cf1ebdca383c1ca2c12f5ec375ff56a4a46707cc18a100b0af2fe94`  
		Last Modified: Sat, 04 Feb 2023 17:24:42 GMT  
		Size: 52.5 MB (52531937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05dfba68eff09a898e5e00541bdeb444f52c9719f2045d19379e969501b6e98c`  
		Last Modified: Sat, 04 Feb 2023 17:24:37 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1341ba060142c109d06e0afc78e4ea0e8d417deec8711f680597dd6099974dcf`  
		Last Modified: Sat, 04 Feb 2023 17:24:37 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d220bd1836270f8ee7590b9aa0747a028bc3d707b94febd2cd4c75f8e85db3`  
		Last Modified: Sat, 04 Feb 2023 17:24:37 GMT  
		Size: 2.2 KB (2185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde49c7224b4154ade30b287c54fc2d2a879480e08a742a12a5f36de68d3c282`  
		Last Modified: Sat, 04 Feb 2023 17:24:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3` - linux; ppc64le

```console
$ docker pull couchdb@sha256:169c08ffd541c72b2a9615587f87774d4b8047b8a2baeea19668987253ed48fb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.7 MB (96660088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcda0be97c2bcc7cd1d4cca5ce768530b9e41fd99a7fb1a0c41e110153f32673`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Sat, 04 Feb 2023 12:25:55 GMT
ADD file:2c82cc89d7ac2efeaf54e7589e28644e3e8436d66f6909bf295a2b030116ac58 in / 
# Sat, 04 Feb 2023 12:25:58 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 12:51:10 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 04 Feb 2023 12:51:12 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 04 Feb 2023 12:51:30 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 12:51:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Sat, 04 Feb 2023 12:51:38 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Sat, 04 Feb 2023 12:51:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 12:51:50 GMT
ENV COUCHDB_VERSION=3.3.1
# Sat, 04 Feb 2023 12:51:51 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Sat, 04 Feb 2023 12:52:14 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 04 Feb 2023 12:52:16 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 04 Feb 2023 12:52:16 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Sat, 04 Feb 2023 12:52:17 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Sat, 04 Feb 2023 12:52:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 04 Feb 2023 12:52:18 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 12:52:19 GMT
VOLUME [/opt/couchdb/data]
# Sat, 04 Feb 2023 12:52:19 GMT
EXPOSE 4369 5984 9100
# Sat, 04 Feb 2023 12:52:19 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:0604364135762a6c4b3503dd7f0396a51396443bf6052b34b8df7f67679b42c0`  
		Last Modified: Sat, 04 Feb 2023 12:32:12 GMT  
		Size: 35.3 MB (35268795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0db1dae9c381949243f87d00a076dd8935eadd9dfbb4a26770b524da132c28`  
		Last Modified: Sat, 04 Feb 2023 12:53:30 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bb94746f03717925610786197b18595ba7711a5da5b2b691065b02f97414f8`  
		Last Modified: Sat, 04 Feb 2023 12:53:30 GMT  
		Size: 6.0 MB (6043885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffda288060566d345a0058dc1b6f9d096be2045f7d3513b4f20c3d02702e267a`  
		Last Modified: Sat, 04 Feb 2023 12:53:28 GMT  
		Size: 1.5 MB (1509213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29955520a52a30117d393a5c4ec1010873a9bdc7b3d20b207b28b405b0ff648c`  
		Last Modified: Sat, 04 Feb 2023 12:53:28 GMT  
		Size: 295.5 KB (295538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb000d7900471baa0e0264363864b8b3eeb4c04cdb58e634bd1269c20845e7c7`  
		Last Modified: Sat, 04 Feb 2023 12:53:28 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a4e664ddc338ba1e6a85ef75b34219f136dbde3d7b1185395835ad562bc6d7`  
		Last Modified: Sat, 04 Feb 2023 12:53:35 GMT  
		Size: 53.5 MB (53535280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b178a6f96077dd23d510229a7e4030f5fc16474f7cc3164854ac56e093b5715d`  
		Last Modified: Sat, 04 Feb 2023 12:53:26 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:952cec49825f14d1b7dda9a2abc0eaae519d7c0a986e8802df091983c330c6ea`  
		Last Modified: Sat, 04 Feb 2023 12:53:26 GMT  
		Size: 1.0 KB (1002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574106f414796bdfe45f81d686c17d256278791e951bb805d23a1864624cd20a`  
		Last Modified: Sat, 04 Feb 2023 12:53:26 GMT  
		Size: 2.2 KB (2183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0dbba1f74a1ce38b5ed919e7bafc5ddf118b6a9111ea35faa296c5a2c2fdb2`  
		Last Modified: Sat, 04 Feb 2023 12:53:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.3.1`

```console
$ docker pull couchdb@sha256:f0934c58b043bd8734f4e51ea528c80b0e123877524d72fca72f82cca15cac42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:c87c0b765c6cfe23561354f6b65c144d3a4a434c2fcc3c0387af6579ff3605d3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91168681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6d3263c547000f0245836d8529790dce4a86314f29bfebdc51087085c22d919`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:44:06 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 09 Feb 2023 09:44:07 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 09 Feb 2023 09:44:14 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:44:18 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 09 Feb 2023 09:44:18 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 09 Feb 2023 09:44:23 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:44:23 GMT
ENV COUCHDB_VERSION=3.3.1
# Thu, 09 Feb 2023 09:44:24 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 09 Feb 2023 09:44:37 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 09 Feb 2023 09:44:37 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 09 Feb 2023 09:44:38 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Thu, 09 Feb 2023 09:44:38 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Thu, 09 Feb 2023 09:44:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 09 Feb 2023 09:44:38 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 09:44:38 GMT
VOLUME [/opt/couchdb/data]
# Thu, 09 Feb 2023 09:44:39 GMT
EXPOSE 4369 5984 9100
# Thu, 09 Feb 2023 09:44:39 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2345cb2c67b59cd95add5b6be1729d91b01d262a2608a908cb694fe66abca041`  
		Last Modified: Thu, 09 Feb 2023 09:46:28 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b099decb39c6e5245f15055a881c64ac470fac937c698c3dbaee1d6bd6b4c1e1`  
		Last Modified: Thu, 09 Feb 2023 09:46:27 GMT  
		Size: 5.2 MB (5224297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fb61b503efee85952ba73c92cc7b7423655632230e1371d61cd5cabdb53890`  
		Last Modified: Thu, 09 Feb 2023 09:46:27 GMT  
		Size: 1.6 MB (1553314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e2e3947bc9363c6751cbf0ef33583a86e265aee42701a08f8fab8d2788b025`  
		Last Modified: Thu, 09 Feb 2023 09:46:26 GMT  
		Size: 295.6 KB (295585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1027b762cc1e59ed2e554a3270bdb420664faa7075e47505085c244f35869a21`  
		Last Modified: Thu, 09 Feb 2023 09:46:26 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644fbc84104dc655bdd2bb4be14754764d745b27b96f861ceb7d81cfd53cdcfb`  
		Last Modified: Thu, 09 Feb 2023 09:46:30 GMT  
		Size: 52.7 MB (52676291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c8ab0a8f425c2b4cb93bdd5bc4cb16a30133aecda1218d06747d42991106ec`  
		Last Modified: Thu, 09 Feb 2023 09:46:25 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3518f4c3e75c54acebad4f7c502275d0930edb50ccf69654e34bb221782db08a`  
		Last Modified: Thu, 09 Feb 2023 09:46:24 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7c6f882dacf6fc131f0726dd7a4c32cce4bec5b7286c69151f4e02539620ea`  
		Last Modified: Thu, 09 Feb 2023 09:46:24 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743e027ade58faf21563babcbb4f5644d0815d9698e0febf31720cd5b800a2f1`  
		Last Modified: Thu, 09 Feb 2023 09:46:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:f47214cda4815057ea91d1e9a4d91162e54a8ac989e95a7967188ed731a0715d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.5 MB (89524965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:087681dc3a72d1ede1dd62e5d9301d995f74db542b76733f7863f4c53b97ea50`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:22:37 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 04 Feb 2023 17:22:37 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 04 Feb 2023 17:22:44 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:22:47 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Sat, 04 Feb 2023 17:22:47 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Sat, 04 Feb 2023 17:22:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:22:51 GMT
ENV COUCHDB_VERSION=3.3.1
# Sat, 04 Feb 2023 17:22:52 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Sat, 04 Feb 2023 17:23:03 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 04 Feb 2023 17:23:03 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 04 Feb 2023 17:23:03 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Sat, 04 Feb 2023 17:23:04 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Sat, 04 Feb 2023 17:23:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 04 Feb 2023 17:23:04 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 17:23:04 GMT
VOLUME [/opt/couchdb/data]
# Sat, 04 Feb 2023 17:23:04 GMT
EXPOSE 4369 5984 9100
# Sat, 04 Feb 2023 17:23:04 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a68b903b215e1326a49d623b968ae9dffb9483f717208de255349c5d90e0c`  
		Last Modified: Sat, 04 Feb 2023 17:24:41 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0896f3d03f5fcf819d2ba488cd714b1f497268a29f42afbc7991c4272f316402`  
		Last Modified: Sat, 04 Feb 2023 17:24:40 GMT  
		Size: 5.2 MB (5209405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1fa2e4021b0341c215eb2ddd910807ff6966a6e4a9053184d0e4697ebe77ac`  
		Last Modified: Sat, 04 Feb 2023 17:24:39 GMT  
		Size: 1.4 MB (1435920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abaa6061145834dec5f9e2b45997678bac8395c13ad3a300ae32657eea68da65`  
		Last Modified: Sat, 04 Feb 2023 17:24:39 GMT  
		Size: 295.5 KB (295512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef10d1c6b240541aefba0be0f0917df8c6a278710eb1bfa84c0d0ad391795228`  
		Last Modified: Sat, 04 Feb 2023 17:24:39 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c0f32f0cf1ebdca383c1ca2c12f5ec375ff56a4a46707cc18a100b0af2fe94`  
		Last Modified: Sat, 04 Feb 2023 17:24:42 GMT  
		Size: 52.5 MB (52531937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05dfba68eff09a898e5e00541bdeb444f52c9719f2045d19379e969501b6e98c`  
		Last Modified: Sat, 04 Feb 2023 17:24:37 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1341ba060142c109d06e0afc78e4ea0e8d417deec8711f680597dd6099974dcf`  
		Last Modified: Sat, 04 Feb 2023 17:24:37 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d220bd1836270f8ee7590b9aa0747a028bc3d707b94febd2cd4c75f8e85db3`  
		Last Modified: Sat, 04 Feb 2023 17:24:37 GMT  
		Size: 2.2 KB (2185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde49c7224b4154ade30b287c54fc2d2a879480e08a742a12a5f36de68d3c282`  
		Last Modified: Sat, 04 Feb 2023 17:24:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3.1` - linux; ppc64le

```console
$ docker pull couchdb@sha256:169c08ffd541c72b2a9615587f87774d4b8047b8a2baeea19668987253ed48fb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.7 MB (96660088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcda0be97c2bcc7cd1d4cca5ce768530b9e41fd99a7fb1a0c41e110153f32673`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Sat, 04 Feb 2023 12:25:55 GMT
ADD file:2c82cc89d7ac2efeaf54e7589e28644e3e8436d66f6909bf295a2b030116ac58 in / 
# Sat, 04 Feb 2023 12:25:58 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 12:51:10 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 04 Feb 2023 12:51:12 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 04 Feb 2023 12:51:30 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 12:51:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Sat, 04 Feb 2023 12:51:38 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Sat, 04 Feb 2023 12:51:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 12:51:50 GMT
ENV COUCHDB_VERSION=3.3.1
# Sat, 04 Feb 2023 12:51:51 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Sat, 04 Feb 2023 12:52:14 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 04 Feb 2023 12:52:16 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 04 Feb 2023 12:52:16 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Sat, 04 Feb 2023 12:52:17 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Sat, 04 Feb 2023 12:52:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 04 Feb 2023 12:52:18 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 12:52:19 GMT
VOLUME [/opt/couchdb/data]
# Sat, 04 Feb 2023 12:52:19 GMT
EXPOSE 4369 5984 9100
# Sat, 04 Feb 2023 12:52:19 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:0604364135762a6c4b3503dd7f0396a51396443bf6052b34b8df7f67679b42c0`  
		Last Modified: Sat, 04 Feb 2023 12:32:12 GMT  
		Size: 35.3 MB (35268795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0db1dae9c381949243f87d00a076dd8935eadd9dfbb4a26770b524da132c28`  
		Last Modified: Sat, 04 Feb 2023 12:53:30 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bb94746f03717925610786197b18595ba7711a5da5b2b691065b02f97414f8`  
		Last Modified: Sat, 04 Feb 2023 12:53:30 GMT  
		Size: 6.0 MB (6043885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffda288060566d345a0058dc1b6f9d096be2045f7d3513b4f20c3d02702e267a`  
		Last Modified: Sat, 04 Feb 2023 12:53:28 GMT  
		Size: 1.5 MB (1509213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29955520a52a30117d393a5c4ec1010873a9bdc7b3d20b207b28b405b0ff648c`  
		Last Modified: Sat, 04 Feb 2023 12:53:28 GMT  
		Size: 295.5 KB (295538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb000d7900471baa0e0264363864b8b3eeb4c04cdb58e634bd1269c20845e7c7`  
		Last Modified: Sat, 04 Feb 2023 12:53:28 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a4e664ddc338ba1e6a85ef75b34219f136dbde3d7b1185395835ad562bc6d7`  
		Last Modified: Sat, 04 Feb 2023 12:53:35 GMT  
		Size: 53.5 MB (53535280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b178a6f96077dd23d510229a7e4030f5fc16474f7cc3164854ac56e093b5715d`  
		Last Modified: Sat, 04 Feb 2023 12:53:26 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:952cec49825f14d1b7dda9a2abc0eaae519d7c0a986e8802df091983c330c6ea`  
		Last Modified: Sat, 04 Feb 2023 12:53:26 GMT  
		Size: 1.0 KB (1002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574106f414796bdfe45f81d686c17d256278791e951bb805d23a1864624cd20a`  
		Last Modified: Sat, 04 Feb 2023 12:53:26 GMT  
		Size: 2.2 KB (2183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0dbba1f74a1ce38b5ed919e7bafc5ddf118b6a9111ea35faa296c5a2c2fdb2`  
		Last Modified: Sat, 04 Feb 2023 12:53:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:latest`

```console
$ docker pull couchdb@sha256:f0934c58b043bd8734f4e51ea528c80b0e123877524d72fca72f82cca15cac42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:c87c0b765c6cfe23561354f6b65c144d3a4a434c2fcc3c0387af6579ff3605d3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91168681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6d3263c547000f0245836d8529790dce4a86314f29bfebdc51087085c22d919`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:44:06 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 09 Feb 2023 09:44:07 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 09 Feb 2023 09:44:14 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:44:18 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 09 Feb 2023 09:44:18 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 09 Feb 2023 09:44:23 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:44:23 GMT
ENV COUCHDB_VERSION=3.3.1
# Thu, 09 Feb 2023 09:44:24 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 09 Feb 2023 09:44:37 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 09 Feb 2023 09:44:37 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 09 Feb 2023 09:44:38 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Thu, 09 Feb 2023 09:44:38 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Thu, 09 Feb 2023 09:44:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 09 Feb 2023 09:44:38 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 09:44:38 GMT
VOLUME [/opt/couchdb/data]
# Thu, 09 Feb 2023 09:44:39 GMT
EXPOSE 4369 5984 9100
# Thu, 09 Feb 2023 09:44:39 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2345cb2c67b59cd95add5b6be1729d91b01d262a2608a908cb694fe66abca041`  
		Last Modified: Thu, 09 Feb 2023 09:46:28 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b099decb39c6e5245f15055a881c64ac470fac937c698c3dbaee1d6bd6b4c1e1`  
		Last Modified: Thu, 09 Feb 2023 09:46:27 GMT  
		Size: 5.2 MB (5224297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fb61b503efee85952ba73c92cc7b7423655632230e1371d61cd5cabdb53890`  
		Last Modified: Thu, 09 Feb 2023 09:46:27 GMT  
		Size: 1.6 MB (1553314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e2e3947bc9363c6751cbf0ef33583a86e265aee42701a08f8fab8d2788b025`  
		Last Modified: Thu, 09 Feb 2023 09:46:26 GMT  
		Size: 295.6 KB (295585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1027b762cc1e59ed2e554a3270bdb420664faa7075e47505085c244f35869a21`  
		Last Modified: Thu, 09 Feb 2023 09:46:26 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644fbc84104dc655bdd2bb4be14754764d745b27b96f861ceb7d81cfd53cdcfb`  
		Last Modified: Thu, 09 Feb 2023 09:46:30 GMT  
		Size: 52.7 MB (52676291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c8ab0a8f425c2b4cb93bdd5bc4cb16a30133aecda1218d06747d42991106ec`  
		Last Modified: Thu, 09 Feb 2023 09:46:25 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3518f4c3e75c54acebad4f7c502275d0930edb50ccf69654e34bb221782db08a`  
		Last Modified: Thu, 09 Feb 2023 09:46:24 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7c6f882dacf6fc131f0726dd7a4c32cce4bec5b7286c69151f4e02539620ea`  
		Last Modified: Thu, 09 Feb 2023 09:46:24 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743e027ade58faf21563babcbb4f5644d0815d9698e0febf31720cd5b800a2f1`  
		Last Modified: Thu, 09 Feb 2023 09:46:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:f47214cda4815057ea91d1e9a4d91162e54a8ac989e95a7967188ed731a0715d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.5 MB (89524965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:087681dc3a72d1ede1dd62e5d9301d995f74db542b76733f7863f4c53b97ea50`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:22:37 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 04 Feb 2023 17:22:37 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 04 Feb 2023 17:22:44 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:22:47 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Sat, 04 Feb 2023 17:22:47 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Sat, 04 Feb 2023 17:22:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:22:51 GMT
ENV COUCHDB_VERSION=3.3.1
# Sat, 04 Feb 2023 17:22:52 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Sat, 04 Feb 2023 17:23:03 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 04 Feb 2023 17:23:03 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 04 Feb 2023 17:23:03 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Sat, 04 Feb 2023 17:23:04 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Sat, 04 Feb 2023 17:23:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 04 Feb 2023 17:23:04 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 17:23:04 GMT
VOLUME [/opt/couchdb/data]
# Sat, 04 Feb 2023 17:23:04 GMT
EXPOSE 4369 5984 9100
# Sat, 04 Feb 2023 17:23:04 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913a68b903b215e1326a49d623b968ae9dffb9483f717208de255349c5d90e0c`  
		Last Modified: Sat, 04 Feb 2023 17:24:41 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0896f3d03f5fcf819d2ba488cd714b1f497268a29f42afbc7991c4272f316402`  
		Last Modified: Sat, 04 Feb 2023 17:24:40 GMT  
		Size: 5.2 MB (5209405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1fa2e4021b0341c215eb2ddd910807ff6966a6e4a9053184d0e4697ebe77ac`  
		Last Modified: Sat, 04 Feb 2023 17:24:39 GMT  
		Size: 1.4 MB (1435920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abaa6061145834dec5f9e2b45997678bac8395c13ad3a300ae32657eea68da65`  
		Last Modified: Sat, 04 Feb 2023 17:24:39 GMT  
		Size: 295.5 KB (295512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef10d1c6b240541aefba0be0f0917df8c6a278710eb1bfa84c0d0ad391795228`  
		Last Modified: Sat, 04 Feb 2023 17:24:39 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c0f32f0cf1ebdca383c1ca2c12f5ec375ff56a4a46707cc18a100b0af2fe94`  
		Last Modified: Sat, 04 Feb 2023 17:24:42 GMT  
		Size: 52.5 MB (52531937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05dfba68eff09a898e5e00541bdeb444f52c9719f2045d19379e969501b6e98c`  
		Last Modified: Sat, 04 Feb 2023 17:24:37 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1341ba060142c109d06e0afc78e4ea0e8d417deec8711f680597dd6099974dcf`  
		Last Modified: Sat, 04 Feb 2023 17:24:37 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d220bd1836270f8ee7590b9aa0747a028bc3d707b94febd2cd4c75f8e85db3`  
		Last Modified: Sat, 04 Feb 2023 17:24:37 GMT  
		Size: 2.2 KB (2185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde49c7224b4154ade30b287c54fc2d2a879480e08a742a12a5f36de68d3c282`  
		Last Modified: Sat, 04 Feb 2023 17:24:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; ppc64le

```console
$ docker pull couchdb@sha256:169c08ffd541c72b2a9615587f87774d4b8047b8a2baeea19668987253ed48fb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.7 MB (96660088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcda0be97c2bcc7cd1d4cca5ce768530b9e41fd99a7fb1a0c41e110153f32673`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Sat, 04 Feb 2023 12:25:55 GMT
ADD file:2c82cc89d7ac2efeaf54e7589e28644e3e8436d66f6909bf295a2b030116ac58 in / 
# Sat, 04 Feb 2023 12:25:58 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 12:51:10 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 04 Feb 2023 12:51:12 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 04 Feb 2023 12:51:30 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 12:51:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Sat, 04 Feb 2023 12:51:38 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Sat, 04 Feb 2023 12:51:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 12:51:50 GMT
ENV COUCHDB_VERSION=3.3.1
# Sat, 04 Feb 2023 12:51:51 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Sat, 04 Feb 2023 12:52:14 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 04 Feb 2023 12:52:16 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 04 Feb 2023 12:52:16 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Sat, 04 Feb 2023 12:52:17 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Sat, 04 Feb 2023 12:52:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 04 Feb 2023 12:52:18 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 12:52:19 GMT
VOLUME [/opt/couchdb/data]
# Sat, 04 Feb 2023 12:52:19 GMT
EXPOSE 4369 5984 9100
# Sat, 04 Feb 2023 12:52:19 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:0604364135762a6c4b3503dd7f0396a51396443bf6052b34b8df7f67679b42c0`  
		Last Modified: Sat, 04 Feb 2023 12:32:12 GMT  
		Size: 35.3 MB (35268795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0db1dae9c381949243f87d00a076dd8935eadd9dfbb4a26770b524da132c28`  
		Last Modified: Sat, 04 Feb 2023 12:53:30 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bb94746f03717925610786197b18595ba7711a5da5b2b691065b02f97414f8`  
		Last Modified: Sat, 04 Feb 2023 12:53:30 GMT  
		Size: 6.0 MB (6043885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffda288060566d345a0058dc1b6f9d096be2045f7d3513b4f20c3d02702e267a`  
		Last Modified: Sat, 04 Feb 2023 12:53:28 GMT  
		Size: 1.5 MB (1509213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29955520a52a30117d393a5c4ec1010873a9bdc7b3d20b207b28b405b0ff648c`  
		Last Modified: Sat, 04 Feb 2023 12:53:28 GMT  
		Size: 295.5 KB (295538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb000d7900471baa0e0264363864b8b3eeb4c04cdb58e634bd1269c20845e7c7`  
		Last Modified: Sat, 04 Feb 2023 12:53:28 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a4e664ddc338ba1e6a85ef75b34219f136dbde3d7b1185395835ad562bc6d7`  
		Last Modified: Sat, 04 Feb 2023 12:53:35 GMT  
		Size: 53.5 MB (53535280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b178a6f96077dd23d510229a7e4030f5fc16474f7cc3164854ac56e093b5715d`  
		Last Modified: Sat, 04 Feb 2023 12:53:26 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:952cec49825f14d1b7dda9a2abc0eaae519d7c0a986e8802df091983c330c6ea`  
		Last Modified: Sat, 04 Feb 2023 12:53:26 GMT  
		Size: 1.0 KB (1002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574106f414796bdfe45f81d686c17d256278791e951bb805d23a1864624cd20a`  
		Last Modified: Sat, 04 Feb 2023 12:53:26 GMT  
		Size: 2.2 KB (2183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0dbba1f74a1ce38b5ed919e7bafc5ddf118b6a9111ea35faa296c5a2c2fdb2`  
		Last Modified: Sat, 04 Feb 2023 12:53:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
