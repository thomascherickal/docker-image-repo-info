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
$ docker pull couchdb@sha256:97c711f7313ed00b4d46ac443394b29e7230e28b2fbf15865e8b6075b1ffb50d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2` - linux; amd64

```console
$ docker pull couchdb@sha256:8006d6b3ab8dbeb7febd3d8c4e2fe20becabc2b76004b8971cae7baf662b5d6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84536850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8eafd61aa02e58606cc4d9ae673a4791ee1dc55827a09d1cf771fdcfbd8c20d8`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 15 Nov 2022 04:05:14 GMT
ADD file:9461639b945ced6fb6164491a7e0131261a1b7d69264cce516e75c71e4df22d2 in / 
# Tue, 15 Nov 2022 04:05:14 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:35:54 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 15 Nov 2022 10:35:55 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 15 Nov 2022 10:36:02 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:36:07 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 15 Nov 2022 10:36:07 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 15 Nov 2022 10:36:14 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:36:35 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 15 Nov 2022 10:36:35 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 15 Nov 2022 10:36:53 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 15 Nov 2022 10:36:54 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 15 Nov 2022 10:36:54 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 15 Nov 2022 10:36:54 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 15 Nov 2022 10:36:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 15 Nov 2022 10:36:55 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 10:36:55 GMT
VOLUME [/opt/couchdb/data]
# Tue, 15 Nov 2022 10:36:55 GMT
EXPOSE 4369 5984 9100
# Tue, 15 Nov 2022 10:36:55 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:32820e52a00eb22dc76d70d992be7082cd24b636cfb597ff3951d29a821b46b9`  
		Last Modified: Tue, 15 Nov 2022 04:09:26 GMT  
		Size: 27.1 MB (27140332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8b386cb12f04cd6f9c67d0c0373d9ba78bbf5fa84562a9898904f6f17805b2`  
		Last Modified: Tue, 15 Nov 2022 10:37:34 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df26f4bfe01cd6f4dfe22fc28ece77009b0f36ab15a099aa5ba5826aa10129e`  
		Last Modified: Tue, 15 Nov 2022 10:37:34 GMT  
		Size: 6.7 MB (6703723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5d10938ed357b3e2264066bfe9e4b3cbed1cca64738d2b4ab40051bc2b5397`  
		Last Modified: Tue, 15 Nov 2022 10:37:33 GMT  
		Size: 1.3 MB (1259579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42738d31e487788abf984684c20e8dfe4d73946b80c79f2d6762693c90f8926c`  
		Last Modified: Tue, 15 Nov 2022 10:37:33 GMT  
		Size: 294.3 KB (294312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58f08cba2d555333f3423e270975b0d1f1128f9849657ed90804899ba735e68`  
		Last Modified: Tue, 15 Nov 2022 10:37:47 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6497056118fcc1be2a38eedb78d8bfd8adf80c94ace4308f833d670752d1026`  
		Last Modified: Tue, 15 Nov 2022 10:37:51 GMT  
		Size: 49.1 MB (49131884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6677a2a06178d126abd08688b890e9b170de7e6f7ae43fd7e6d19aa6b2f72fac`  
		Last Modified: Tue, 15 Nov 2022 10:37:45 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc71e04926fd08a75ccf8c8737aeb4b0890c56741f2517556883f718d3e438f8`  
		Last Modified: Tue, 15 Nov 2022 10:37:45 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c359198d0d373ec3be93920dbaf92373a9c45d857d86cefeab64245ee6aeedab`  
		Last Modified: Tue, 15 Nov 2022 10:37:45 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4280f4fa73e5058630c094d6c2afdc21941ff86c16b4a759d40e990d8c4f2b4b`  
		Last Modified: Tue, 15 Nov 2022 10:37:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:9f307fa651f324e321e9c10d043e219353a113607cc7666d9146d0ee05f53d1c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72987738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:855bd9e057ab058b2ed7e1c1dd230c5d17809363ac11fffe5a697407bbd1d3c4`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:34 GMT
ADD file:aaead8e4dd08d41c8d1692bbe76b673119289836428e1f713ca550c2468711ac in / 
# Tue, 15 Nov 2022 01:41:34 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 06:08:41 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 15 Nov 2022 06:08:42 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 15 Nov 2022 06:08:48 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 06:08:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 15 Nov 2022 06:08:52 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 15 Nov 2022 06:08:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 06:09:15 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 15 Nov 2022 06:09:15 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 15 Nov 2022 06:09:26 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 15 Nov 2022 06:09:27 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 15 Nov 2022 06:09:27 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 15 Nov 2022 06:09:27 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 15 Nov 2022 06:09:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 15 Nov 2022 06:09:27 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 06:09:27 GMT
VOLUME [/opt/couchdb/data]
# Tue, 15 Nov 2022 06:09:27 GMT
EXPOSE 4369 5984 9100
# Tue, 15 Nov 2022 06:09:27 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:cc457132e077d684a6cecad3331c35341d814c5d364f3cf24d698a6d8e76d0e7`  
		Last Modified: Tue, 15 Nov 2022 01:45:13 GMT  
		Size: 25.9 MB (25914924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510e02d58fa2dbfebc3aa5cfabf2a30c7b284888399969b4ca2ee82e466cf088`  
		Last Modified: Tue, 15 Nov 2022 06:10:18 GMT  
		Size: 3.4 KB (3436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ebeecce1b4027a2486f99101198a916d89cdf12eead09d3ba2783466915604`  
		Last Modified: Tue, 15 Nov 2022 06:10:16 GMT  
		Size: 6.6 MB (6577064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9d360df926f74081761ca41bff2e01aee885becd0213001d61839f3bc0158f`  
		Last Modified: Tue, 15 Nov 2022 06:10:15 GMT  
		Size: 1.2 MB (1164513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f743716d719aed881a6a611d2d969baec0c3e94ff6974d284c9e7a57b541fd84`  
		Last Modified: Tue, 15 Nov 2022 06:10:16 GMT  
		Size: 294.2 KB (294180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd9e350ef9f8feb04d51c27d8f2636e71a575635ea83ae8b61f4b688815340b`  
		Last Modified: Tue, 15 Nov 2022 06:10:35 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880e3352d5251a74334f500a7294c4cd10108e345015b9a1688ee3ae102688f3`  
		Last Modified: Tue, 15 Nov 2022 06:10:36 GMT  
		Size: 39.0 MB (39030020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f533504f2c59ef0e5e9a1088b9af375337605049ff15586729086f5aad3b1807`  
		Last Modified: Tue, 15 Nov 2022 06:10:32 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8411bc9f8002c7fea3c38fecd8ea2ab50bd6c27e8f84a511e1251409d9878830`  
		Last Modified: Tue, 15 Nov 2022 06:10:32 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d5beaf61f99cbd4da12db29664319e00de112c2dad856aaaac2d4d8df3f52f`  
		Last Modified: Tue, 15 Nov 2022 06:10:32 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa55ce56adb4fffb9a288ce4588a071bd038c76d32b38d6ff260febb6305e35`  
		Last Modified: Tue, 15 Nov 2022 06:10:32 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3`

```console
$ docker pull couchdb@sha256:97c711f7313ed00b4d46ac443394b29e7230e28b2fbf15865e8b6075b1ffb50d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:8006d6b3ab8dbeb7febd3d8c4e2fe20becabc2b76004b8971cae7baf662b5d6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84536850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8eafd61aa02e58606cc4d9ae673a4791ee1dc55827a09d1cf771fdcfbd8c20d8`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 15 Nov 2022 04:05:14 GMT
ADD file:9461639b945ced6fb6164491a7e0131261a1b7d69264cce516e75c71e4df22d2 in / 
# Tue, 15 Nov 2022 04:05:14 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:35:54 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 15 Nov 2022 10:35:55 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 15 Nov 2022 10:36:02 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:36:07 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 15 Nov 2022 10:36:07 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 15 Nov 2022 10:36:14 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:36:35 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 15 Nov 2022 10:36:35 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 15 Nov 2022 10:36:53 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 15 Nov 2022 10:36:54 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 15 Nov 2022 10:36:54 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 15 Nov 2022 10:36:54 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 15 Nov 2022 10:36:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 15 Nov 2022 10:36:55 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 10:36:55 GMT
VOLUME [/opt/couchdb/data]
# Tue, 15 Nov 2022 10:36:55 GMT
EXPOSE 4369 5984 9100
# Tue, 15 Nov 2022 10:36:55 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:32820e52a00eb22dc76d70d992be7082cd24b636cfb597ff3951d29a821b46b9`  
		Last Modified: Tue, 15 Nov 2022 04:09:26 GMT  
		Size: 27.1 MB (27140332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8b386cb12f04cd6f9c67d0c0373d9ba78bbf5fa84562a9898904f6f17805b2`  
		Last Modified: Tue, 15 Nov 2022 10:37:34 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df26f4bfe01cd6f4dfe22fc28ece77009b0f36ab15a099aa5ba5826aa10129e`  
		Last Modified: Tue, 15 Nov 2022 10:37:34 GMT  
		Size: 6.7 MB (6703723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5d10938ed357b3e2264066bfe9e4b3cbed1cca64738d2b4ab40051bc2b5397`  
		Last Modified: Tue, 15 Nov 2022 10:37:33 GMT  
		Size: 1.3 MB (1259579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42738d31e487788abf984684c20e8dfe4d73946b80c79f2d6762693c90f8926c`  
		Last Modified: Tue, 15 Nov 2022 10:37:33 GMT  
		Size: 294.3 KB (294312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58f08cba2d555333f3423e270975b0d1f1128f9849657ed90804899ba735e68`  
		Last Modified: Tue, 15 Nov 2022 10:37:47 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6497056118fcc1be2a38eedb78d8bfd8adf80c94ace4308f833d670752d1026`  
		Last Modified: Tue, 15 Nov 2022 10:37:51 GMT  
		Size: 49.1 MB (49131884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6677a2a06178d126abd08688b890e9b170de7e6f7ae43fd7e6d19aa6b2f72fac`  
		Last Modified: Tue, 15 Nov 2022 10:37:45 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc71e04926fd08a75ccf8c8737aeb4b0890c56741f2517556883f718d3e438f8`  
		Last Modified: Tue, 15 Nov 2022 10:37:45 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c359198d0d373ec3be93920dbaf92373a9c45d857d86cefeab64245ee6aeedab`  
		Last Modified: Tue, 15 Nov 2022 10:37:45 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4280f4fa73e5058630c094d6c2afdc21941ff86c16b4a759d40e990d8c4f2b4b`  
		Last Modified: Tue, 15 Nov 2022 10:37:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:9f307fa651f324e321e9c10d043e219353a113607cc7666d9146d0ee05f53d1c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72987738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:855bd9e057ab058b2ed7e1c1dd230c5d17809363ac11fffe5a697407bbd1d3c4`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:34 GMT
ADD file:aaead8e4dd08d41c8d1692bbe76b673119289836428e1f713ca550c2468711ac in / 
# Tue, 15 Nov 2022 01:41:34 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 06:08:41 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 15 Nov 2022 06:08:42 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 15 Nov 2022 06:08:48 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 06:08:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 15 Nov 2022 06:08:52 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 15 Nov 2022 06:08:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 06:09:15 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 15 Nov 2022 06:09:15 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 15 Nov 2022 06:09:26 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 15 Nov 2022 06:09:27 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 15 Nov 2022 06:09:27 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 15 Nov 2022 06:09:27 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 15 Nov 2022 06:09:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 15 Nov 2022 06:09:27 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 06:09:27 GMT
VOLUME [/opt/couchdb/data]
# Tue, 15 Nov 2022 06:09:27 GMT
EXPOSE 4369 5984 9100
# Tue, 15 Nov 2022 06:09:27 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:cc457132e077d684a6cecad3331c35341d814c5d364f3cf24d698a6d8e76d0e7`  
		Last Modified: Tue, 15 Nov 2022 01:45:13 GMT  
		Size: 25.9 MB (25914924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510e02d58fa2dbfebc3aa5cfabf2a30c7b284888399969b4ca2ee82e466cf088`  
		Last Modified: Tue, 15 Nov 2022 06:10:18 GMT  
		Size: 3.4 KB (3436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ebeecce1b4027a2486f99101198a916d89cdf12eead09d3ba2783466915604`  
		Last Modified: Tue, 15 Nov 2022 06:10:16 GMT  
		Size: 6.6 MB (6577064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9d360df926f74081761ca41bff2e01aee885becd0213001d61839f3bc0158f`  
		Last Modified: Tue, 15 Nov 2022 06:10:15 GMT  
		Size: 1.2 MB (1164513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f743716d719aed881a6a611d2d969baec0c3e94ff6974d284c9e7a57b541fd84`  
		Last Modified: Tue, 15 Nov 2022 06:10:16 GMT  
		Size: 294.2 KB (294180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd9e350ef9f8feb04d51c27d8f2636e71a575635ea83ae8b61f4b688815340b`  
		Last Modified: Tue, 15 Nov 2022 06:10:35 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880e3352d5251a74334f500a7294c4cd10108e345015b9a1688ee3ae102688f3`  
		Last Modified: Tue, 15 Nov 2022 06:10:36 GMT  
		Size: 39.0 MB (39030020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f533504f2c59ef0e5e9a1088b9af375337605049ff15586729086f5aad3b1807`  
		Last Modified: Tue, 15 Nov 2022 06:10:32 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8411bc9f8002c7fea3c38fecd8ea2ab50bd6c27e8f84a511e1251409d9878830`  
		Last Modified: Tue, 15 Nov 2022 06:10:32 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d5beaf61f99cbd4da12db29664319e00de112c2dad856aaaac2d4d8df3f52f`  
		Last Modified: Tue, 15 Nov 2022 06:10:32 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa55ce56adb4fffb9a288ce4588a071bd038c76d32b38d6ff260febb6305e35`  
		Last Modified: Tue, 15 Nov 2022 06:10:32 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3.1`

```console
$ docker pull couchdb@sha256:97c711f7313ed00b4d46ac443394b29e7230e28b2fbf15865e8b6075b1ffb50d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:8006d6b3ab8dbeb7febd3d8c4e2fe20becabc2b76004b8971cae7baf662b5d6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84536850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8eafd61aa02e58606cc4d9ae673a4791ee1dc55827a09d1cf771fdcfbd8c20d8`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 15 Nov 2022 04:05:14 GMT
ADD file:9461639b945ced6fb6164491a7e0131261a1b7d69264cce516e75c71e4df22d2 in / 
# Tue, 15 Nov 2022 04:05:14 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:35:54 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 15 Nov 2022 10:35:55 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 15 Nov 2022 10:36:02 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:36:07 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 15 Nov 2022 10:36:07 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 15 Nov 2022 10:36:14 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:36:35 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 15 Nov 2022 10:36:35 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 15 Nov 2022 10:36:53 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 15 Nov 2022 10:36:54 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 15 Nov 2022 10:36:54 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 15 Nov 2022 10:36:54 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 15 Nov 2022 10:36:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 15 Nov 2022 10:36:55 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 10:36:55 GMT
VOLUME [/opt/couchdb/data]
# Tue, 15 Nov 2022 10:36:55 GMT
EXPOSE 4369 5984 9100
# Tue, 15 Nov 2022 10:36:55 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:32820e52a00eb22dc76d70d992be7082cd24b636cfb597ff3951d29a821b46b9`  
		Last Modified: Tue, 15 Nov 2022 04:09:26 GMT  
		Size: 27.1 MB (27140332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8b386cb12f04cd6f9c67d0c0373d9ba78bbf5fa84562a9898904f6f17805b2`  
		Last Modified: Tue, 15 Nov 2022 10:37:34 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df26f4bfe01cd6f4dfe22fc28ece77009b0f36ab15a099aa5ba5826aa10129e`  
		Last Modified: Tue, 15 Nov 2022 10:37:34 GMT  
		Size: 6.7 MB (6703723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5d10938ed357b3e2264066bfe9e4b3cbed1cca64738d2b4ab40051bc2b5397`  
		Last Modified: Tue, 15 Nov 2022 10:37:33 GMT  
		Size: 1.3 MB (1259579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42738d31e487788abf984684c20e8dfe4d73946b80c79f2d6762693c90f8926c`  
		Last Modified: Tue, 15 Nov 2022 10:37:33 GMT  
		Size: 294.3 KB (294312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58f08cba2d555333f3423e270975b0d1f1128f9849657ed90804899ba735e68`  
		Last Modified: Tue, 15 Nov 2022 10:37:47 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6497056118fcc1be2a38eedb78d8bfd8adf80c94ace4308f833d670752d1026`  
		Last Modified: Tue, 15 Nov 2022 10:37:51 GMT  
		Size: 49.1 MB (49131884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6677a2a06178d126abd08688b890e9b170de7e6f7ae43fd7e6d19aa6b2f72fac`  
		Last Modified: Tue, 15 Nov 2022 10:37:45 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc71e04926fd08a75ccf8c8737aeb4b0890c56741f2517556883f718d3e438f8`  
		Last Modified: Tue, 15 Nov 2022 10:37:45 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c359198d0d373ec3be93920dbaf92373a9c45d857d86cefeab64245ee6aeedab`  
		Last Modified: Tue, 15 Nov 2022 10:37:45 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4280f4fa73e5058630c094d6c2afdc21941ff86c16b4a759d40e990d8c4f2b4b`  
		Last Modified: Tue, 15 Nov 2022 10:37:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:9f307fa651f324e321e9c10d043e219353a113607cc7666d9146d0ee05f53d1c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72987738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:855bd9e057ab058b2ed7e1c1dd230c5d17809363ac11fffe5a697407bbd1d3c4`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:34 GMT
ADD file:aaead8e4dd08d41c8d1692bbe76b673119289836428e1f713ca550c2468711ac in / 
# Tue, 15 Nov 2022 01:41:34 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 06:08:41 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 15 Nov 2022 06:08:42 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 15 Nov 2022 06:08:48 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 06:08:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 15 Nov 2022 06:08:52 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 15 Nov 2022 06:08:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 06:09:15 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 15 Nov 2022 06:09:15 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 15 Nov 2022 06:09:26 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 15 Nov 2022 06:09:27 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 15 Nov 2022 06:09:27 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 15 Nov 2022 06:09:27 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 15 Nov 2022 06:09:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 15 Nov 2022 06:09:27 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 06:09:27 GMT
VOLUME [/opt/couchdb/data]
# Tue, 15 Nov 2022 06:09:27 GMT
EXPOSE 4369 5984 9100
# Tue, 15 Nov 2022 06:09:27 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:cc457132e077d684a6cecad3331c35341d814c5d364f3cf24d698a6d8e76d0e7`  
		Last Modified: Tue, 15 Nov 2022 01:45:13 GMT  
		Size: 25.9 MB (25914924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510e02d58fa2dbfebc3aa5cfabf2a30c7b284888399969b4ca2ee82e466cf088`  
		Last Modified: Tue, 15 Nov 2022 06:10:18 GMT  
		Size: 3.4 KB (3436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ebeecce1b4027a2486f99101198a916d89cdf12eead09d3ba2783466915604`  
		Last Modified: Tue, 15 Nov 2022 06:10:16 GMT  
		Size: 6.6 MB (6577064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9d360df926f74081761ca41bff2e01aee885becd0213001d61839f3bc0158f`  
		Last Modified: Tue, 15 Nov 2022 06:10:15 GMT  
		Size: 1.2 MB (1164513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f743716d719aed881a6a611d2d969baec0c3e94ff6974d284c9e7a57b541fd84`  
		Last Modified: Tue, 15 Nov 2022 06:10:16 GMT  
		Size: 294.2 KB (294180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd9e350ef9f8feb04d51c27d8f2636e71a575635ea83ae8b61f4b688815340b`  
		Last Modified: Tue, 15 Nov 2022 06:10:35 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880e3352d5251a74334f500a7294c4cd10108e345015b9a1688ee3ae102688f3`  
		Last Modified: Tue, 15 Nov 2022 06:10:36 GMT  
		Size: 39.0 MB (39030020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f533504f2c59ef0e5e9a1088b9af375337605049ff15586729086f5aad3b1807`  
		Last Modified: Tue, 15 Nov 2022 06:10:32 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8411bc9f8002c7fea3c38fecd8ea2ab50bd6c27e8f84a511e1251409d9878830`  
		Last Modified: Tue, 15 Nov 2022 06:10:32 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d5beaf61f99cbd4da12db29664319e00de112c2dad856aaaac2d4d8df3f52f`  
		Last Modified: Tue, 15 Nov 2022 06:10:32 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa55ce56adb4fffb9a288ce4588a071bd038c76d32b38d6ff260febb6305e35`  
		Last Modified: Tue, 15 Nov 2022 06:10:32 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3`

```console
$ docker pull couchdb@sha256:d3346c205f96be4ce36c245ff08e44331115437ff8760cccb685df64e4470434
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3` - linux; amd64

```console
$ docker pull couchdb@sha256:18b447eb4aa7371763ad1e65fb21b89e867e4e38fbaf87340e401c0d2b48672d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87542993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86d51a034b33057b01caf54d400a6f527ce26b7894ee8d93ea5e8c478307c77e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:35:14 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 15 Nov 2022 10:35:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 15 Nov 2022 10:35:22 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:35:26 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 15 Nov 2022 10:35:26 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 15 Nov 2022 10:35:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:35:32 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 15 Nov 2022 10:35:33 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 15 Nov 2022 10:35:46 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 15 Nov 2022 10:35:47 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 15 Nov 2022 10:35:47 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 15 Nov 2022 10:35:47 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 15 Nov 2022 10:35:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 15 Nov 2022 10:35:48 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 10:35:48 GMT
VOLUME [/opt/couchdb/data]
# Tue, 15 Nov 2022 10:35:48 GMT
EXPOSE 4369 5984 9100
# Tue, 15 Nov 2022 10:35:48 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ac309e879645bf78b5b51a81163cbbaec1a07acab50160803d720a2cd20faa`  
		Last Modified: Tue, 15 Nov 2022 10:37:15 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49844afe089a8ae2b28167131e091ee4187c088c6a872e9325c1d31958cb820e`  
		Last Modified: Tue, 15 Nov 2022 10:37:14 GMT  
		Size: 5.2 MB (5225827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8627dd11a7afca5ddbc0d10ad202fc8c0cc3f7b4e616c5aa496ece15c69c41`  
		Last Modified: Tue, 15 Nov 2022 10:37:13 GMT  
		Size: 1.6 MB (1554043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74501422620a7da2c637583baba5da1d30f26f6914e9904901fe2d1fbcbd0e76`  
		Last Modified: Tue, 15 Nov 2022 10:37:13 GMT  
		Size: 296.3 KB (296279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36940d23f9815532c5e6f5ac48eac39ee6851584fad38d584af6e2d7e08868f8`  
		Last Modified: Tue, 15 Nov 2022 10:37:13 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc41a6e08f50ee957aa8bbdc82b5d63ec2c6070b39131eb7294753615a8a4525`  
		Last Modified: Tue, 15 Nov 2022 10:37:16 GMT  
		Size: 49.0 MB (49047070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64abb1d4412cba2191e7a32e467c78dcc0dc5f66248b85909e2585fcf9da9e6e`  
		Last Modified: Tue, 15 Nov 2022 10:37:11 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c470c6cf30f98b8c7dedcfbb51c7d3b31e28b9b4b054fc28defbc4b849a7c24d`  
		Last Modified: Tue, 15 Nov 2022 10:37:11 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28986f7c1a1bb4a3100d2af60b12e1819fff375e5ffd528ef2e948d4d9606a6b`  
		Last Modified: Tue, 15 Nov 2022 10:37:11 GMT  
		Size: 2.2 KB (2188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2411adc92296964132673b2cbd12ace5e926c6baf3d7f381e7475258440563`  
		Last Modified: Tue, 15 Nov 2022 10:37:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; arm64 variant v8

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
$ docker pull couchdb@sha256:f3a5561153cdd2d8117866feac97c07520e92412a49ec2d4667fb8ee8174ae45
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:7b39bd5a1e42135efafa5b969fe7fdaba5a9635f8aa62b96a3493ec3c7a292a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80023492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53cc4782ab9377854f055bcc9e7ad0b040794ca4a8c898742bfcd5fa9a818bfc`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 15 Nov 2022 04:05:14 GMT
ADD file:9461639b945ced6fb6164491a7e0131261a1b7d69264cce516e75c71e4df22d2 in / 
# Tue, 15 Nov 2022 04:05:14 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:35:54 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 15 Nov 2022 10:35:55 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 15 Nov 2022 10:36:02 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:36:07 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 15 Nov 2022 10:36:07 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 15 Nov 2022 10:36:14 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:36:14 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 15 Nov 2022 10:36:15 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 15 Nov 2022 10:36:29 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 15 Nov 2022 10:36:29 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 15 Nov 2022 10:36:29 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 15 Nov 2022 10:36:30 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 15 Nov 2022 10:36:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 15 Nov 2022 10:36:30 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 10:36:30 GMT
VOLUME [/opt/couchdb/data]
# Tue, 15 Nov 2022 10:36:30 GMT
EXPOSE 4369 5984 9100
# Tue, 15 Nov 2022 10:36:31 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:32820e52a00eb22dc76d70d992be7082cd24b636cfb597ff3951d29a821b46b9`  
		Last Modified: Tue, 15 Nov 2022 04:09:26 GMT  
		Size: 27.1 MB (27140332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8b386cb12f04cd6f9c67d0c0373d9ba78bbf5fa84562a9898904f6f17805b2`  
		Last Modified: Tue, 15 Nov 2022 10:37:34 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df26f4bfe01cd6f4dfe22fc28ece77009b0f36ab15a099aa5ba5826aa10129e`  
		Last Modified: Tue, 15 Nov 2022 10:37:34 GMT  
		Size: 6.7 MB (6703723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5d10938ed357b3e2264066bfe9e4b3cbed1cca64738d2b4ab40051bc2b5397`  
		Last Modified: Tue, 15 Nov 2022 10:37:33 GMT  
		Size: 1.3 MB (1259579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42738d31e487788abf984684c20e8dfe4d73946b80c79f2d6762693c90f8926c`  
		Last Modified: Tue, 15 Nov 2022 10:37:33 GMT  
		Size: 294.3 KB (294312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c8fff565fab486613ac3d15b45bb312a702ff6f222a903dc7c5a6d6d98a0f9`  
		Last Modified: Tue, 15 Nov 2022 10:37:32 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62f66cee9b45db68f6b1cb887d7695c071fb29957e72744957cc9950fc51ec2`  
		Last Modified: Tue, 15 Nov 2022 10:37:36 GMT  
		Size: 44.6 MB (44618537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2354cbf0561fe5f84c7fd90faceab75e1c44c1225c4939ef7685f9454c20d849`  
		Last Modified: Tue, 15 Nov 2022 10:37:30 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4e08c3ee4175a8be3ca54cbb71de31fe256a801ee8b33550a1295c6ccc439f`  
		Last Modified: Tue, 15 Nov 2022 10:37:30 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100dc05f176c141aa69c4fec8dd543cea1b1683e9d69604e618e0976fdc7adec`  
		Last Modified: Tue, 15 Nov 2022 10:37:31 GMT  
		Size: 2.1 KB (2056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14542c43a715195d747204fa11753b7a248b105b452c9f01e02d36bb2b7fc24`  
		Last Modified: Tue, 15 Nov 2022 10:37:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:930c9f1531c2cc9c937d00a8cc5fb46a227d32e406730d7111e1ed5500eb08e2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75079535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f12d0a699ab20ac1dba8aaf2ae74a73a88500be0b6d22048d08112ffb5095a7`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:34 GMT
ADD file:aaead8e4dd08d41c8d1692bbe76b673119289836428e1f713ca550c2468711ac in / 
# Tue, 15 Nov 2022 01:41:34 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 06:08:41 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 15 Nov 2022 06:08:42 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 15 Nov 2022 06:08:48 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 06:08:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 15 Nov 2022 06:08:52 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 15 Nov 2022 06:08:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 06:08:58 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 15 Nov 2022 06:08:58 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 15 Nov 2022 06:09:09 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 15 Nov 2022 06:09:10 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 15 Nov 2022 06:09:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 15 Nov 2022 06:09:10 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 15 Nov 2022 06:09:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 15 Nov 2022 06:09:10 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 06:09:10 GMT
VOLUME [/opt/couchdb/data]
# Tue, 15 Nov 2022 06:09:10 GMT
EXPOSE 4369 5984 9100
# Tue, 15 Nov 2022 06:09:11 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:cc457132e077d684a6cecad3331c35341d814c5d364f3cf24d698a6d8e76d0e7`  
		Last Modified: Tue, 15 Nov 2022 01:45:13 GMT  
		Size: 25.9 MB (25914924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510e02d58fa2dbfebc3aa5cfabf2a30c7b284888399969b4ca2ee82e466cf088`  
		Last Modified: Tue, 15 Nov 2022 06:10:18 GMT  
		Size: 3.4 KB (3436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ebeecce1b4027a2486f99101198a916d89cdf12eead09d3ba2783466915604`  
		Last Modified: Tue, 15 Nov 2022 06:10:16 GMT  
		Size: 6.6 MB (6577064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9d360df926f74081761ca41bff2e01aee885becd0213001d61839f3bc0158f`  
		Last Modified: Tue, 15 Nov 2022 06:10:15 GMT  
		Size: 1.2 MB (1164513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f743716d719aed881a6a611d2d969baec0c3e94ff6974d284c9e7a57b541fd84`  
		Last Modified: Tue, 15 Nov 2022 06:10:16 GMT  
		Size: 294.2 KB (294180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1976d15700a3e538cf0dc3e023e9d1b586ce5ff24bbddecdd1720d007c84f61c`  
		Last Modified: Tue, 15 Nov 2022 06:10:14 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87eb4344f07ee5c1704eafabce4eb53137661611d38126e683099e7b33516996`  
		Last Modified: Tue, 15 Nov 2022 06:10:16 GMT  
		Size: 41.1 MB (41121816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6c8ef0379ddc55db17ea10a99e09f0b2785df7ab07d51cb9b5f04b91b1a9bd`  
		Last Modified: Tue, 15 Nov 2022 06:10:12 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c176fa832e8815ccdbb89ff2e7891ef53e812a74eabe135c0bba56ea8160b2`  
		Last Modified: Tue, 15 Nov 2022 06:10:12 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd34a481b212433d028515433fbadb203117367c8071e4c9146da251e7a53861`  
		Last Modified: Tue, 15 Nov 2022 06:10:13 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36340467232d3fcd89c4448a2183d1fdec6c764fcc163bebf8ab70b551eb8e7b`  
		Last Modified: Tue, 15 Nov 2022 06:10:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1.2`

```console
$ docker pull couchdb@sha256:f3a5561153cdd2d8117866feac97c07520e92412a49ec2d4667fb8ee8174ae45
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1.2` - linux; amd64

```console
$ docker pull couchdb@sha256:7b39bd5a1e42135efafa5b969fe7fdaba5a9635f8aa62b96a3493ec3c7a292a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80023492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53cc4782ab9377854f055bcc9e7ad0b040794ca4a8c898742bfcd5fa9a818bfc`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 15 Nov 2022 04:05:14 GMT
ADD file:9461639b945ced6fb6164491a7e0131261a1b7d69264cce516e75c71e4df22d2 in / 
# Tue, 15 Nov 2022 04:05:14 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:35:54 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 15 Nov 2022 10:35:55 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 15 Nov 2022 10:36:02 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:36:07 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 15 Nov 2022 10:36:07 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 15 Nov 2022 10:36:14 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:36:14 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 15 Nov 2022 10:36:15 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 15 Nov 2022 10:36:29 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 15 Nov 2022 10:36:29 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 15 Nov 2022 10:36:29 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 15 Nov 2022 10:36:30 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 15 Nov 2022 10:36:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 15 Nov 2022 10:36:30 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 10:36:30 GMT
VOLUME [/opt/couchdb/data]
# Tue, 15 Nov 2022 10:36:30 GMT
EXPOSE 4369 5984 9100
# Tue, 15 Nov 2022 10:36:31 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:32820e52a00eb22dc76d70d992be7082cd24b636cfb597ff3951d29a821b46b9`  
		Last Modified: Tue, 15 Nov 2022 04:09:26 GMT  
		Size: 27.1 MB (27140332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8b386cb12f04cd6f9c67d0c0373d9ba78bbf5fa84562a9898904f6f17805b2`  
		Last Modified: Tue, 15 Nov 2022 10:37:34 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df26f4bfe01cd6f4dfe22fc28ece77009b0f36ab15a099aa5ba5826aa10129e`  
		Last Modified: Tue, 15 Nov 2022 10:37:34 GMT  
		Size: 6.7 MB (6703723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5d10938ed357b3e2264066bfe9e4b3cbed1cca64738d2b4ab40051bc2b5397`  
		Last Modified: Tue, 15 Nov 2022 10:37:33 GMT  
		Size: 1.3 MB (1259579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42738d31e487788abf984684c20e8dfe4d73946b80c79f2d6762693c90f8926c`  
		Last Modified: Tue, 15 Nov 2022 10:37:33 GMT  
		Size: 294.3 KB (294312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c8fff565fab486613ac3d15b45bb312a702ff6f222a903dc7c5a6d6d98a0f9`  
		Last Modified: Tue, 15 Nov 2022 10:37:32 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62f66cee9b45db68f6b1cb887d7695c071fb29957e72744957cc9950fc51ec2`  
		Last Modified: Tue, 15 Nov 2022 10:37:36 GMT  
		Size: 44.6 MB (44618537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2354cbf0561fe5f84c7fd90faceab75e1c44c1225c4939ef7685f9454c20d849`  
		Last Modified: Tue, 15 Nov 2022 10:37:30 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4e08c3ee4175a8be3ca54cbb71de31fe256a801ee8b33550a1295c6ccc439f`  
		Last Modified: Tue, 15 Nov 2022 10:37:30 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100dc05f176c141aa69c4fec8dd543cea1b1683e9d69604e618e0976fdc7adec`  
		Last Modified: Tue, 15 Nov 2022 10:37:31 GMT  
		Size: 2.1 KB (2056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14542c43a715195d747204fa11753b7a248b105b452c9f01e02d36bb2b7fc24`  
		Last Modified: Tue, 15 Nov 2022 10:37:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:930c9f1531c2cc9c937d00a8cc5fb46a227d32e406730d7111e1ed5500eb08e2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75079535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f12d0a699ab20ac1dba8aaf2ae74a73a88500be0b6d22048d08112ffb5095a7`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:34 GMT
ADD file:aaead8e4dd08d41c8d1692bbe76b673119289836428e1f713ca550c2468711ac in / 
# Tue, 15 Nov 2022 01:41:34 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 06:08:41 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 15 Nov 2022 06:08:42 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 15 Nov 2022 06:08:48 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 06:08:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 15 Nov 2022 06:08:52 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 15 Nov 2022 06:08:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 06:08:58 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 15 Nov 2022 06:08:58 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 15 Nov 2022 06:09:09 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 15 Nov 2022 06:09:10 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 15 Nov 2022 06:09:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 15 Nov 2022 06:09:10 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 15 Nov 2022 06:09:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 15 Nov 2022 06:09:10 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 06:09:10 GMT
VOLUME [/opt/couchdb/data]
# Tue, 15 Nov 2022 06:09:10 GMT
EXPOSE 4369 5984 9100
# Tue, 15 Nov 2022 06:09:11 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:cc457132e077d684a6cecad3331c35341d814c5d364f3cf24d698a6d8e76d0e7`  
		Last Modified: Tue, 15 Nov 2022 01:45:13 GMT  
		Size: 25.9 MB (25914924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510e02d58fa2dbfebc3aa5cfabf2a30c7b284888399969b4ca2ee82e466cf088`  
		Last Modified: Tue, 15 Nov 2022 06:10:18 GMT  
		Size: 3.4 KB (3436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ebeecce1b4027a2486f99101198a916d89cdf12eead09d3ba2783466915604`  
		Last Modified: Tue, 15 Nov 2022 06:10:16 GMT  
		Size: 6.6 MB (6577064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9d360df926f74081761ca41bff2e01aee885becd0213001d61839f3bc0158f`  
		Last Modified: Tue, 15 Nov 2022 06:10:15 GMT  
		Size: 1.2 MB (1164513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f743716d719aed881a6a611d2d969baec0c3e94ff6974d284c9e7a57b541fd84`  
		Last Modified: Tue, 15 Nov 2022 06:10:16 GMT  
		Size: 294.2 KB (294180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1976d15700a3e538cf0dc3e023e9d1b586ce5ff24bbddecdd1720d007c84f61c`  
		Last Modified: Tue, 15 Nov 2022 06:10:14 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87eb4344f07ee5c1704eafabce4eb53137661611d38126e683099e7b33516996`  
		Last Modified: Tue, 15 Nov 2022 06:10:16 GMT  
		Size: 41.1 MB (41121816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6c8ef0379ddc55db17ea10a99e09f0b2785df7ab07d51cb9b5f04b91b1a9bd`  
		Last Modified: Tue, 15 Nov 2022 06:10:12 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c176fa832e8815ccdbb89ff2e7891ef53e812a74eabe135c0bba56ea8160b2`  
		Last Modified: Tue, 15 Nov 2022 06:10:12 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd34a481b212433d028515433fbadb203117367c8071e4c9146da251e7a53861`  
		Last Modified: Tue, 15 Nov 2022 06:10:13 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36340467232d3fcd89c4448a2183d1fdec6c764fcc163bebf8ab70b551eb8e7b`  
		Last Modified: Tue, 15 Nov 2022 06:10:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2`

```console
$ docker pull couchdb@sha256:d3346c205f96be4ce36c245ff08e44331115437ff8760cccb685df64e4470434
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2` - linux; amd64

```console
$ docker pull couchdb@sha256:18b447eb4aa7371763ad1e65fb21b89e867e4e38fbaf87340e401c0d2b48672d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87542993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86d51a034b33057b01caf54d400a6f527ce26b7894ee8d93ea5e8c478307c77e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:35:14 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 15 Nov 2022 10:35:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 15 Nov 2022 10:35:22 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:35:26 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 15 Nov 2022 10:35:26 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 15 Nov 2022 10:35:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:35:32 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 15 Nov 2022 10:35:33 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 15 Nov 2022 10:35:46 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 15 Nov 2022 10:35:47 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 15 Nov 2022 10:35:47 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 15 Nov 2022 10:35:47 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 15 Nov 2022 10:35:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 15 Nov 2022 10:35:48 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 10:35:48 GMT
VOLUME [/opt/couchdb/data]
# Tue, 15 Nov 2022 10:35:48 GMT
EXPOSE 4369 5984 9100
# Tue, 15 Nov 2022 10:35:48 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ac309e879645bf78b5b51a81163cbbaec1a07acab50160803d720a2cd20faa`  
		Last Modified: Tue, 15 Nov 2022 10:37:15 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49844afe089a8ae2b28167131e091ee4187c088c6a872e9325c1d31958cb820e`  
		Last Modified: Tue, 15 Nov 2022 10:37:14 GMT  
		Size: 5.2 MB (5225827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8627dd11a7afca5ddbc0d10ad202fc8c0cc3f7b4e616c5aa496ece15c69c41`  
		Last Modified: Tue, 15 Nov 2022 10:37:13 GMT  
		Size: 1.6 MB (1554043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74501422620a7da2c637583baba5da1d30f26f6914e9904901fe2d1fbcbd0e76`  
		Last Modified: Tue, 15 Nov 2022 10:37:13 GMT  
		Size: 296.3 KB (296279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36940d23f9815532c5e6f5ac48eac39ee6851584fad38d584af6e2d7e08868f8`  
		Last Modified: Tue, 15 Nov 2022 10:37:13 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc41a6e08f50ee957aa8bbdc82b5d63ec2c6070b39131eb7294753615a8a4525`  
		Last Modified: Tue, 15 Nov 2022 10:37:16 GMT  
		Size: 49.0 MB (49047070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64abb1d4412cba2191e7a32e467c78dcc0dc5f66248b85909e2585fcf9da9e6e`  
		Last Modified: Tue, 15 Nov 2022 10:37:11 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c470c6cf30f98b8c7dedcfbb51c7d3b31e28b9b4b054fc28defbc4b849a7c24d`  
		Last Modified: Tue, 15 Nov 2022 10:37:11 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28986f7c1a1bb4a3100d2af60b12e1819fff375e5ffd528ef2e948d4d9606a6b`  
		Last Modified: Tue, 15 Nov 2022 10:37:11 GMT  
		Size: 2.2 KB (2188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2411adc92296964132673b2cbd12ace5e926c6baf3d7f381e7475258440563`  
		Last Modified: Tue, 15 Nov 2022 10:37:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; arm64 variant v8

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
$ docker pull couchdb@sha256:d3346c205f96be4ce36c245ff08e44331115437ff8760cccb685df64e4470434
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2.2` - linux; amd64

```console
$ docker pull couchdb@sha256:18b447eb4aa7371763ad1e65fb21b89e867e4e38fbaf87340e401c0d2b48672d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87542993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86d51a034b33057b01caf54d400a6f527ce26b7894ee8d93ea5e8c478307c77e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:35:14 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 15 Nov 2022 10:35:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 15 Nov 2022 10:35:22 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:35:26 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 15 Nov 2022 10:35:26 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 15 Nov 2022 10:35:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:35:32 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 15 Nov 2022 10:35:33 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 15 Nov 2022 10:35:46 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 15 Nov 2022 10:35:47 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 15 Nov 2022 10:35:47 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 15 Nov 2022 10:35:47 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 15 Nov 2022 10:35:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 15 Nov 2022 10:35:48 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 10:35:48 GMT
VOLUME [/opt/couchdb/data]
# Tue, 15 Nov 2022 10:35:48 GMT
EXPOSE 4369 5984 9100
# Tue, 15 Nov 2022 10:35:48 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ac309e879645bf78b5b51a81163cbbaec1a07acab50160803d720a2cd20faa`  
		Last Modified: Tue, 15 Nov 2022 10:37:15 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49844afe089a8ae2b28167131e091ee4187c088c6a872e9325c1d31958cb820e`  
		Last Modified: Tue, 15 Nov 2022 10:37:14 GMT  
		Size: 5.2 MB (5225827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8627dd11a7afca5ddbc0d10ad202fc8c0cc3f7b4e616c5aa496ece15c69c41`  
		Last Modified: Tue, 15 Nov 2022 10:37:13 GMT  
		Size: 1.6 MB (1554043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74501422620a7da2c637583baba5da1d30f26f6914e9904901fe2d1fbcbd0e76`  
		Last Modified: Tue, 15 Nov 2022 10:37:13 GMT  
		Size: 296.3 KB (296279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36940d23f9815532c5e6f5ac48eac39ee6851584fad38d584af6e2d7e08868f8`  
		Last Modified: Tue, 15 Nov 2022 10:37:13 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc41a6e08f50ee957aa8bbdc82b5d63ec2c6070b39131eb7294753615a8a4525`  
		Last Modified: Tue, 15 Nov 2022 10:37:16 GMT  
		Size: 49.0 MB (49047070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64abb1d4412cba2191e7a32e467c78dcc0dc5f66248b85909e2585fcf9da9e6e`  
		Last Modified: Tue, 15 Nov 2022 10:37:11 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c470c6cf30f98b8c7dedcfbb51c7d3b31e28b9b4b054fc28defbc4b849a7c24d`  
		Last Modified: Tue, 15 Nov 2022 10:37:11 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28986f7c1a1bb4a3100d2af60b12e1819fff375e5ffd528ef2e948d4d9606a6b`  
		Last Modified: Tue, 15 Nov 2022 10:37:11 GMT  
		Size: 2.2 KB (2188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2411adc92296964132673b2cbd12ace5e926c6baf3d7f381e7475258440563`  
		Last Modified: Tue, 15 Nov 2022 10:37:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2.2` - linux; arm64 variant v8

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
$ docker pull couchdb@sha256:d3346c205f96be4ce36c245ff08e44331115437ff8760cccb685df64e4470434
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:18b447eb4aa7371763ad1e65fb21b89e867e4e38fbaf87340e401c0d2b48672d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87542993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86d51a034b33057b01caf54d400a6f527ce26b7894ee8d93ea5e8c478307c77e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:35:14 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 15 Nov 2022 10:35:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 15 Nov 2022 10:35:22 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:35:26 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 15 Nov 2022 10:35:26 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 15 Nov 2022 10:35:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:35:32 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 15 Nov 2022 10:35:33 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 15 Nov 2022 10:35:46 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 15 Nov 2022 10:35:47 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 15 Nov 2022 10:35:47 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 15 Nov 2022 10:35:47 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 15 Nov 2022 10:35:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 15 Nov 2022 10:35:48 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 10:35:48 GMT
VOLUME [/opt/couchdb/data]
# Tue, 15 Nov 2022 10:35:48 GMT
EXPOSE 4369 5984 9100
# Tue, 15 Nov 2022 10:35:48 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ac309e879645bf78b5b51a81163cbbaec1a07acab50160803d720a2cd20faa`  
		Last Modified: Tue, 15 Nov 2022 10:37:15 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49844afe089a8ae2b28167131e091ee4187c088c6a872e9325c1d31958cb820e`  
		Last Modified: Tue, 15 Nov 2022 10:37:14 GMT  
		Size: 5.2 MB (5225827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8627dd11a7afca5ddbc0d10ad202fc8c0cc3f7b4e616c5aa496ece15c69c41`  
		Last Modified: Tue, 15 Nov 2022 10:37:13 GMT  
		Size: 1.6 MB (1554043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74501422620a7da2c637583baba5da1d30f26f6914e9904901fe2d1fbcbd0e76`  
		Last Modified: Tue, 15 Nov 2022 10:37:13 GMT  
		Size: 296.3 KB (296279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36940d23f9815532c5e6f5ac48eac39ee6851584fad38d584af6e2d7e08868f8`  
		Last Modified: Tue, 15 Nov 2022 10:37:13 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc41a6e08f50ee957aa8bbdc82b5d63ec2c6070b39131eb7294753615a8a4525`  
		Last Modified: Tue, 15 Nov 2022 10:37:16 GMT  
		Size: 49.0 MB (49047070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64abb1d4412cba2191e7a32e467c78dcc0dc5f66248b85909e2585fcf9da9e6e`  
		Last Modified: Tue, 15 Nov 2022 10:37:11 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c470c6cf30f98b8c7dedcfbb51c7d3b31e28b9b4b054fc28defbc4b849a7c24d`  
		Last Modified: Tue, 15 Nov 2022 10:37:11 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28986f7c1a1bb4a3100d2af60b12e1819fff375e5ffd528ef2e948d4d9606a6b`  
		Last Modified: Tue, 15 Nov 2022 10:37:11 GMT  
		Size: 2.2 KB (2188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2411adc92296964132673b2cbd12ace5e926c6baf3d7f381e7475258440563`  
		Last Modified: Tue, 15 Nov 2022 10:37:11 GMT  
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
