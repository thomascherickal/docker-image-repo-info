## `couchdb:latest`

```console
$ docker pull couchdb@sha256:72de0dfa76d1434e5007819d1822c9c6c018daf6eb24eeb37fc116551d25925e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:519caf3c55ed85d51a089aae019e644d41d0f5efc5b06438cc4e9b082d4b981a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.6 MB (87550414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a590854b75758f7a94546b92898510c95535130df869c210b49eafb7e650deb5`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:17:40 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 25 Oct 2022 09:17:40 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 25 Oct 2022 09:17:48 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:17:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 25 Oct 2022 09:17:52 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 25 Oct 2022 09:17:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:17:57 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 25 Oct 2022 09:17:58 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 25 Oct 2022 09:18:11 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 25 Oct 2022 09:18:12 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 25 Oct 2022 09:18:12 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 25 Oct 2022 09:18:12 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 25 Oct 2022 09:18:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 25 Oct 2022 09:18:13 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 25 Oct 2022 09:18:13 GMT
VOLUME [/opt/couchdb/data]
# Tue, 25 Oct 2022 09:18:13 GMT
EXPOSE 4369 5984 9100
# Tue, 25 Oct 2022 09:18:13 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c8d4eccee0c23ceb4548f9d7a80e7a2beb2fc3231e95bcbc10ce51d9ce8f7c`  
		Last Modified: Tue, 25 Oct 2022 09:19:49 GMT  
		Size: 3.4 KB (3404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d8f2d33b7f6b474de18bf60a4dc267ea80282cbc0aae79ba8b0e9a06658424`  
		Last Modified: Tue, 25 Oct 2022 09:19:48 GMT  
		Size: 5.2 MB (5225811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad439fb993c0c805c9588a5868696135080edbda50dcf2fa4b8a1007305f0fda`  
		Last Modified: Tue, 25 Oct 2022 09:19:48 GMT  
		Size: 1.6 MB (1554054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2c416c4678614330f9436643f7c64bde257e05b2a790bf601f9bc03aef4a25`  
		Last Modified: Tue, 25 Oct 2022 09:19:47 GMT  
		Size: 296.2 KB (296235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ced4d7e8b139b3e64b55f6c69cfb1475ed61d6d7ded51a84afef652052d6a1f`  
		Last Modified: Tue, 25 Oct 2022 09:19:47 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d8a9368e26807a964039f3c48f99396e3821767f6f96b06ecfa8d50e4efe45`  
		Last Modified: Tue, 25 Oct 2022 09:19:51 GMT  
		Size: 49.0 MB (49047140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58f10ab03a9aad25df6c817f4d6b4d4762a78c8e6e446e5414971b81d4e02bc`  
		Last Modified: Tue, 25 Oct 2022 09:19:45 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4164a43d6f3645ea52a35674080d7d58b541d4f289e2d883c3357caa0a4dc20b`  
		Last Modified: Tue, 25 Oct 2022 09:19:45 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c57c5dabf38e81f9590fc5eed18bfda8d715c481748d987022dadfd709b69a2c`  
		Last Modified: Tue, 25 Oct 2022 09:19:45 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153bea6472d1c2378fba5855f559ff09771f9979ee44f0f3569b23f27e1d9fdf`  
		Last Modified: Tue, 25 Oct 2022 09:19:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:145b882d47cf070745d1083f897ebaeb71613e1c1d98802ce61f5cc22f5211d9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.1 MB (86076939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b1c91fccf1233a9c5ed5557c71155c1408a9768d335e0427c78873713b6ab12`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 06:08:08 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 15 Nov 2022 06:08:09 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 15 Nov 2022 06:08:15 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 06:08:18 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 15 Nov 2022 06:08:18 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 15 Nov 2022 06:08:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 06:08:22 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 15 Nov 2022 06:08:23 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 15 Nov 2022 06:08:34 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 15 Nov 2022 06:08:34 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 15 Nov 2022 06:08:34 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 15 Nov 2022 06:08:34 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 15 Nov 2022 06:08:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 15 Nov 2022 06:08:35 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 06:08:35 GMT
VOLUME [/opt/couchdb/data]
# Tue, 15 Nov 2022 06:08:35 GMT
EXPOSE 4369 5984 9100
# Tue, 15 Nov 2022 06:08:35 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca6c0e3b79ff42b19fb2907c93838f2c30e31cb79eed92408fc7443d943a8d7`  
		Last Modified: Tue, 15 Nov 2022 06:09:52 GMT  
		Size: 3.4 KB (3436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e682ad9c82bd3c65fdab62ffbf7be2b011955313fb18dc56730e92d4eddf90`  
		Last Modified: Tue, 15 Nov 2022 06:09:51 GMT  
		Size: 5.2 MB (5210599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f03b46ce4aa4779bdf19667515611a6ae222f096db65961b3f6fc0e6c57a863`  
		Last Modified: Tue, 15 Nov 2022 06:09:51 GMT  
		Size: 1.4 MB (1436818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27088fad5fb401bf05b573a81c4844a991396cb9ad5be964a726fbdd4aaa49c8`  
		Last Modified: Tue, 15 Nov 2022 06:09:50 GMT  
		Size: 296.1 KB (296126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa1689beaff13fae635fb526be396788f17adbc03415e6ed8912a05f4f2be49`  
		Last Modified: Tue, 15 Nov 2022 06:09:50 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65ba22482ef211f329bf5308c0d86060cedef943961913b2d597e3f60ef2ab5`  
		Last Modified: Tue, 15 Nov 2022 06:09:51 GMT  
		Size: 49.1 MB (49065630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded53d34cc59036e4f3aab1d692de013f6317525d2ecc6946ec0503df7a90ca4`  
		Last Modified: Tue, 15 Nov 2022 06:09:47 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb8e51cbd9a45e80ddd3e30e71bade9f5cfac0abfd5c27c416a7c861c0927f8`  
		Last Modified: Tue, 15 Nov 2022 06:09:46 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ca6be1509b683fd9f97847f75e998337368d84cf17261b16bbea18f98f9b08`  
		Last Modified: Tue, 15 Nov 2022 06:09:46 GMT  
		Size: 2.2 KB (2184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800d28c7ee97018ef48c058bb988f1a2cb17854dc762e9f01886667ebcf6c70d`  
		Last Modified: Tue, 15 Nov 2022 06:09:47 GMT  
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
