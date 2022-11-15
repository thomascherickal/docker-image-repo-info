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
$ docker pull couchdb@sha256:60364b008ee2e21d3be258f2863b68f203a2865ada9b418c40f2b37eb631d331
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2` - linux; amd64

```console
$ docker pull couchdb@sha256:ed975072e8d21c9a3a3a9520ba08c6c2c9c05b6ef94aa24a1af9e866d83606d3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84542530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36e30b14a6e5edd9fe7afa8187e13a661a1e3d7940f669be8c8e1a6a37d9b37e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:18:20 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 25 Oct 2022 09:18:21 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 25 Oct 2022 09:18:32 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:18:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 25 Oct 2022 09:18:36 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 25 Oct 2022 09:18:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:19:08 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 25 Oct 2022 09:19:09 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 25 Oct 2022 09:19:28 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 25 Oct 2022 09:19:28 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 25 Oct 2022 09:19:28 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 25 Oct 2022 09:19:29 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 25 Oct 2022 09:19:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 25 Oct 2022 09:19:29 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 25 Oct 2022 09:19:29 GMT
VOLUME [/opt/couchdb/data]
# Tue, 25 Oct 2022 09:19:29 GMT
EXPOSE 4369 5984 9100
# Tue, 25 Oct 2022 09:19:30 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c09589ee2015314be997187593a730a53253ecb4efa6f1e0e7ec31337539b0`  
		Last Modified: Tue, 25 Oct 2022 09:20:11 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71829f8994c9da5480c3cb2bf07761017ddbb004e090eb018d2e85a4d7b4b152`  
		Last Modified: Tue, 25 Oct 2022 09:20:10 GMT  
		Size: 6.7 MB (6703801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd841ba89db9a1936a0d51fbd52911f1812c2b718c85dd524137674fa9e54c05`  
		Last Modified: Tue, 25 Oct 2022 09:20:09 GMT  
		Size: 1.3 MB (1259571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae8b0cb4b7b23be58c6e90c9be853b7c59a610bcba7379ca4750bfe7b4c424a`  
		Last Modified: Tue, 25 Oct 2022 09:20:09 GMT  
		Size: 294.3 KB (294288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cb99bf562916aacb4c9d92350fef6dc873beda54bb61bbe660085be3ab38bc`  
		Last Modified: Tue, 25 Oct 2022 09:20:23 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c2fa01be3011bd2cef3f65a75c60ed5e0bb27ccb6c4bc8ec28e6d47e019534`  
		Last Modified: Tue, 25 Oct 2022 09:20:28 GMT  
		Size: 49.1 MB (49137024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c779a49ab4bbc037cb2a5d6337be71430899a3dbfee948484e5070f2a66e3365`  
		Last Modified: Tue, 25 Oct 2022 09:20:21 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82cddca273848775760fb4bb5b184c60f53e8ed4914dfd9bd1e32c734d47a8d5`  
		Last Modified: Tue, 25 Oct 2022 09:20:21 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37fcbb8bdd88a0231d8cbef6852d612830bef93769879d96e0c97d4c48e2097d`  
		Last Modified: Tue, 25 Oct 2022 09:20:22 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bbcdc21fb64b74a42cf23fea379d514b50609a6935c50a0993a3a8e60f7746`  
		Last Modified: Tue, 25 Oct 2022 09:20:22 GMT  
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
$ docker pull couchdb@sha256:60364b008ee2e21d3be258f2863b68f203a2865ada9b418c40f2b37eb631d331
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:ed975072e8d21c9a3a3a9520ba08c6c2c9c05b6ef94aa24a1af9e866d83606d3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84542530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36e30b14a6e5edd9fe7afa8187e13a661a1e3d7940f669be8c8e1a6a37d9b37e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:18:20 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 25 Oct 2022 09:18:21 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 25 Oct 2022 09:18:32 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:18:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 25 Oct 2022 09:18:36 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 25 Oct 2022 09:18:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:19:08 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 25 Oct 2022 09:19:09 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 25 Oct 2022 09:19:28 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 25 Oct 2022 09:19:28 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 25 Oct 2022 09:19:28 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 25 Oct 2022 09:19:29 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 25 Oct 2022 09:19:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 25 Oct 2022 09:19:29 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 25 Oct 2022 09:19:29 GMT
VOLUME [/opt/couchdb/data]
# Tue, 25 Oct 2022 09:19:29 GMT
EXPOSE 4369 5984 9100
# Tue, 25 Oct 2022 09:19:30 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c09589ee2015314be997187593a730a53253ecb4efa6f1e0e7ec31337539b0`  
		Last Modified: Tue, 25 Oct 2022 09:20:11 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71829f8994c9da5480c3cb2bf07761017ddbb004e090eb018d2e85a4d7b4b152`  
		Last Modified: Tue, 25 Oct 2022 09:20:10 GMT  
		Size: 6.7 MB (6703801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd841ba89db9a1936a0d51fbd52911f1812c2b718c85dd524137674fa9e54c05`  
		Last Modified: Tue, 25 Oct 2022 09:20:09 GMT  
		Size: 1.3 MB (1259571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae8b0cb4b7b23be58c6e90c9be853b7c59a610bcba7379ca4750bfe7b4c424a`  
		Last Modified: Tue, 25 Oct 2022 09:20:09 GMT  
		Size: 294.3 KB (294288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cb99bf562916aacb4c9d92350fef6dc873beda54bb61bbe660085be3ab38bc`  
		Last Modified: Tue, 25 Oct 2022 09:20:23 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c2fa01be3011bd2cef3f65a75c60ed5e0bb27ccb6c4bc8ec28e6d47e019534`  
		Last Modified: Tue, 25 Oct 2022 09:20:28 GMT  
		Size: 49.1 MB (49137024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c779a49ab4bbc037cb2a5d6337be71430899a3dbfee948484e5070f2a66e3365`  
		Last Modified: Tue, 25 Oct 2022 09:20:21 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82cddca273848775760fb4bb5b184c60f53e8ed4914dfd9bd1e32c734d47a8d5`  
		Last Modified: Tue, 25 Oct 2022 09:20:21 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37fcbb8bdd88a0231d8cbef6852d612830bef93769879d96e0c97d4c48e2097d`  
		Last Modified: Tue, 25 Oct 2022 09:20:22 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bbcdc21fb64b74a42cf23fea379d514b50609a6935c50a0993a3a8e60f7746`  
		Last Modified: Tue, 25 Oct 2022 09:20:22 GMT  
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
$ docker pull couchdb@sha256:60364b008ee2e21d3be258f2863b68f203a2865ada9b418c40f2b37eb631d331
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:ed975072e8d21c9a3a3a9520ba08c6c2c9c05b6ef94aa24a1af9e866d83606d3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84542530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36e30b14a6e5edd9fe7afa8187e13a661a1e3d7940f669be8c8e1a6a37d9b37e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:18:20 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 25 Oct 2022 09:18:21 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 25 Oct 2022 09:18:32 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:18:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 25 Oct 2022 09:18:36 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 25 Oct 2022 09:18:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:19:08 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 25 Oct 2022 09:19:09 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 25 Oct 2022 09:19:28 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 25 Oct 2022 09:19:28 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 25 Oct 2022 09:19:28 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 25 Oct 2022 09:19:29 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 25 Oct 2022 09:19:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 25 Oct 2022 09:19:29 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 25 Oct 2022 09:19:29 GMT
VOLUME [/opt/couchdb/data]
# Tue, 25 Oct 2022 09:19:29 GMT
EXPOSE 4369 5984 9100
# Tue, 25 Oct 2022 09:19:30 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c09589ee2015314be997187593a730a53253ecb4efa6f1e0e7ec31337539b0`  
		Last Modified: Tue, 25 Oct 2022 09:20:11 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71829f8994c9da5480c3cb2bf07761017ddbb004e090eb018d2e85a4d7b4b152`  
		Last Modified: Tue, 25 Oct 2022 09:20:10 GMT  
		Size: 6.7 MB (6703801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd841ba89db9a1936a0d51fbd52911f1812c2b718c85dd524137674fa9e54c05`  
		Last Modified: Tue, 25 Oct 2022 09:20:09 GMT  
		Size: 1.3 MB (1259571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae8b0cb4b7b23be58c6e90c9be853b7c59a610bcba7379ca4750bfe7b4c424a`  
		Last Modified: Tue, 25 Oct 2022 09:20:09 GMT  
		Size: 294.3 KB (294288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cb99bf562916aacb4c9d92350fef6dc873beda54bb61bbe660085be3ab38bc`  
		Last Modified: Tue, 25 Oct 2022 09:20:23 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c2fa01be3011bd2cef3f65a75c60ed5e0bb27ccb6c4bc8ec28e6d47e019534`  
		Last Modified: Tue, 25 Oct 2022 09:20:28 GMT  
		Size: 49.1 MB (49137024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c779a49ab4bbc037cb2a5d6337be71430899a3dbfee948484e5070f2a66e3365`  
		Last Modified: Tue, 25 Oct 2022 09:20:21 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82cddca273848775760fb4bb5b184c60f53e8ed4914dfd9bd1e32c734d47a8d5`  
		Last Modified: Tue, 25 Oct 2022 09:20:21 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37fcbb8bdd88a0231d8cbef6852d612830bef93769879d96e0c97d4c48e2097d`  
		Last Modified: Tue, 25 Oct 2022 09:20:22 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bbcdc21fb64b74a42cf23fea379d514b50609a6935c50a0993a3a8e60f7746`  
		Last Modified: Tue, 25 Oct 2022 09:20:22 GMT  
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
$ docker pull couchdb@sha256:72de0dfa76d1434e5007819d1822c9c6c018daf6eb24eeb37fc116551d25925e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3` - linux; amd64

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
$ docker pull couchdb@sha256:ab4ead399a0ffd0401e7917902c916c6c997fe7ff87d2f916433348b33fa0335
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:1a5d0865d795406f0fb22a3929bca750b5588a16311c8d116d276750adee0fbe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80024122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d77aafe105bd1faf2334b134836beb8a4bb5b04d8111d3a6622e704b380e8dfd`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:18:20 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 25 Oct 2022 09:18:21 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 25 Oct 2022 09:18:32 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:18:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 25 Oct 2022 09:18:36 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 25 Oct 2022 09:18:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:18:44 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 25 Oct 2022 09:18:45 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 25 Oct 2022 09:18:59 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 25 Oct 2022 09:18:59 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 25 Oct 2022 09:18:59 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 25 Oct 2022 09:19:00 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 25 Oct 2022 09:19:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 25 Oct 2022 09:19:00 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 25 Oct 2022 09:19:00 GMT
VOLUME [/opt/couchdb/data]
# Tue, 25 Oct 2022 09:19:00 GMT
EXPOSE 4369 5984 9100
# Tue, 25 Oct 2022 09:19:01 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c09589ee2015314be997187593a730a53253ecb4efa6f1e0e7ec31337539b0`  
		Last Modified: Tue, 25 Oct 2022 09:20:11 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71829f8994c9da5480c3cb2bf07761017ddbb004e090eb018d2e85a4d7b4b152`  
		Last Modified: Tue, 25 Oct 2022 09:20:10 GMT  
		Size: 6.7 MB (6703801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd841ba89db9a1936a0d51fbd52911f1812c2b718c85dd524137674fa9e54c05`  
		Last Modified: Tue, 25 Oct 2022 09:20:09 GMT  
		Size: 1.3 MB (1259571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae8b0cb4b7b23be58c6e90c9be853b7c59a610bcba7379ca4750bfe7b4c424a`  
		Last Modified: Tue, 25 Oct 2022 09:20:09 GMT  
		Size: 294.3 KB (294288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:075b813277986ae91146077ca01c33b2f93a38c2ba6590ac4113b17a60ac0d2f`  
		Last Modified: Tue, 25 Oct 2022 09:20:09 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def4486e53f229d3f23a24b73e5dd538899002d0d2a8fa0c60e309fb578da779`  
		Last Modified: Tue, 25 Oct 2022 09:20:12 GMT  
		Size: 44.6 MB (44618609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da74d879ae097442ce120efa226880eb7e648d5b6cf1f71702462c953d8a0c8`  
		Last Modified: Tue, 25 Oct 2022 09:20:07 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6386883a5fd79a06e3932dd772d2018c6a034ce2c23289ae149150a8f3def8`  
		Last Modified: Tue, 25 Oct 2022 09:20:07 GMT  
		Size: 769.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34ef44a3c1036e5fd1d3527dff52fb2c34d157324a7d05d519b6150ff8a4f67`  
		Last Modified: Tue, 25 Oct 2022 09:20:07 GMT  
		Size: 2.1 KB (2061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ccfb91695ddfe6e694e6fe862c5115b1643895c2878aa2c4798a64cb6b0cc08`  
		Last Modified: Tue, 25 Oct 2022 09:20:07 GMT  
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
$ docker pull couchdb@sha256:ab4ead399a0ffd0401e7917902c916c6c997fe7ff87d2f916433348b33fa0335
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1.2` - linux; amd64

```console
$ docker pull couchdb@sha256:1a5d0865d795406f0fb22a3929bca750b5588a16311c8d116d276750adee0fbe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80024122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d77aafe105bd1faf2334b134836beb8a4bb5b04d8111d3a6622e704b380e8dfd`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:12 GMT
ADD file:14c4aa7a136ce9eb1fae0ba0f394509990d44126be801a2713cf8722fbb2e6b9 in / 
# Tue, 25 Oct 2022 01:44:12 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:18:20 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 25 Oct 2022 09:18:21 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 25 Oct 2022 09:18:32 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:18:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 25 Oct 2022 09:18:36 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 25 Oct 2022 09:18:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 09:18:44 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 25 Oct 2022 09:18:45 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 25 Oct 2022 09:18:59 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 25 Oct 2022 09:18:59 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 25 Oct 2022 09:18:59 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 25 Oct 2022 09:19:00 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 25 Oct 2022 09:19:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 25 Oct 2022 09:19:00 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 25 Oct 2022 09:19:00 GMT
VOLUME [/opt/couchdb/data]
# Tue, 25 Oct 2022 09:19:00 GMT
EXPOSE 4369 5984 9100
# Tue, 25 Oct 2022 09:19:01 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:4500a762c54620411ae491a547c66b61d577c1369ecbf5a7e91b4e153181854b`  
		Last Modified: Tue, 25 Oct 2022 01:48:40 GMT  
		Size: 27.1 MB (27140832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c09589ee2015314be997187593a730a53253ecb4efa6f1e0e7ec31337539b0`  
		Last Modified: Tue, 25 Oct 2022 09:20:11 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71829f8994c9da5480c3cb2bf07761017ddbb004e090eb018d2e85a4d7b4b152`  
		Last Modified: Tue, 25 Oct 2022 09:20:10 GMT  
		Size: 6.7 MB (6703801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd841ba89db9a1936a0d51fbd52911f1812c2b718c85dd524137674fa9e54c05`  
		Last Modified: Tue, 25 Oct 2022 09:20:09 GMT  
		Size: 1.3 MB (1259571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae8b0cb4b7b23be58c6e90c9be853b7c59a610bcba7379ca4750bfe7b4c424a`  
		Last Modified: Tue, 25 Oct 2022 09:20:09 GMT  
		Size: 294.3 KB (294288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:075b813277986ae91146077ca01c33b2f93a38c2ba6590ac4113b17a60ac0d2f`  
		Last Modified: Tue, 25 Oct 2022 09:20:09 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def4486e53f229d3f23a24b73e5dd538899002d0d2a8fa0c60e309fb578da779`  
		Last Modified: Tue, 25 Oct 2022 09:20:12 GMT  
		Size: 44.6 MB (44618609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da74d879ae097442ce120efa226880eb7e648d5b6cf1f71702462c953d8a0c8`  
		Last Modified: Tue, 25 Oct 2022 09:20:07 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6386883a5fd79a06e3932dd772d2018c6a034ce2c23289ae149150a8f3def8`  
		Last Modified: Tue, 25 Oct 2022 09:20:07 GMT  
		Size: 769.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34ef44a3c1036e5fd1d3527dff52fb2c34d157324a7d05d519b6150ff8a4f67`  
		Last Modified: Tue, 25 Oct 2022 09:20:07 GMT  
		Size: 2.1 KB (2061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ccfb91695ddfe6e694e6fe862c5115b1643895c2878aa2c4798a64cb6b0cc08`  
		Last Modified: Tue, 25 Oct 2022 09:20:07 GMT  
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
$ docker pull couchdb@sha256:72de0dfa76d1434e5007819d1822c9c6c018daf6eb24eeb37fc116551d25925e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2` - linux; amd64

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
$ docker pull couchdb@sha256:72de0dfa76d1434e5007819d1822c9c6c018daf6eb24eeb37fc116551d25925e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2.2` - linux; amd64

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
