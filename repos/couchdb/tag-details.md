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
$ docker pull couchdb@sha256:16739ea471ef700df680c43cad5cef4965a3468532f9d80f286f2c2033be60ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2` - linux; amd64

```console
$ docker pull couchdb@sha256:8ea05770cacfc3e4293f6c6825c280bc49fc9e2358c81e671a3b9473a8792c7d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84525044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99d0cd0445244d76222a24265f1e3a6edf1b9d9334d2900418fe5639bb8e1d52`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:05:14 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 May 2022 02:05:15 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 May 2022 02:05:22 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:05:26 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 May 2022 02:05:26 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 May 2022 02:05:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:05:54 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 11 May 2022 02:05:55 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 May 2022 02:06:12 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 May 2022 02:06:13 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 11 May 2022 02:06:13 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 May 2022 02:06:13 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 11 May 2022 02:06:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 May 2022 02:06:14 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 May 2022 02:06:14 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 May 2022 02:06:14 GMT
EXPOSE 4369 5984 9100
# Wed, 11 May 2022 02:06:14 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d03d9847c338f80e8fbca52fd94a0a0aad2792cbe1341cc3fb6067a4ee567c5`  
		Last Modified: Wed, 11 May 2022 02:06:56 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2aee334c57e9fec0f83f4955b20262ce02650c108b878c73d7ccd9039b76c6a`  
		Last Modified: Wed, 11 May 2022 02:06:55 GMT  
		Size: 6.7 MB (6698559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c6798238438f93c309f2ad6c50de5f6fcf0aab2e17b5c902179e27d163a639`  
		Last Modified: Wed, 11 May 2022 02:06:54 GMT  
		Size: 1.3 MB (1258367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db74e747e5b05e04bffbfdaa41b5ad4a2db907a70aa1ab9902ef36fa7474482`  
		Last Modified: Wed, 11 May 2022 02:06:54 GMT  
		Size: 293.0 KB (293001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fbd90e3f7c935db6713aeb78963813c26419b896aa8202166e13851f5eaa52c`  
		Last Modified: Wed, 11 May 2022 02:07:08 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b215fdce3c26a6756a900982913487ee75db89a8739b8438f3f27f4a93c10f`  
		Last Modified: Wed, 11 May 2022 02:07:12 GMT  
		Size: 49.1 MB (49127385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d10b2297c1dfda106e356ce6e7a7ce214fb9e47225c79a37c273bc2d2d6e45b`  
		Last Modified: Wed, 11 May 2022 02:07:06 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5e42599e3dbcd331001f448fdb1a8ee10d0fbbf739549e082550bae490723b`  
		Last Modified: Wed, 11 May 2022 02:07:06 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d60aad0805e79cf9a6223c764013ce852942843a8b028e2d8243d6ed841e8e`  
		Last Modified: Wed, 11 May 2022 02:07:06 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1b84c4db843d2e00ef78f9a44fb16f3401b0161cc770ca96d94d310f400f48`  
		Last Modified: Wed, 11 May 2022 02:07:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:e73034e7e1fd3ab38e8093476d0376533314735436cafb87633c75926f5c924a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72527241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d88a2d4f99da857f9e233207ada61c8cc5504b032ce62387fea10cbe03300fb7`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 May 2022 00:47:26 GMT
ADD file:2536146c773d09db1a8fbbff00933acc459d8929feb3cff5b93ca4c23b577845 in / 
# Wed, 11 May 2022 00:47:26 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:45:11 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 May 2022 01:45:12 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 May 2022 01:45:20 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:45:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 May 2022 01:45:25 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 May 2022 01:45:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:46:03 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 11 May 2022 01:46:04 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 May 2022 01:46:18 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 May 2022 01:46:19 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 11 May 2022 01:46:20 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 May 2022 01:46:21 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 11 May 2022 01:46:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 May 2022 01:46:22 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 May 2022 01:46:23 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 May 2022 01:46:24 GMT
EXPOSE 4369 5984 9100
# Wed, 11 May 2022 01:46:25 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:383d573fdcf2c6da56fdb61e120549d7bc200471208ca4c7c6605c57a0a87ef6`  
		Last Modified: Wed, 11 May 2022 00:54:36 GMT  
		Size: 25.9 MB (25909014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a538c8ac927fa268f7107913c05d740399cce6245cc44b0f5cfd5fd14318434`  
		Last Modified: Wed, 11 May 2022 01:47:19 GMT  
		Size: 3.3 KB (3319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f730aee3592d57a6764bb9172710619552bf2c89fad6d64ac0056fbc02876266`  
		Last Modified: Wed, 11 May 2022 01:47:19 GMT  
		Size: 6.6 MB (6556393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c5923e32b1016f381ab756a45e1ce6897491277064f3d1fea69b0f0f22af0c`  
		Last Modified: Wed, 11 May 2022 01:47:18 GMT  
		Size: 951.2 KB (951181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff679ff3f207b333f7ea83a9b137230853a2a787b55b612885f192bba5f80719`  
		Last Modified: Wed, 11 May 2022 01:47:17 GMT  
		Size: 80.0 KB (79971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc333406fdaf9c77e64c600b3f138ddf28952951799f86525899401052f791e`  
		Last Modified: Wed, 11 May 2022 01:47:33 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93542b97e7d05d7c549d16a7af3b3605ac183e5c4b97eb3ed825fc2dcc82eb3`  
		Last Modified: Wed, 11 May 2022 01:47:36 GMT  
		Size: 39.0 MB (39023759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d2c966afb9941dc766e4098adef1d8c1cff34b720a920f454dde7c4c924dd0`  
		Last Modified: Wed, 11 May 2022 01:47:31 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68175c1f75bbcad6b45c984822604a02bd39276b9011108471c5e4bac76cca1`  
		Last Modified: Wed, 11 May 2022 01:47:31 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84cc361861fe639e5cd29a5a314024cae6c0e8ea0812cbc42a2a1157ce5a737c`  
		Last Modified: Wed, 11 May 2022 01:47:31 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41322fae2f166bfab864c1f2f7d88cf2a82eb053bd0aad5627cad9948ede19c`  
		Last Modified: Wed, 11 May 2022 01:47:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3`

```console
$ docker pull couchdb@sha256:16739ea471ef700df680c43cad5cef4965a3468532f9d80f286f2c2033be60ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:8ea05770cacfc3e4293f6c6825c280bc49fc9e2358c81e671a3b9473a8792c7d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84525044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99d0cd0445244d76222a24265f1e3a6edf1b9d9334d2900418fe5639bb8e1d52`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:05:14 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 May 2022 02:05:15 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 May 2022 02:05:22 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:05:26 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 May 2022 02:05:26 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 May 2022 02:05:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:05:54 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 11 May 2022 02:05:55 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 May 2022 02:06:12 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 May 2022 02:06:13 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 11 May 2022 02:06:13 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 May 2022 02:06:13 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 11 May 2022 02:06:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 May 2022 02:06:14 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 May 2022 02:06:14 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 May 2022 02:06:14 GMT
EXPOSE 4369 5984 9100
# Wed, 11 May 2022 02:06:14 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d03d9847c338f80e8fbca52fd94a0a0aad2792cbe1341cc3fb6067a4ee567c5`  
		Last Modified: Wed, 11 May 2022 02:06:56 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2aee334c57e9fec0f83f4955b20262ce02650c108b878c73d7ccd9039b76c6a`  
		Last Modified: Wed, 11 May 2022 02:06:55 GMT  
		Size: 6.7 MB (6698559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c6798238438f93c309f2ad6c50de5f6fcf0aab2e17b5c902179e27d163a639`  
		Last Modified: Wed, 11 May 2022 02:06:54 GMT  
		Size: 1.3 MB (1258367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db74e747e5b05e04bffbfdaa41b5ad4a2db907a70aa1ab9902ef36fa7474482`  
		Last Modified: Wed, 11 May 2022 02:06:54 GMT  
		Size: 293.0 KB (293001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fbd90e3f7c935db6713aeb78963813c26419b896aa8202166e13851f5eaa52c`  
		Last Modified: Wed, 11 May 2022 02:07:08 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b215fdce3c26a6756a900982913487ee75db89a8739b8438f3f27f4a93c10f`  
		Last Modified: Wed, 11 May 2022 02:07:12 GMT  
		Size: 49.1 MB (49127385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d10b2297c1dfda106e356ce6e7a7ce214fb9e47225c79a37c273bc2d2d6e45b`  
		Last Modified: Wed, 11 May 2022 02:07:06 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5e42599e3dbcd331001f448fdb1a8ee10d0fbbf739549e082550bae490723b`  
		Last Modified: Wed, 11 May 2022 02:07:06 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d60aad0805e79cf9a6223c764013ce852942843a8b028e2d8243d6ed841e8e`  
		Last Modified: Wed, 11 May 2022 02:07:06 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1b84c4db843d2e00ef78f9a44fb16f3401b0161cc770ca96d94d310f400f48`  
		Last Modified: Wed, 11 May 2022 02:07:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:e73034e7e1fd3ab38e8093476d0376533314735436cafb87633c75926f5c924a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72527241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d88a2d4f99da857f9e233207ada61c8cc5504b032ce62387fea10cbe03300fb7`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 May 2022 00:47:26 GMT
ADD file:2536146c773d09db1a8fbbff00933acc459d8929feb3cff5b93ca4c23b577845 in / 
# Wed, 11 May 2022 00:47:26 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:45:11 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 May 2022 01:45:12 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 May 2022 01:45:20 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:45:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 May 2022 01:45:25 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 May 2022 01:45:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:46:03 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 11 May 2022 01:46:04 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 May 2022 01:46:18 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 May 2022 01:46:19 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 11 May 2022 01:46:20 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 May 2022 01:46:21 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 11 May 2022 01:46:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 May 2022 01:46:22 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 May 2022 01:46:23 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 May 2022 01:46:24 GMT
EXPOSE 4369 5984 9100
# Wed, 11 May 2022 01:46:25 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:383d573fdcf2c6da56fdb61e120549d7bc200471208ca4c7c6605c57a0a87ef6`  
		Last Modified: Wed, 11 May 2022 00:54:36 GMT  
		Size: 25.9 MB (25909014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a538c8ac927fa268f7107913c05d740399cce6245cc44b0f5cfd5fd14318434`  
		Last Modified: Wed, 11 May 2022 01:47:19 GMT  
		Size: 3.3 KB (3319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f730aee3592d57a6764bb9172710619552bf2c89fad6d64ac0056fbc02876266`  
		Last Modified: Wed, 11 May 2022 01:47:19 GMT  
		Size: 6.6 MB (6556393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c5923e32b1016f381ab756a45e1ce6897491277064f3d1fea69b0f0f22af0c`  
		Last Modified: Wed, 11 May 2022 01:47:18 GMT  
		Size: 951.2 KB (951181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff679ff3f207b333f7ea83a9b137230853a2a787b55b612885f192bba5f80719`  
		Last Modified: Wed, 11 May 2022 01:47:17 GMT  
		Size: 80.0 KB (79971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc333406fdaf9c77e64c600b3f138ddf28952951799f86525899401052f791e`  
		Last Modified: Wed, 11 May 2022 01:47:33 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93542b97e7d05d7c549d16a7af3b3605ac183e5c4b97eb3ed825fc2dcc82eb3`  
		Last Modified: Wed, 11 May 2022 01:47:36 GMT  
		Size: 39.0 MB (39023759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d2c966afb9941dc766e4098adef1d8c1cff34b720a920f454dde7c4c924dd0`  
		Last Modified: Wed, 11 May 2022 01:47:31 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68175c1f75bbcad6b45c984822604a02bd39276b9011108471c5e4bac76cca1`  
		Last Modified: Wed, 11 May 2022 01:47:31 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84cc361861fe639e5cd29a5a314024cae6c0e8ea0812cbc42a2a1157ce5a737c`  
		Last Modified: Wed, 11 May 2022 01:47:31 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41322fae2f166bfab864c1f2f7d88cf2a82eb053bd0aad5627cad9948ede19c`  
		Last Modified: Wed, 11 May 2022 01:47:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3.1`

```console
$ docker pull couchdb@sha256:16739ea471ef700df680c43cad5cef4965a3468532f9d80f286f2c2033be60ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:8ea05770cacfc3e4293f6c6825c280bc49fc9e2358c81e671a3b9473a8792c7d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84525044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99d0cd0445244d76222a24265f1e3a6edf1b9d9334d2900418fe5639bb8e1d52`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:05:14 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 May 2022 02:05:15 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 May 2022 02:05:22 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:05:26 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 May 2022 02:05:26 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 May 2022 02:05:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:05:54 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 11 May 2022 02:05:55 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 May 2022 02:06:12 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 May 2022 02:06:13 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 11 May 2022 02:06:13 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 May 2022 02:06:13 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 11 May 2022 02:06:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 May 2022 02:06:14 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 May 2022 02:06:14 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 May 2022 02:06:14 GMT
EXPOSE 4369 5984 9100
# Wed, 11 May 2022 02:06:14 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d03d9847c338f80e8fbca52fd94a0a0aad2792cbe1341cc3fb6067a4ee567c5`  
		Last Modified: Wed, 11 May 2022 02:06:56 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2aee334c57e9fec0f83f4955b20262ce02650c108b878c73d7ccd9039b76c6a`  
		Last Modified: Wed, 11 May 2022 02:06:55 GMT  
		Size: 6.7 MB (6698559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c6798238438f93c309f2ad6c50de5f6fcf0aab2e17b5c902179e27d163a639`  
		Last Modified: Wed, 11 May 2022 02:06:54 GMT  
		Size: 1.3 MB (1258367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db74e747e5b05e04bffbfdaa41b5ad4a2db907a70aa1ab9902ef36fa7474482`  
		Last Modified: Wed, 11 May 2022 02:06:54 GMT  
		Size: 293.0 KB (293001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fbd90e3f7c935db6713aeb78963813c26419b896aa8202166e13851f5eaa52c`  
		Last Modified: Wed, 11 May 2022 02:07:08 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b215fdce3c26a6756a900982913487ee75db89a8739b8438f3f27f4a93c10f`  
		Last Modified: Wed, 11 May 2022 02:07:12 GMT  
		Size: 49.1 MB (49127385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d10b2297c1dfda106e356ce6e7a7ce214fb9e47225c79a37c273bc2d2d6e45b`  
		Last Modified: Wed, 11 May 2022 02:07:06 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5e42599e3dbcd331001f448fdb1a8ee10d0fbbf739549e082550bae490723b`  
		Last Modified: Wed, 11 May 2022 02:07:06 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d60aad0805e79cf9a6223c764013ce852942843a8b028e2d8243d6ed841e8e`  
		Last Modified: Wed, 11 May 2022 02:07:06 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1b84c4db843d2e00ef78f9a44fb16f3401b0161cc770ca96d94d310f400f48`  
		Last Modified: Wed, 11 May 2022 02:07:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:e73034e7e1fd3ab38e8093476d0376533314735436cafb87633c75926f5c924a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72527241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d88a2d4f99da857f9e233207ada61c8cc5504b032ce62387fea10cbe03300fb7`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 May 2022 00:47:26 GMT
ADD file:2536146c773d09db1a8fbbff00933acc459d8929feb3cff5b93ca4c23b577845 in / 
# Wed, 11 May 2022 00:47:26 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:45:11 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 May 2022 01:45:12 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 May 2022 01:45:20 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:45:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 May 2022 01:45:25 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 May 2022 01:45:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:46:03 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 11 May 2022 01:46:04 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 May 2022 01:46:18 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 May 2022 01:46:19 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 11 May 2022 01:46:20 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 May 2022 01:46:21 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 11 May 2022 01:46:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 May 2022 01:46:22 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 May 2022 01:46:23 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 May 2022 01:46:24 GMT
EXPOSE 4369 5984 9100
# Wed, 11 May 2022 01:46:25 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:383d573fdcf2c6da56fdb61e120549d7bc200471208ca4c7c6605c57a0a87ef6`  
		Last Modified: Wed, 11 May 2022 00:54:36 GMT  
		Size: 25.9 MB (25909014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a538c8ac927fa268f7107913c05d740399cce6245cc44b0f5cfd5fd14318434`  
		Last Modified: Wed, 11 May 2022 01:47:19 GMT  
		Size: 3.3 KB (3319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f730aee3592d57a6764bb9172710619552bf2c89fad6d64ac0056fbc02876266`  
		Last Modified: Wed, 11 May 2022 01:47:19 GMT  
		Size: 6.6 MB (6556393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c5923e32b1016f381ab756a45e1ce6897491277064f3d1fea69b0f0f22af0c`  
		Last Modified: Wed, 11 May 2022 01:47:18 GMT  
		Size: 951.2 KB (951181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff679ff3f207b333f7ea83a9b137230853a2a787b55b612885f192bba5f80719`  
		Last Modified: Wed, 11 May 2022 01:47:17 GMT  
		Size: 80.0 KB (79971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc333406fdaf9c77e64c600b3f138ddf28952951799f86525899401052f791e`  
		Last Modified: Wed, 11 May 2022 01:47:33 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93542b97e7d05d7c549d16a7af3b3605ac183e5c4b97eb3ed825fc2dcc82eb3`  
		Last Modified: Wed, 11 May 2022 01:47:36 GMT  
		Size: 39.0 MB (39023759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d2c966afb9941dc766e4098adef1d8c1cff34b720a920f454dde7c4c924dd0`  
		Last Modified: Wed, 11 May 2022 01:47:31 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68175c1f75bbcad6b45c984822604a02bd39276b9011108471c5e4bac76cca1`  
		Last Modified: Wed, 11 May 2022 01:47:31 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84cc361861fe639e5cd29a5a314024cae6c0e8ea0812cbc42a2a1157ce5a737c`  
		Last Modified: Wed, 11 May 2022 01:47:31 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41322fae2f166bfab864c1f2f7d88cf2a82eb053bd0aad5627cad9948ede19c`  
		Last Modified: Wed, 11 May 2022 01:47:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3`

```console
$ docker pull couchdb@sha256:cc42149ff90acd44ebeaa67d99f5a66168d5dce3f053f605c68a2bc1a545062d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3` - linux; amd64

```console
$ docker pull couchdb@sha256:0e9eb882ea5cc96a465b9f4cfe311e0ac5cbd015ea1590651698131e527ff14e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87498752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c0a436cab577526883ce8f439fb5f63e16b150745e7d3d0aac1f2335c2ae6dc`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:04:40 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 May 2022 02:04:41 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 May 2022 02:04:48 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:04:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 May 2022 02:04:52 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 May 2022 02:04:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:04:57 GMT
ENV COUCHDB_VERSION=3.2.2
# Wed, 11 May 2022 02:04:57 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 May 2022 02:05:10 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 May 2022 02:05:10 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 11 May 2022 02:05:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 May 2022 02:05:11 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 11 May 2022 02:05:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 May 2022 02:05:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 May 2022 02:05:11 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 May 2022 02:05:11 GMT
EXPOSE 4369 5984 9100
# Wed, 11 May 2022 02:05:12 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ee85690522b1a5c1c261140c51987cedd0ac69838cd6a247cebfdb741dc209`  
		Last Modified: Wed, 11 May 2022 02:06:34 GMT  
		Size: 3.4 KB (3408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31e683cf3744502c13dc5eed428041c4403dba7b657bdf4baf1f62fb9a14d81`  
		Last Modified: Wed, 11 May 2022 02:06:33 GMT  
		Size: 5.2 MB (5223783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69184d8d2d701731278588e13e3acf0736dce829ac7b16d288ffb5f4a9b50641`  
		Last Modified: Wed, 11 May 2022 02:06:32 GMT  
		Size: 1.6 MB (1553317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7ff2bf2271e33167f12be0e13e1c8e7e4f51d1df70857d5b333fa43ca0f16b`  
		Last Modified: Wed, 11 May 2022 02:06:32 GMT  
		Size: 295.6 KB (295594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad60259958773deb0d46469b50bd923b25d0896ad625ad0935296d2f8d3122f`  
		Last Modified: Wed, 11 May 2022 02:06:31 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf925925077913e0bc336f89aad09bdcec3d9c03b334a07aa388a9da3a9a257b`  
		Last Modified: Wed, 11 May 2022 02:06:35 GMT  
		Size: 49.0 MB (49039446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8473eb1b9790d6b877a07f65baf502d2f00a6edcaa3858b32a939b215a7dba4b`  
		Last Modified: Wed, 11 May 2022 02:06:29 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c6a25d70616f8170336fb950a3a20bf9df514af10af91f7bd211600ec4eee6`  
		Last Modified: Wed, 11 May 2022 02:06:29 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c635531529db21d489424dc255b4b23d41ff1e6e0f1e76244f1770e014cf669d`  
		Last Modified: Wed, 11 May 2022 02:06:29 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0891e5f9c83ee343beb2d0a6ba6fdff9de433d0320a52233f0cde8e96cecc14c`  
		Last Modified: Wed, 11 May 2022 02:06:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:3776e5f2efb49f384e95d61f3603be387b3fb92f893fe67826bb10cd18517b2b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.4 MB (85427129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6b75ff4bc043175bdce94848a541cac230db909ca76f0784ea402fd2adbcab2`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:44:19 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 May 2022 01:44:20 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 May 2022 01:44:28 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:44:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 May 2022 01:44:33 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 May 2022 01:44:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:44:39 GMT
ENV COUCHDB_VERSION=3.2.2
# Wed, 11 May 2022 01:44:40 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 May 2022 01:44:54 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 May 2022 01:44:55 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 11 May 2022 01:44:56 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 May 2022 01:44:57 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 11 May 2022 01:44:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 May 2022 01:44:58 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 May 2022 01:44:59 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 May 2022 01:45:00 GMT
EXPOSE 4369 5984 9100
# Wed, 11 May 2022 01:45:01 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47eb3485a7f2023d85cb0dfb1e9a9be50f468e36f59ddda7f690c6dc8591bd2`  
		Last Modified: Wed, 11 May 2022 01:46:56 GMT  
		Size: 3.3 KB (3319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99b0f84bc54cbbaac226062cb40e48f71aab04071b0bfd3af4fc288f94024e1`  
		Last Modified: Wed, 11 May 2022 01:46:55 GMT  
		Size: 5.0 MB (5002969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932e35e02ef3eb4b94b90ee78ba1e0b543f48dedd24db2faf0a44df657b24d21`  
		Last Modified: Wed, 11 May 2022 01:46:54 GMT  
		Size: 1.2 MB (1221128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872a013b49f66bfa1e40fe5757aa1641024e14a1c0281bb5040bddba42cd62a8`  
		Last Modified: Wed, 11 May 2022 01:46:53 GMT  
		Size: 79.2 KB (79185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51202850aa4bf5caba027daccada9694f98b470cebb8bcff7f6a5914554be62b`  
		Last Modified: Wed, 11 May 2022 01:46:53 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7208b445d3203b59e4444f334cdee31b019bca4d629045af4f702cfba8ccaf17`  
		Last Modified: Wed, 11 May 2022 01:46:56 GMT  
		Size: 49.1 MB (49051109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff350ded2de4fac19a6141c701f1ea3f8c665112641799a54e6cbdc9bc9e3fcf`  
		Last Modified: Wed, 11 May 2022 01:46:51 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d554e59a0648821bbcfbc62ec3524ec7b029f0474f79b1a63d09e6f46fd6649`  
		Last Modified: Wed, 11 May 2022 01:46:51 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae08ec0a016ada08c1003b1769bd753e53e80762f97ff2bf74c691e5ee2a9213`  
		Last Modified: Wed, 11 May 2022 01:46:52 GMT  
		Size: 2.2 KB (2182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf16752e43a4c99f036c8d532b1a58d944edfe892065e7ab4328077b5e02257e`  
		Last Modified: Wed, 11 May 2022 01:46:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; ppc64le

```console
$ docker pull couchdb@sha256:2774d021f2ec7122da9a2d24c153e70c92bbff47c8608c8c99f681447ec30dd1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93223893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbd6b0d3fe9a02e0fa3d5ef15549a3ec8c4f6909334bfe85b6737c3421c53899`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 May 2022 01:32:29 GMT
ADD file:1e94716789ec21981460f74be38a668bc212bd804c1d41cecf90036a5bccac5a in / 
# Wed, 11 May 2022 01:32:34 GMT
CMD ["bash"]
# Wed, 11 May 2022 03:53:11 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 May 2022 03:53:23 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 May 2022 03:54:51 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:55:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 May 2022 03:55:27 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 May 2022 03:56:34 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:56:40 GMT
ENV COUCHDB_VERSION=3.2.2
# Wed, 11 May 2022 03:56:59 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 May 2022 03:58:23 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 May 2022 03:58:28 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 11 May 2022 03:58:34 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 May 2022 03:58:40 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 11 May 2022 03:58:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 May 2022 03:58:56 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 May 2022 03:58:59 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 May 2022 03:59:03 GMT
EXPOSE 4369 5984 9100
# Wed, 11 May 2022 03:59:08 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:2533109ed11eefd6415e0370d6d7a3ea879b582b1887c98b819a598ad18fca24`  
		Last Modified: Wed, 11 May 2022 01:43:03 GMT  
		Size: 35.3 MB (35286467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62610198665bf7ba0256e568d5b533eb4e86ea7f0d929be775a0edf50ebe6dc1`  
		Last Modified: Wed, 11 May 2022 03:59:43 GMT  
		Size: 3.4 KB (3420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924366ccb76483e136508811146cb69efe23b89757b2bd2275986b5774755ad0`  
		Last Modified: Wed, 11 May 2022 03:59:42 GMT  
		Size: 6.0 MB (6043834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e66a4e119d34d65b8c9643522e2c01733a94e0e8597177f4147500a9378efcd9`  
		Last Modified: Wed, 11 May 2022 03:59:41 GMT  
		Size: 1.5 MB (1509406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49dbb3458296e8bed85cdb20ce2cdf724d7d32d1cad906bbfab48f30a0e33c3d`  
		Last Modified: Wed, 11 May 2022 03:59:40 GMT  
		Size: 295.8 KB (295806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c39bf83571d20caef422c066a90fe7046ae845342df092c85e52e4a41b551f`  
		Last Modified: Wed, 11 May 2022 03:59:40 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f869c09e50b754b4b85542688e149abd8b44f5fd83675ef3302efc7d19841fa`  
		Last Modified: Wed, 11 May 2022 03:59:44 GMT  
		Size: 50.1 MB (50081223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d9045ae6ae651b94c46fbd30c331cbc0ed8744fb4f74457e84bca35db4f535`  
		Last Modified: Wed, 11 May 2022 03:59:37 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86d7cc3cfc58048e044f5d8a637fceda45c5512800db339db878ee4985d2f43`  
		Last Modified: Wed, 11 May 2022 03:59:36 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4181a6fd70115927a806d685a3235d0e0e80b50449a8ee03840b960bf5924173`  
		Last Modified: Wed, 11 May 2022 03:59:36 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6343a3495bb02e302378fb4d0983462a14d9398bdac27e9d30d3f18e4ebe59bc`  
		Last Modified: Wed, 11 May 2022 03:59:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1`

```console
$ docker pull couchdb@sha256:458e0159318d667ffbdb778898a73be3473ceafe4c8d02116b294cc8555492f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:8a38931c6b72aedee1bf8a5458a032428fed8d6795366128f6d260f3615d4c83
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80009871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d2e02774cef1df6b4e51e93fad904bdc23e2a13e42df537c23e681068cddc1a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:05:14 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 May 2022 02:05:15 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 May 2022 02:05:22 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:05:26 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 May 2022 02:05:26 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 May 2022 02:05:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:05:32 GMT
ENV COUCHDB_VERSION=3.1.2
# Wed, 11 May 2022 02:05:33 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 May 2022 02:05:46 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 May 2022 02:05:46 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 11 May 2022 02:05:46 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 May 2022 02:05:46 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 11 May 2022 02:05:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 May 2022 02:05:47 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 May 2022 02:05:47 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 May 2022 02:05:47 GMT
EXPOSE 4369 5984 9100
# Wed, 11 May 2022 02:05:47 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d03d9847c338f80e8fbca52fd94a0a0aad2792cbe1341cc3fb6067a4ee567c5`  
		Last Modified: Wed, 11 May 2022 02:06:56 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2aee334c57e9fec0f83f4955b20262ce02650c108b878c73d7ccd9039b76c6a`  
		Last Modified: Wed, 11 May 2022 02:06:55 GMT  
		Size: 6.7 MB (6698559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c6798238438f93c309f2ad6c50de5f6fcf0aab2e17b5c902179e27d163a639`  
		Last Modified: Wed, 11 May 2022 02:06:54 GMT  
		Size: 1.3 MB (1258367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db74e747e5b05e04bffbfdaa41b5ad4a2db907a70aa1ab9902ef36fa7474482`  
		Last Modified: Wed, 11 May 2022 02:06:54 GMT  
		Size: 293.0 KB (293001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a8588c0372f1849a87febfe18c3d0888267b14d36f5affe2e37c6df038792e`  
		Last Modified: Wed, 11 May 2022 02:06:53 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9fe15d90f0465f9899ba1faa24de69fd7f5dd734a1a9d2e44367879a042f6de`  
		Last Modified: Wed, 11 May 2022 02:06:56 GMT  
		Size: 44.6 MB (44612218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd5afc1db0326deb0c311415199cc21433431521b08e27dc3fed00801a1729e`  
		Last Modified: Wed, 11 May 2022 02:06:51 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2608973a6eabea97da9b1cfd1163a8f145ed272151bc287a03e9cd05d3fff4b3`  
		Last Modified: Wed, 11 May 2022 02:06:51 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad702d4eb5b42e93540eecbec19b75c2243683bfa39aafc8260a23ec049c8c6`  
		Last Modified: Wed, 11 May 2022 02:06:51 GMT  
		Size: 2.1 KB (2056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd823b0c9570186ccc5ec4084198c41d70aaf620389db4ddfc8b2e8393e00d3c`  
		Last Modified: Wed, 11 May 2022 02:06:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:804d8a06c7228d2114fadd186abb2385965f4196878c02752e084c9121a28966
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74615962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33e7db78756b4224bf45be22c38b148bfc00592f30d2b053d005026a9a46bf38`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 May 2022 00:47:26 GMT
ADD file:2536146c773d09db1a8fbbff00933acc459d8929feb3cff5b93ca4c23b577845 in / 
# Wed, 11 May 2022 00:47:26 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:45:11 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 May 2022 01:45:12 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 May 2022 01:45:20 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:45:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 May 2022 01:45:25 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 May 2022 01:45:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:45:32 GMT
ENV COUCHDB_VERSION=3.1.2
# Wed, 11 May 2022 01:45:33 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 May 2022 01:45:51 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 May 2022 01:45:52 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 11 May 2022 01:45:53 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 May 2022 01:45:54 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 11 May 2022 01:45:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 May 2022 01:45:55 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 May 2022 01:45:56 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 May 2022 01:45:57 GMT
EXPOSE 4369 5984 9100
# Wed, 11 May 2022 01:45:58 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:383d573fdcf2c6da56fdb61e120549d7bc200471208ca4c7c6605c57a0a87ef6`  
		Last Modified: Wed, 11 May 2022 00:54:36 GMT  
		Size: 25.9 MB (25909014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a538c8ac927fa268f7107913c05d740399cce6245cc44b0f5cfd5fd14318434`  
		Last Modified: Wed, 11 May 2022 01:47:19 GMT  
		Size: 3.3 KB (3319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f730aee3592d57a6764bb9172710619552bf2c89fad6d64ac0056fbc02876266`  
		Last Modified: Wed, 11 May 2022 01:47:19 GMT  
		Size: 6.6 MB (6556393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c5923e32b1016f381ab756a45e1ce6897491277064f3d1fea69b0f0f22af0c`  
		Last Modified: Wed, 11 May 2022 01:47:18 GMT  
		Size: 951.2 KB (951181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff679ff3f207b333f7ea83a9b137230853a2a787b55b612885f192bba5f80719`  
		Last Modified: Wed, 11 May 2022 01:47:17 GMT  
		Size: 80.0 KB (79971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b682d34c8619c23fa255ba66b10b06e2a2b8544ee3cdc675441f8776b2f2d69b`  
		Last Modified: Wed, 11 May 2022 01:47:17 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a329ee1144ab0f0c8654a6eb74e3488fae5648a20149fb9bb3b9b8b5e54e54b`  
		Last Modified: Wed, 11 May 2022 01:47:20 GMT  
		Size: 41.1 MB (41112483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e443361821ceffdac2fec5be9e41e9fb3d3ee4bf10a531af7c7b916a27ad42`  
		Last Modified: Wed, 11 May 2022 01:47:15 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6235edec13b8364bd2c7f1436e0f62c0ee0916fb5b85da492bd264e339769a37`  
		Last Modified: Wed, 11 May 2022 01:47:15 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eec979d587d510e7dc6c589f9791e99ece8f9c4a1853e4a17eed4ed06d8ac76`  
		Last Modified: Wed, 11 May 2022 01:47:15 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b677236d1bbc09479e7ff2c74c64ecb335a15070b7d0b3163cb9d0995461b00c`  
		Last Modified: Wed, 11 May 2022 01:47:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1.2`

```console
$ docker pull couchdb@sha256:458e0159318d667ffbdb778898a73be3473ceafe4c8d02116b294cc8555492f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1.2` - linux; amd64

```console
$ docker pull couchdb@sha256:8a38931c6b72aedee1bf8a5458a032428fed8d6795366128f6d260f3615d4c83
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80009871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d2e02774cef1df6b4e51e93fad904bdc23e2a13e42df537c23e681068cddc1a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:05:14 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 May 2022 02:05:15 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 May 2022 02:05:22 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:05:26 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 May 2022 02:05:26 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 May 2022 02:05:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:05:32 GMT
ENV COUCHDB_VERSION=3.1.2
# Wed, 11 May 2022 02:05:33 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 May 2022 02:05:46 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 May 2022 02:05:46 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 11 May 2022 02:05:46 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 May 2022 02:05:46 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 11 May 2022 02:05:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 May 2022 02:05:47 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 May 2022 02:05:47 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 May 2022 02:05:47 GMT
EXPOSE 4369 5984 9100
# Wed, 11 May 2022 02:05:47 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d03d9847c338f80e8fbca52fd94a0a0aad2792cbe1341cc3fb6067a4ee567c5`  
		Last Modified: Wed, 11 May 2022 02:06:56 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2aee334c57e9fec0f83f4955b20262ce02650c108b878c73d7ccd9039b76c6a`  
		Last Modified: Wed, 11 May 2022 02:06:55 GMT  
		Size: 6.7 MB (6698559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c6798238438f93c309f2ad6c50de5f6fcf0aab2e17b5c902179e27d163a639`  
		Last Modified: Wed, 11 May 2022 02:06:54 GMT  
		Size: 1.3 MB (1258367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db74e747e5b05e04bffbfdaa41b5ad4a2db907a70aa1ab9902ef36fa7474482`  
		Last Modified: Wed, 11 May 2022 02:06:54 GMT  
		Size: 293.0 KB (293001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a8588c0372f1849a87febfe18c3d0888267b14d36f5affe2e37c6df038792e`  
		Last Modified: Wed, 11 May 2022 02:06:53 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9fe15d90f0465f9899ba1faa24de69fd7f5dd734a1a9d2e44367879a042f6de`  
		Last Modified: Wed, 11 May 2022 02:06:56 GMT  
		Size: 44.6 MB (44612218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd5afc1db0326deb0c311415199cc21433431521b08e27dc3fed00801a1729e`  
		Last Modified: Wed, 11 May 2022 02:06:51 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2608973a6eabea97da9b1cfd1163a8f145ed272151bc287a03e9cd05d3fff4b3`  
		Last Modified: Wed, 11 May 2022 02:06:51 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad702d4eb5b42e93540eecbec19b75c2243683bfa39aafc8260a23ec049c8c6`  
		Last Modified: Wed, 11 May 2022 02:06:51 GMT  
		Size: 2.1 KB (2056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd823b0c9570186ccc5ec4084198c41d70aaf620389db4ddfc8b2e8393e00d3c`  
		Last Modified: Wed, 11 May 2022 02:06:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:804d8a06c7228d2114fadd186abb2385965f4196878c02752e084c9121a28966
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74615962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33e7db78756b4224bf45be22c38b148bfc00592f30d2b053d005026a9a46bf38`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 May 2022 00:47:26 GMT
ADD file:2536146c773d09db1a8fbbff00933acc459d8929feb3cff5b93ca4c23b577845 in / 
# Wed, 11 May 2022 00:47:26 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:45:11 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 May 2022 01:45:12 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 May 2022 01:45:20 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:45:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 May 2022 01:45:25 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 May 2022 01:45:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:45:32 GMT
ENV COUCHDB_VERSION=3.1.2
# Wed, 11 May 2022 01:45:33 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 May 2022 01:45:51 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 May 2022 01:45:52 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 11 May 2022 01:45:53 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 May 2022 01:45:54 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 11 May 2022 01:45:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 May 2022 01:45:55 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 May 2022 01:45:56 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 May 2022 01:45:57 GMT
EXPOSE 4369 5984 9100
# Wed, 11 May 2022 01:45:58 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:383d573fdcf2c6da56fdb61e120549d7bc200471208ca4c7c6605c57a0a87ef6`  
		Last Modified: Wed, 11 May 2022 00:54:36 GMT  
		Size: 25.9 MB (25909014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a538c8ac927fa268f7107913c05d740399cce6245cc44b0f5cfd5fd14318434`  
		Last Modified: Wed, 11 May 2022 01:47:19 GMT  
		Size: 3.3 KB (3319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f730aee3592d57a6764bb9172710619552bf2c89fad6d64ac0056fbc02876266`  
		Last Modified: Wed, 11 May 2022 01:47:19 GMT  
		Size: 6.6 MB (6556393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c5923e32b1016f381ab756a45e1ce6897491277064f3d1fea69b0f0f22af0c`  
		Last Modified: Wed, 11 May 2022 01:47:18 GMT  
		Size: 951.2 KB (951181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff679ff3f207b333f7ea83a9b137230853a2a787b55b612885f192bba5f80719`  
		Last Modified: Wed, 11 May 2022 01:47:17 GMT  
		Size: 80.0 KB (79971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b682d34c8619c23fa255ba66b10b06e2a2b8544ee3cdc675441f8776b2f2d69b`  
		Last Modified: Wed, 11 May 2022 01:47:17 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a329ee1144ab0f0c8654a6eb74e3488fae5648a20149fb9bb3b9b8b5e54e54b`  
		Last Modified: Wed, 11 May 2022 01:47:20 GMT  
		Size: 41.1 MB (41112483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e443361821ceffdac2fec5be9e41e9fb3d3ee4bf10a531af7c7b916a27ad42`  
		Last Modified: Wed, 11 May 2022 01:47:15 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6235edec13b8364bd2c7f1436e0f62c0ee0916fb5b85da492bd264e339769a37`  
		Last Modified: Wed, 11 May 2022 01:47:15 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eec979d587d510e7dc6c589f9791e99ece8f9c4a1853e4a17eed4ed06d8ac76`  
		Last Modified: Wed, 11 May 2022 01:47:15 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b677236d1bbc09479e7ff2c74c64ecb335a15070b7d0b3163cb9d0995461b00c`  
		Last Modified: Wed, 11 May 2022 01:47:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2`

```console
$ docker pull couchdb@sha256:cc42149ff90acd44ebeaa67d99f5a66168d5dce3f053f605c68a2bc1a545062d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2` - linux; amd64

```console
$ docker pull couchdb@sha256:0e9eb882ea5cc96a465b9f4cfe311e0ac5cbd015ea1590651698131e527ff14e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87498752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c0a436cab577526883ce8f439fb5f63e16b150745e7d3d0aac1f2335c2ae6dc`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:04:40 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 May 2022 02:04:41 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 May 2022 02:04:48 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:04:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 May 2022 02:04:52 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 May 2022 02:04:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:04:57 GMT
ENV COUCHDB_VERSION=3.2.2
# Wed, 11 May 2022 02:04:57 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 May 2022 02:05:10 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 May 2022 02:05:10 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 11 May 2022 02:05:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 May 2022 02:05:11 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 11 May 2022 02:05:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 May 2022 02:05:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 May 2022 02:05:11 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 May 2022 02:05:11 GMT
EXPOSE 4369 5984 9100
# Wed, 11 May 2022 02:05:12 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ee85690522b1a5c1c261140c51987cedd0ac69838cd6a247cebfdb741dc209`  
		Last Modified: Wed, 11 May 2022 02:06:34 GMT  
		Size: 3.4 KB (3408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31e683cf3744502c13dc5eed428041c4403dba7b657bdf4baf1f62fb9a14d81`  
		Last Modified: Wed, 11 May 2022 02:06:33 GMT  
		Size: 5.2 MB (5223783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69184d8d2d701731278588e13e3acf0736dce829ac7b16d288ffb5f4a9b50641`  
		Last Modified: Wed, 11 May 2022 02:06:32 GMT  
		Size: 1.6 MB (1553317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7ff2bf2271e33167f12be0e13e1c8e7e4f51d1df70857d5b333fa43ca0f16b`  
		Last Modified: Wed, 11 May 2022 02:06:32 GMT  
		Size: 295.6 KB (295594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad60259958773deb0d46469b50bd923b25d0896ad625ad0935296d2f8d3122f`  
		Last Modified: Wed, 11 May 2022 02:06:31 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf925925077913e0bc336f89aad09bdcec3d9c03b334a07aa388a9da3a9a257b`  
		Last Modified: Wed, 11 May 2022 02:06:35 GMT  
		Size: 49.0 MB (49039446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8473eb1b9790d6b877a07f65baf502d2f00a6edcaa3858b32a939b215a7dba4b`  
		Last Modified: Wed, 11 May 2022 02:06:29 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c6a25d70616f8170336fb950a3a20bf9df514af10af91f7bd211600ec4eee6`  
		Last Modified: Wed, 11 May 2022 02:06:29 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c635531529db21d489424dc255b4b23d41ff1e6e0f1e76244f1770e014cf669d`  
		Last Modified: Wed, 11 May 2022 02:06:29 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0891e5f9c83ee343beb2d0a6ba6fdff9de433d0320a52233f0cde8e96cecc14c`  
		Last Modified: Wed, 11 May 2022 02:06:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:3776e5f2efb49f384e95d61f3603be387b3fb92f893fe67826bb10cd18517b2b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.4 MB (85427129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6b75ff4bc043175bdce94848a541cac230db909ca76f0784ea402fd2adbcab2`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:44:19 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 May 2022 01:44:20 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 May 2022 01:44:28 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:44:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 May 2022 01:44:33 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 May 2022 01:44:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:44:39 GMT
ENV COUCHDB_VERSION=3.2.2
# Wed, 11 May 2022 01:44:40 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 May 2022 01:44:54 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 May 2022 01:44:55 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 11 May 2022 01:44:56 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 May 2022 01:44:57 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 11 May 2022 01:44:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 May 2022 01:44:58 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 May 2022 01:44:59 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 May 2022 01:45:00 GMT
EXPOSE 4369 5984 9100
# Wed, 11 May 2022 01:45:01 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47eb3485a7f2023d85cb0dfb1e9a9be50f468e36f59ddda7f690c6dc8591bd2`  
		Last Modified: Wed, 11 May 2022 01:46:56 GMT  
		Size: 3.3 KB (3319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99b0f84bc54cbbaac226062cb40e48f71aab04071b0bfd3af4fc288f94024e1`  
		Last Modified: Wed, 11 May 2022 01:46:55 GMT  
		Size: 5.0 MB (5002969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932e35e02ef3eb4b94b90ee78ba1e0b543f48dedd24db2faf0a44df657b24d21`  
		Last Modified: Wed, 11 May 2022 01:46:54 GMT  
		Size: 1.2 MB (1221128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872a013b49f66bfa1e40fe5757aa1641024e14a1c0281bb5040bddba42cd62a8`  
		Last Modified: Wed, 11 May 2022 01:46:53 GMT  
		Size: 79.2 KB (79185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51202850aa4bf5caba027daccada9694f98b470cebb8bcff7f6a5914554be62b`  
		Last Modified: Wed, 11 May 2022 01:46:53 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7208b445d3203b59e4444f334cdee31b019bca4d629045af4f702cfba8ccaf17`  
		Last Modified: Wed, 11 May 2022 01:46:56 GMT  
		Size: 49.1 MB (49051109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff350ded2de4fac19a6141c701f1ea3f8c665112641799a54e6cbdc9bc9e3fcf`  
		Last Modified: Wed, 11 May 2022 01:46:51 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d554e59a0648821bbcfbc62ec3524ec7b029f0474f79b1a63d09e6f46fd6649`  
		Last Modified: Wed, 11 May 2022 01:46:51 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae08ec0a016ada08c1003b1769bd753e53e80762f97ff2bf74c691e5ee2a9213`  
		Last Modified: Wed, 11 May 2022 01:46:52 GMT  
		Size: 2.2 KB (2182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf16752e43a4c99f036c8d532b1a58d944edfe892065e7ab4328077b5e02257e`  
		Last Modified: Wed, 11 May 2022 01:46:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; ppc64le

```console
$ docker pull couchdb@sha256:2774d021f2ec7122da9a2d24c153e70c92bbff47c8608c8c99f681447ec30dd1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93223893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbd6b0d3fe9a02e0fa3d5ef15549a3ec8c4f6909334bfe85b6737c3421c53899`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 May 2022 01:32:29 GMT
ADD file:1e94716789ec21981460f74be38a668bc212bd804c1d41cecf90036a5bccac5a in / 
# Wed, 11 May 2022 01:32:34 GMT
CMD ["bash"]
# Wed, 11 May 2022 03:53:11 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 May 2022 03:53:23 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 May 2022 03:54:51 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:55:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 May 2022 03:55:27 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 May 2022 03:56:34 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:56:40 GMT
ENV COUCHDB_VERSION=3.2.2
# Wed, 11 May 2022 03:56:59 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 May 2022 03:58:23 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 May 2022 03:58:28 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 11 May 2022 03:58:34 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 May 2022 03:58:40 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 11 May 2022 03:58:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 May 2022 03:58:56 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 May 2022 03:58:59 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 May 2022 03:59:03 GMT
EXPOSE 4369 5984 9100
# Wed, 11 May 2022 03:59:08 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:2533109ed11eefd6415e0370d6d7a3ea879b582b1887c98b819a598ad18fca24`  
		Last Modified: Wed, 11 May 2022 01:43:03 GMT  
		Size: 35.3 MB (35286467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62610198665bf7ba0256e568d5b533eb4e86ea7f0d929be775a0edf50ebe6dc1`  
		Last Modified: Wed, 11 May 2022 03:59:43 GMT  
		Size: 3.4 KB (3420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924366ccb76483e136508811146cb69efe23b89757b2bd2275986b5774755ad0`  
		Last Modified: Wed, 11 May 2022 03:59:42 GMT  
		Size: 6.0 MB (6043834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e66a4e119d34d65b8c9643522e2c01733a94e0e8597177f4147500a9378efcd9`  
		Last Modified: Wed, 11 May 2022 03:59:41 GMT  
		Size: 1.5 MB (1509406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49dbb3458296e8bed85cdb20ce2cdf724d7d32d1cad906bbfab48f30a0e33c3d`  
		Last Modified: Wed, 11 May 2022 03:59:40 GMT  
		Size: 295.8 KB (295806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c39bf83571d20caef422c066a90fe7046ae845342df092c85e52e4a41b551f`  
		Last Modified: Wed, 11 May 2022 03:59:40 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f869c09e50b754b4b85542688e149abd8b44f5fd83675ef3302efc7d19841fa`  
		Last Modified: Wed, 11 May 2022 03:59:44 GMT  
		Size: 50.1 MB (50081223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d9045ae6ae651b94c46fbd30c331cbc0ed8744fb4f74457e84bca35db4f535`  
		Last Modified: Wed, 11 May 2022 03:59:37 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86d7cc3cfc58048e044f5d8a637fceda45c5512800db339db878ee4985d2f43`  
		Last Modified: Wed, 11 May 2022 03:59:36 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4181a6fd70115927a806d685a3235d0e0e80b50449a8ee03840b960bf5924173`  
		Last Modified: Wed, 11 May 2022 03:59:36 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6343a3495bb02e302378fb4d0983462a14d9398bdac27e9d30d3f18e4ebe59bc`  
		Last Modified: Wed, 11 May 2022 03:59:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2.2`

```console
$ docker pull couchdb@sha256:cc42149ff90acd44ebeaa67d99f5a66168d5dce3f053f605c68a2bc1a545062d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2.2` - linux; amd64

```console
$ docker pull couchdb@sha256:0e9eb882ea5cc96a465b9f4cfe311e0ac5cbd015ea1590651698131e527ff14e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87498752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c0a436cab577526883ce8f439fb5f63e16b150745e7d3d0aac1f2335c2ae6dc`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:04:40 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 May 2022 02:04:41 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 May 2022 02:04:48 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:04:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 May 2022 02:04:52 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 May 2022 02:04:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:04:57 GMT
ENV COUCHDB_VERSION=3.2.2
# Wed, 11 May 2022 02:04:57 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 May 2022 02:05:10 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 May 2022 02:05:10 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 11 May 2022 02:05:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 May 2022 02:05:11 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 11 May 2022 02:05:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 May 2022 02:05:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 May 2022 02:05:11 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 May 2022 02:05:11 GMT
EXPOSE 4369 5984 9100
# Wed, 11 May 2022 02:05:12 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ee85690522b1a5c1c261140c51987cedd0ac69838cd6a247cebfdb741dc209`  
		Last Modified: Wed, 11 May 2022 02:06:34 GMT  
		Size: 3.4 KB (3408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31e683cf3744502c13dc5eed428041c4403dba7b657bdf4baf1f62fb9a14d81`  
		Last Modified: Wed, 11 May 2022 02:06:33 GMT  
		Size: 5.2 MB (5223783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69184d8d2d701731278588e13e3acf0736dce829ac7b16d288ffb5f4a9b50641`  
		Last Modified: Wed, 11 May 2022 02:06:32 GMT  
		Size: 1.6 MB (1553317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7ff2bf2271e33167f12be0e13e1c8e7e4f51d1df70857d5b333fa43ca0f16b`  
		Last Modified: Wed, 11 May 2022 02:06:32 GMT  
		Size: 295.6 KB (295594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad60259958773deb0d46469b50bd923b25d0896ad625ad0935296d2f8d3122f`  
		Last Modified: Wed, 11 May 2022 02:06:31 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf925925077913e0bc336f89aad09bdcec3d9c03b334a07aa388a9da3a9a257b`  
		Last Modified: Wed, 11 May 2022 02:06:35 GMT  
		Size: 49.0 MB (49039446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8473eb1b9790d6b877a07f65baf502d2f00a6edcaa3858b32a939b215a7dba4b`  
		Last Modified: Wed, 11 May 2022 02:06:29 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c6a25d70616f8170336fb950a3a20bf9df514af10af91f7bd211600ec4eee6`  
		Last Modified: Wed, 11 May 2022 02:06:29 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c635531529db21d489424dc255b4b23d41ff1e6e0f1e76244f1770e014cf669d`  
		Last Modified: Wed, 11 May 2022 02:06:29 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0891e5f9c83ee343beb2d0a6ba6fdff9de433d0320a52233f0cde8e96cecc14c`  
		Last Modified: Wed, 11 May 2022 02:06:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:3776e5f2efb49f384e95d61f3603be387b3fb92f893fe67826bb10cd18517b2b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.4 MB (85427129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6b75ff4bc043175bdce94848a541cac230db909ca76f0784ea402fd2adbcab2`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:44:19 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 May 2022 01:44:20 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 May 2022 01:44:28 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:44:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 May 2022 01:44:33 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 May 2022 01:44:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:44:39 GMT
ENV COUCHDB_VERSION=3.2.2
# Wed, 11 May 2022 01:44:40 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 May 2022 01:44:54 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 May 2022 01:44:55 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 11 May 2022 01:44:56 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 May 2022 01:44:57 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 11 May 2022 01:44:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 May 2022 01:44:58 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 May 2022 01:44:59 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 May 2022 01:45:00 GMT
EXPOSE 4369 5984 9100
# Wed, 11 May 2022 01:45:01 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47eb3485a7f2023d85cb0dfb1e9a9be50f468e36f59ddda7f690c6dc8591bd2`  
		Last Modified: Wed, 11 May 2022 01:46:56 GMT  
		Size: 3.3 KB (3319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99b0f84bc54cbbaac226062cb40e48f71aab04071b0bfd3af4fc288f94024e1`  
		Last Modified: Wed, 11 May 2022 01:46:55 GMT  
		Size: 5.0 MB (5002969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932e35e02ef3eb4b94b90ee78ba1e0b543f48dedd24db2faf0a44df657b24d21`  
		Last Modified: Wed, 11 May 2022 01:46:54 GMT  
		Size: 1.2 MB (1221128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872a013b49f66bfa1e40fe5757aa1641024e14a1c0281bb5040bddba42cd62a8`  
		Last Modified: Wed, 11 May 2022 01:46:53 GMT  
		Size: 79.2 KB (79185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51202850aa4bf5caba027daccada9694f98b470cebb8bcff7f6a5914554be62b`  
		Last Modified: Wed, 11 May 2022 01:46:53 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7208b445d3203b59e4444f334cdee31b019bca4d629045af4f702cfba8ccaf17`  
		Last Modified: Wed, 11 May 2022 01:46:56 GMT  
		Size: 49.1 MB (49051109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff350ded2de4fac19a6141c701f1ea3f8c665112641799a54e6cbdc9bc9e3fcf`  
		Last Modified: Wed, 11 May 2022 01:46:51 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d554e59a0648821bbcfbc62ec3524ec7b029f0474f79b1a63d09e6f46fd6649`  
		Last Modified: Wed, 11 May 2022 01:46:51 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae08ec0a016ada08c1003b1769bd753e53e80762f97ff2bf74c691e5ee2a9213`  
		Last Modified: Wed, 11 May 2022 01:46:52 GMT  
		Size: 2.2 KB (2182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf16752e43a4c99f036c8d532b1a58d944edfe892065e7ab4328077b5e02257e`  
		Last Modified: Wed, 11 May 2022 01:46:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2.2` - linux; ppc64le

```console
$ docker pull couchdb@sha256:2774d021f2ec7122da9a2d24c153e70c92bbff47c8608c8c99f681447ec30dd1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93223893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbd6b0d3fe9a02e0fa3d5ef15549a3ec8c4f6909334bfe85b6737c3421c53899`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 May 2022 01:32:29 GMT
ADD file:1e94716789ec21981460f74be38a668bc212bd804c1d41cecf90036a5bccac5a in / 
# Wed, 11 May 2022 01:32:34 GMT
CMD ["bash"]
# Wed, 11 May 2022 03:53:11 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 May 2022 03:53:23 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 May 2022 03:54:51 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:55:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 May 2022 03:55:27 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 May 2022 03:56:34 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:56:40 GMT
ENV COUCHDB_VERSION=3.2.2
# Wed, 11 May 2022 03:56:59 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 May 2022 03:58:23 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 May 2022 03:58:28 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 11 May 2022 03:58:34 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 May 2022 03:58:40 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 11 May 2022 03:58:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 May 2022 03:58:56 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 May 2022 03:58:59 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 May 2022 03:59:03 GMT
EXPOSE 4369 5984 9100
# Wed, 11 May 2022 03:59:08 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:2533109ed11eefd6415e0370d6d7a3ea879b582b1887c98b819a598ad18fca24`  
		Last Modified: Wed, 11 May 2022 01:43:03 GMT  
		Size: 35.3 MB (35286467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62610198665bf7ba0256e568d5b533eb4e86ea7f0d929be775a0edf50ebe6dc1`  
		Last Modified: Wed, 11 May 2022 03:59:43 GMT  
		Size: 3.4 KB (3420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924366ccb76483e136508811146cb69efe23b89757b2bd2275986b5774755ad0`  
		Last Modified: Wed, 11 May 2022 03:59:42 GMT  
		Size: 6.0 MB (6043834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e66a4e119d34d65b8c9643522e2c01733a94e0e8597177f4147500a9378efcd9`  
		Last Modified: Wed, 11 May 2022 03:59:41 GMT  
		Size: 1.5 MB (1509406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49dbb3458296e8bed85cdb20ce2cdf724d7d32d1cad906bbfab48f30a0e33c3d`  
		Last Modified: Wed, 11 May 2022 03:59:40 GMT  
		Size: 295.8 KB (295806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c39bf83571d20caef422c066a90fe7046ae845342df092c85e52e4a41b551f`  
		Last Modified: Wed, 11 May 2022 03:59:40 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f869c09e50b754b4b85542688e149abd8b44f5fd83675ef3302efc7d19841fa`  
		Last Modified: Wed, 11 May 2022 03:59:44 GMT  
		Size: 50.1 MB (50081223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d9045ae6ae651b94c46fbd30c331cbc0ed8744fb4f74457e84bca35db4f535`  
		Last Modified: Wed, 11 May 2022 03:59:37 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86d7cc3cfc58048e044f5d8a637fceda45c5512800db339db878ee4985d2f43`  
		Last Modified: Wed, 11 May 2022 03:59:36 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4181a6fd70115927a806d685a3235d0e0e80b50449a8ee03840b960bf5924173`  
		Last Modified: Wed, 11 May 2022 03:59:36 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6343a3495bb02e302378fb4d0983462a14d9398bdac27e9d30d3f18e4ebe59bc`  
		Last Modified: Wed, 11 May 2022 03:59:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:latest`

```console
$ docker pull couchdb@sha256:cc42149ff90acd44ebeaa67d99f5a66168d5dce3f053f605c68a2bc1a545062d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:0e9eb882ea5cc96a465b9f4cfe311e0ac5cbd015ea1590651698131e527ff14e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87498752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c0a436cab577526883ce8f439fb5f63e16b150745e7d3d0aac1f2335c2ae6dc`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:04:40 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 May 2022 02:04:41 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 May 2022 02:04:48 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:04:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 May 2022 02:04:52 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 May 2022 02:04:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:04:57 GMT
ENV COUCHDB_VERSION=3.2.2
# Wed, 11 May 2022 02:04:57 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 May 2022 02:05:10 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 May 2022 02:05:10 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 11 May 2022 02:05:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 May 2022 02:05:11 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 11 May 2022 02:05:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 May 2022 02:05:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 May 2022 02:05:11 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 May 2022 02:05:11 GMT
EXPOSE 4369 5984 9100
# Wed, 11 May 2022 02:05:12 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ee85690522b1a5c1c261140c51987cedd0ac69838cd6a247cebfdb741dc209`  
		Last Modified: Wed, 11 May 2022 02:06:34 GMT  
		Size: 3.4 KB (3408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31e683cf3744502c13dc5eed428041c4403dba7b657bdf4baf1f62fb9a14d81`  
		Last Modified: Wed, 11 May 2022 02:06:33 GMT  
		Size: 5.2 MB (5223783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69184d8d2d701731278588e13e3acf0736dce829ac7b16d288ffb5f4a9b50641`  
		Last Modified: Wed, 11 May 2022 02:06:32 GMT  
		Size: 1.6 MB (1553317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7ff2bf2271e33167f12be0e13e1c8e7e4f51d1df70857d5b333fa43ca0f16b`  
		Last Modified: Wed, 11 May 2022 02:06:32 GMT  
		Size: 295.6 KB (295594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad60259958773deb0d46469b50bd923b25d0896ad625ad0935296d2f8d3122f`  
		Last Modified: Wed, 11 May 2022 02:06:31 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf925925077913e0bc336f89aad09bdcec3d9c03b334a07aa388a9da3a9a257b`  
		Last Modified: Wed, 11 May 2022 02:06:35 GMT  
		Size: 49.0 MB (49039446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8473eb1b9790d6b877a07f65baf502d2f00a6edcaa3858b32a939b215a7dba4b`  
		Last Modified: Wed, 11 May 2022 02:06:29 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c6a25d70616f8170336fb950a3a20bf9df514af10af91f7bd211600ec4eee6`  
		Last Modified: Wed, 11 May 2022 02:06:29 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c635531529db21d489424dc255b4b23d41ff1e6e0f1e76244f1770e014cf669d`  
		Last Modified: Wed, 11 May 2022 02:06:29 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0891e5f9c83ee343beb2d0a6ba6fdff9de433d0320a52233f0cde8e96cecc14c`  
		Last Modified: Wed, 11 May 2022 02:06:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:3776e5f2efb49f384e95d61f3603be387b3fb92f893fe67826bb10cd18517b2b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.4 MB (85427129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6b75ff4bc043175bdce94848a541cac230db909ca76f0784ea402fd2adbcab2`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:44:19 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 May 2022 01:44:20 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 May 2022 01:44:28 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:44:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 May 2022 01:44:33 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 May 2022 01:44:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:44:39 GMT
ENV COUCHDB_VERSION=3.2.2
# Wed, 11 May 2022 01:44:40 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 May 2022 01:44:54 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 May 2022 01:44:55 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 11 May 2022 01:44:56 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 May 2022 01:44:57 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 11 May 2022 01:44:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 May 2022 01:44:58 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 May 2022 01:44:59 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 May 2022 01:45:00 GMT
EXPOSE 4369 5984 9100
# Wed, 11 May 2022 01:45:01 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47eb3485a7f2023d85cb0dfb1e9a9be50f468e36f59ddda7f690c6dc8591bd2`  
		Last Modified: Wed, 11 May 2022 01:46:56 GMT  
		Size: 3.3 KB (3319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99b0f84bc54cbbaac226062cb40e48f71aab04071b0bfd3af4fc288f94024e1`  
		Last Modified: Wed, 11 May 2022 01:46:55 GMT  
		Size: 5.0 MB (5002969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932e35e02ef3eb4b94b90ee78ba1e0b543f48dedd24db2faf0a44df657b24d21`  
		Last Modified: Wed, 11 May 2022 01:46:54 GMT  
		Size: 1.2 MB (1221128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872a013b49f66bfa1e40fe5757aa1641024e14a1c0281bb5040bddba42cd62a8`  
		Last Modified: Wed, 11 May 2022 01:46:53 GMT  
		Size: 79.2 KB (79185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51202850aa4bf5caba027daccada9694f98b470cebb8bcff7f6a5914554be62b`  
		Last Modified: Wed, 11 May 2022 01:46:53 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7208b445d3203b59e4444f334cdee31b019bca4d629045af4f702cfba8ccaf17`  
		Last Modified: Wed, 11 May 2022 01:46:56 GMT  
		Size: 49.1 MB (49051109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff350ded2de4fac19a6141c701f1ea3f8c665112641799a54e6cbdc9bc9e3fcf`  
		Last Modified: Wed, 11 May 2022 01:46:51 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d554e59a0648821bbcfbc62ec3524ec7b029f0474f79b1a63d09e6f46fd6649`  
		Last Modified: Wed, 11 May 2022 01:46:51 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae08ec0a016ada08c1003b1769bd753e53e80762f97ff2bf74c691e5ee2a9213`  
		Last Modified: Wed, 11 May 2022 01:46:52 GMT  
		Size: 2.2 KB (2182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf16752e43a4c99f036c8d532b1a58d944edfe892065e7ab4328077b5e02257e`  
		Last Modified: Wed, 11 May 2022 01:46:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; ppc64le

```console
$ docker pull couchdb@sha256:2774d021f2ec7122da9a2d24c153e70c92bbff47c8608c8c99f681447ec30dd1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93223893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbd6b0d3fe9a02e0fa3d5ef15549a3ec8c4f6909334bfe85b6737c3421c53899`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 May 2022 01:32:29 GMT
ADD file:1e94716789ec21981460f74be38a668bc212bd804c1d41cecf90036a5bccac5a in / 
# Wed, 11 May 2022 01:32:34 GMT
CMD ["bash"]
# Wed, 11 May 2022 03:53:11 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 May 2022 03:53:23 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 May 2022 03:54:51 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:55:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 May 2022 03:55:27 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 May 2022 03:56:34 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:56:40 GMT
ENV COUCHDB_VERSION=3.2.2
# Wed, 11 May 2022 03:56:59 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 May 2022 03:58:23 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 May 2022 03:58:28 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 11 May 2022 03:58:34 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 May 2022 03:58:40 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 11 May 2022 03:58:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 May 2022 03:58:56 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 May 2022 03:58:59 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 May 2022 03:59:03 GMT
EXPOSE 4369 5984 9100
# Wed, 11 May 2022 03:59:08 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:2533109ed11eefd6415e0370d6d7a3ea879b582b1887c98b819a598ad18fca24`  
		Last Modified: Wed, 11 May 2022 01:43:03 GMT  
		Size: 35.3 MB (35286467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62610198665bf7ba0256e568d5b533eb4e86ea7f0d929be775a0edf50ebe6dc1`  
		Last Modified: Wed, 11 May 2022 03:59:43 GMT  
		Size: 3.4 KB (3420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924366ccb76483e136508811146cb69efe23b89757b2bd2275986b5774755ad0`  
		Last Modified: Wed, 11 May 2022 03:59:42 GMT  
		Size: 6.0 MB (6043834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e66a4e119d34d65b8c9643522e2c01733a94e0e8597177f4147500a9378efcd9`  
		Last Modified: Wed, 11 May 2022 03:59:41 GMT  
		Size: 1.5 MB (1509406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49dbb3458296e8bed85cdb20ce2cdf724d7d32d1cad906bbfab48f30a0e33c3d`  
		Last Modified: Wed, 11 May 2022 03:59:40 GMT  
		Size: 295.8 KB (295806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c39bf83571d20caef422c066a90fe7046ae845342df092c85e52e4a41b551f`  
		Last Modified: Wed, 11 May 2022 03:59:40 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f869c09e50b754b4b85542688e149abd8b44f5fd83675ef3302efc7d19841fa`  
		Last Modified: Wed, 11 May 2022 03:59:44 GMT  
		Size: 50.1 MB (50081223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d9045ae6ae651b94c46fbd30c331cbc0ed8744fb4f74457e84bca35db4f535`  
		Last Modified: Wed, 11 May 2022 03:59:37 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86d7cc3cfc58048e044f5d8a637fceda45c5512800db339db878ee4985d2f43`  
		Last Modified: Wed, 11 May 2022 03:59:36 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4181a6fd70115927a806d685a3235d0e0e80b50449a8ee03840b960bf5924173`  
		Last Modified: Wed, 11 May 2022 03:59:36 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6343a3495bb02e302378fb4d0983462a14d9398bdac27e9d30d3f18e4ebe59bc`  
		Last Modified: Wed, 11 May 2022 03:59:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
