<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `couchdb`

-	[`couchdb:2`](#couchdb2)
-	[`couchdb:2.3`](#couchdb23)
-	[`couchdb:2.3.1`](#couchdb231)
-	[`couchdb:3`](#couchdb3)
-	[`couchdb:3.1`](#couchdb31)
-	[`couchdb:3.1.2`](#couchdb312)
-	[`couchdb:3.2`](#couchdb32)
-	[`couchdb:3.2.3`](#couchdb323)
-	[`couchdb:3.3`](#couchdb33)
-	[`couchdb:3.3.2`](#couchdb332)
-	[`couchdb:latest`](#couchdblatest)

## `couchdb:2`

```console
$ docker pull couchdb@sha256:4387e70176adeece3597a04f6576da11f14acb02d406dde91024f45a42aeced3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2` - linux; amd64

```console
$ docker pull couchdb@sha256:19be5733a588e013e2c291d4859912263be55b51ccf536eb1bd7bc1d43c1ae57
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.6 MB (84601725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04ee8e9e2374fc1d5a8f7e6ace34246c2ce60e99b8566c0d1ce0f9d307c41b83`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:33 GMT
ADD file:29d3eb64d192a97184f2aa169407b58e969b06268c6372b49eefb72bcadb6e99 in / 
# Wed, 01 Nov 2023 00:21:34 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:47:35 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Nov 2023 01:47:36 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Nov 2023 01:47:43 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:47:47 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Nov 2023 01:47:47 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Nov 2023 01:47:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:48:16 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 01 Nov 2023 01:48:17 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Nov 2023 01:48:34 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Nov 2023 01:48:35 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Nov 2023 01:48:35 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 01 Nov 2023 01:48:35 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 01 Nov 2023 01:48:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Nov 2023 01:48:36 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 01:48:36 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Nov 2023 01:48:36 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Nov 2023 01:48:36 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:113c6ad4754853f4a2ae632cff7d90eba9145cca0bd6fa4d60aa432bd26be6c7`  
		Last Modified: Wed, 01 Nov 2023 00:26:56 GMT  
		Size: 27.2 MB (27187422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365ea17356912d8ab65ea5e3a1e839d36823f7303a6f99fec14eb169f5a4f2e1`  
		Last Modified: Wed, 01 Nov 2023 01:49:33 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2706b6ad14bfc13aa94a94269c8479e367a22ebbf64f230b4a133b8198b51523`  
		Last Modified: Wed, 01 Nov 2023 01:49:32 GMT  
		Size: 6.7 MB (6704557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3cbd037256b0218774d56e4d3151275a32733815758ef37784eae1b624c9831`  
		Last Modified: Wed, 01 Nov 2023 01:49:31 GMT  
		Size: 1.3 MB (1259891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7bc073931afdef902766bdbf4440108b63b7e7a8afc61c51d5132e2b366910`  
		Last Modified: Wed, 01 Nov 2023 01:49:31 GMT  
		Size: 294.5 KB (294533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b65f0118e1821e295770007c76deb6fe634a42524867a48e15ec8f7a13ae28`  
		Last Modified: Wed, 01 Nov 2023 01:49:45 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba2feaa281f86c66f6d3385abb0a3c253bb921c23c2fb5b7f037c54dfd0e9fc`  
		Last Modified: Wed, 01 Nov 2023 01:49:48 GMT  
		Size: 49.1 MB (49148308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f60a8b754ebf89dcda4a9b032fc7d76cfaf67b4d1cdd88a92fd548bfdde80785`  
		Last Modified: Wed, 01 Nov 2023 01:49:43 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199951c325e2234c69de9082ae7590bd8eeb37f76ccf34d718f5393cdbe10f76`  
		Last Modified: Wed, 01 Nov 2023 01:49:43 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f41fd1ccaf8d2e0c1c37dc2a8a78d3d6ebe9650c37c188cc04833e726242a4a`  
		Last Modified: Wed, 01 Nov 2023 01:49:43 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7ad5245583de27094c466123980bca3addac07d4fc43887ea3f7598abcec934`  
		Last Modified: Wed, 01 Nov 2023 01:49:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:291a39d9d52c976c3b07e67a57be626b0f83205d2f26ad546d5b6891ab60915d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (73042646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5b77f96368a9013f98c4f9425996a649c9a179a02a530cb4b33a56346a9327f`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:09 GMT
ADD file:ad1947b1fc97bcc228c004c15afeb2d9006d47167db69cf7b05c3e634c648166 in / 
# Wed, 01 Nov 2023 00:40:10 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:54:28 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Nov 2023 02:54:28 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Nov 2023 02:54:35 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:54:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Nov 2023 02:54:39 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Nov 2023 02:54:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:55:02 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 01 Nov 2023 02:55:02 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Nov 2023 02:55:14 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Nov 2023 02:55:14 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Nov 2023 02:55:14 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 01 Nov 2023 02:55:14 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 01 Nov 2023 02:55:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Nov 2023 02:55:15 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 02:55:15 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Nov 2023 02:55:15 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Nov 2023 02:55:15 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:094e0a7927f79c559fdab346774d7de6e5fc38e2d998e82dd663850ebbff4648`  
		Last Modified: Wed, 01 Nov 2023 00:44:25 GMT  
		Size: 26.0 MB (25967703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc5be3d4f1542e6fc11ee7fcc29abb4753366751c6c627a92ba68dc7bf2e012`  
		Last Modified: Wed, 01 Nov 2023 02:55:49 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0f557682501a5ca3e65c0c48b65e6645c396a0471d6a8d63a8f2f1bb92fb08`  
		Last Modified: Wed, 01 Nov 2023 02:55:48 GMT  
		Size: 6.6 MB (6577623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec4b7957cee1703ce1207b0b11d9e4aed5a56dd9eac981116cf46305e545576`  
		Last Modified: Wed, 01 Nov 2023 02:55:48 GMT  
		Size: 1.2 MB (1164824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6921da86aad61db9f07f1b09e040f85e1c3422fe0459bd50995cb939273ea0c3`  
		Last Modified: Wed, 01 Nov 2023 02:55:47 GMT  
		Size: 294.4 KB (294429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211f122432c707b57ebca03e3fa5f27b068bf3cd74c78eca0da6eabac5bb76a9`  
		Last Modified: Wed, 01 Nov 2023 02:56:00 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9027dfc611eb1065fc87a43b2b7ae9f7293a3d56f427fb4f9bc907bdfbd8ccfa`  
		Last Modified: Wed, 01 Nov 2023 02:56:02 GMT  
		Size: 39.0 MB (39031029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8516ef915614bd4d14d6a7d09b4fccd1fd9898f2d40608b66fb36c07394ac4`  
		Last Modified: Wed, 01 Nov 2023 02:55:58 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101ad0361456d69925fc4ed4ef94f898485509d9e8e434f451bf5cd2d8246ecb`  
		Last Modified: Wed, 01 Nov 2023 02:55:58 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f82fe2fd4239fec4bd6cea4a118d6ddebabed66d02aa9a9d28691a06dc2b69b1`  
		Last Modified: Wed, 01 Nov 2023 02:55:58 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1e4c9c7523c47b309f02dc4b4913ae2c7dde40c14fb82793ccf8ccfd54e7a6`  
		Last Modified: Wed, 01 Nov 2023 02:55:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3`

```console
$ docker pull couchdb@sha256:4387e70176adeece3597a04f6576da11f14acb02d406dde91024f45a42aeced3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:19be5733a588e013e2c291d4859912263be55b51ccf536eb1bd7bc1d43c1ae57
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.6 MB (84601725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04ee8e9e2374fc1d5a8f7e6ace34246c2ce60e99b8566c0d1ce0f9d307c41b83`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:33 GMT
ADD file:29d3eb64d192a97184f2aa169407b58e969b06268c6372b49eefb72bcadb6e99 in / 
# Wed, 01 Nov 2023 00:21:34 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:47:35 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Nov 2023 01:47:36 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Nov 2023 01:47:43 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:47:47 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Nov 2023 01:47:47 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Nov 2023 01:47:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:48:16 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 01 Nov 2023 01:48:17 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Nov 2023 01:48:34 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Nov 2023 01:48:35 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Nov 2023 01:48:35 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 01 Nov 2023 01:48:35 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 01 Nov 2023 01:48:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Nov 2023 01:48:36 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 01:48:36 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Nov 2023 01:48:36 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Nov 2023 01:48:36 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:113c6ad4754853f4a2ae632cff7d90eba9145cca0bd6fa4d60aa432bd26be6c7`  
		Last Modified: Wed, 01 Nov 2023 00:26:56 GMT  
		Size: 27.2 MB (27187422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365ea17356912d8ab65ea5e3a1e839d36823f7303a6f99fec14eb169f5a4f2e1`  
		Last Modified: Wed, 01 Nov 2023 01:49:33 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2706b6ad14bfc13aa94a94269c8479e367a22ebbf64f230b4a133b8198b51523`  
		Last Modified: Wed, 01 Nov 2023 01:49:32 GMT  
		Size: 6.7 MB (6704557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3cbd037256b0218774d56e4d3151275a32733815758ef37784eae1b624c9831`  
		Last Modified: Wed, 01 Nov 2023 01:49:31 GMT  
		Size: 1.3 MB (1259891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7bc073931afdef902766bdbf4440108b63b7e7a8afc61c51d5132e2b366910`  
		Last Modified: Wed, 01 Nov 2023 01:49:31 GMT  
		Size: 294.5 KB (294533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b65f0118e1821e295770007c76deb6fe634a42524867a48e15ec8f7a13ae28`  
		Last Modified: Wed, 01 Nov 2023 01:49:45 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba2feaa281f86c66f6d3385abb0a3c253bb921c23c2fb5b7f037c54dfd0e9fc`  
		Last Modified: Wed, 01 Nov 2023 01:49:48 GMT  
		Size: 49.1 MB (49148308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f60a8b754ebf89dcda4a9b032fc7d76cfaf67b4d1cdd88a92fd548bfdde80785`  
		Last Modified: Wed, 01 Nov 2023 01:49:43 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199951c325e2234c69de9082ae7590bd8eeb37f76ccf34d718f5393cdbe10f76`  
		Last Modified: Wed, 01 Nov 2023 01:49:43 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f41fd1ccaf8d2e0c1c37dc2a8a78d3d6ebe9650c37c188cc04833e726242a4a`  
		Last Modified: Wed, 01 Nov 2023 01:49:43 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7ad5245583de27094c466123980bca3addac07d4fc43887ea3f7598abcec934`  
		Last Modified: Wed, 01 Nov 2023 01:49:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:291a39d9d52c976c3b07e67a57be626b0f83205d2f26ad546d5b6891ab60915d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (73042646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5b77f96368a9013f98c4f9425996a649c9a179a02a530cb4b33a56346a9327f`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:09 GMT
ADD file:ad1947b1fc97bcc228c004c15afeb2d9006d47167db69cf7b05c3e634c648166 in / 
# Wed, 01 Nov 2023 00:40:10 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:54:28 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Nov 2023 02:54:28 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Nov 2023 02:54:35 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:54:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Nov 2023 02:54:39 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Nov 2023 02:54:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:55:02 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 01 Nov 2023 02:55:02 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Nov 2023 02:55:14 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Nov 2023 02:55:14 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Nov 2023 02:55:14 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 01 Nov 2023 02:55:14 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 01 Nov 2023 02:55:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Nov 2023 02:55:15 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 02:55:15 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Nov 2023 02:55:15 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Nov 2023 02:55:15 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:094e0a7927f79c559fdab346774d7de6e5fc38e2d998e82dd663850ebbff4648`  
		Last Modified: Wed, 01 Nov 2023 00:44:25 GMT  
		Size: 26.0 MB (25967703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc5be3d4f1542e6fc11ee7fcc29abb4753366751c6c627a92ba68dc7bf2e012`  
		Last Modified: Wed, 01 Nov 2023 02:55:49 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0f557682501a5ca3e65c0c48b65e6645c396a0471d6a8d63a8f2f1bb92fb08`  
		Last Modified: Wed, 01 Nov 2023 02:55:48 GMT  
		Size: 6.6 MB (6577623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec4b7957cee1703ce1207b0b11d9e4aed5a56dd9eac981116cf46305e545576`  
		Last Modified: Wed, 01 Nov 2023 02:55:48 GMT  
		Size: 1.2 MB (1164824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6921da86aad61db9f07f1b09e040f85e1c3422fe0459bd50995cb939273ea0c3`  
		Last Modified: Wed, 01 Nov 2023 02:55:47 GMT  
		Size: 294.4 KB (294429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211f122432c707b57ebca03e3fa5f27b068bf3cd74c78eca0da6eabac5bb76a9`  
		Last Modified: Wed, 01 Nov 2023 02:56:00 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9027dfc611eb1065fc87a43b2b7ae9f7293a3d56f427fb4f9bc907bdfbd8ccfa`  
		Last Modified: Wed, 01 Nov 2023 02:56:02 GMT  
		Size: 39.0 MB (39031029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8516ef915614bd4d14d6a7d09b4fccd1fd9898f2d40608b66fb36c07394ac4`  
		Last Modified: Wed, 01 Nov 2023 02:55:58 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101ad0361456d69925fc4ed4ef94f898485509d9e8e434f451bf5cd2d8246ecb`  
		Last Modified: Wed, 01 Nov 2023 02:55:58 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f82fe2fd4239fec4bd6cea4a118d6ddebabed66d02aa9a9d28691a06dc2b69b1`  
		Last Modified: Wed, 01 Nov 2023 02:55:58 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1e4c9c7523c47b309f02dc4b4913ae2c7dde40c14fb82793ccf8ccfd54e7a6`  
		Last Modified: Wed, 01 Nov 2023 02:55:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3.1`

```console
$ docker pull couchdb@sha256:4387e70176adeece3597a04f6576da11f14acb02d406dde91024f45a42aeced3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:19be5733a588e013e2c291d4859912263be55b51ccf536eb1bd7bc1d43c1ae57
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.6 MB (84601725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04ee8e9e2374fc1d5a8f7e6ace34246c2ce60e99b8566c0d1ce0f9d307c41b83`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:33 GMT
ADD file:29d3eb64d192a97184f2aa169407b58e969b06268c6372b49eefb72bcadb6e99 in / 
# Wed, 01 Nov 2023 00:21:34 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:47:35 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Nov 2023 01:47:36 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Nov 2023 01:47:43 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:47:47 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Nov 2023 01:47:47 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Nov 2023 01:47:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:48:16 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 01 Nov 2023 01:48:17 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Nov 2023 01:48:34 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Nov 2023 01:48:35 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Nov 2023 01:48:35 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 01 Nov 2023 01:48:35 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 01 Nov 2023 01:48:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Nov 2023 01:48:36 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 01:48:36 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Nov 2023 01:48:36 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Nov 2023 01:48:36 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:113c6ad4754853f4a2ae632cff7d90eba9145cca0bd6fa4d60aa432bd26be6c7`  
		Last Modified: Wed, 01 Nov 2023 00:26:56 GMT  
		Size: 27.2 MB (27187422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365ea17356912d8ab65ea5e3a1e839d36823f7303a6f99fec14eb169f5a4f2e1`  
		Last Modified: Wed, 01 Nov 2023 01:49:33 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2706b6ad14bfc13aa94a94269c8479e367a22ebbf64f230b4a133b8198b51523`  
		Last Modified: Wed, 01 Nov 2023 01:49:32 GMT  
		Size: 6.7 MB (6704557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3cbd037256b0218774d56e4d3151275a32733815758ef37784eae1b624c9831`  
		Last Modified: Wed, 01 Nov 2023 01:49:31 GMT  
		Size: 1.3 MB (1259891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7bc073931afdef902766bdbf4440108b63b7e7a8afc61c51d5132e2b366910`  
		Last Modified: Wed, 01 Nov 2023 01:49:31 GMT  
		Size: 294.5 KB (294533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b65f0118e1821e295770007c76deb6fe634a42524867a48e15ec8f7a13ae28`  
		Last Modified: Wed, 01 Nov 2023 01:49:45 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba2feaa281f86c66f6d3385abb0a3c253bb921c23c2fb5b7f037c54dfd0e9fc`  
		Last Modified: Wed, 01 Nov 2023 01:49:48 GMT  
		Size: 49.1 MB (49148308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f60a8b754ebf89dcda4a9b032fc7d76cfaf67b4d1cdd88a92fd548bfdde80785`  
		Last Modified: Wed, 01 Nov 2023 01:49:43 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199951c325e2234c69de9082ae7590bd8eeb37f76ccf34d718f5393cdbe10f76`  
		Last Modified: Wed, 01 Nov 2023 01:49:43 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f41fd1ccaf8d2e0c1c37dc2a8a78d3d6ebe9650c37c188cc04833e726242a4a`  
		Last Modified: Wed, 01 Nov 2023 01:49:43 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7ad5245583de27094c466123980bca3addac07d4fc43887ea3f7598abcec934`  
		Last Modified: Wed, 01 Nov 2023 01:49:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:291a39d9d52c976c3b07e67a57be626b0f83205d2f26ad546d5b6891ab60915d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (73042646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5b77f96368a9013f98c4f9425996a649c9a179a02a530cb4b33a56346a9327f`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:09 GMT
ADD file:ad1947b1fc97bcc228c004c15afeb2d9006d47167db69cf7b05c3e634c648166 in / 
# Wed, 01 Nov 2023 00:40:10 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:54:28 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Nov 2023 02:54:28 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Nov 2023 02:54:35 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:54:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Nov 2023 02:54:39 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Nov 2023 02:54:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:55:02 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 01 Nov 2023 02:55:02 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Nov 2023 02:55:14 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Nov 2023 02:55:14 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Nov 2023 02:55:14 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 01 Nov 2023 02:55:14 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 01 Nov 2023 02:55:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Nov 2023 02:55:15 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 02:55:15 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Nov 2023 02:55:15 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Nov 2023 02:55:15 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:094e0a7927f79c559fdab346774d7de6e5fc38e2d998e82dd663850ebbff4648`  
		Last Modified: Wed, 01 Nov 2023 00:44:25 GMT  
		Size: 26.0 MB (25967703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc5be3d4f1542e6fc11ee7fcc29abb4753366751c6c627a92ba68dc7bf2e012`  
		Last Modified: Wed, 01 Nov 2023 02:55:49 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0f557682501a5ca3e65c0c48b65e6645c396a0471d6a8d63a8f2f1bb92fb08`  
		Last Modified: Wed, 01 Nov 2023 02:55:48 GMT  
		Size: 6.6 MB (6577623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec4b7957cee1703ce1207b0b11d9e4aed5a56dd9eac981116cf46305e545576`  
		Last Modified: Wed, 01 Nov 2023 02:55:48 GMT  
		Size: 1.2 MB (1164824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6921da86aad61db9f07f1b09e040f85e1c3422fe0459bd50995cb939273ea0c3`  
		Last Modified: Wed, 01 Nov 2023 02:55:47 GMT  
		Size: 294.4 KB (294429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211f122432c707b57ebca03e3fa5f27b068bf3cd74c78eca0da6eabac5bb76a9`  
		Last Modified: Wed, 01 Nov 2023 02:56:00 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9027dfc611eb1065fc87a43b2b7ae9f7293a3d56f427fb4f9bc907bdfbd8ccfa`  
		Last Modified: Wed, 01 Nov 2023 02:56:02 GMT  
		Size: 39.0 MB (39031029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8516ef915614bd4d14d6a7d09b4fccd1fd9898f2d40608b66fb36c07394ac4`  
		Last Modified: Wed, 01 Nov 2023 02:55:58 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101ad0361456d69925fc4ed4ef94f898485509d9e8e434f451bf5cd2d8246ecb`  
		Last Modified: Wed, 01 Nov 2023 02:55:58 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f82fe2fd4239fec4bd6cea4a118d6ddebabed66d02aa9a9d28691a06dc2b69b1`  
		Last Modified: Wed, 01 Nov 2023 02:55:58 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1e4c9c7523c47b309f02dc4b4913ae2c7dde40c14fb82793ccf8ccfd54e7a6`  
		Last Modified: Wed, 01 Nov 2023 02:55:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3`

```console
$ docker pull couchdb@sha256:482d73fa450a18bce6ff591740b7a69f21a1cf94ffcd295a500e5214981e18d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `couchdb:3` - linux; amd64

```console
$ docker pull couchdb@sha256:3c609bc33e472d4cb0a4ea0b117359bd0c9ed4f0628899131e8344fd13fbe01a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90245671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fff4b56666dbf396fc0b2eedb70c70b8990ccb6dc5d8447206f2243d21c1986c`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:46:40 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Nov 2023 01:46:41 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Nov 2023 01:46:47 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:46:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 01 Nov 2023 01:46:51 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Nov 2023 01:46:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:46:56 GMT
ENV COUCHDB_VERSION=3.3.2
# Wed, 01 Nov 2023 01:46:56 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Nov 2023 01:47:10 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Nov 2023 01:47:10 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Nov 2023 01:47:10 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 01 Nov 2023 01:47:11 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 01 Nov 2023 01:47:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Nov 2023 01:47:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 01:47:11 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Nov 2023 01:47:11 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Nov 2023 01:47:11 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbba1a29bfe2ee9664ccd0caa145b5aa7a5480c276f1c42fd77ac32ef2c440c1`  
		Last Modified: Wed, 01 Nov 2023 01:48:53 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b21d450d3bd9333c8a5efb4081f440607452820e295142168061b2216f3986c`  
		Last Modified: Wed, 01 Nov 2023 01:48:53 GMT  
		Size: 5.2 MB (5226554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c93767e1cbf8a0b2d24469dbe0f750b73d88204210f83f7faa87b8be37dfaa`  
		Last Modified: Wed, 01 Nov 2023 01:48:52 GMT  
		Size: 610.9 KB (610919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24dc783ed2d49dd34054350d1a680091886de94bd264352e835184065e394e64`  
		Last Modified: Wed, 01 Nov 2023 01:48:52 GMT  
		Size: 295.2 KB (295153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8597086eac85cffb9306a84cfa8414bcda5500cb8092b1ba307a38e9e56540f`  
		Last Modified: Wed, 01 Nov 2023 01:48:52 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4fefd748372d68972d6fb14014c7813ac7837a6380b957f3092da518331958`  
		Last Modified: Wed, 01 Nov 2023 01:48:55 GMT  
		Size: 52.7 MB (52687716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ff2441b3a4073bbf88542aaf2d970fd2eb11cc4bd01c846d1245dae6187068`  
		Last Modified: Wed, 01 Nov 2023 01:48:50 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c29c7241d3a11a9dcf62611e3563275d0b24d32fa9f65fb5be837b13ef1cfb4`  
		Last Modified: Wed, 01 Nov 2023 01:48:50 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacd4b2ce1758697d4898b78068d98430738b73f2f0171222ea8fc970a567603`  
		Last Modified: Wed, 01 Nov 2023 01:48:50 GMT  
		Size: 2.2 KB (2228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7254e813570e08d636b0b367fb2dfe8c25dfa8b3a07a24b4dcf9574a9e238270`  
		Last Modified: Wed, 01 Nov 2023 01:48:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:a4d2708520335bec287044683aa008f3ee0af0174c4844f4c27d73581ef39326
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88693209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a609af91aa2f1677f43a122b8a919068545adc446fc3857244fe5a8d89b703d5`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:53:44 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Nov 2023 02:53:44 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Nov 2023 02:53:50 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:53:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 01 Nov 2023 02:53:53 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Nov 2023 02:53:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:53:58 GMT
ENV COUCHDB_VERSION=3.3.2
# Wed, 01 Nov 2023 02:53:58 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Nov 2023 02:54:11 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Nov 2023 02:54:12 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Nov 2023 02:54:12 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 01 Nov 2023 02:54:12 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 01 Nov 2023 02:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Nov 2023 02:54:12 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 02:54:12 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Nov 2023 02:54:12 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Nov 2023 02:54:13 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b614568051476b61815cad57612a54fb357dce26265c2d8a93d3603e65f67bb`  
		Last Modified: Wed, 01 Nov 2023 02:55:30 GMT  
		Size: 3.4 KB (3431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c7e0362f1203d4c8eb75046c1009a66141067e9cb7a5e02ac76702b3a4fc5e`  
		Last Modified: Wed, 01 Nov 2023 02:55:29 GMT  
		Size: 5.2 MB (5210837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936a7f3d3f0f461eb2f034fa209eb834d4f53ab52e315c1ea90e4436d100cc12`  
		Last Modified: Wed, 01 Nov 2023 02:55:29 GMT  
		Size: 567.1 KB (567066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cea30aeda14f6e14599fb09aa79b3a41556b7509b7d4835f0d97a0e131aff2c`  
		Last Modified: Wed, 01 Nov 2023 02:55:29 GMT  
		Size: 295.0 KB (295032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a6600b43b5af044cab2a8316adbf77eed718e07be3a49b46d0d40f52bd9142`  
		Last Modified: Wed, 01 Nov 2023 02:55:28 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb3d645b10a8f7621c93c74d0ef540bf7eaa4110c0aeb1c226e7a3fde645671`  
		Last Modified: Wed, 01 Nov 2023 02:55:31 GMT  
		Size: 52.5 MB (52548927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0231949bd50a35a558a786ffd81b537869d8c2008032cf8f763cf817364efbc`  
		Last Modified: Wed, 01 Nov 2023 02:55:26 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce55a94b61b5a276dbee100f2f54d927ab8e493c9eef066a8604e6d29c611ab9`  
		Last Modified: Wed, 01 Nov 2023 02:55:26 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c997e552c1313a4b038f571f70da3ddf3a0b62fade23a017f7ba4dfbbeecc46`  
		Last Modified: Wed, 01 Nov 2023 02:55:26 GMT  
		Size: 2.2 KB (2230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15920850d8d556ea5c5d6b5a45df1b59867930cd37d1d15f1f712d12ee66edaf`  
		Last Modified: Wed, 01 Nov 2023 02:55:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; ppc64le

```console
$ docker pull couchdb@sha256:ccf9e925a92c4e47c922173bb8a6541607469de85a3d23b8f709a5b2f9fa4571
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.0 MB (95968231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0d5240fcc3525a7c996865649016d229a3b75d1447c7ade86132d7ede52ffe8`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:43 GMT
ADD file:b0d18f2d04821eb50d1faecc1a64916f5c63dd386ae71a3b2cb1d6c4aac6e1c4 in / 
# Tue, 21 Nov 2023 04:24:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:12:10 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Nov 2023 07:12:12 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Nov 2023 07:12:31 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:12:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 21 Nov 2023 07:12:37 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Nov 2023 07:12:47 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:12:47 GMT
ENV COUCHDB_VERSION=3.3.2
# Tue, 21 Nov 2023 07:12:49 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Nov 2023 07:13:13 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Nov 2023 07:13:17 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Nov 2023 07:13:17 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 21 Nov 2023 07:13:17 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 21 Nov 2023 07:13:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Nov 2023 07:13:20 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Nov 2023 07:13:20 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Nov 2023 07:13:20 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Nov 2023 07:13:21 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:60239a74847cd7e9a928353188f3cf096ca8cf648e2b27c765058e169d568fd9`  
		Last Modified: Tue, 21 Nov 2023 04:29:47 GMT  
		Size: 35.3 MB (35293727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f63eed5db2c906b6108908d9dc6976c9a23f1bb19a0e617257decd133e7592d`  
		Last Modified: Tue, 21 Nov 2023 07:14:05 GMT  
		Size: 3.4 KB (3408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941bb642de45bb343a873e9c819cd85bffe05a010a6da631d1723612f69c794c`  
		Last Modified: Tue, 21 Nov 2023 07:14:04 GMT  
		Size: 6.0 MB (6046203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f2659433b58c3235f1e9085447d55d5c442efc597e42f97dfce11b106d84c0`  
		Last Modified: Tue, 21 Nov 2023 07:14:04 GMT  
		Size: 662.9 KB (662883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d777a7fd59124bb1d1eed56bddee9639f6ea57c6eaf67610a97a4a8c833814e9`  
		Last Modified: Tue, 21 Nov 2023 07:14:03 GMT  
		Size: 295.1 KB (295091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef322b815f454b44be7fc5bbc3f2c179419841031a40a753c25cb71a704158f4`  
		Last Modified: Tue, 21 Nov 2023 07:14:03 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6180ccba02f37081c0d1523baa72b7df6183b2284a575cc84c8f245ed21624fc`  
		Last Modified: Tue, 21 Nov 2023 07:14:07 GMT  
		Size: 53.7 MB (53662909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991739364f41cbdef5c3adb115b1f41c51bbafbd6555e32316cad98f1cae7e54`  
		Last Modified: Tue, 21 Nov 2023 07:14:01 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f539c1a9af058023c294a0b078bb81ec732ba18d3e4c624af45c5e3a877c5dd`  
		Last Modified: Tue, 21 Nov 2023 07:14:01 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27abb88fb75707dd945625a5a2734aa790dcd4330e5d257d13fde86d69630c4`  
		Last Modified: Tue, 21 Nov 2023 07:14:01 GMT  
		Size: 2.2 KB (2232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7837c78696f2a9940c752105b06aeb98a48f8a6eacab80ba3a467f89fbe31ee5`  
		Last Modified: Tue, 21 Nov 2023 07:14:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; s390x

```console
$ docker pull couchdb@sha256:21965f0438b454449366375d4c6bfd319e83dec568e9907669ba2b6a1c077563
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.0 MB (87002806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba071f2f075a8263e2e67f1fc0f844debd3e57242ac3165ff9adcfacf2338049`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Nov 2023 05:05:18 GMT
ADD file:a545f27075704ce13e33e539170d3f47007424d2cc2bea5aecfd2608a5194151 in / 
# Tue, 21 Nov 2023 05:05:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:20:22 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Nov 2023 06:20:22 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Nov 2023 06:20:28 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:20:31 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 21 Nov 2023 06:20:31 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Nov 2023 06:20:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:20:36 GMT
ENV COUCHDB_VERSION=3.3.2
# Tue, 21 Nov 2023 06:20:36 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Nov 2023 06:20:53 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Nov 2023 06:20:55 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Nov 2023 06:20:55 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 21 Nov 2023 06:20:55 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 21 Nov 2023 06:20:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Nov 2023 06:20:56 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Nov 2023 06:20:56 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Nov 2023 06:20:56 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Nov 2023 06:20:56 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b114072f1cab66b7376d690985b12816aebab2e4e41fc170e32f111df27951dc`  
		Last Modified: Tue, 21 Nov 2023 05:10:48 GMT  
		Size: 29.7 MB (29656938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72dba253785a5e917fdd9064f61b676b4080ff3073424ff387308d70579c728b`  
		Last Modified: Tue, 21 Nov 2023 06:21:15 GMT  
		Size: 3.4 KB (3431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a299cd04ea14bbc3034e11001a1ec06dd4b5e1aaa78317dc803570f8a4c6437`  
		Last Modified: Tue, 21 Nov 2023 06:21:15 GMT  
		Size: 5.1 MB (5111719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c684e5bcbb93c8f0c9da5b81b4a1d19274f7ad0c7e3b17eb12cbe45cd2514989`  
		Last Modified: Tue, 21 Nov 2023 06:21:14 GMT  
		Size: 573.6 KB (573635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d916370cd04b7352346fee3edc1ac77bdb9393e24c5bc62c4cb0803a682836`  
		Last Modified: Tue, 21 Nov 2023 06:21:14 GMT  
		Size: 295.1 KB (295096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e602d723a112bfbe3ebaca9b99e2e9636dac8b07c69947311ceb07666d40ed`  
		Last Modified: Tue, 21 Nov 2023 06:21:14 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbafbeffdc5d29b56e0ccf672e48ead551f49aa23534b4fd9aefcd339587dc5`  
		Last Modified: Tue, 21 Nov 2023 06:21:18 GMT  
		Size: 51.4 MB (51357976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f08f21ade417458e581ec8afdf835c5d165444c0e93fdc330cbd6146af1da3`  
		Last Modified: Tue, 21 Nov 2023 06:21:13 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a4bc9e282fe338ed74c99dbb5cb5777e0ba1a2d068de6e102a8adbb34acc14`  
		Last Modified: Tue, 21 Nov 2023 06:21:13 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c93f5a64665780dfb559adfed9587064e52e00c9c515834a97cf26e3529da9`  
		Last Modified: Tue, 21 Nov 2023 06:21:13 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f6f407505b71a14801c0c71da8d0ce2a85d8c65d58e7998784a75dcde3cfb6`  
		Last Modified: Tue, 21 Nov 2023 06:21:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1`

```console
$ docker pull couchdb@sha256:bb6adfda153f4deb7df949817e186fb66e25e9d309eb5f54b24b6e7980f5655f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:d64439bcd931bfe3b2b48135529b514beab649fa0259881fd04c774f2c3d5422
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.1 MB (80075635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:205e57c6f99f40a4d603140fe6501754b9f090f9630e35f08a02887e35b43e91`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:33 GMT
ADD file:29d3eb64d192a97184f2aa169407b58e969b06268c6372b49eefb72bcadb6e99 in / 
# Wed, 01 Nov 2023 00:21:34 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:47:35 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Nov 2023 01:47:36 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Nov 2023 01:47:43 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:47:47 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Nov 2023 01:47:47 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Nov 2023 01:47:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:47:53 GMT
ENV COUCHDB_VERSION=3.1.2
# Wed, 01 Nov 2023 01:47:54 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Nov 2023 01:48:07 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Nov 2023 01:48:08 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Nov 2023 01:48:08 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 01 Nov 2023 01:48:08 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 01 Nov 2023 01:48:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Nov 2023 01:48:09 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 01:48:09 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Nov 2023 01:48:09 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Nov 2023 01:48:09 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:113c6ad4754853f4a2ae632cff7d90eba9145cca0bd6fa4d60aa432bd26be6c7`  
		Last Modified: Wed, 01 Nov 2023 00:26:56 GMT  
		Size: 27.2 MB (27187422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365ea17356912d8ab65ea5e3a1e839d36823f7303a6f99fec14eb169f5a4f2e1`  
		Last Modified: Wed, 01 Nov 2023 01:49:33 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2706b6ad14bfc13aa94a94269c8479e367a22ebbf64f230b4a133b8198b51523`  
		Last Modified: Wed, 01 Nov 2023 01:49:32 GMT  
		Size: 6.7 MB (6704557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3cbd037256b0218774d56e4d3151275a32733815758ef37784eae1b624c9831`  
		Last Modified: Wed, 01 Nov 2023 01:49:31 GMT  
		Size: 1.3 MB (1259891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7bc073931afdef902766bdbf4440108b63b7e7a8afc61c51d5132e2b366910`  
		Last Modified: Wed, 01 Nov 2023 01:49:31 GMT  
		Size: 294.5 KB (294533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4debe8d86185b55779861ac36695c6d3d6f33c7b19c8b4d6d8b1edf847264fc8`  
		Last Modified: Wed, 01 Nov 2023 01:49:30 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:771c29924f094333de4b98cd2e8acaa0f6bd0f0737f62f73c3ff771764790fb0`  
		Last Modified: Wed, 01 Nov 2023 01:49:33 GMT  
		Size: 44.6 MB (44622218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04407e3339446bef5cd7c3a5bdadbe859d94da08f9f3387a2c933c5c3a701289`  
		Last Modified: Wed, 01 Nov 2023 01:49:29 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4e74a59eb1bbbac0433a03c3df812810095d2f7d1e03133d6501fd8c29ba83`  
		Last Modified: Wed, 01 Nov 2023 01:49:29 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4c433447043d6daa20d54cff95f75f0e1f42b9f8a3e91ae1f28e5964d2f7b08`  
		Last Modified: Wed, 01 Nov 2023 01:49:29 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74642c019385d2d0c4880e20c048b3e1ca10a9ac41ee087a3d2aa1472198bece`  
		Last Modified: Wed, 01 Nov 2023 01:49:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:50f56bb00da2283699ec0177ad4d593641e785821ae5bc4b73178c6774cd4646
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75138217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cb71bb390f93796c3435d6dde62d5d085fd1a5c35075e2185e308f4a59fe527`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:09 GMT
ADD file:ad1947b1fc97bcc228c004c15afeb2d9006d47167db69cf7b05c3e634c648166 in / 
# Wed, 01 Nov 2023 00:40:10 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:54:28 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Nov 2023 02:54:28 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Nov 2023 02:54:35 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:54:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Nov 2023 02:54:39 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Nov 2023 02:54:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:54:45 GMT
ENV COUCHDB_VERSION=3.1.2
# Wed, 01 Nov 2023 02:54:45 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Nov 2023 02:54:57 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Nov 2023 02:54:57 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Nov 2023 02:54:58 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 01 Nov 2023 02:54:58 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 01 Nov 2023 02:54:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Nov 2023 02:54:58 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 02:54:58 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Nov 2023 02:54:58 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Nov 2023 02:54:58 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:094e0a7927f79c559fdab346774d7de6e5fc38e2d998e82dd663850ebbff4648`  
		Last Modified: Wed, 01 Nov 2023 00:44:25 GMT  
		Size: 26.0 MB (25967703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc5be3d4f1542e6fc11ee7fcc29abb4753366751c6c627a92ba68dc7bf2e012`  
		Last Modified: Wed, 01 Nov 2023 02:55:49 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0f557682501a5ca3e65c0c48b65e6645c396a0471d6a8d63a8f2f1bb92fb08`  
		Last Modified: Wed, 01 Nov 2023 02:55:48 GMT  
		Size: 6.6 MB (6577623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec4b7957cee1703ce1207b0b11d9e4aed5a56dd9eac981116cf46305e545576`  
		Last Modified: Wed, 01 Nov 2023 02:55:48 GMT  
		Size: 1.2 MB (1164824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6921da86aad61db9f07f1b09e040f85e1c3422fe0459bd50995cb939273ea0c3`  
		Last Modified: Wed, 01 Nov 2023 02:55:47 GMT  
		Size: 294.4 KB (294429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79097584adbd9784fe2820ee58e141e35ad2fe24698689ccda6611a1dea0e12e`  
		Last Modified: Wed, 01 Nov 2023 02:55:47 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74d1d83ec6199277ee40155b597f4be2ad06f5cdca5fdcd4674527e44842453`  
		Last Modified: Wed, 01 Nov 2023 02:55:49 GMT  
		Size: 41.1 MB (41126602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677bfaf6801ddda0fdc709426dae691125b41131143a833766f4865851105155`  
		Last Modified: Wed, 01 Nov 2023 02:55:45 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a7d176e5ec1d80b8cb76448b8c58d1bf17052aa8d17e3a3b3def4a1b920fe6`  
		Last Modified: Wed, 01 Nov 2023 02:55:45 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:004003e8fce0ec36a28e071d501c6030975b5755df76b670cf5379635c548cea`  
		Last Modified: Wed, 01 Nov 2023 02:55:45 GMT  
		Size: 2.1 KB (2061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ea814937b8626214404c0637f94752bf93d701b23ff94235faec3439c3f822`  
		Last Modified: Wed, 01 Nov 2023 02:55:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1.2`

```console
$ docker pull couchdb@sha256:bb6adfda153f4deb7df949817e186fb66e25e9d309eb5f54b24b6e7980f5655f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1.2` - linux; amd64

```console
$ docker pull couchdb@sha256:d64439bcd931bfe3b2b48135529b514beab649fa0259881fd04c774f2c3d5422
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.1 MB (80075635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:205e57c6f99f40a4d603140fe6501754b9f090f9630e35f08a02887e35b43e91`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:33 GMT
ADD file:29d3eb64d192a97184f2aa169407b58e969b06268c6372b49eefb72bcadb6e99 in / 
# Wed, 01 Nov 2023 00:21:34 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:47:35 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Nov 2023 01:47:36 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Nov 2023 01:47:43 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:47:47 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Nov 2023 01:47:47 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Nov 2023 01:47:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:47:53 GMT
ENV COUCHDB_VERSION=3.1.2
# Wed, 01 Nov 2023 01:47:54 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Nov 2023 01:48:07 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Nov 2023 01:48:08 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Nov 2023 01:48:08 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 01 Nov 2023 01:48:08 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 01 Nov 2023 01:48:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Nov 2023 01:48:09 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 01:48:09 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Nov 2023 01:48:09 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Nov 2023 01:48:09 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:113c6ad4754853f4a2ae632cff7d90eba9145cca0bd6fa4d60aa432bd26be6c7`  
		Last Modified: Wed, 01 Nov 2023 00:26:56 GMT  
		Size: 27.2 MB (27187422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365ea17356912d8ab65ea5e3a1e839d36823f7303a6f99fec14eb169f5a4f2e1`  
		Last Modified: Wed, 01 Nov 2023 01:49:33 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2706b6ad14bfc13aa94a94269c8479e367a22ebbf64f230b4a133b8198b51523`  
		Last Modified: Wed, 01 Nov 2023 01:49:32 GMT  
		Size: 6.7 MB (6704557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3cbd037256b0218774d56e4d3151275a32733815758ef37784eae1b624c9831`  
		Last Modified: Wed, 01 Nov 2023 01:49:31 GMT  
		Size: 1.3 MB (1259891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7bc073931afdef902766bdbf4440108b63b7e7a8afc61c51d5132e2b366910`  
		Last Modified: Wed, 01 Nov 2023 01:49:31 GMT  
		Size: 294.5 KB (294533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4debe8d86185b55779861ac36695c6d3d6f33c7b19c8b4d6d8b1edf847264fc8`  
		Last Modified: Wed, 01 Nov 2023 01:49:30 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:771c29924f094333de4b98cd2e8acaa0f6bd0f0737f62f73c3ff771764790fb0`  
		Last Modified: Wed, 01 Nov 2023 01:49:33 GMT  
		Size: 44.6 MB (44622218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04407e3339446bef5cd7c3a5bdadbe859d94da08f9f3387a2c933c5c3a701289`  
		Last Modified: Wed, 01 Nov 2023 01:49:29 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4e74a59eb1bbbac0433a03c3df812810095d2f7d1e03133d6501fd8c29ba83`  
		Last Modified: Wed, 01 Nov 2023 01:49:29 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4c433447043d6daa20d54cff95f75f0e1f42b9f8a3e91ae1f28e5964d2f7b08`  
		Last Modified: Wed, 01 Nov 2023 01:49:29 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74642c019385d2d0c4880e20c048b3e1ca10a9ac41ee087a3d2aa1472198bece`  
		Last Modified: Wed, 01 Nov 2023 01:49:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:50f56bb00da2283699ec0177ad4d593641e785821ae5bc4b73178c6774cd4646
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75138217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cb71bb390f93796c3435d6dde62d5d085fd1a5c35075e2185e308f4a59fe527`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:09 GMT
ADD file:ad1947b1fc97bcc228c004c15afeb2d9006d47167db69cf7b05c3e634c648166 in / 
# Wed, 01 Nov 2023 00:40:10 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:54:28 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Nov 2023 02:54:28 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Nov 2023 02:54:35 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:54:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Nov 2023 02:54:39 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Nov 2023 02:54:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:54:45 GMT
ENV COUCHDB_VERSION=3.1.2
# Wed, 01 Nov 2023 02:54:45 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Nov 2023 02:54:57 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Nov 2023 02:54:57 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Nov 2023 02:54:58 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 01 Nov 2023 02:54:58 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 01 Nov 2023 02:54:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Nov 2023 02:54:58 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 02:54:58 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Nov 2023 02:54:58 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Nov 2023 02:54:58 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:094e0a7927f79c559fdab346774d7de6e5fc38e2d998e82dd663850ebbff4648`  
		Last Modified: Wed, 01 Nov 2023 00:44:25 GMT  
		Size: 26.0 MB (25967703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc5be3d4f1542e6fc11ee7fcc29abb4753366751c6c627a92ba68dc7bf2e012`  
		Last Modified: Wed, 01 Nov 2023 02:55:49 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0f557682501a5ca3e65c0c48b65e6645c396a0471d6a8d63a8f2f1bb92fb08`  
		Last Modified: Wed, 01 Nov 2023 02:55:48 GMT  
		Size: 6.6 MB (6577623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec4b7957cee1703ce1207b0b11d9e4aed5a56dd9eac981116cf46305e545576`  
		Last Modified: Wed, 01 Nov 2023 02:55:48 GMT  
		Size: 1.2 MB (1164824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6921da86aad61db9f07f1b09e040f85e1c3422fe0459bd50995cb939273ea0c3`  
		Last Modified: Wed, 01 Nov 2023 02:55:47 GMT  
		Size: 294.4 KB (294429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79097584adbd9784fe2820ee58e141e35ad2fe24698689ccda6611a1dea0e12e`  
		Last Modified: Wed, 01 Nov 2023 02:55:47 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74d1d83ec6199277ee40155b597f4be2ad06f5cdca5fdcd4674527e44842453`  
		Last Modified: Wed, 01 Nov 2023 02:55:49 GMT  
		Size: 41.1 MB (41126602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677bfaf6801ddda0fdc709426dae691125b41131143a833766f4865851105155`  
		Last Modified: Wed, 01 Nov 2023 02:55:45 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a7d176e5ec1d80b8cb76448b8c58d1bf17052aa8d17e3a3b3def4a1b920fe6`  
		Last Modified: Wed, 01 Nov 2023 02:55:45 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:004003e8fce0ec36a28e071d501c6030975b5755df76b670cf5379635c548cea`  
		Last Modified: Wed, 01 Nov 2023 02:55:45 GMT  
		Size: 2.1 KB (2061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ea814937b8626214404c0637f94752bf93d701b23ff94235faec3439c3f822`  
		Last Modified: Wed, 01 Nov 2023 02:55:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2`

```console
$ docker pull couchdb@sha256:8a5147883071d0704020753781b7fbd7e24fbeb8c49d1004c2da3e78d484939e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2` - linux; amd64

```console
$ docker pull couchdb@sha256:920faa468ec44afab004cc39e9768aa379a91eb2b08df506bcdc5aaa18765bff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.7 MB (89746808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e098381214be901b170999d456be51caf296a2a26345be64f33d40dd2421f30`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:46:40 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Nov 2023 01:46:41 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Nov 2023 01:46:47 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:46:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 01 Nov 2023 01:46:51 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Nov 2023 01:46:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:47:15 GMT
ENV COUCHDB_VERSION=3.2.3
# Wed, 01 Nov 2023 01:47:15 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Nov 2023 01:47:28 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Nov 2023 01:47:29 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Nov 2023 01:47:29 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 01 Nov 2023 01:47:29 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 01 Nov 2023 01:47:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Nov 2023 01:47:30 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 01:47:30 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Nov 2023 01:47:30 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Nov 2023 01:47:30 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbba1a29bfe2ee9664ccd0caa145b5aa7a5480c276f1c42fd77ac32ef2c440c1`  
		Last Modified: Wed, 01 Nov 2023 01:48:53 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b21d450d3bd9333c8a5efb4081f440607452820e295142168061b2216f3986c`  
		Last Modified: Wed, 01 Nov 2023 01:48:53 GMT  
		Size: 5.2 MB (5226554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c93767e1cbf8a0b2d24469dbe0f750b73d88204210f83f7faa87b8be37dfaa`  
		Last Modified: Wed, 01 Nov 2023 01:48:52 GMT  
		Size: 610.9 KB (610919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24dc783ed2d49dd34054350d1a680091886de94bd264352e835184065e394e64`  
		Last Modified: Wed, 01 Nov 2023 01:48:52 GMT  
		Size: 295.2 KB (295153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3095226c333171f329b0b302f35b809cee56c32b4129b1faa460f655ca1da73a`  
		Last Modified: Wed, 01 Nov 2023 01:49:17 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05b8c804244b1c762a3d12f9ce96d57339dbfd5e4f2f514e001c76114d90362`  
		Last Modified: Wed, 01 Nov 2023 01:49:20 GMT  
		Size: 52.2 MB (52188854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608652e0912931c13140293ddf5859b35e9dc3ec420a7b7cdb66335dd8d4aa25`  
		Last Modified: Wed, 01 Nov 2023 01:49:15 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0740499e7d320dbadd105454a7a5783a998c0cecb76d1db6794baade4e8e715`  
		Last Modified: Wed, 01 Nov 2023 01:49:15 GMT  
		Size: 997.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f15b969faacebc224c92b52534e1bf59e947e6c973aa304d8502a732331de84`  
		Last Modified: Wed, 01 Nov 2023 01:49:15 GMT  
		Size: 2.2 KB (2230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bafbb4496c4b925498eea59607a6cd21da7da01a3d8e67d869a0558b1506c8a`  
		Last Modified: Wed, 01 Nov 2023 01:49:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:960305e9b35826163f173e8b89eab4112410bee3725c3f0773140932dd9f7877
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.2 MB (85205205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:352add31bc606968e9b4695dc003a06de6c7ca3682ea0d3145b972feb8dabfee`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:33:39 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 12 Apr 2023 01:33:39 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 12 Apr 2023 01:33:45 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:33:48 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 12 Apr 2023 01:33:48 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 12 Apr 2023 01:33:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:34:12 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Wed, 12 Apr 2023 01:34:12 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 12 Apr 2023 01:34:24 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 12 Apr 2023 01:34:24 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 12 Apr 2023 01:34:24 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 12 Apr 2023 01:34:24 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 12 Apr 2023 01:34:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 12 Apr 2023 01:34:25 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 01:34:25 GMT
VOLUME [/opt/couchdb/data]
# Wed, 12 Apr 2023 01:34:25 GMT
EXPOSE 4369 5984 9100
# Wed, 12 Apr 2023 01:34:25 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f522824805b9b3818de882a514dd5454399e3c21b512a09e64274bf12d18ab4`  
		Last Modified: Wed, 12 Apr 2023 01:35:29 GMT  
		Size: 3.4 KB (3434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdfaf598c101b0427a73a7b5a1edb3b6229985b64794e6d215eb049125bbd25`  
		Last Modified: Wed, 12 Apr 2023 01:35:27 GMT  
		Size: 5.2 MB (5209561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc33796685833f0fdacecb6c4f2078915729822d8fb7a21aada1b767c48b377`  
		Last Modified: Wed, 12 Apr 2023 01:35:27 GMT  
		Size: 566.3 KB (566295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356323e70f7127294f4bee19c211582a4af79acc6d1f696d70fc94229c84aa52`  
		Last Modified: Wed, 12 Apr 2023 01:35:27 GMT  
		Size: 294.3 KB (294328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9652526d42f149093060de62ac3b39905fb0bfb8457d6148e4314ef71058a153`  
		Last Modified: Wed, 12 Apr 2023 01:35:44 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d95be693dac094ea4fe70ff2bd1f44b66a9ede007474a31cafcb829c361429`  
		Last Modified: Wed, 12 Apr 2023 01:35:47 GMT  
		Size: 49.1 MB (49063995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61eb7f6826c8440901fb275f2b3c5f6be3e97d95482db6770215d5bd31899ed1`  
		Last Modified: Wed, 12 Apr 2023 01:35:42 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d81fa00cdd93053287b1afda2f3cfda4475c6ac6307dc22125a76f843f21415`  
		Last Modified: Wed, 12 Apr 2023 01:35:43 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16e726b19dd008ea8df7bf3ce90fa1947f685d2f6fdd3caa36e1f3b6e40526d0`  
		Last Modified: Wed, 12 Apr 2023 01:35:43 GMT  
		Size: 2.2 KB (2227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c78146fce98da16e884fde6d22f444849c69c3da90555e336827ceb2b6a039`  
		Last Modified: Wed, 12 Apr 2023 01:35:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; ppc64le

```console
$ docker pull couchdb@sha256:90a95123b16f3f08c9e3b862a7e628ead429c8602d5dc110db1b038b5b47db9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.4 MB (92383985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7c0714b286e5789d8b829c846536d1f8a5308d8cf419fa60995af8b91ab3b55`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 12 Apr 2023 00:08:20 GMT
ADD file:63eb52aaff02c15bceabb87a78eb1b36389066ff4774cf8a754160ca7d509816 in / 
# Wed, 12 Apr 2023 00:08:23 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:23:31 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 12 Apr 2023 01:23:35 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 12 Apr 2023 01:23:57 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:24:07 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 12 Apr 2023 01:24:08 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 12 Apr 2023 01:24:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:25:25 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Wed, 12 Apr 2023 01:25:27 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 12 Apr 2023 01:25:58 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 12 Apr 2023 01:26:02 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 12 Apr 2023 01:26:02 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 12 Apr 2023 01:26:03 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 12 Apr 2023 01:26:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 12 Apr 2023 01:26:05 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 01:26:06 GMT
VOLUME [/opt/couchdb/data]
# Wed, 12 Apr 2023 01:26:06 GMT
EXPOSE 4369 5984 9100
# Wed, 12 Apr 2023 01:26:07 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:5b41d5ec640939cf684959234ad3b80909268a32bfd520a31c6720a91521c2fa`  
		Last Modified: Wed, 12 Apr 2023 00:13:13 GMT  
		Size: 35.3 MB (35291995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7569dcea363c11bb071b416ea27193dbe62d8a210fa1f829efabb35b46600dae`  
		Last Modified: Wed, 12 Apr 2023 01:26:25 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a685c575c0e899abc0410edf84715dd5cf4184fcbd447fdbbcac069795eadd05`  
		Last Modified: Wed, 12 Apr 2023 01:26:26 GMT  
		Size: 6.0 MB (6044117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0283a2882808914c7a35f392d4ad2d2921ccf8b8855ab399e2998c22d061f16e`  
		Last Modified: Wed, 12 Apr 2023 01:26:24 GMT  
		Size: 662.1 KB (662116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17deb4c48f5c43beee592bed99d27502afe8c8f60cde1cb4bebb7dce00e877c`  
		Last Modified: Wed, 12 Apr 2023 01:26:24 GMT  
		Size: 294.3 KB (294319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7661a9384c6767a073bc8e86df2ec2c60bef8bad55fac7ab22d7ecffcdb1f1`  
		Last Modified: Wed, 12 Apr 2023 01:26:48 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74733b44093de42db86284861068e909838a6bca4f3ecf0bfd04eb99d5bf8c79`  
		Last Modified: Wed, 12 Apr 2023 01:26:56 GMT  
		Size: 50.1 MB (50084252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c567dbfb6ac3167b1cd2d6532940fd6fb66d9b5b6a1dedf22d61b92a7b4095eb`  
		Last Modified: Wed, 12 Apr 2023 01:26:46 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf08299e06354b4674e5fabd7e99da65832d26bc98826c051d261e7a03195099`  
		Last Modified: Wed, 12 Apr 2023 01:26:46 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5861e0f3152c23eda58111aaac02f82ed4973711f9a55c51cb55ebb9af6220`  
		Last Modified: Wed, 12 Apr 2023 01:26:46 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54774512e47b4b9a6dee9f79bf7ec483b3c7c234e949bc4f6c96fb22a3e8237`  
		Last Modified: Wed, 12 Apr 2023 01:26:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2.3`

```console
$ docker pull couchdb@sha256:eac50b3e16c45fed8c14501e6fd3f157a3b662291de7997d9625e770589dbbea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchdb:3.2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:920faa468ec44afab004cc39e9768aa379a91eb2b08df506bcdc5aaa18765bff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.7 MB (89746808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e098381214be901b170999d456be51caf296a2a26345be64f33d40dd2421f30`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:46:40 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Nov 2023 01:46:41 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Nov 2023 01:46:47 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:46:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 01 Nov 2023 01:46:51 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Nov 2023 01:46:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:47:15 GMT
ENV COUCHDB_VERSION=3.2.3
# Wed, 01 Nov 2023 01:47:15 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Nov 2023 01:47:28 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Nov 2023 01:47:29 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Nov 2023 01:47:29 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 01 Nov 2023 01:47:29 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 01 Nov 2023 01:47:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Nov 2023 01:47:30 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 01:47:30 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Nov 2023 01:47:30 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Nov 2023 01:47:30 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbba1a29bfe2ee9664ccd0caa145b5aa7a5480c276f1c42fd77ac32ef2c440c1`  
		Last Modified: Wed, 01 Nov 2023 01:48:53 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b21d450d3bd9333c8a5efb4081f440607452820e295142168061b2216f3986c`  
		Last Modified: Wed, 01 Nov 2023 01:48:53 GMT  
		Size: 5.2 MB (5226554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c93767e1cbf8a0b2d24469dbe0f750b73d88204210f83f7faa87b8be37dfaa`  
		Last Modified: Wed, 01 Nov 2023 01:48:52 GMT  
		Size: 610.9 KB (610919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24dc783ed2d49dd34054350d1a680091886de94bd264352e835184065e394e64`  
		Last Modified: Wed, 01 Nov 2023 01:48:52 GMT  
		Size: 295.2 KB (295153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3095226c333171f329b0b302f35b809cee56c32b4129b1faa460f655ca1da73a`  
		Last Modified: Wed, 01 Nov 2023 01:49:17 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05b8c804244b1c762a3d12f9ce96d57339dbfd5e4f2f514e001c76114d90362`  
		Last Modified: Wed, 01 Nov 2023 01:49:20 GMT  
		Size: 52.2 MB (52188854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608652e0912931c13140293ddf5859b35e9dc3ec420a7b7cdb66335dd8d4aa25`  
		Last Modified: Wed, 01 Nov 2023 01:49:15 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0740499e7d320dbadd105454a7a5783a998c0cecb76d1db6794baade4e8e715`  
		Last Modified: Wed, 01 Nov 2023 01:49:15 GMT  
		Size: 997.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f15b969faacebc224c92b52534e1bf59e947e6c973aa304d8502a732331de84`  
		Last Modified: Wed, 01 Nov 2023 01:49:15 GMT  
		Size: 2.2 KB (2230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bafbb4496c4b925498eea59607a6cd21da7da01a3d8e67d869a0558b1506c8a`  
		Last Modified: Wed, 01 Nov 2023 01:49:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.3`

```console
$ docker pull couchdb@sha256:482d73fa450a18bce6ff591740b7a69f21a1cf94ffcd295a500e5214981e18d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `couchdb:3.3` - linux; amd64

```console
$ docker pull couchdb@sha256:3c609bc33e472d4cb0a4ea0b117359bd0c9ed4f0628899131e8344fd13fbe01a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90245671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fff4b56666dbf396fc0b2eedb70c70b8990ccb6dc5d8447206f2243d21c1986c`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:46:40 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Nov 2023 01:46:41 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Nov 2023 01:46:47 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:46:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 01 Nov 2023 01:46:51 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Nov 2023 01:46:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:46:56 GMT
ENV COUCHDB_VERSION=3.3.2
# Wed, 01 Nov 2023 01:46:56 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Nov 2023 01:47:10 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Nov 2023 01:47:10 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Nov 2023 01:47:10 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 01 Nov 2023 01:47:11 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 01 Nov 2023 01:47:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Nov 2023 01:47:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 01:47:11 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Nov 2023 01:47:11 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Nov 2023 01:47:11 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbba1a29bfe2ee9664ccd0caa145b5aa7a5480c276f1c42fd77ac32ef2c440c1`  
		Last Modified: Wed, 01 Nov 2023 01:48:53 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b21d450d3bd9333c8a5efb4081f440607452820e295142168061b2216f3986c`  
		Last Modified: Wed, 01 Nov 2023 01:48:53 GMT  
		Size: 5.2 MB (5226554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c93767e1cbf8a0b2d24469dbe0f750b73d88204210f83f7faa87b8be37dfaa`  
		Last Modified: Wed, 01 Nov 2023 01:48:52 GMT  
		Size: 610.9 KB (610919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24dc783ed2d49dd34054350d1a680091886de94bd264352e835184065e394e64`  
		Last Modified: Wed, 01 Nov 2023 01:48:52 GMT  
		Size: 295.2 KB (295153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8597086eac85cffb9306a84cfa8414bcda5500cb8092b1ba307a38e9e56540f`  
		Last Modified: Wed, 01 Nov 2023 01:48:52 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4fefd748372d68972d6fb14014c7813ac7837a6380b957f3092da518331958`  
		Last Modified: Wed, 01 Nov 2023 01:48:55 GMT  
		Size: 52.7 MB (52687716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ff2441b3a4073bbf88542aaf2d970fd2eb11cc4bd01c846d1245dae6187068`  
		Last Modified: Wed, 01 Nov 2023 01:48:50 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c29c7241d3a11a9dcf62611e3563275d0b24d32fa9f65fb5be837b13ef1cfb4`  
		Last Modified: Wed, 01 Nov 2023 01:48:50 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacd4b2ce1758697d4898b78068d98430738b73f2f0171222ea8fc970a567603`  
		Last Modified: Wed, 01 Nov 2023 01:48:50 GMT  
		Size: 2.2 KB (2228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7254e813570e08d636b0b367fb2dfe8c25dfa8b3a07a24b4dcf9574a9e238270`  
		Last Modified: Wed, 01 Nov 2023 01:48:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:a4d2708520335bec287044683aa008f3ee0af0174c4844f4c27d73581ef39326
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88693209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a609af91aa2f1677f43a122b8a919068545adc446fc3857244fe5a8d89b703d5`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:53:44 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Nov 2023 02:53:44 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Nov 2023 02:53:50 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:53:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 01 Nov 2023 02:53:53 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Nov 2023 02:53:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:53:58 GMT
ENV COUCHDB_VERSION=3.3.2
# Wed, 01 Nov 2023 02:53:58 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Nov 2023 02:54:11 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Nov 2023 02:54:12 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Nov 2023 02:54:12 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 01 Nov 2023 02:54:12 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 01 Nov 2023 02:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Nov 2023 02:54:12 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 02:54:12 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Nov 2023 02:54:12 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Nov 2023 02:54:13 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b614568051476b61815cad57612a54fb357dce26265c2d8a93d3603e65f67bb`  
		Last Modified: Wed, 01 Nov 2023 02:55:30 GMT  
		Size: 3.4 KB (3431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c7e0362f1203d4c8eb75046c1009a66141067e9cb7a5e02ac76702b3a4fc5e`  
		Last Modified: Wed, 01 Nov 2023 02:55:29 GMT  
		Size: 5.2 MB (5210837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936a7f3d3f0f461eb2f034fa209eb834d4f53ab52e315c1ea90e4436d100cc12`  
		Last Modified: Wed, 01 Nov 2023 02:55:29 GMT  
		Size: 567.1 KB (567066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cea30aeda14f6e14599fb09aa79b3a41556b7509b7d4835f0d97a0e131aff2c`  
		Last Modified: Wed, 01 Nov 2023 02:55:29 GMT  
		Size: 295.0 KB (295032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a6600b43b5af044cab2a8316adbf77eed718e07be3a49b46d0d40f52bd9142`  
		Last Modified: Wed, 01 Nov 2023 02:55:28 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb3d645b10a8f7621c93c74d0ef540bf7eaa4110c0aeb1c226e7a3fde645671`  
		Last Modified: Wed, 01 Nov 2023 02:55:31 GMT  
		Size: 52.5 MB (52548927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0231949bd50a35a558a786ffd81b537869d8c2008032cf8f763cf817364efbc`  
		Last Modified: Wed, 01 Nov 2023 02:55:26 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce55a94b61b5a276dbee100f2f54d927ab8e493c9eef066a8604e6d29c611ab9`  
		Last Modified: Wed, 01 Nov 2023 02:55:26 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c997e552c1313a4b038f571f70da3ddf3a0b62fade23a017f7ba4dfbbeecc46`  
		Last Modified: Wed, 01 Nov 2023 02:55:26 GMT  
		Size: 2.2 KB (2230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15920850d8d556ea5c5d6b5a45df1b59867930cd37d1d15f1f712d12ee66edaf`  
		Last Modified: Wed, 01 Nov 2023 02:55:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3` - linux; ppc64le

```console
$ docker pull couchdb@sha256:ccf9e925a92c4e47c922173bb8a6541607469de85a3d23b8f709a5b2f9fa4571
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.0 MB (95968231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0d5240fcc3525a7c996865649016d229a3b75d1447c7ade86132d7ede52ffe8`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:43 GMT
ADD file:b0d18f2d04821eb50d1faecc1a64916f5c63dd386ae71a3b2cb1d6c4aac6e1c4 in / 
# Tue, 21 Nov 2023 04:24:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:12:10 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Nov 2023 07:12:12 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Nov 2023 07:12:31 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:12:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 21 Nov 2023 07:12:37 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Nov 2023 07:12:47 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:12:47 GMT
ENV COUCHDB_VERSION=3.3.2
# Tue, 21 Nov 2023 07:12:49 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Nov 2023 07:13:13 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Nov 2023 07:13:17 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Nov 2023 07:13:17 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 21 Nov 2023 07:13:17 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 21 Nov 2023 07:13:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Nov 2023 07:13:20 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Nov 2023 07:13:20 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Nov 2023 07:13:20 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Nov 2023 07:13:21 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:60239a74847cd7e9a928353188f3cf096ca8cf648e2b27c765058e169d568fd9`  
		Last Modified: Tue, 21 Nov 2023 04:29:47 GMT  
		Size: 35.3 MB (35293727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f63eed5db2c906b6108908d9dc6976c9a23f1bb19a0e617257decd133e7592d`  
		Last Modified: Tue, 21 Nov 2023 07:14:05 GMT  
		Size: 3.4 KB (3408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941bb642de45bb343a873e9c819cd85bffe05a010a6da631d1723612f69c794c`  
		Last Modified: Tue, 21 Nov 2023 07:14:04 GMT  
		Size: 6.0 MB (6046203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f2659433b58c3235f1e9085447d55d5c442efc597e42f97dfce11b106d84c0`  
		Last Modified: Tue, 21 Nov 2023 07:14:04 GMT  
		Size: 662.9 KB (662883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d777a7fd59124bb1d1eed56bddee9639f6ea57c6eaf67610a97a4a8c833814e9`  
		Last Modified: Tue, 21 Nov 2023 07:14:03 GMT  
		Size: 295.1 KB (295091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef322b815f454b44be7fc5bbc3f2c179419841031a40a753c25cb71a704158f4`  
		Last Modified: Tue, 21 Nov 2023 07:14:03 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6180ccba02f37081c0d1523baa72b7df6183b2284a575cc84c8f245ed21624fc`  
		Last Modified: Tue, 21 Nov 2023 07:14:07 GMT  
		Size: 53.7 MB (53662909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991739364f41cbdef5c3adb115b1f41c51bbafbd6555e32316cad98f1cae7e54`  
		Last Modified: Tue, 21 Nov 2023 07:14:01 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f539c1a9af058023c294a0b078bb81ec732ba18d3e4c624af45c5e3a877c5dd`  
		Last Modified: Tue, 21 Nov 2023 07:14:01 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27abb88fb75707dd945625a5a2734aa790dcd4330e5d257d13fde86d69630c4`  
		Last Modified: Tue, 21 Nov 2023 07:14:01 GMT  
		Size: 2.2 KB (2232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7837c78696f2a9940c752105b06aeb98a48f8a6eacab80ba3a467f89fbe31ee5`  
		Last Modified: Tue, 21 Nov 2023 07:14:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3` - linux; s390x

```console
$ docker pull couchdb@sha256:21965f0438b454449366375d4c6bfd319e83dec568e9907669ba2b6a1c077563
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.0 MB (87002806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba071f2f075a8263e2e67f1fc0f844debd3e57242ac3165ff9adcfacf2338049`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Nov 2023 05:05:18 GMT
ADD file:a545f27075704ce13e33e539170d3f47007424d2cc2bea5aecfd2608a5194151 in / 
# Tue, 21 Nov 2023 05:05:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:20:22 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Nov 2023 06:20:22 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Nov 2023 06:20:28 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:20:31 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 21 Nov 2023 06:20:31 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Nov 2023 06:20:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:20:36 GMT
ENV COUCHDB_VERSION=3.3.2
# Tue, 21 Nov 2023 06:20:36 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Nov 2023 06:20:53 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Nov 2023 06:20:55 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Nov 2023 06:20:55 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 21 Nov 2023 06:20:55 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 21 Nov 2023 06:20:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Nov 2023 06:20:56 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Nov 2023 06:20:56 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Nov 2023 06:20:56 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Nov 2023 06:20:56 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b114072f1cab66b7376d690985b12816aebab2e4e41fc170e32f111df27951dc`  
		Last Modified: Tue, 21 Nov 2023 05:10:48 GMT  
		Size: 29.7 MB (29656938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72dba253785a5e917fdd9064f61b676b4080ff3073424ff387308d70579c728b`  
		Last Modified: Tue, 21 Nov 2023 06:21:15 GMT  
		Size: 3.4 KB (3431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a299cd04ea14bbc3034e11001a1ec06dd4b5e1aaa78317dc803570f8a4c6437`  
		Last Modified: Tue, 21 Nov 2023 06:21:15 GMT  
		Size: 5.1 MB (5111719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c684e5bcbb93c8f0c9da5b81b4a1d19274f7ad0c7e3b17eb12cbe45cd2514989`  
		Last Modified: Tue, 21 Nov 2023 06:21:14 GMT  
		Size: 573.6 KB (573635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d916370cd04b7352346fee3edc1ac77bdb9393e24c5bc62c4cb0803a682836`  
		Last Modified: Tue, 21 Nov 2023 06:21:14 GMT  
		Size: 295.1 KB (295096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e602d723a112bfbe3ebaca9b99e2e9636dac8b07c69947311ceb07666d40ed`  
		Last Modified: Tue, 21 Nov 2023 06:21:14 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbafbeffdc5d29b56e0ccf672e48ead551f49aa23534b4fd9aefcd339587dc5`  
		Last Modified: Tue, 21 Nov 2023 06:21:18 GMT  
		Size: 51.4 MB (51357976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f08f21ade417458e581ec8afdf835c5d165444c0e93fdc330cbd6146af1da3`  
		Last Modified: Tue, 21 Nov 2023 06:21:13 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a4bc9e282fe338ed74c99dbb5cb5777e0ba1a2d068de6e102a8adbb34acc14`  
		Last Modified: Tue, 21 Nov 2023 06:21:13 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c93f5a64665780dfb559adfed9587064e52e00c9c515834a97cf26e3529da9`  
		Last Modified: Tue, 21 Nov 2023 06:21:13 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f6f407505b71a14801c0c71da8d0ce2a85d8c65d58e7998784a75dcde3cfb6`  
		Last Modified: Tue, 21 Nov 2023 06:21:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.3.2`

```console
$ docker pull couchdb@sha256:482d73fa450a18bce6ff591740b7a69f21a1cf94ffcd295a500e5214981e18d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `couchdb:3.3.2` - linux; amd64

```console
$ docker pull couchdb@sha256:3c609bc33e472d4cb0a4ea0b117359bd0c9ed4f0628899131e8344fd13fbe01a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90245671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fff4b56666dbf396fc0b2eedb70c70b8990ccb6dc5d8447206f2243d21c1986c`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:46:40 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Nov 2023 01:46:41 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Nov 2023 01:46:47 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:46:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 01 Nov 2023 01:46:51 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Nov 2023 01:46:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:46:56 GMT
ENV COUCHDB_VERSION=3.3.2
# Wed, 01 Nov 2023 01:46:56 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Nov 2023 01:47:10 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Nov 2023 01:47:10 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Nov 2023 01:47:10 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 01 Nov 2023 01:47:11 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 01 Nov 2023 01:47:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Nov 2023 01:47:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 01:47:11 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Nov 2023 01:47:11 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Nov 2023 01:47:11 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbba1a29bfe2ee9664ccd0caa145b5aa7a5480c276f1c42fd77ac32ef2c440c1`  
		Last Modified: Wed, 01 Nov 2023 01:48:53 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b21d450d3bd9333c8a5efb4081f440607452820e295142168061b2216f3986c`  
		Last Modified: Wed, 01 Nov 2023 01:48:53 GMT  
		Size: 5.2 MB (5226554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c93767e1cbf8a0b2d24469dbe0f750b73d88204210f83f7faa87b8be37dfaa`  
		Last Modified: Wed, 01 Nov 2023 01:48:52 GMT  
		Size: 610.9 KB (610919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24dc783ed2d49dd34054350d1a680091886de94bd264352e835184065e394e64`  
		Last Modified: Wed, 01 Nov 2023 01:48:52 GMT  
		Size: 295.2 KB (295153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8597086eac85cffb9306a84cfa8414bcda5500cb8092b1ba307a38e9e56540f`  
		Last Modified: Wed, 01 Nov 2023 01:48:52 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4fefd748372d68972d6fb14014c7813ac7837a6380b957f3092da518331958`  
		Last Modified: Wed, 01 Nov 2023 01:48:55 GMT  
		Size: 52.7 MB (52687716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ff2441b3a4073bbf88542aaf2d970fd2eb11cc4bd01c846d1245dae6187068`  
		Last Modified: Wed, 01 Nov 2023 01:48:50 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c29c7241d3a11a9dcf62611e3563275d0b24d32fa9f65fb5be837b13ef1cfb4`  
		Last Modified: Wed, 01 Nov 2023 01:48:50 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacd4b2ce1758697d4898b78068d98430738b73f2f0171222ea8fc970a567603`  
		Last Modified: Wed, 01 Nov 2023 01:48:50 GMT  
		Size: 2.2 KB (2228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7254e813570e08d636b0b367fb2dfe8c25dfa8b3a07a24b4dcf9574a9e238270`  
		Last Modified: Wed, 01 Nov 2023 01:48:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:a4d2708520335bec287044683aa008f3ee0af0174c4844f4c27d73581ef39326
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88693209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a609af91aa2f1677f43a122b8a919068545adc446fc3857244fe5a8d89b703d5`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:53:44 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Nov 2023 02:53:44 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Nov 2023 02:53:50 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:53:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 01 Nov 2023 02:53:53 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Nov 2023 02:53:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:53:58 GMT
ENV COUCHDB_VERSION=3.3.2
# Wed, 01 Nov 2023 02:53:58 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Nov 2023 02:54:11 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Nov 2023 02:54:12 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Nov 2023 02:54:12 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 01 Nov 2023 02:54:12 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 01 Nov 2023 02:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Nov 2023 02:54:12 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 02:54:12 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Nov 2023 02:54:12 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Nov 2023 02:54:13 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b614568051476b61815cad57612a54fb357dce26265c2d8a93d3603e65f67bb`  
		Last Modified: Wed, 01 Nov 2023 02:55:30 GMT  
		Size: 3.4 KB (3431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c7e0362f1203d4c8eb75046c1009a66141067e9cb7a5e02ac76702b3a4fc5e`  
		Last Modified: Wed, 01 Nov 2023 02:55:29 GMT  
		Size: 5.2 MB (5210837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936a7f3d3f0f461eb2f034fa209eb834d4f53ab52e315c1ea90e4436d100cc12`  
		Last Modified: Wed, 01 Nov 2023 02:55:29 GMT  
		Size: 567.1 KB (567066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cea30aeda14f6e14599fb09aa79b3a41556b7509b7d4835f0d97a0e131aff2c`  
		Last Modified: Wed, 01 Nov 2023 02:55:29 GMT  
		Size: 295.0 KB (295032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a6600b43b5af044cab2a8316adbf77eed718e07be3a49b46d0d40f52bd9142`  
		Last Modified: Wed, 01 Nov 2023 02:55:28 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb3d645b10a8f7621c93c74d0ef540bf7eaa4110c0aeb1c226e7a3fde645671`  
		Last Modified: Wed, 01 Nov 2023 02:55:31 GMT  
		Size: 52.5 MB (52548927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0231949bd50a35a558a786ffd81b537869d8c2008032cf8f763cf817364efbc`  
		Last Modified: Wed, 01 Nov 2023 02:55:26 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce55a94b61b5a276dbee100f2f54d927ab8e493c9eef066a8604e6d29c611ab9`  
		Last Modified: Wed, 01 Nov 2023 02:55:26 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c997e552c1313a4b038f571f70da3ddf3a0b62fade23a017f7ba4dfbbeecc46`  
		Last Modified: Wed, 01 Nov 2023 02:55:26 GMT  
		Size: 2.2 KB (2230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15920850d8d556ea5c5d6b5a45df1b59867930cd37d1d15f1f712d12ee66edaf`  
		Last Modified: Wed, 01 Nov 2023 02:55:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3.2` - linux; ppc64le

```console
$ docker pull couchdb@sha256:ccf9e925a92c4e47c922173bb8a6541607469de85a3d23b8f709a5b2f9fa4571
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.0 MB (95968231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0d5240fcc3525a7c996865649016d229a3b75d1447c7ade86132d7ede52ffe8`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:43 GMT
ADD file:b0d18f2d04821eb50d1faecc1a64916f5c63dd386ae71a3b2cb1d6c4aac6e1c4 in / 
# Tue, 21 Nov 2023 04:24:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:12:10 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Nov 2023 07:12:12 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Nov 2023 07:12:31 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:12:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 21 Nov 2023 07:12:37 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Nov 2023 07:12:47 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:12:47 GMT
ENV COUCHDB_VERSION=3.3.2
# Tue, 21 Nov 2023 07:12:49 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Nov 2023 07:13:13 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Nov 2023 07:13:17 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Nov 2023 07:13:17 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 21 Nov 2023 07:13:17 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 21 Nov 2023 07:13:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Nov 2023 07:13:20 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Nov 2023 07:13:20 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Nov 2023 07:13:20 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Nov 2023 07:13:21 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:60239a74847cd7e9a928353188f3cf096ca8cf648e2b27c765058e169d568fd9`  
		Last Modified: Tue, 21 Nov 2023 04:29:47 GMT  
		Size: 35.3 MB (35293727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f63eed5db2c906b6108908d9dc6976c9a23f1bb19a0e617257decd133e7592d`  
		Last Modified: Tue, 21 Nov 2023 07:14:05 GMT  
		Size: 3.4 KB (3408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941bb642de45bb343a873e9c819cd85bffe05a010a6da631d1723612f69c794c`  
		Last Modified: Tue, 21 Nov 2023 07:14:04 GMT  
		Size: 6.0 MB (6046203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f2659433b58c3235f1e9085447d55d5c442efc597e42f97dfce11b106d84c0`  
		Last Modified: Tue, 21 Nov 2023 07:14:04 GMT  
		Size: 662.9 KB (662883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d777a7fd59124bb1d1eed56bddee9639f6ea57c6eaf67610a97a4a8c833814e9`  
		Last Modified: Tue, 21 Nov 2023 07:14:03 GMT  
		Size: 295.1 KB (295091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef322b815f454b44be7fc5bbc3f2c179419841031a40a753c25cb71a704158f4`  
		Last Modified: Tue, 21 Nov 2023 07:14:03 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6180ccba02f37081c0d1523baa72b7df6183b2284a575cc84c8f245ed21624fc`  
		Last Modified: Tue, 21 Nov 2023 07:14:07 GMT  
		Size: 53.7 MB (53662909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991739364f41cbdef5c3adb115b1f41c51bbafbd6555e32316cad98f1cae7e54`  
		Last Modified: Tue, 21 Nov 2023 07:14:01 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f539c1a9af058023c294a0b078bb81ec732ba18d3e4c624af45c5e3a877c5dd`  
		Last Modified: Tue, 21 Nov 2023 07:14:01 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27abb88fb75707dd945625a5a2734aa790dcd4330e5d257d13fde86d69630c4`  
		Last Modified: Tue, 21 Nov 2023 07:14:01 GMT  
		Size: 2.2 KB (2232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7837c78696f2a9940c752105b06aeb98a48f8a6eacab80ba3a467f89fbe31ee5`  
		Last Modified: Tue, 21 Nov 2023 07:14:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3.2` - linux; s390x

```console
$ docker pull couchdb@sha256:21965f0438b454449366375d4c6bfd319e83dec568e9907669ba2b6a1c077563
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.0 MB (87002806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba071f2f075a8263e2e67f1fc0f844debd3e57242ac3165ff9adcfacf2338049`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Nov 2023 05:05:18 GMT
ADD file:a545f27075704ce13e33e539170d3f47007424d2cc2bea5aecfd2608a5194151 in / 
# Tue, 21 Nov 2023 05:05:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:20:22 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Nov 2023 06:20:22 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Nov 2023 06:20:28 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:20:31 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 21 Nov 2023 06:20:31 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Nov 2023 06:20:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:20:36 GMT
ENV COUCHDB_VERSION=3.3.2
# Tue, 21 Nov 2023 06:20:36 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Nov 2023 06:20:53 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Nov 2023 06:20:55 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Nov 2023 06:20:55 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 21 Nov 2023 06:20:55 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 21 Nov 2023 06:20:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Nov 2023 06:20:56 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Nov 2023 06:20:56 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Nov 2023 06:20:56 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Nov 2023 06:20:56 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b114072f1cab66b7376d690985b12816aebab2e4e41fc170e32f111df27951dc`  
		Last Modified: Tue, 21 Nov 2023 05:10:48 GMT  
		Size: 29.7 MB (29656938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72dba253785a5e917fdd9064f61b676b4080ff3073424ff387308d70579c728b`  
		Last Modified: Tue, 21 Nov 2023 06:21:15 GMT  
		Size: 3.4 KB (3431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a299cd04ea14bbc3034e11001a1ec06dd4b5e1aaa78317dc803570f8a4c6437`  
		Last Modified: Tue, 21 Nov 2023 06:21:15 GMT  
		Size: 5.1 MB (5111719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c684e5bcbb93c8f0c9da5b81b4a1d19274f7ad0c7e3b17eb12cbe45cd2514989`  
		Last Modified: Tue, 21 Nov 2023 06:21:14 GMT  
		Size: 573.6 KB (573635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d916370cd04b7352346fee3edc1ac77bdb9393e24c5bc62c4cb0803a682836`  
		Last Modified: Tue, 21 Nov 2023 06:21:14 GMT  
		Size: 295.1 KB (295096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e602d723a112bfbe3ebaca9b99e2e9636dac8b07c69947311ceb07666d40ed`  
		Last Modified: Tue, 21 Nov 2023 06:21:14 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbafbeffdc5d29b56e0ccf672e48ead551f49aa23534b4fd9aefcd339587dc5`  
		Last Modified: Tue, 21 Nov 2023 06:21:18 GMT  
		Size: 51.4 MB (51357976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f08f21ade417458e581ec8afdf835c5d165444c0e93fdc330cbd6146af1da3`  
		Last Modified: Tue, 21 Nov 2023 06:21:13 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a4bc9e282fe338ed74c99dbb5cb5777e0ba1a2d068de6e102a8adbb34acc14`  
		Last Modified: Tue, 21 Nov 2023 06:21:13 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c93f5a64665780dfb559adfed9587064e52e00c9c515834a97cf26e3529da9`  
		Last Modified: Tue, 21 Nov 2023 06:21:13 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f6f407505b71a14801c0c71da8d0ce2a85d8c65d58e7998784a75dcde3cfb6`  
		Last Modified: Tue, 21 Nov 2023 06:21:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:latest`

```console
$ docker pull couchdb@sha256:482d73fa450a18bce6ff591740b7a69f21a1cf94ffcd295a500e5214981e18d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:3c609bc33e472d4cb0a4ea0b117359bd0c9ed4f0628899131e8344fd13fbe01a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90245671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fff4b56666dbf396fc0b2eedb70c70b8990ccb6dc5d8447206f2243d21c1986c`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:46:40 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Nov 2023 01:46:41 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Nov 2023 01:46:47 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:46:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 01 Nov 2023 01:46:51 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Nov 2023 01:46:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:46:56 GMT
ENV COUCHDB_VERSION=3.3.2
# Wed, 01 Nov 2023 01:46:56 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Nov 2023 01:47:10 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Nov 2023 01:47:10 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Nov 2023 01:47:10 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 01 Nov 2023 01:47:11 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 01 Nov 2023 01:47:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Nov 2023 01:47:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 01:47:11 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Nov 2023 01:47:11 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Nov 2023 01:47:11 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbba1a29bfe2ee9664ccd0caa145b5aa7a5480c276f1c42fd77ac32ef2c440c1`  
		Last Modified: Wed, 01 Nov 2023 01:48:53 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b21d450d3bd9333c8a5efb4081f440607452820e295142168061b2216f3986c`  
		Last Modified: Wed, 01 Nov 2023 01:48:53 GMT  
		Size: 5.2 MB (5226554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c93767e1cbf8a0b2d24469dbe0f750b73d88204210f83f7faa87b8be37dfaa`  
		Last Modified: Wed, 01 Nov 2023 01:48:52 GMT  
		Size: 610.9 KB (610919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24dc783ed2d49dd34054350d1a680091886de94bd264352e835184065e394e64`  
		Last Modified: Wed, 01 Nov 2023 01:48:52 GMT  
		Size: 295.2 KB (295153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8597086eac85cffb9306a84cfa8414bcda5500cb8092b1ba307a38e9e56540f`  
		Last Modified: Wed, 01 Nov 2023 01:48:52 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4fefd748372d68972d6fb14014c7813ac7837a6380b957f3092da518331958`  
		Last Modified: Wed, 01 Nov 2023 01:48:55 GMT  
		Size: 52.7 MB (52687716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ff2441b3a4073bbf88542aaf2d970fd2eb11cc4bd01c846d1245dae6187068`  
		Last Modified: Wed, 01 Nov 2023 01:48:50 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c29c7241d3a11a9dcf62611e3563275d0b24d32fa9f65fb5be837b13ef1cfb4`  
		Last Modified: Wed, 01 Nov 2023 01:48:50 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacd4b2ce1758697d4898b78068d98430738b73f2f0171222ea8fc970a567603`  
		Last Modified: Wed, 01 Nov 2023 01:48:50 GMT  
		Size: 2.2 KB (2228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7254e813570e08d636b0b367fb2dfe8c25dfa8b3a07a24b4dcf9574a9e238270`  
		Last Modified: Wed, 01 Nov 2023 01:48:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:a4d2708520335bec287044683aa008f3ee0af0174c4844f4c27d73581ef39326
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88693209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a609af91aa2f1677f43a122b8a919068545adc446fc3857244fe5a8d89b703d5`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:53:44 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Nov 2023 02:53:44 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Nov 2023 02:53:50 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:53:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 01 Nov 2023 02:53:53 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Nov 2023 02:53:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:53:58 GMT
ENV COUCHDB_VERSION=3.3.2
# Wed, 01 Nov 2023 02:53:58 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Nov 2023 02:54:11 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Nov 2023 02:54:12 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Nov 2023 02:54:12 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 01 Nov 2023 02:54:12 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 01 Nov 2023 02:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Nov 2023 02:54:12 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Nov 2023 02:54:12 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Nov 2023 02:54:12 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Nov 2023 02:54:13 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b614568051476b61815cad57612a54fb357dce26265c2d8a93d3603e65f67bb`  
		Last Modified: Wed, 01 Nov 2023 02:55:30 GMT  
		Size: 3.4 KB (3431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c7e0362f1203d4c8eb75046c1009a66141067e9cb7a5e02ac76702b3a4fc5e`  
		Last Modified: Wed, 01 Nov 2023 02:55:29 GMT  
		Size: 5.2 MB (5210837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936a7f3d3f0f461eb2f034fa209eb834d4f53ab52e315c1ea90e4436d100cc12`  
		Last Modified: Wed, 01 Nov 2023 02:55:29 GMT  
		Size: 567.1 KB (567066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cea30aeda14f6e14599fb09aa79b3a41556b7509b7d4835f0d97a0e131aff2c`  
		Last Modified: Wed, 01 Nov 2023 02:55:29 GMT  
		Size: 295.0 KB (295032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a6600b43b5af044cab2a8316adbf77eed718e07be3a49b46d0d40f52bd9142`  
		Last Modified: Wed, 01 Nov 2023 02:55:28 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb3d645b10a8f7621c93c74d0ef540bf7eaa4110c0aeb1c226e7a3fde645671`  
		Last Modified: Wed, 01 Nov 2023 02:55:31 GMT  
		Size: 52.5 MB (52548927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0231949bd50a35a558a786ffd81b537869d8c2008032cf8f763cf817364efbc`  
		Last Modified: Wed, 01 Nov 2023 02:55:26 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce55a94b61b5a276dbee100f2f54d927ab8e493c9eef066a8604e6d29c611ab9`  
		Last Modified: Wed, 01 Nov 2023 02:55:26 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c997e552c1313a4b038f571f70da3ddf3a0b62fade23a017f7ba4dfbbeecc46`  
		Last Modified: Wed, 01 Nov 2023 02:55:26 GMT  
		Size: 2.2 KB (2230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15920850d8d556ea5c5d6b5a45df1b59867930cd37d1d15f1f712d12ee66edaf`  
		Last Modified: Wed, 01 Nov 2023 02:55:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; ppc64le

```console
$ docker pull couchdb@sha256:ccf9e925a92c4e47c922173bb8a6541607469de85a3d23b8f709a5b2f9fa4571
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.0 MB (95968231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0d5240fcc3525a7c996865649016d229a3b75d1447c7ade86132d7ede52ffe8`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:43 GMT
ADD file:b0d18f2d04821eb50d1faecc1a64916f5c63dd386ae71a3b2cb1d6c4aac6e1c4 in / 
# Tue, 21 Nov 2023 04:24:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:12:10 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Nov 2023 07:12:12 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Nov 2023 07:12:31 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:12:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 21 Nov 2023 07:12:37 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Nov 2023 07:12:47 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:12:47 GMT
ENV COUCHDB_VERSION=3.3.2
# Tue, 21 Nov 2023 07:12:49 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Nov 2023 07:13:13 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Nov 2023 07:13:17 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Nov 2023 07:13:17 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 21 Nov 2023 07:13:17 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 21 Nov 2023 07:13:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Nov 2023 07:13:20 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Nov 2023 07:13:20 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Nov 2023 07:13:20 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Nov 2023 07:13:21 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:60239a74847cd7e9a928353188f3cf096ca8cf648e2b27c765058e169d568fd9`  
		Last Modified: Tue, 21 Nov 2023 04:29:47 GMT  
		Size: 35.3 MB (35293727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f63eed5db2c906b6108908d9dc6976c9a23f1bb19a0e617257decd133e7592d`  
		Last Modified: Tue, 21 Nov 2023 07:14:05 GMT  
		Size: 3.4 KB (3408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941bb642de45bb343a873e9c819cd85bffe05a010a6da631d1723612f69c794c`  
		Last Modified: Tue, 21 Nov 2023 07:14:04 GMT  
		Size: 6.0 MB (6046203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f2659433b58c3235f1e9085447d55d5c442efc597e42f97dfce11b106d84c0`  
		Last Modified: Tue, 21 Nov 2023 07:14:04 GMT  
		Size: 662.9 KB (662883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d777a7fd59124bb1d1eed56bddee9639f6ea57c6eaf67610a97a4a8c833814e9`  
		Last Modified: Tue, 21 Nov 2023 07:14:03 GMT  
		Size: 295.1 KB (295091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef322b815f454b44be7fc5bbc3f2c179419841031a40a753c25cb71a704158f4`  
		Last Modified: Tue, 21 Nov 2023 07:14:03 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6180ccba02f37081c0d1523baa72b7df6183b2284a575cc84c8f245ed21624fc`  
		Last Modified: Tue, 21 Nov 2023 07:14:07 GMT  
		Size: 53.7 MB (53662909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991739364f41cbdef5c3adb115b1f41c51bbafbd6555e32316cad98f1cae7e54`  
		Last Modified: Tue, 21 Nov 2023 07:14:01 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f539c1a9af058023c294a0b078bb81ec732ba18d3e4c624af45c5e3a877c5dd`  
		Last Modified: Tue, 21 Nov 2023 07:14:01 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27abb88fb75707dd945625a5a2734aa790dcd4330e5d257d13fde86d69630c4`  
		Last Modified: Tue, 21 Nov 2023 07:14:01 GMT  
		Size: 2.2 KB (2232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7837c78696f2a9940c752105b06aeb98a48f8a6eacab80ba3a467f89fbe31ee5`  
		Last Modified: Tue, 21 Nov 2023 07:14:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; s390x

```console
$ docker pull couchdb@sha256:21965f0438b454449366375d4c6bfd319e83dec568e9907669ba2b6a1c077563
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.0 MB (87002806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba071f2f075a8263e2e67f1fc0f844debd3e57242ac3165ff9adcfacf2338049`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Nov 2023 05:05:18 GMT
ADD file:a545f27075704ce13e33e539170d3f47007424d2cc2bea5aecfd2608a5194151 in / 
# Tue, 21 Nov 2023 05:05:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:20:22 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Nov 2023 06:20:22 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Nov 2023 06:20:28 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:20:31 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 21 Nov 2023 06:20:31 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Nov 2023 06:20:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:20:36 GMT
ENV COUCHDB_VERSION=3.3.2
# Tue, 21 Nov 2023 06:20:36 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Nov 2023 06:20:53 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Nov 2023 06:20:55 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Nov 2023 06:20:55 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 21 Nov 2023 06:20:55 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 21 Nov 2023 06:20:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Nov 2023 06:20:56 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Nov 2023 06:20:56 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Nov 2023 06:20:56 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Nov 2023 06:20:56 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b114072f1cab66b7376d690985b12816aebab2e4e41fc170e32f111df27951dc`  
		Last Modified: Tue, 21 Nov 2023 05:10:48 GMT  
		Size: 29.7 MB (29656938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72dba253785a5e917fdd9064f61b676b4080ff3073424ff387308d70579c728b`  
		Last Modified: Tue, 21 Nov 2023 06:21:15 GMT  
		Size: 3.4 KB (3431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a299cd04ea14bbc3034e11001a1ec06dd4b5e1aaa78317dc803570f8a4c6437`  
		Last Modified: Tue, 21 Nov 2023 06:21:15 GMT  
		Size: 5.1 MB (5111719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c684e5bcbb93c8f0c9da5b81b4a1d19274f7ad0c7e3b17eb12cbe45cd2514989`  
		Last Modified: Tue, 21 Nov 2023 06:21:14 GMT  
		Size: 573.6 KB (573635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d916370cd04b7352346fee3edc1ac77bdb9393e24c5bc62c4cb0803a682836`  
		Last Modified: Tue, 21 Nov 2023 06:21:14 GMT  
		Size: 295.1 KB (295096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07e602d723a112bfbe3ebaca9b99e2e9636dac8b07c69947311ceb07666d40ed`  
		Last Modified: Tue, 21 Nov 2023 06:21:14 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbafbeffdc5d29b56e0ccf672e48ead551f49aa23534b4fd9aefcd339587dc5`  
		Last Modified: Tue, 21 Nov 2023 06:21:18 GMT  
		Size: 51.4 MB (51357976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f08f21ade417458e581ec8afdf835c5d165444c0e93fdc330cbd6146af1da3`  
		Last Modified: Tue, 21 Nov 2023 06:21:13 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a4bc9e282fe338ed74c99dbb5cb5777e0ba1a2d068de6e102a8adbb34acc14`  
		Last Modified: Tue, 21 Nov 2023 06:21:13 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c93f5a64665780dfb559adfed9587064e52e00c9c515834a97cf26e3529da9`  
		Last Modified: Tue, 21 Nov 2023 06:21:13 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f6f407505b71a14801c0c71da8d0ce2a85d8c65d58e7998784a75dcde3cfb6`  
		Last Modified: Tue, 21 Nov 2023 06:21:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
