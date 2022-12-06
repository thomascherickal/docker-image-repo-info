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
$ docker pull couchdb@sha256:eee452f7a3a4095e3bcecd69e1d35703f57c456382c74427745d27de6b247f54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2` - linux; amd64

```console
$ docker pull couchdb@sha256:3c7d8286f67c29955af85b6ba2f4d91f3552e777b3c874cf5bd9e41c39c79a28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84537182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d6e4679d3b7613cf02f73fc3720de2422e75fa511e607802edb94bb65c98c28`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 06 Dec 2022 01:21:18 GMT
ADD file:30180333dcb9028c0d2776f05042f6f309238b100863a050f3981fb80604e871 in / 
# Tue, 06 Dec 2022 01:21:18 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:21:54 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 06 Dec 2022 08:21:55 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 06 Dec 2022 08:22:03 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:22:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 06 Dec 2022 08:22:08 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 06 Dec 2022 08:22:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:22:34 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 06 Dec 2022 08:22:35 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 06 Dec 2022 08:22:54 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 06 Dec 2022 08:22:54 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 06 Dec 2022 08:22:54 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 06 Dec 2022 08:22:54 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 06 Dec 2022 08:22:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 06 Dec 2022 08:22:55 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:22:55 GMT
VOLUME [/opt/couchdb/data]
# Tue, 06 Dec 2022 08:22:55 GMT
EXPOSE 4369 5984 9100
# Tue, 06 Dec 2022 08:22:55 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6eab20599fab240a56b06125a77b4921dd39662d3b9f9008da7306531772a1d0`  
		Last Modified: Tue, 06 Dec 2022 01:25:52 GMT  
		Size: 27.1 MB (27140356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4720346cf00540581f250d77bc14105378f5f6c5f57aaf95dbf48ad01f23c437`  
		Last Modified: Tue, 06 Dec 2022 08:23:34 GMT  
		Size: 3.4 KB (3410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e47f32f97db51de97153633566181d354d8e7982184e479f9f30ff22085d0a`  
		Last Modified: Tue, 06 Dec 2022 08:23:33 GMT  
		Size: 6.7 MB (6703777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678de994a38a7bb738252752bacf83baf21fdcbf4a377a6a2c8c26da41bef513`  
		Last Modified: Tue, 06 Dec 2022 08:23:33 GMT  
		Size: 1.3 MB (1259611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0958a4046459da3e707046ca5da18f2c0fb640df4b71073180b6d7c43acf6196`  
		Last Modified: Tue, 06 Dec 2022 08:23:32 GMT  
		Size: 294.4 KB (294371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb82207bba13bc1d2acfd2c289b54a8d4c8dc2aed9d0584fc3660b5e9866df2`  
		Last Modified: Tue, 06 Dec 2022 08:23:45 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3782919365a4f6e7968c80561eb2fee4e953c3a39b6ce33a50f26baf70317a50`  
		Last Modified: Tue, 06 Dec 2022 08:23:50 GMT  
		Size: 49.1 MB (49132053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8323343b67afcc3d0a3679a38bf4cee973f3ca409373bb28c05bc8f83bdd15d2`  
		Last Modified: Tue, 06 Dec 2022 08:23:44 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1825aaaaaaefe2e3f90feb55d29c9e3729cc43d00a57e1c8031301e927d73e`  
		Last Modified: Tue, 06 Dec 2022 08:23:43 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14b50efd6ae9fca48cb222002f520d6650fb8d8ed73747ad005e81dc0cf1e47`  
		Last Modified: Tue, 06 Dec 2022 08:23:44 GMT  
		Size: 2.1 KB (2056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426992ba753d5c5d2a194987c791edd0258afb272557e99c371f9f41008ecddf`  
		Last Modified: Tue, 06 Dec 2022 08:23:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:21054e97140089d142e745baf6c98e7e2c97c4d4f6f0299565fbd8a56ff9a2e8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72987485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0002af8d850591fbca889f6047a4a4bc29941b54819e0928f66cf32733826ace`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:34 GMT
ADD file:764288ad3920160093c500e1a7277f174a656030bbe3a0511e7925e84495b6ee in / 
# Tue, 06 Dec 2022 01:40:34 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:37:08 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 06 Dec 2022 02:37:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 06 Dec 2022 02:37:15 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:37:18 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 06 Dec 2022 02:37:18 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 06 Dec 2022 02:37:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:37:41 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 06 Dec 2022 02:37:42 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 06 Dec 2022 02:37:53 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 06 Dec 2022 02:37:53 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 06 Dec 2022 02:37:54 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 06 Dec 2022 02:37:54 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 06 Dec 2022 02:37:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 06 Dec 2022 02:37:54 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 02:37:54 GMT
VOLUME [/opt/couchdb/data]
# Tue, 06 Dec 2022 02:37:54 GMT
EXPOSE 4369 5984 9100
# Tue, 06 Dec 2022 02:37:54 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b473b36a3d93c888196b326b1aad1f802bb6a9fa6fcbc5d2614d99a67899d587`  
		Last Modified: Tue, 06 Dec 2022 01:44:33 GMT  
		Size: 25.9 MB (25914951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa4cd43a0448eef68b0cb6dec18ea5533732271e60ca08d219e19646bce854b`  
		Last Modified: Tue, 06 Dec 2022 02:38:31 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e4122820f112f3d7a65eb655a09df0186564b7c5697d14e007c3090b2b97395`  
		Last Modified: Tue, 06 Dec 2022 02:38:31 GMT  
		Size: 6.6 MB (6577031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97185d0a17fb0863c9a24d3fa01871e9302d438e6b693ebbfe27573e4da289eb`  
		Last Modified: Tue, 06 Dec 2022 02:38:30 GMT  
		Size: 1.2 MB (1164503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da625903a8b5a1b460de4bff4479f9ed3c01c00aa481fc777c3ce0d2615b65cd`  
		Last Modified: Tue, 06 Dec 2022 02:38:30 GMT  
		Size: 294.1 KB (294124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:042831a023d1382c8e69c939943de0550b36233f2bf7ac90ca1615a932a24c7f`  
		Last Modified: Tue, 06 Dec 2022 02:38:43 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd04475a79e193ed810245962b2685b3a9c0523dd7557711bc40aced83fbf383`  
		Last Modified: Tue, 06 Dec 2022 02:38:44 GMT  
		Size: 39.0 MB (39029837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bde3cb9155fe10594f524cef76dc63066528c91555f791e5a2e465d1dbcc2ef`  
		Last Modified: Tue, 06 Dec 2022 02:38:41 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565d0881508f210055e66499a1a8f8f16f5b39403b29f3eead48caac02f53b91`  
		Last Modified: Tue, 06 Dec 2022 02:38:41 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:831fea526803bb427d0f5c8b80a1343318e83c110faee8e84fcfb3cc93874e21`  
		Last Modified: Tue, 06 Dec 2022 02:38:41 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed8756cb78c425652d5d8e6d6e3873a5149c19d7973d9285d234e2be88a3c7c`  
		Last Modified: Tue, 06 Dec 2022 02:38:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3`

```console
$ docker pull couchdb@sha256:eee452f7a3a4095e3bcecd69e1d35703f57c456382c74427745d27de6b247f54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:3c7d8286f67c29955af85b6ba2f4d91f3552e777b3c874cf5bd9e41c39c79a28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84537182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d6e4679d3b7613cf02f73fc3720de2422e75fa511e607802edb94bb65c98c28`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 06 Dec 2022 01:21:18 GMT
ADD file:30180333dcb9028c0d2776f05042f6f309238b100863a050f3981fb80604e871 in / 
# Tue, 06 Dec 2022 01:21:18 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:21:54 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 06 Dec 2022 08:21:55 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 06 Dec 2022 08:22:03 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:22:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 06 Dec 2022 08:22:08 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 06 Dec 2022 08:22:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:22:34 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 06 Dec 2022 08:22:35 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 06 Dec 2022 08:22:54 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 06 Dec 2022 08:22:54 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 06 Dec 2022 08:22:54 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 06 Dec 2022 08:22:54 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 06 Dec 2022 08:22:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 06 Dec 2022 08:22:55 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:22:55 GMT
VOLUME [/opt/couchdb/data]
# Tue, 06 Dec 2022 08:22:55 GMT
EXPOSE 4369 5984 9100
# Tue, 06 Dec 2022 08:22:55 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6eab20599fab240a56b06125a77b4921dd39662d3b9f9008da7306531772a1d0`  
		Last Modified: Tue, 06 Dec 2022 01:25:52 GMT  
		Size: 27.1 MB (27140356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4720346cf00540581f250d77bc14105378f5f6c5f57aaf95dbf48ad01f23c437`  
		Last Modified: Tue, 06 Dec 2022 08:23:34 GMT  
		Size: 3.4 KB (3410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e47f32f97db51de97153633566181d354d8e7982184e479f9f30ff22085d0a`  
		Last Modified: Tue, 06 Dec 2022 08:23:33 GMT  
		Size: 6.7 MB (6703777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678de994a38a7bb738252752bacf83baf21fdcbf4a377a6a2c8c26da41bef513`  
		Last Modified: Tue, 06 Dec 2022 08:23:33 GMT  
		Size: 1.3 MB (1259611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0958a4046459da3e707046ca5da18f2c0fb640df4b71073180b6d7c43acf6196`  
		Last Modified: Tue, 06 Dec 2022 08:23:32 GMT  
		Size: 294.4 KB (294371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb82207bba13bc1d2acfd2c289b54a8d4c8dc2aed9d0584fc3660b5e9866df2`  
		Last Modified: Tue, 06 Dec 2022 08:23:45 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3782919365a4f6e7968c80561eb2fee4e953c3a39b6ce33a50f26baf70317a50`  
		Last Modified: Tue, 06 Dec 2022 08:23:50 GMT  
		Size: 49.1 MB (49132053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8323343b67afcc3d0a3679a38bf4cee973f3ca409373bb28c05bc8f83bdd15d2`  
		Last Modified: Tue, 06 Dec 2022 08:23:44 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1825aaaaaaefe2e3f90feb55d29c9e3729cc43d00a57e1c8031301e927d73e`  
		Last Modified: Tue, 06 Dec 2022 08:23:43 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14b50efd6ae9fca48cb222002f520d6650fb8d8ed73747ad005e81dc0cf1e47`  
		Last Modified: Tue, 06 Dec 2022 08:23:44 GMT  
		Size: 2.1 KB (2056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426992ba753d5c5d2a194987c791edd0258afb272557e99c371f9f41008ecddf`  
		Last Modified: Tue, 06 Dec 2022 08:23:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:21054e97140089d142e745baf6c98e7e2c97c4d4f6f0299565fbd8a56ff9a2e8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72987485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0002af8d850591fbca889f6047a4a4bc29941b54819e0928f66cf32733826ace`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:34 GMT
ADD file:764288ad3920160093c500e1a7277f174a656030bbe3a0511e7925e84495b6ee in / 
# Tue, 06 Dec 2022 01:40:34 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:37:08 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 06 Dec 2022 02:37:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 06 Dec 2022 02:37:15 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:37:18 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 06 Dec 2022 02:37:18 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 06 Dec 2022 02:37:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:37:41 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 06 Dec 2022 02:37:42 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 06 Dec 2022 02:37:53 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 06 Dec 2022 02:37:53 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 06 Dec 2022 02:37:54 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 06 Dec 2022 02:37:54 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 06 Dec 2022 02:37:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 06 Dec 2022 02:37:54 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 02:37:54 GMT
VOLUME [/opt/couchdb/data]
# Tue, 06 Dec 2022 02:37:54 GMT
EXPOSE 4369 5984 9100
# Tue, 06 Dec 2022 02:37:54 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b473b36a3d93c888196b326b1aad1f802bb6a9fa6fcbc5d2614d99a67899d587`  
		Last Modified: Tue, 06 Dec 2022 01:44:33 GMT  
		Size: 25.9 MB (25914951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa4cd43a0448eef68b0cb6dec18ea5533732271e60ca08d219e19646bce854b`  
		Last Modified: Tue, 06 Dec 2022 02:38:31 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e4122820f112f3d7a65eb655a09df0186564b7c5697d14e007c3090b2b97395`  
		Last Modified: Tue, 06 Dec 2022 02:38:31 GMT  
		Size: 6.6 MB (6577031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97185d0a17fb0863c9a24d3fa01871e9302d438e6b693ebbfe27573e4da289eb`  
		Last Modified: Tue, 06 Dec 2022 02:38:30 GMT  
		Size: 1.2 MB (1164503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da625903a8b5a1b460de4bff4479f9ed3c01c00aa481fc777c3ce0d2615b65cd`  
		Last Modified: Tue, 06 Dec 2022 02:38:30 GMT  
		Size: 294.1 KB (294124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:042831a023d1382c8e69c939943de0550b36233f2bf7ac90ca1615a932a24c7f`  
		Last Modified: Tue, 06 Dec 2022 02:38:43 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd04475a79e193ed810245962b2685b3a9c0523dd7557711bc40aced83fbf383`  
		Last Modified: Tue, 06 Dec 2022 02:38:44 GMT  
		Size: 39.0 MB (39029837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bde3cb9155fe10594f524cef76dc63066528c91555f791e5a2e465d1dbcc2ef`  
		Last Modified: Tue, 06 Dec 2022 02:38:41 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565d0881508f210055e66499a1a8f8f16f5b39403b29f3eead48caac02f53b91`  
		Last Modified: Tue, 06 Dec 2022 02:38:41 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:831fea526803bb427d0f5c8b80a1343318e83c110faee8e84fcfb3cc93874e21`  
		Last Modified: Tue, 06 Dec 2022 02:38:41 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed8756cb78c425652d5d8e6d6e3873a5149c19d7973d9285d234e2be88a3c7c`  
		Last Modified: Tue, 06 Dec 2022 02:38:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3.1`

```console
$ docker pull couchdb@sha256:eee452f7a3a4095e3bcecd69e1d35703f57c456382c74427745d27de6b247f54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:3c7d8286f67c29955af85b6ba2f4d91f3552e777b3c874cf5bd9e41c39c79a28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84537182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d6e4679d3b7613cf02f73fc3720de2422e75fa511e607802edb94bb65c98c28`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 06 Dec 2022 01:21:18 GMT
ADD file:30180333dcb9028c0d2776f05042f6f309238b100863a050f3981fb80604e871 in / 
# Tue, 06 Dec 2022 01:21:18 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:21:54 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 06 Dec 2022 08:21:55 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 06 Dec 2022 08:22:03 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:22:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 06 Dec 2022 08:22:08 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 06 Dec 2022 08:22:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:22:34 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 06 Dec 2022 08:22:35 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 06 Dec 2022 08:22:54 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 06 Dec 2022 08:22:54 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 06 Dec 2022 08:22:54 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 06 Dec 2022 08:22:54 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 06 Dec 2022 08:22:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 06 Dec 2022 08:22:55 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:22:55 GMT
VOLUME [/opt/couchdb/data]
# Tue, 06 Dec 2022 08:22:55 GMT
EXPOSE 4369 5984 9100
# Tue, 06 Dec 2022 08:22:55 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6eab20599fab240a56b06125a77b4921dd39662d3b9f9008da7306531772a1d0`  
		Last Modified: Tue, 06 Dec 2022 01:25:52 GMT  
		Size: 27.1 MB (27140356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4720346cf00540581f250d77bc14105378f5f6c5f57aaf95dbf48ad01f23c437`  
		Last Modified: Tue, 06 Dec 2022 08:23:34 GMT  
		Size: 3.4 KB (3410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e47f32f97db51de97153633566181d354d8e7982184e479f9f30ff22085d0a`  
		Last Modified: Tue, 06 Dec 2022 08:23:33 GMT  
		Size: 6.7 MB (6703777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678de994a38a7bb738252752bacf83baf21fdcbf4a377a6a2c8c26da41bef513`  
		Last Modified: Tue, 06 Dec 2022 08:23:33 GMT  
		Size: 1.3 MB (1259611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0958a4046459da3e707046ca5da18f2c0fb640df4b71073180b6d7c43acf6196`  
		Last Modified: Tue, 06 Dec 2022 08:23:32 GMT  
		Size: 294.4 KB (294371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb82207bba13bc1d2acfd2c289b54a8d4c8dc2aed9d0584fc3660b5e9866df2`  
		Last Modified: Tue, 06 Dec 2022 08:23:45 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3782919365a4f6e7968c80561eb2fee4e953c3a39b6ce33a50f26baf70317a50`  
		Last Modified: Tue, 06 Dec 2022 08:23:50 GMT  
		Size: 49.1 MB (49132053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8323343b67afcc3d0a3679a38bf4cee973f3ca409373bb28c05bc8f83bdd15d2`  
		Last Modified: Tue, 06 Dec 2022 08:23:44 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1825aaaaaaefe2e3f90feb55d29c9e3729cc43d00a57e1c8031301e927d73e`  
		Last Modified: Tue, 06 Dec 2022 08:23:43 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14b50efd6ae9fca48cb222002f520d6650fb8d8ed73747ad005e81dc0cf1e47`  
		Last Modified: Tue, 06 Dec 2022 08:23:44 GMT  
		Size: 2.1 KB (2056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426992ba753d5c5d2a194987c791edd0258afb272557e99c371f9f41008ecddf`  
		Last Modified: Tue, 06 Dec 2022 08:23:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:21054e97140089d142e745baf6c98e7e2c97c4d4f6f0299565fbd8a56ff9a2e8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72987485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0002af8d850591fbca889f6047a4a4bc29941b54819e0928f66cf32733826ace`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:34 GMT
ADD file:764288ad3920160093c500e1a7277f174a656030bbe3a0511e7925e84495b6ee in / 
# Tue, 06 Dec 2022 01:40:34 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:37:08 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 06 Dec 2022 02:37:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 06 Dec 2022 02:37:15 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:37:18 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 06 Dec 2022 02:37:18 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 06 Dec 2022 02:37:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:37:41 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 06 Dec 2022 02:37:42 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 06 Dec 2022 02:37:53 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 06 Dec 2022 02:37:53 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 06 Dec 2022 02:37:54 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 06 Dec 2022 02:37:54 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 06 Dec 2022 02:37:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 06 Dec 2022 02:37:54 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 02:37:54 GMT
VOLUME [/opt/couchdb/data]
# Tue, 06 Dec 2022 02:37:54 GMT
EXPOSE 4369 5984 9100
# Tue, 06 Dec 2022 02:37:54 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b473b36a3d93c888196b326b1aad1f802bb6a9fa6fcbc5d2614d99a67899d587`  
		Last Modified: Tue, 06 Dec 2022 01:44:33 GMT  
		Size: 25.9 MB (25914951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa4cd43a0448eef68b0cb6dec18ea5533732271e60ca08d219e19646bce854b`  
		Last Modified: Tue, 06 Dec 2022 02:38:31 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e4122820f112f3d7a65eb655a09df0186564b7c5697d14e007c3090b2b97395`  
		Last Modified: Tue, 06 Dec 2022 02:38:31 GMT  
		Size: 6.6 MB (6577031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97185d0a17fb0863c9a24d3fa01871e9302d438e6b693ebbfe27573e4da289eb`  
		Last Modified: Tue, 06 Dec 2022 02:38:30 GMT  
		Size: 1.2 MB (1164503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da625903a8b5a1b460de4bff4479f9ed3c01c00aa481fc777c3ce0d2615b65cd`  
		Last Modified: Tue, 06 Dec 2022 02:38:30 GMT  
		Size: 294.1 KB (294124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:042831a023d1382c8e69c939943de0550b36233f2bf7ac90ca1615a932a24c7f`  
		Last Modified: Tue, 06 Dec 2022 02:38:43 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd04475a79e193ed810245962b2685b3a9c0523dd7557711bc40aced83fbf383`  
		Last Modified: Tue, 06 Dec 2022 02:38:44 GMT  
		Size: 39.0 MB (39029837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bde3cb9155fe10594f524cef76dc63066528c91555f791e5a2e465d1dbcc2ef`  
		Last Modified: Tue, 06 Dec 2022 02:38:41 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565d0881508f210055e66499a1a8f8f16f5b39403b29f3eead48caac02f53b91`  
		Last Modified: Tue, 06 Dec 2022 02:38:41 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:831fea526803bb427d0f5c8b80a1343318e83c110faee8e84fcfb3cc93874e21`  
		Last Modified: Tue, 06 Dec 2022 02:38:41 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed8756cb78c425652d5d8e6d6e3873a5149c19d7973d9285d234e2be88a3c7c`  
		Last Modified: Tue, 06 Dec 2022 02:38:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3`

```console
$ docker pull couchdb@sha256:b5a484405703078f9a58dea9dccea077d322664e0b9ed6fc1114a8d467f9a8fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3` - linux; amd64

```console
$ docker pull couchdb@sha256:08c8be9a9c54a3fcbf7b689830194cb86bd55e7a59a815fbf2d49e35e76b05d9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87543235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6911a540dd968fe1478b9b500798b164794007387923521be46eb47d99587af`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:21:13 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 06 Dec 2022 08:21:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 06 Dec 2022 08:21:22 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:21:26 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 06 Dec 2022 08:21:27 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 06 Dec 2022 08:21:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:21:33 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 06 Dec 2022 08:21:33 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 06 Dec 2022 08:21:47 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 06 Dec 2022 08:21:48 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 06 Dec 2022 08:21:48 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 06 Dec 2022 08:21:48 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 06 Dec 2022 08:21:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 06 Dec 2022 08:21:49 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:21:49 GMT
VOLUME [/opt/couchdb/data]
# Tue, 06 Dec 2022 08:21:49 GMT
EXPOSE 4369 5984 9100
# Tue, 06 Dec 2022 08:21:49 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bb4afed80e312afc90dddaaa6438df3533f5daa49acff45c16bba875251a01`  
		Last Modified: Tue, 06 Dec 2022 08:23:16 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e491958ff0bf330c113b1f2d36b2c3ece5c47136459694026bb2faa633be728`  
		Last Modified: Tue, 06 Dec 2022 08:23:15 GMT  
		Size: 5.2 MB (5225850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32f9e1cbb5588db7768285bcef98b51da711d331fa72cdd76bfdec18c2b92eb`  
		Last Modified: Tue, 06 Dec 2022 08:23:15 GMT  
		Size: 1.6 MB (1554049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49a082bebdadf80f5cbadefe1fe8fbe52bcc5029c60aeb47fa360be09abc7e5`  
		Last Modified: Tue, 06 Dec 2022 08:23:14 GMT  
		Size: 296.2 KB (296245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e51747b2e733242116d083778cd840dcc9bf2bd7dec710e119be0e46b6e7a89`  
		Last Modified: Tue, 06 Dec 2022 08:23:14 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c3e92a00a7166bf855a2de1f49ab13db229fe44ce43d9096e8f5341b0ec63c`  
		Last Modified: Tue, 06 Dec 2022 08:23:18 GMT  
		Size: 49.0 MB (49047099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9712f2bedab91689d069dcccc1abebfec2bd434e31470ffa53320d53d63294ab`  
		Last Modified: Tue, 06 Dec 2022 08:23:12 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611b5c5f7df92186e277a7c8fb0176c096ae2387abc8f59dabb26fdc2c0f5d3d`  
		Last Modified: Tue, 06 Dec 2022 08:23:12 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7597f2951735385cabea4989eb4b64fbebf06f263b0415f25087abb3c60483`  
		Last Modified: Tue, 06 Dec 2022 08:23:12 GMT  
		Size: 2.2 KB (2188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4f7c3dccc96eb7750187013bcc169daea36abcfd143fd4e275d1046c9aa301`  
		Last Modified: Tue, 06 Dec 2022 08:23:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:01018d93a18c79773dd7bbe769325e38d19ba48c318ccfc2ef441d8ad7b61d5e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.1 MB (86075918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cead15cfe5d467c356162256c209623d5d5982246c130d1147be026e05ef98c0`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:36:34 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 06 Dec 2022 02:36:35 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 06 Dec 2022 02:36:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:36:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 06 Dec 2022 02:36:44 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 06 Dec 2022 02:36:48 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:36:48 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 06 Dec 2022 02:36:49 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 06 Dec 2022 02:37:00 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 06 Dec 2022 02:37:00 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 06 Dec 2022 02:37:00 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 06 Dec 2022 02:37:00 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 06 Dec 2022 02:37:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 06 Dec 2022 02:37:01 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 02:37:01 GMT
VOLUME [/opt/couchdb/data]
# Tue, 06 Dec 2022 02:37:01 GMT
EXPOSE 4369 5984 9100
# Tue, 06 Dec 2022 02:37:01 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52978b09e2554ffbd028007d31a4a2833c7a8cfe23376f79ad433f0a0f467b04`  
		Last Modified: Tue, 06 Dec 2022 02:38:13 GMT  
		Size: 3.4 KB (3432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7363660f0290f9bf69f9ab50f5cffc179c5adc83a5540cf98b171237f816cf9c`  
		Last Modified: Tue, 06 Dec 2022 02:38:12 GMT  
		Size: 5.2 MB (5210587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d423be69a434de8ce0a40b5c1a09c920f45dff093382eb6ee57ee2f000feb3`  
		Last Modified: Tue, 06 Dec 2022 02:38:12 GMT  
		Size: 1.4 MB (1436872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e968973ab936bac3d8a1a603cd5e2610eab8338066238a66c2fb8bf561a783d0`  
		Last Modified: Tue, 06 Dec 2022 02:38:12 GMT  
		Size: 296.2 KB (296157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cb0772563c207436f69961c46ff4164931f8597263861f5552b1ee6d03679a`  
		Last Modified: Tue, 06 Dec 2022 02:38:11 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7e348c01e0f44562a3e0f4ee7ce7ca54478f014bfb250b87048be67cc6d560`  
		Last Modified: Tue, 06 Dec 2022 02:38:14 GMT  
		Size: 49.1 MB (49064819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f2e45be5bc4db8b1d6450de17e8f4f516dc7495720184856472fd43e9539f7`  
		Last Modified: Tue, 06 Dec 2022 02:38:10 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9796347789b28192a0f4425fc6bda42d858708e7628262250c191e5709a4fd9c`  
		Last Modified: Tue, 06 Dec 2022 02:38:10 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13768b759ebbcb8fba738a44e9895e1fa9a72f899587e0c60d8273b6ea59bc7`  
		Last Modified: Tue, 06 Dec 2022 02:38:10 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7526c3a368d90235506e6ccd9932bf1345ba9b39fe0e0c12eff0ca7d813c1560`  
		Last Modified: Tue, 06 Dec 2022 02:38:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; ppc64le

```console
$ docker pull couchdb@sha256:c4d14a5a09618880cab6e3e8433192d8281e0e97346b7600fe82eb20867bd44d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93230341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49c2d3582f74ff15b8a063817e6cb657a7861160f88cbc16e1bacb2a4f494cee`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 06 Dec 2022 01:18:04 GMT
ADD file:2231a44ea52d93df58e23883ba6b6911d4c554f4c1d172d80fb21c751ddcbbfc in / 
# Tue, 06 Dec 2022 01:18:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:43:09 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 06 Dec 2022 01:43:11 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 06 Dec 2022 01:43:26 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 01:43:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 06 Dec 2022 01:43:33 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 06 Dec 2022 01:43:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 01:43:45 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 06 Dec 2022 01:43:47 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 06 Dec 2022 01:44:08 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 06 Dec 2022 01:44:10 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 06 Dec 2022 01:44:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 06 Dec 2022 01:44:11 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 06 Dec 2022 01:44:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 06 Dec 2022 01:44:12 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 01:44:13 GMT
VOLUME [/opt/couchdb/data]
# Tue, 06 Dec 2022 01:44:13 GMT
EXPOSE 4369 5984 9100
# Tue, 06 Dec 2022 01:44:14 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:1f72e1168976861c676bf86a6c149129baba7e13200e8b70e6f24dc2ac2797df`  
		Last Modified: Tue, 06 Dec 2022 01:24:18 GMT  
		Size: 35.3 MB (35285293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9651219ecb35e4178b548721d7d579b5bcad3527e218e212f22f49f1d0e737d`  
		Last Modified: Tue, 06 Dec 2022 01:44:37 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a6ae87d9066bfad2d47cacfb42b74ac3ea08ac23f95401d3ead11129b183e6`  
		Last Modified: Tue, 06 Dec 2022 01:44:37 GMT  
		Size: 6.0 MB (6045482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12bc23b90a71bd7b552b15d2eaebdada16d19778cb84909bcdf0a765b1c9e2c`  
		Last Modified: Tue, 06 Dec 2022 01:44:35 GMT  
		Size: 1.5 MB (1509788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b816512cc9ab4899e2488ff00e7575bcc5bf658ead8cfa8a385b8cdc2d69c89`  
		Last Modified: Tue, 06 Dec 2022 01:44:35 GMT  
		Size: 296.2 KB (296210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e052f116409b694b5f652845866ef6a296c7402a169355d9e101b62d4c4aa94`  
		Last Modified: Tue, 06 Dec 2022 01:44:35 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f424b3f99465a604107ba0d3286aebb6515a17c8d01c2b29a6ead5e6b46714`  
		Last Modified: Tue, 06 Dec 2022 01:44:42 GMT  
		Size: 50.1 MB (50086420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b0bb886f364f867efe9470c1cc85dcb481b9ab2b447cf42306ce8676d09dee`  
		Last Modified: Tue, 06 Dec 2022 01:44:33 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073409bf834d911edf2a2911adc4caef2428d48e577c9ae57fa86c4cb5c6eecb`  
		Last Modified: Tue, 06 Dec 2022 01:44:33 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7c8a9cef21a2d437cbb4d2236784a5d38e6bc56e563908c03f8a3cb10c66ce`  
		Last Modified: Tue, 06 Dec 2022 01:44:33 GMT  
		Size: 2.2 KB (2187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b3e69b9284e828a40354df4b63224c55b3b9413b6592e7e6659599846c75db`  
		Last Modified: Tue, 06 Dec 2022 01:44:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1`

```console
$ docker pull couchdb@sha256:ab1cdfc13a64e8dec374e8305763d1c8f9d30ca8569bd56feaab4b9be920d910
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:5490c3b60652d614ebc06459e36d97b1c0df522507fee0e14fbfe4417afc9ddd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80023920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:077dfa25b4b0383a62a666cbb315697e5c21f309ae8bd56647de6c7f9d0935a1`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 06 Dec 2022 01:21:18 GMT
ADD file:30180333dcb9028c0d2776f05042f6f309238b100863a050f3981fb80604e871 in / 
# Tue, 06 Dec 2022 01:21:18 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:21:54 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 06 Dec 2022 08:21:55 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 06 Dec 2022 08:22:03 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:22:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 06 Dec 2022 08:22:08 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 06 Dec 2022 08:22:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:22:15 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 06 Dec 2022 08:22:16 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 06 Dec 2022 08:22:30 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 06 Dec 2022 08:22:30 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 06 Dec 2022 08:22:30 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 06 Dec 2022 08:22:31 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 06 Dec 2022 08:22:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 06 Dec 2022 08:22:31 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:22:31 GMT
VOLUME [/opt/couchdb/data]
# Tue, 06 Dec 2022 08:22:31 GMT
EXPOSE 4369 5984 9100
# Tue, 06 Dec 2022 08:22:32 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6eab20599fab240a56b06125a77b4921dd39662d3b9f9008da7306531772a1d0`  
		Last Modified: Tue, 06 Dec 2022 01:25:52 GMT  
		Size: 27.1 MB (27140356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4720346cf00540581f250d77bc14105378f5f6c5f57aaf95dbf48ad01f23c437`  
		Last Modified: Tue, 06 Dec 2022 08:23:34 GMT  
		Size: 3.4 KB (3410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e47f32f97db51de97153633566181d354d8e7982184e479f9f30ff22085d0a`  
		Last Modified: Tue, 06 Dec 2022 08:23:33 GMT  
		Size: 6.7 MB (6703777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678de994a38a7bb738252752bacf83baf21fdcbf4a377a6a2c8c26da41bef513`  
		Last Modified: Tue, 06 Dec 2022 08:23:33 GMT  
		Size: 1.3 MB (1259611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0958a4046459da3e707046ca5da18f2c0fb640df4b71073180b6d7c43acf6196`  
		Last Modified: Tue, 06 Dec 2022 08:23:32 GMT  
		Size: 294.4 KB (294371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebf893cab73e78c7b86332632d1ec634d2b0f740324ff5a0928248f55408709`  
		Last Modified: Tue, 06 Dec 2022 08:23:32 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ed64e46a0130c456173aa10f6437512f02a7605ba8aff4065bb77aea2dd4b3`  
		Last Modified: Tue, 06 Dec 2022 08:23:35 GMT  
		Size: 44.6 MB (44618793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6852b39098eb5067bde29416e78ba673372f56b10a9151c3e4e39f2bff2d7cfe`  
		Last Modified: Tue, 06 Dec 2022 08:23:30 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4d6aef560309ad43f39b1fa80f13e9e43137ed0af27c87182f0c5a8290ee97`  
		Last Modified: Tue, 06 Dec 2022 08:23:30 GMT  
		Size: 768.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df35fceee3df97973cf6ae9faf4b02157f9ec1be440cec5851f4f08c2cb0c05a`  
		Last Modified: Tue, 06 Dec 2022 08:23:30 GMT  
		Size: 2.1 KB (2056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e415c3454b344a726481f8514acbc24fefce563070452c4bf0c7dd89dae47c68`  
		Last Modified: Tue, 06 Dec 2022 08:23:30 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:fb48a2f011367f82db30c64f2967697cb2123170ffe5ecdfc6e3a581f6639bc1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75079550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1fcea3fe9997872b17a80bed0364aace4f94466d245e215f177d59d9195c67a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:34 GMT
ADD file:764288ad3920160093c500e1a7277f174a656030bbe3a0511e7925e84495b6ee in / 
# Tue, 06 Dec 2022 01:40:34 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:37:08 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 06 Dec 2022 02:37:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 06 Dec 2022 02:37:15 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:37:18 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 06 Dec 2022 02:37:18 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 06 Dec 2022 02:37:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:37:24 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 06 Dec 2022 02:37:24 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 06 Dec 2022 02:37:36 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 06 Dec 2022 02:37:36 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 06 Dec 2022 02:37:36 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 06 Dec 2022 02:37:36 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 06 Dec 2022 02:37:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 06 Dec 2022 02:37:37 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 02:37:37 GMT
VOLUME [/opt/couchdb/data]
# Tue, 06 Dec 2022 02:37:37 GMT
EXPOSE 4369 5984 9100
# Tue, 06 Dec 2022 02:37:37 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b473b36a3d93c888196b326b1aad1f802bb6a9fa6fcbc5d2614d99a67899d587`  
		Last Modified: Tue, 06 Dec 2022 01:44:33 GMT  
		Size: 25.9 MB (25914951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa4cd43a0448eef68b0cb6dec18ea5533732271e60ca08d219e19646bce854b`  
		Last Modified: Tue, 06 Dec 2022 02:38:31 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e4122820f112f3d7a65eb655a09df0186564b7c5697d14e007c3090b2b97395`  
		Last Modified: Tue, 06 Dec 2022 02:38:31 GMT  
		Size: 6.6 MB (6577031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97185d0a17fb0863c9a24d3fa01871e9302d438e6b693ebbfe27573e4da289eb`  
		Last Modified: Tue, 06 Dec 2022 02:38:30 GMT  
		Size: 1.2 MB (1164503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da625903a8b5a1b460de4bff4479f9ed3c01c00aa481fc777c3ce0d2615b65cd`  
		Last Modified: Tue, 06 Dec 2022 02:38:30 GMT  
		Size: 294.1 KB (294124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f14b8a596acc8afa56faf1c000b1b69f96dc7b581dcbc6945ec5271099075bb`  
		Last Modified: Tue, 06 Dec 2022 02:38:30 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ac85bb15c25ca628b6cbd4ae5cdd71328bb8830f8baacee9b4307aa89c94aa`  
		Last Modified: Tue, 06 Dec 2022 02:38:32 GMT  
		Size: 41.1 MB (41121905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef11b1eabd26ea65c93d245682f9cab7fad33165dd8dd33ffa8a0f3c5c28791c`  
		Last Modified: Tue, 06 Dec 2022 02:38:28 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88ca8539aeb997b6b9fecee4bc2656004e5d50d9d39c33797af30887f5246d1`  
		Last Modified: Tue, 06 Dec 2022 02:38:28 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a2e34cb08123dc03eda52bac747d2ffbc7d5c483cf93573611a7e8098695735`  
		Last Modified: Tue, 06 Dec 2022 02:38:28 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15d51e3805166230beaecf447465f391a4bf66940b8f4bb46cda6ee7e3c217f`  
		Last Modified: Tue, 06 Dec 2022 02:38:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1.2`

```console
$ docker pull couchdb@sha256:ab1cdfc13a64e8dec374e8305763d1c8f9d30ca8569bd56feaab4b9be920d910
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1.2` - linux; amd64

```console
$ docker pull couchdb@sha256:5490c3b60652d614ebc06459e36d97b1c0df522507fee0e14fbfe4417afc9ddd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80023920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:077dfa25b4b0383a62a666cbb315697e5c21f309ae8bd56647de6c7f9d0935a1`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 06 Dec 2022 01:21:18 GMT
ADD file:30180333dcb9028c0d2776f05042f6f309238b100863a050f3981fb80604e871 in / 
# Tue, 06 Dec 2022 01:21:18 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:21:54 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 06 Dec 2022 08:21:55 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 06 Dec 2022 08:22:03 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:22:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 06 Dec 2022 08:22:08 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 06 Dec 2022 08:22:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:22:15 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 06 Dec 2022 08:22:16 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 06 Dec 2022 08:22:30 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 06 Dec 2022 08:22:30 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 06 Dec 2022 08:22:30 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 06 Dec 2022 08:22:31 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 06 Dec 2022 08:22:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 06 Dec 2022 08:22:31 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:22:31 GMT
VOLUME [/opt/couchdb/data]
# Tue, 06 Dec 2022 08:22:31 GMT
EXPOSE 4369 5984 9100
# Tue, 06 Dec 2022 08:22:32 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6eab20599fab240a56b06125a77b4921dd39662d3b9f9008da7306531772a1d0`  
		Last Modified: Tue, 06 Dec 2022 01:25:52 GMT  
		Size: 27.1 MB (27140356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4720346cf00540581f250d77bc14105378f5f6c5f57aaf95dbf48ad01f23c437`  
		Last Modified: Tue, 06 Dec 2022 08:23:34 GMT  
		Size: 3.4 KB (3410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e47f32f97db51de97153633566181d354d8e7982184e479f9f30ff22085d0a`  
		Last Modified: Tue, 06 Dec 2022 08:23:33 GMT  
		Size: 6.7 MB (6703777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678de994a38a7bb738252752bacf83baf21fdcbf4a377a6a2c8c26da41bef513`  
		Last Modified: Tue, 06 Dec 2022 08:23:33 GMT  
		Size: 1.3 MB (1259611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0958a4046459da3e707046ca5da18f2c0fb640df4b71073180b6d7c43acf6196`  
		Last Modified: Tue, 06 Dec 2022 08:23:32 GMT  
		Size: 294.4 KB (294371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebf893cab73e78c7b86332632d1ec634d2b0f740324ff5a0928248f55408709`  
		Last Modified: Tue, 06 Dec 2022 08:23:32 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ed64e46a0130c456173aa10f6437512f02a7605ba8aff4065bb77aea2dd4b3`  
		Last Modified: Tue, 06 Dec 2022 08:23:35 GMT  
		Size: 44.6 MB (44618793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6852b39098eb5067bde29416e78ba673372f56b10a9151c3e4e39f2bff2d7cfe`  
		Last Modified: Tue, 06 Dec 2022 08:23:30 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4d6aef560309ad43f39b1fa80f13e9e43137ed0af27c87182f0c5a8290ee97`  
		Last Modified: Tue, 06 Dec 2022 08:23:30 GMT  
		Size: 768.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df35fceee3df97973cf6ae9faf4b02157f9ec1be440cec5851f4f08c2cb0c05a`  
		Last Modified: Tue, 06 Dec 2022 08:23:30 GMT  
		Size: 2.1 KB (2056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e415c3454b344a726481f8514acbc24fefce563070452c4bf0c7dd89dae47c68`  
		Last Modified: Tue, 06 Dec 2022 08:23:30 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:fb48a2f011367f82db30c64f2967697cb2123170ffe5ecdfc6e3a581f6639bc1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75079550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1fcea3fe9997872b17a80bed0364aace4f94466d245e215f177d59d9195c67a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:34 GMT
ADD file:764288ad3920160093c500e1a7277f174a656030bbe3a0511e7925e84495b6ee in / 
# Tue, 06 Dec 2022 01:40:34 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:37:08 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 06 Dec 2022 02:37:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 06 Dec 2022 02:37:15 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:37:18 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 06 Dec 2022 02:37:18 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 06 Dec 2022 02:37:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:37:24 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 06 Dec 2022 02:37:24 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 06 Dec 2022 02:37:36 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 06 Dec 2022 02:37:36 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 06 Dec 2022 02:37:36 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 06 Dec 2022 02:37:36 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 06 Dec 2022 02:37:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 06 Dec 2022 02:37:37 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 02:37:37 GMT
VOLUME [/opt/couchdb/data]
# Tue, 06 Dec 2022 02:37:37 GMT
EXPOSE 4369 5984 9100
# Tue, 06 Dec 2022 02:37:37 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b473b36a3d93c888196b326b1aad1f802bb6a9fa6fcbc5d2614d99a67899d587`  
		Last Modified: Tue, 06 Dec 2022 01:44:33 GMT  
		Size: 25.9 MB (25914951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa4cd43a0448eef68b0cb6dec18ea5533732271e60ca08d219e19646bce854b`  
		Last Modified: Tue, 06 Dec 2022 02:38:31 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e4122820f112f3d7a65eb655a09df0186564b7c5697d14e007c3090b2b97395`  
		Last Modified: Tue, 06 Dec 2022 02:38:31 GMT  
		Size: 6.6 MB (6577031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97185d0a17fb0863c9a24d3fa01871e9302d438e6b693ebbfe27573e4da289eb`  
		Last Modified: Tue, 06 Dec 2022 02:38:30 GMT  
		Size: 1.2 MB (1164503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da625903a8b5a1b460de4bff4479f9ed3c01c00aa481fc777c3ce0d2615b65cd`  
		Last Modified: Tue, 06 Dec 2022 02:38:30 GMT  
		Size: 294.1 KB (294124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f14b8a596acc8afa56faf1c000b1b69f96dc7b581dcbc6945ec5271099075bb`  
		Last Modified: Tue, 06 Dec 2022 02:38:30 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ac85bb15c25ca628b6cbd4ae5cdd71328bb8830f8baacee9b4307aa89c94aa`  
		Last Modified: Tue, 06 Dec 2022 02:38:32 GMT  
		Size: 41.1 MB (41121905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef11b1eabd26ea65c93d245682f9cab7fad33165dd8dd33ffa8a0f3c5c28791c`  
		Last Modified: Tue, 06 Dec 2022 02:38:28 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88ca8539aeb997b6b9fecee4bc2656004e5d50d9d39c33797af30887f5246d1`  
		Last Modified: Tue, 06 Dec 2022 02:38:28 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a2e34cb08123dc03eda52bac747d2ffbc7d5c483cf93573611a7e8098695735`  
		Last Modified: Tue, 06 Dec 2022 02:38:28 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15d51e3805166230beaecf447465f391a4bf66940b8f4bb46cda6ee7e3c217f`  
		Last Modified: Tue, 06 Dec 2022 02:38:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2`

```console
$ docker pull couchdb@sha256:b5a484405703078f9a58dea9dccea077d322664e0b9ed6fc1114a8d467f9a8fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2` - linux; amd64

```console
$ docker pull couchdb@sha256:08c8be9a9c54a3fcbf7b689830194cb86bd55e7a59a815fbf2d49e35e76b05d9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87543235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6911a540dd968fe1478b9b500798b164794007387923521be46eb47d99587af`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:21:13 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 06 Dec 2022 08:21:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 06 Dec 2022 08:21:22 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:21:26 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 06 Dec 2022 08:21:27 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 06 Dec 2022 08:21:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:21:33 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 06 Dec 2022 08:21:33 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 06 Dec 2022 08:21:47 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 06 Dec 2022 08:21:48 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 06 Dec 2022 08:21:48 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 06 Dec 2022 08:21:48 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 06 Dec 2022 08:21:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 06 Dec 2022 08:21:49 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:21:49 GMT
VOLUME [/opt/couchdb/data]
# Tue, 06 Dec 2022 08:21:49 GMT
EXPOSE 4369 5984 9100
# Tue, 06 Dec 2022 08:21:49 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bb4afed80e312afc90dddaaa6438df3533f5daa49acff45c16bba875251a01`  
		Last Modified: Tue, 06 Dec 2022 08:23:16 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e491958ff0bf330c113b1f2d36b2c3ece5c47136459694026bb2faa633be728`  
		Last Modified: Tue, 06 Dec 2022 08:23:15 GMT  
		Size: 5.2 MB (5225850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32f9e1cbb5588db7768285bcef98b51da711d331fa72cdd76bfdec18c2b92eb`  
		Last Modified: Tue, 06 Dec 2022 08:23:15 GMT  
		Size: 1.6 MB (1554049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49a082bebdadf80f5cbadefe1fe8fbe52bcc5029c60aeb47fa360be09abc7e5`  
		Last Modified: Tue, 06 Dec 2022 08:23:14 GMT  
		Size: 296.2 KB (296245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e51747b2e733242116d083778cd840dcc9bf2bd7dec710e119be0e46b6e7a89`  
		Last Modified: Tue, 06 Dec 2022 08:23:14 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c3e92a00a7166bf855a2de1f49ab13db229fe44ce43d9096e8f5341b0ec63c`  
		Last Modified: Tue, 06 Dec 2022 08:23:18 GMT  
		Size: 49.0 MB (49047099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9712f2bedab91689d069dcccc1abebfec2bd434e31470ffa53320d53d63294ab`  
		Last Modified: Tue, 06 Dec 2022 08:23:12 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611b5c5f7df92186e277a7c8fb0176c096ae2387abc8f59dabb26fdc2c0f5d3d`  
		Last Modified: Tue, 06 Dec 2022 08:23:12 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7597f2951735385cabea4989eb4b64fbebf06f263b0415f25087abb3c60483`  
		Last Modified: Tue, 06 Dec 2022 08:23:12 GMT  
		Size: 2.2 KB (2188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4f7c3dccc96eb7750187013bcc169daea36abcfd143fd4e275d1046c9aa301`  
		Last Modified: Tue, 06 Dec 2022 08:23:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:01018d93a18c79773dd7bbe769325e38d19ba48c318ccfc2ef441d8ad7b61d5e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.1 MB (86075918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cead15cfe5d467c356162256c209623d5d5982246c130d1147be026e05ef98c0`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:36:34 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 06 Dec 2022 02:36:35 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 06 Dec 2022 02:36:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:36:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 06 Dec 2022 02:36:44 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 06 Dec 2022 02:36:48 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:36:48 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 06 Dec 2022 02:36:49 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 06 Dec 2022 02:37:00 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 06 Dec 2022 02:37:00 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 06 Dec 2022 02:37:00 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 06 Dec 2022 02:37:00 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 06 Dec 2022 02:37:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 06 Dec 2022 02:37:01 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 02:37:01 GMT
VOLUME [/opt/couchdb/data]
# Tue, 06 Dec 2022 02:37:01 GMT
EXPOSE 4369 5984 9100
# Tue, 06 Dec 2022 02:37:01 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52978b09e2554ffbd028007d31a4a2833c7a8cfe23376f79ad433f0a0f467b04`  
		Last Modified: Tue, 06 Dec 2022 02:38:13 GMT  
		Size: 3.4 KB (3432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7363660f0290f9bf69f9ab50f5cffc179c5adc83a5540cf98b171237f816cf9c`  
		Last Modified: Tue, 06 Dec 2022 02:38:12 GMT  
		Size: 5.2 MB (5210587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d423be69a434de8ce0a40b5c1a09c920f45dff093382eb6ee57ee2f000feb3`  
		Last Modified: Tue, 06 Dec 2022 02:38:12 GMT  
		Size: 1.4 MB (1436872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e968973ab936bac3d8a1a603cd5e2610eab8338066238a66c2fb8bf561a783d0`  
		Last Modified: Tue, 06 Dec 2022 02:38:12 GMT  
		Size: 296.2 KB (296157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cb0772563c207436f69961c46ff4164931f8597263861f5552b1ee6d03679a`  
		Last Modified: Tue, 06 Dec 2022 02:38:11 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7e348c01e0f44562a3e0f4ee7ce7ca54478f014bfb250b87048be67cc6d560`  
		Last Modified: Tue, 06 Dec 2022 02:38:14 GMT  
		Size: 49.1 MB (49064819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f2e45be5bc4db8b1d6450de17e8f4f516dc7495720184856472fd43e9539f7`  
		Last Modified: Tue, 06 Dec 2022 02:38:10 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9796347789b28192a0f4425fc6bda42d858708e7628262250c191e5709a4fd9c`  
		Last Modified: Tue, 06 Dec 2022 02:38:10 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13768b759ebbcb8fba738a44e9895e1fa9a72f899587e0c60d8273b6ea59bc7`  
		Last Modified: Tue, 06 Dec 2022 02:38:10 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7526c3a368d90235506e6ccd9932bf1345ba9b39fe0e0c12eff0ca7d813c1560`  
		Last Modified: Tue, 06 Dec 2022 02:38:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; ppc64le

```console
$ docker pull couchdb@sha256:c4d14a5a09618880cab6e3e8433192d8281e0e97346b7600fe82eb20867bd44d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93230341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49c2d3582f74ff15b8a063817e6cb657a7861160f88cbc16e1bacb2a4f494cee`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 06 Dec 2022 01:18:04 GMT
ADD file:2231a44ea52d93df58e23883ba6b6911d4c554f4c1d172d80fb21c751ddcbbfc in / 
# Tue, 06 Dec 2022 01:18:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:43:09 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 06 Dec 2022 01:43:11 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 06 Dec 2022 01:43:26 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 01:43:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 06 Dec 2022 01:43:33 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 06 Dec 2022 01:43:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 01:43:45 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 06 Dec 2022 01:43:47 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 06 Dec 2022 01:44:08 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 06 Dec 2022 01:44:10 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 06 Dec 2022 01:44:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 06 Dec 2022 01:44:11 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 06 Dec 2022 01:44:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 06 Dec 2022 01:44:12 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 01:44:13 GMT
VOLUME [/opt/couchdb/data]
# Tue, 06 Dec 2022 01:44:13 GMT
EXPOSE 4369 5984 9100
# Tue, 06 Dec 2022 01:44:14 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:1f72e1168976861c676bf86a6c149129baba7e13200e8b70e6f24dc2ac2797df`  
		Last Modified: Tue, 06 Dec 2022 01:24:18 GMT  
		Size: 35.3 MB (35285293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9651219ecb35e4178b548721d7d579b5bcad3527e218e212f22f49f1d0e737d`  
		Last Modified: Tue, 06 Dec 2022 01:44:37 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a6ae87d9066bfad2d47cacfb42b74ac3ea08ac23f95401d3ead11129b183e6`  
		Last Modified: Tue, 06 Dec 2022 01:44:37 GMT  
		Size: 6.0 MB (6045482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12bc23b90a71bd7b552b15d2eaebdada16d19778cb84909bcdf0a765b1c9e2c`  
		Last Modified: Tue, 06 Dec 2022 01:44:35 GMT  
		Size: 1.5 MB (1509788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b816512cc9ab4899e2488ff00e7575bcc5bf658ead8cfa8a385b8cdc2d69c89`  
		Last Modified: Tue, 06 Dec 2022 01:44:35 GMT  
		Size: 296.2 KB (296210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e052f116409b694b5f652845866ef6a296c7402a169355d9e101b62d4c4aa94`  
		Last Modified: Tue, 06 Dec 2022 01:44:35 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f424b3f99465a604107ba0d3286aebb6515a17c8d01c2b29a6ead5e6b46714`  
		Last Modified: Tue, 06 Dec 2022 01:44:42 GMT  
		Size: 50.1 MB (50086420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b0bb886f364f867efe9470c1cc85dcb481b9ab2b447cf42306ce8676d09dee`  
		Last Modified: Tue, 06 Dec 2022 01:44:33 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073409bf834d911edf2a2911adc4caef2428d48e577c9ae57fa86c4cb5c6eecb`  
		Last Modified: Tue, 06 Dec 2022 01:44:33 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7c8a9cef21a2d437cbb4d2236784a5d38e6bc56e563908c03f8a3cb10c66ce`  
		Last Modified: Tue, 06 Dec 2022 01:44:33 GMT  
		Size: 2.2 KB (2187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b3e69b9284e828a40354df4b63224c55b3b9413b6592e7e6659599846c75db`  
		Last Modified: Tue, 06 Dec 2022 01:44:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2.2`

```console
$ docker pull couchdb@sha256:b5a484405703078f9a58dea9dccea077d322664e0b9ed6fc1114a8d467f9a8fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2.2` - linux; amd64

```console
$ docker pull couchdb@sha256:08c8be9a9c54a3fcbf7b689830194cb86bd55e7a59a815fbf2d49e35e76b05d9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87543235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6911a540dd968fe1478b9b500798b164794007387923521be46eb47d99587af`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:21:13 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 06 Dec 2022 08:21:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 06 Dec 2022 08:21:22 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:21:26 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 06 Dec 2022 08:21:27 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 06 Dec 2022 08:21:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:21:33 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 06 Dec 2022 08:21:33 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 06 Dec 2022 08:21:47 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 06 Dec 2022 08:21:48 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 06 Dec 2022 08:21:48 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 06 Dec 2022 08:21:48 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 06 Dec 2022 08:21:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 06 Dec 2022 08:21:49 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:21:49 GMT
VOLUME [/opt/couchdb/data]
# Tue, 06 Dec 2022 08:21:49 GMT
EXPOSE 4369 5984 9100
# Tue, 06 Dec 2022 08:21:49 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bb4afed80e312afc90dddaaa6438df3533f5daa49acff45c16bba875251a01`  
		Last Modified: Tue, 06 Dec 2022 08:23:16 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e491958ff0bf330c113b1f2d36b2c3ece5c47136459694026bb2faa633be728`  
		Last Modified: Tue, 06 Dec 2022 08:23:15 GMT  
		Size: 5.2 MB (5225850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32f9e1cbb5588db7768285bcef98b51da711d331fa72cdd76bfdec18c2b92eb`  
		Last Modified: Tue, 06 Dec 2022 08:23:15 GMT  
		Size: 1.6 MB (1554049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49a082bebdadf80f5cbadefe1fe8fbe52bcc5029c60aeb47fa360be09abc7e5`  
		Last Modified: Tue, 06 Dec 2022 08:23:14 GMT  
		Size: 296.2 KB (296245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e51747b2e733242116d083778cd840dcc9bf2bd7dec710e119be0e46b6e7a89`  
		Last Modified: Tue, 06 Dec 2022 08:23:14 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c3e92a00a7166bf855a2de1f49ab13db229fe44ce43d9096e8f5341b0ec63c`  
		Last Modified: Tue, 06 Dec 2022 08:23:18 GMT  
		Size: 49.0 MB (49047099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9712f2bedab91689d069dcccc1abebfec2bd434e31470ffa53320d53d63294ab`  
		Last Modified: Tue, 06 Dec 2022 08:23:12 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611b5c5f7df92186e277a7c8fb0176c096ae2387abc8f59dabb26fdc2c0f5d3d`  
		Last Modified: Tue, 06 Dec 2022 08:23:12 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7597f2951735385cabea4989eb4b64fbebf06f263b0415f25087abb3c60483`  
		Last Modified: Tue, 06 Dec 2022 08:23:12 GMT  
		Size: 2.2 KB (2188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4f7c3dccc96eb7750187013bcc169daea36abcfd143fd4e275d1046c9aa301`  
		Last Modified: Tue, 06 Dec 2022 08:23:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:01018d93a18c79773dd7bbe769325e38d19ba48c318ccfc2ef441d8ad7b61d5e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.1 MB (86075918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cead15cfe5d467c356162256c209623d5d5982246c130d1147be026e05ef98c0`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:36:34 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 06 Dec 2022 02:36:35 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 06 Dec 2022 02:36:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:36:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 06 Dec 2022 02:36:44 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 06 Dec 2022 02:36:48 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:36:48 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 06 Dec 2022 02:36:49 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 06 Dec 2022 02:37:00 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 06 Dec 2022 02:37:00 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 06 Dec 2022 02:37:00 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 06 Dec 2022 02:37:00 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 06 Dec 2022 02:37:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 06 Dec 2022 02:37:01 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 02:37:01 GMT
VOLUME [/opt/couchdb/data]
# Tue, 06 Dec 2022 02:37:01 GMT
EXPOSE 4369 5984 9100
# Tue, 06 Dec 2022 02:37:01 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52978b09e2554ffbd028007d31a4a2833c7a8cfe23376f79ad433f0a0f467b04`  
		Last Modified: Tue, 06 Dec 2022 02:38:13 GMT  
		Size: 3.4 KB (3432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7363660f0290f9bf69f9ab50f5cffc179c5adc83a5540cf98b171237f816cf9c`  
		Last Modified: Tue, 06 Dec 2022 02:38:12 GMT  
		Size: 5.2 MB (5210587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d423be69a434de8ce0a40b5c1a09c920f45dff093382eb6ee57ee2f000feb3`  
		Last Modified: Tue, 06 Dec 2022 02:38:12 GMT  
		Size: 1.4 MB (1436872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e968973ab936bac3d8a1a603cd5e2610eab8338066238a66c2fb8bf561a783d0`  
		Last Modified: Tue, 06 Dec 2022 02:38:12 GMT  
		Size: 296.2 KB (296157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cb0772563c207436f69961c46ff4164931f8597263861f5552b1ee6d03679a`  
		Last Modified: Tue, 06 Dec 2022 02:38:11 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7e348c01e0f44562a3e0f4ee7ce7ca54478f014bfb250b87048be67cc6d560`  
		Last Modified: Tue, 06 Dec 2022 02:38:14 GMT  
		Size: 49.1 MB (49064819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f2e45be5bc4db8b1d6450de17e8f4f516dc7495720184856472fd43e9539f7`  
		Last Modified: Tue, 06 Dec 2022 02:38:10 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9796347789b28192a0f4425fc6bda42d858708e7628262250c191e5709a4fd9c`  
		Last Modified: Tue, 06 Dec 2022 02:38:10 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13768b759ebbcb8fba738a44e9895e1fa9a72f899587e0c60d8273b6ea59bc7`  
		Last Modified: Tue, 06 Dec 2022 02:38:10 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7526c3a368d90235506e6ccd9932bf1345ba9b39fe0e0c12eff0ca7d813c1560`  
		Last Modified: Tue, 06 Dec 2022 02:38:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2.2` - linux; ppc64le

```console
$ docker pull couchdb@sha256:c4d14a5a09618880cab6e3e8433192d8281e0e97346b7600fe82eb20867bd44d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93230341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49c2d3582f74ff15b8a063817e6cb657a7861160f88cbc16e1bacb2a4f494cee`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 06 Dec 2022 01:18:04 GMT
ADD file:2231a44ea52d93df58e23883ba6b6911d4c554f4c1d172d80fb21c751ddcbbfc in / 
# Tue, 06 Dec 2022 01:18:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:43:09 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 06 Dec 2022 01:43:11 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 06 Dec 2022 01:43:26 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 01:43:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 06 Dec 2022 01:43:33 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 06 Dec 2022 01:43:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 01:43:45 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 06 Dec 2022 01:43:47 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 06 Dec 2022 01:44:08 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 06 Dec 2022 01:44:10 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 06 Dec 2022 01:44:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 06 Dec 2022 01:44:11 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 06 Dec 2022 01:44:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 06 Dec 2022 01:44:12 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 01:44:13 GMT
VOLUME [/opt/couchdb/data]
# Tue, 06 Dec 2022 01:44:13 GMT
EXPOSE 4369 5984 9100
# Tue, 06 Dec 2022 01:44:14 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:1f72e1168976861c676bf86a6c149129baba7e13200e8b70e6f24dc2ac2797df`  
		Last Modified: Tue, 06 Dec 2022 01:24:18 GMT  
		Size: 35.3 MB (35285293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9651219ecb35e4178b548721d7d579b5bcad3527e218e212f22f49f1d0e737d`  
		Last Modified: Tue, 06 Dec 2022 01:44:37 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a6ae87d9066bfad2d47cacfb42b74ac3ea08ac23f95401d3ead11129b183e6`  
		Last Modified: Tue, 06 Dec 2022 01:44:37 GMT  
		Size: 6.0 MB (6045482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12bc23b90a71bd7b552b15d2eaebdada16d19778cb84909bcdf0a765b1c9e2c`  
		Last Modified: Tue, 06 Dec 2022 01:44:35 GMT  
		Size: 1.5 MB (1509788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b816512cc9ab4899e2488ff00e7575bcc5bf658ead8cfa8a385b8cdc2d69c89`  
		Last Modified: Tue, 06 Dec 2022 01:44:35 GMT  
		Size: 296.2 KB (296210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e052f116409b694b5f652845866ef6a296c7402a169355d9e101b62d4c4aa94`  
		Last Modified: Tue, 06 Dec 2022 01:44:35 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f424b3f99465a604107ba0d3286aebb6515a17c8d01c2b29a6ead5e6b46714`  
		Last Modified: Tue, 06 Dec 2022 01:44:42 GMT  
		Size: 50.1 MB (50086420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b0bb886f364f867efe9470c1cc85dcb481b9ab2b447cf42306ce8676d09dee`  
		Last Modified: Tue, 06 Dec 2022 01:44:33 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073409bf834d911edf2a2911adc4caef2428d48e577c9ae57fa86c4cb5c6eecb`  
		Last Modified: Tue, 06 Dec 2022 01:44:33 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7c8a9cef21a2d437cbb4d2236784a5d38e6bc56e563908c03f8a3cb10c66ce`  
		Last Modified: Tue, 06 Dec 2022 01:44:33 GMT  
		Size: 2.2 KB (2187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b3e69b9284e828a40354df4b63224c55b3b9413b6592e7e6659599846c75db`  
		Last Modified: Tue, 06 Dec 2022 01:44:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:latest`

```console
$ docker pull couchdb@sha256:b5a484405703078f9a58dea9dccea077d322664e0b9ed6fc1114a8d467f9a8fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:08c8be9a9c54a3fcbf7b689830194cb86bd55e7a59a815fbf2d49e35e76b05d9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87543235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6911a540dd968fe1478b9b500798b164794007387923521be46eb47d99587af`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 08:21:13 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 06 Dec 2022 08:21:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 06 Dec 2022 08:21:22 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:21:26 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 06 Dec 2022 08:21:27 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 06 Dec 2022 08:21:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 08:21:33 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 06 Dec 2022 08:21:33 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 06 Dec 2022 08:21:47 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 06 Dec 2022 08:21:48 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 06 Dec 2022 08:21:48 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 06 Dec 2022 08:21:48 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 06 Dec 2022 08:21:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 06 Dec 2022 08:21:49 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 08:21:49 GMT
VOLUME [/opt/couchdb/data]
# Tue, 06 Dec 2022 08:21:49 GMT
EXPOSE 4369 5984 9100
# Tue, 06 Dec 2022 08:21:49 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bb4afed80e312afc90dddaaa6438df3533f5daa49acff45c16bba875251a01`  
		Last Modified: Tue, 06 Dec 2022 08:23:16 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e491958ff0bf330c113b1f2d36b2c3ece5c47136459694026bb2faa633be728`  
		Last Modified: Tue, 06 Dec 2022 08:23:15 GMT  
		Size: 5.2 MB (5225850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32f9e1cbb5588db7768285bcef98b51da711d331fa72cdd76bfdec18c2b92eb`  
		Last Modified: Tue, 06 Dec 2022 08:23:15 GMT  
		Size: 1.6 MB (1554049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49a082bebdadf80f5cbadefe1fe8fbe52bcc5029c60aeb47fa360be09abc7e5`  
		Last Modified: Tue, 06 Dec 2022 08:23:14 GMT  
		Size: 296.2 KB (296245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e51747b2e733242116d083778cd840dcc9bf2bd7dec710e119be0e46b6e7a89`  
		Last Modified: Tue, 06 Dec 2022 08:23:14 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c3e92a00a7166bf855a2de1f49ab13db229fe44ce43d9096e8f5341b0ec63c`  
		Last Modified: Tue, 06 Dec 2022 08:23:18 GMT  
		Size: 49.0 MB (49047099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9712f2bedab91689d069dcccc1abebfec2bd434e31470ffa53320d53d63294ab`  
		Last Modified: Tue, 06 Dec 2022 08:23:12 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611b5c5f7df92186e277a7c8fb0176c096ae2387abc8f59dabb26fdc2c0f5d3d`  
		Last Modified: Tue, 06 Dec 2022 08:23:12 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7597f2951735385cabea4989eb4b64fbebf06f263b0415f25087abb3c60483`  
		Last Modified: Tue, 06 Dec 2022 08:23:12 GMT  
		Size: 2.2 KB (2188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4f7c3dccc96eb7750187013bcc169daea36abcfd143fd4e275d1046c9aa301`  
		Last Modified: Tue, 06 Dec 2022 08:23:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:01018d93a18c79773dd7bbe769325e38d19ba48c318ccfc2ef441d8ad7b61d5e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.1 MB (86075918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cead15cfe5d467c356162256c209623d5d5982246c130d1147be026e05ef98c0`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:36:34 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 06 Dec 2022 02:36:35 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 06 Dec 2022 02:36:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:36:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 06 Dec 2022 02:36:44 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 06 Dec 2022 02:36:48 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:36:48 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 06 Dec 2022 02:36:49 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 06 Dec 2022 02:37:00 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 06 Dec 2022 02:37:00 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 06 Dec 2022 02:37:00 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 06 Dec 2022 02:37:00 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 06 Dec 2022 02:37:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 06 Dec 2022 02:37:01 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 02:37:01 GMT
VOLUME [/opt/couchdb/data]
# Tue, 06 Dec 2022 02:37:01 GMT
EXPOSE 4369 5984 9100
# Tue, 06 Dec 2022 02:37:01 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52978b09e2554ffbd028007d31a4a2833c7a8cfe23376f79ad433f0a0f467b04`  
		Last Modified: Tue, 06 Dec 2022 02:38:13 GMT  
		Size: 3.4 KB (3432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7363660f0290f9bf69f9ab50f5cffc179c5adc83a5540cf98b171237f816cf9c`  
		Last Modified: Tue, 06 Dec 2022 02:38:12 GMT  
		Size: 5.2 MB (5210587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d423be69a434de8ce0a40b5c1a09c920f45dff093382eb6ee57ee2f000feb3`  
		Last Modified: Tue, 06 Dec 2022 02:38:12 GMT  
		Size: 1.4 MB (1436872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e968973ab936bac3d8a1a603cd5e2610eab8338066238a66c2fb8bf561a783d0`  
		Last Modified: Tue, 06 Dec 2022 02:38:12 GMT  
		Size: 296.2 KB (296157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cb0772563c207436f69961c46ff4164931f8597263861f5552b1ee6d03679a`  
		Last Modified: Tue, 06 Dec 2022 02:38:11 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7e348c01e0f44562a3e0f4ee7ce7ca54478f014bfb250b87048be67cc6d560`  
		Last Modified: Tue, 06 Dec 2022 02:38:14 GMT  
		Size: 49.1 MB (49064819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f2e45be5bc4db8b1d6450de17e8f4f516dc7495720184856472fd43e9539f7`  
		Last Modified: Tue, 06 Dec 2022 02:38:10 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9796347789b28192a0f4425fc6bda42d858708e7628262250c191e5709a4fd9c`  
		Last Modified: Tue, 06 Dec 2022 02:38:10 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13768b759ebbcb8fba738a44e9895e1fa9a72f899587e0c60d8273b6ea59bc7`  
		Last Modified: Tue, 06 Dec 2022 02:38:10 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7526c3a368d90235506e6ccd9932bf1345ba9b39fe0e0c12eff0ca7d813c1560`  
		Last Modified: Tue, 06 Dec 2022 02:38:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; ppc64le

```console
$ docker pull couchdb@sha256:c4d14a5a09618880cab6e3e8433192d8281e0e97346b7600fe82eb20867bd44d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93230341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49c2d3582f74ff15b8a063817e6cb657a7861160f88cbc16e1bacb2a4f494cee`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 06 Dec 2022 01:18:04 GMT
ADD file:2231a44ea52d93df58e23883ba6b6911d4c554f4c1d172d80fb21c751ddcbbfc in / 
# Tue, 06 Dec 2022 01:18:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:43:09 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 06 Dec 2022 01:43:11 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 06 Dec 2022 01:43:26 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 01:43:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 06 Dec 2022 01:43:33 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 06 Dec 2022 01:43:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 01:43:45 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 06 Dec 2022 01:43:47 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 06 Dec 2022 01:44:08 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 06 Dec 2022 01:44:10 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 06 Dec 2022 01:44:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 06 Dec 2022 01:44:11 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 06 Dec 2022 01:44:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 06 Dec 2022 01:44:12 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 01:44:13 GMT
VOLUME [/opt/couchdb/data]
# Tue, 06 Dec 2022 01:44:13 GMT
EXPOSE 4369 5984 9100
# Tue, 06 Dec 2022 01:44:14 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:1f72e1168976861c676bf86a6c149129baba7e13200e8b70e6f24dc2ac2797df`  
		Last Modified: Tue, 06 Dec 2022 01:24:18 GMT  
		Size: 35.3 MB (35285293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9651219ecb35e4178b548721d7d579b5bcad3527e218e212f22f49f1d0e737d`  
		Last Modified: Tue, 06 Dec 2022 01:44:37 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a6ae87d9066bfad2d47cacfb42b74ac3ea08ac23f95401d3ead11129b183e6`  
		Last Modified: Tue, 06 Dec 2022 01:44:37 GMT  
		Size: 6.0 MB (6045482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12bc23b90a71bd7b552b15d2eaebdada16d19778cb84909bcdf0a765b1c9e2c`  
		Last Modified: Tue, 06 Dec 2022 01:44:35 GMT  
		Size: 1.5 MB (1509788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b816512cc9ab4899e2488ff00e7575bcc5bf658ead8cfa8a385b8cdc2d69c89`  
		Last Modified: Tue, 06 Dec 2022 01:44:35 GMT  
		Size: 296.2 KB (296210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e052f116409b694b5f652845866ef6a296c7402a169355d9e101b62d4c4aa94`  
		Last Modified: Tue, 06 Dec 2022 01:44:35 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f424b3f99465a604107ba0d3286aebb6515a17c8d01c2b29a6ead5e6b46714`  
		Last Modified: Tue, 06 Dec 2022 01:44:42 GMT  
		Size: 50.1 MB (50086420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b0bb886f364f867efe9470c1cc85dcb481b9ab2b447cf42306ce8676d09dee`  
		Last Modified: Tue, 06 Dec 2022 01:44:33 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073409bf834d911edf2a2911adc4caef2428d48e577c9ae57fa86c4cb5c6eecb`  
		Last Modified: Tue, 06 Dec 2022 01:44:33 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7c8a9cef21a2d437cbb4d2236784a5d38e6bc56e563908c03f8a3cb10c66ce`  
		Last Modified: Tue, 06 Dec 2022 01:44:33 GMT  
		Size: 2.2 KB (2187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b3e69b9284e828a40354df4b63224c55b3b9413b6592e7e6659599846c75db`  
		Last Modified: Tue, 06 Dec 2022 01:44:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
