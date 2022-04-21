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
$ docker pull couchdb@sha256:3c83c1aa4eb6548948f1af9098feba08a3b4cf792880b3748b5a519d9ed6aed6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2` - linux; amd64

```console
$ docker pull couchdb@sha256:c9959132c680bfc45b160e168d8af0773e70dcdc164202f128d6db3ddabf1107
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84524914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9efd7cbb09732e24bd26b3a1869601e84aafa300304e8b692ef909b15a6e559`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:11:10 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 20 Apr 2022 07:11:10 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 20 Apr 2022 07:11:17 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:11:21 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 20 Apr 2022 07:11:21 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 20 Apr 2022 07:11:28 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:11:50 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 20 Apr 2022 07:11:50 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 20 Apr 2022 07:12:07 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 20 Apr 2022 07:12:08 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 20 Apr 2022 07:12:08 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 20 Apr 2022 07:12:08 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 20 Apr 2022 07:12:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 20 Apr 2022 07:12:09 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 20 Apr 2022 07:12:09 GMT
VOLUME [/opt/couchdb/data]
# Wed, 20 Apr 2022 07:12:09 GMT
EXPOSE 4369 5984 9100
# Wed, 20 Apr 2022 07:12:09 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cda2a4a9a9c0972a269e783092de1ff725f53eb1d78a8fb9e9fc7edd249003e`  
		Last Modified: Wed, 20 Apr 2022 07:12:52 GMT  
		Size: 3.4 KB (3408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35595421e132bd4b6bbcb5ce7de4cab1b3e6166ff0310ec3a445baf267b0ee49`  
		Last Modified: Wed, 20 Apr 2022 07:12:51 GMT  
		Size: 6.7 MB (6698605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e21c134e694eaf537fbfa0a926df693f490ddccc20da9b4d1e1b72c3fa4415d`  
		Last Modified: Wed, 20 Apr 2022 07:12:50 GMT  
		Size: 1.3 MB (1258366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613f17690642b0eb670154685591206b152fc004ce6c451fef9a943551fadcd3`  
		Last Modified: Wed, 20 Apr 2022 07:12:50 GMT  
		Size: 293.0 KB (292999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a2e12c8171ada18637a2283a72671a543337a37bbcf331b52278c4409757ec`  
		Last Modified: Wed, 20 Apr 2022 07:13:06 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a639ecaab8e86d7b523cf05522c1368c600adcc2062aad176ca5b33ab77a3300`  
		Last Modified: Wed, 20 Apr 2022 07:13:10 GMT  
		Size: 49.1 MB (49127269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74051b123e4939a6f3bc7c39cbd5375d52d623529e0f08613660a9f9cb0e49c`  
		Last Modified: Wed, 20 Apr 2022 07:13:03 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ce5af6c9b47c385cfac931450b252cb048e43cc36ea2ca931fffb8c0f32cf9`  
		Last Modified: Wed, 20 Apr 2022 07:13:03 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33cdb258daba32d5410b3bf8f776d939f04a73695db1e82e1c991cee7639cb6e`  
		Last Modified: Wed, 20 Apr 2022 07:13:04 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292ed1f8c554bf529de54064d74415a35f7086568a5d6d8c6018782bfcd126e4`  
		Last Modified: Wed, 20 Apr 2022 07:13:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:92e5b524b1215273cec9b7d952e01e5f3f1f1c2734a01d7394333ac6c5c8f31e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72526018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e35c2d9fe0697fc396bd4fd20cc54ff94766f709742995d1059b0232d413bc0a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:36 GMT
ADD file:5de4397c1295f7249c93907be599d96efbd9cd25909340d245ec8d1c9770f444 in / 
# Wed, 20 Apr 2022 04:29:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:03:39 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 20 Apr 2022 07:03:40 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 20 Apr 2022 07:03:48 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:03:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 20 Apr 2022 07:03:53 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 20 Apr 2022 07:04:00 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:04:41 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 20 Apr 2022 07:04:41 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 20 Apr 2022 07:04:59 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 20 Apr 2022 07:05:00 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 20 Apr 2022 07:05:01 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 20 Apr 2022 07:05:02 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 20 Apr 2022 07:05:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 20 Apr 2022 07:05:03 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 20 Apr 2022 07:05:04 GMT
VOLUME [/opt/couchdb/data]
# Wed, 20 Apr 2022 07:05:05 GMT
EXPOSE 4369 5984 9100
# Wed, 20 Apr 2022 07:05:06 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6c3e5b218d6477ff77053280968d5bdeaa5dcf16a803e917d98dd0ea8b93ac82`  
		Last Modified: Wed, 20 Apr 2022 04:36:38 GMT  
		Size: 25.9 MB (25908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15dfa2d73c72258f50f849a1f31a09fb838258553d12e341020e966370d0b858`  
		Last Modified: Wed, 20 Apr 2022 07:06:01 GMT  
		Size: 3.3 KB (3316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcdad7b881f9dd0b2907bb1dc0f751b78915b2de7b6ddc44cd02157372005dfd`  
		Last Modified: Wed, 20 Apr 2022 07:06:01 GMT  
		Size: 6.6 MB (6556359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2262e1b6750144c60a72a0ef3a2a8f8b12096df0ed32f784a1fd0b002e95bba1`  
		Last Modified: Wed, 20 Apr 2022 07:05:59 GMT  
		Size: 951.1 KB (951150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7d0666a4c86366363b1a4fcb9e452af0faa020dc867402e9b609b49fde965e`  
		Last Modified: Wed, 20 Apr 2022 07:05:59 GMT  
		Size: 79.9 KB (79922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe46b4b25438b885ee9c1fec6a6050ec924f6bc5952ebf6d7059afdc0008af78`  
		Last Modified: Wed, 20 Apr 2022 07:06:21 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3917d45454bb9c84ab2b897b3490ecac6432b87fa0464823f05a23b84dcf1ead`  
		Last Modified: Wed, 20 Apr 2022 07:06:23 GMT  
		Size: 39.0 MB (39023324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a7136770d795096863da4852e9df05db997c93b6ae2e0fe29bc6f6fe60e74a3`  
		Last Modified: Wed, 20 Apr 2022 07:06:19 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237c1405fed0ce55bcb0715c109ef8e4709dea268796aed7c16edb9fe091f7bf`  
		Last Modified: Wed, 20 Apr 2022 07:06:19 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5a4d4209b43365059e75cd2681333a4824abc4c903b8732b5401728b03c59a`  
		Last Modified: Wed, 20 Apr 2022 07:06:18 GMT  
		Size: 2.1 KB (2055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690005ade0aceb8251d459dcd83208087d6d57d7c11d4fee40f4d290fe3d7776`  
		Last Modified: Wed, 20 Apr 2022 07:06:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3`

```console
$ docker pull couchdb@sha256:3c83c1aa4eb6548948f1af9098feba08a3b4cf792880b3748b5a519d9ed6aed6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:c9959132c680bfc45b160e168d8af0773e70dcdc164202f128d6db3ddabf1107
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84524914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9efd7cbb09732e24bd26b3a1869601e84aafa300304e8b692ef909b15a6e559`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:11:10 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 20 Apr 2022 07:11:10 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 20 Apr 2022 07:11:17 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:11:21 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 20 Apr 2022 07:11:21 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 20 Apr 2022 07:11:28 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:11:50 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 20 Apr 2022 07:11:50 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 20 Apr 2022 07:12:07 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 20 Apr 2022 07:12:08 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 20 Apr 2022 07:12:08 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 20 Apr 2022 07:12:08 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 20 Apr 2022 07:12:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 20 Apr 2022 07:12:09 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 20 Apr 2022 07:12:09 GMT
VOLUME [/opt/couchdb/data]
# Wed, 20 Apr 2022 07:12:09 GMT
EXPOSE 4369 5984 9100
# Wed, 20 Apr 2022 07:12:09 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cda2a4a9a9c0972a269e783092de1ff725f53eb1d78a8fb9e9fc7edd249003e`  
		Last Modified: Wed, 20 Apr 2022 07:12:52 GMT  
		Size: 3.4 KB (3408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35595421e132bd4b6bbcb5ce7de4cab1b3e6166ff0310ec3a445baf267b0ee49`  
		Last Modified: Wed, 20 Apr 2022 07:12:51 GMT  
		Size: 6.7 MB (6698605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e21c134e694eaf537fbfa0a926df693f490ddccc20da9b4d1e1b72c3fa4415d`  
		Last Modified: Wed, 20 Apr 2022 07:12:50 GMT  
		Size: 1.3 MB (1258366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613f17690642b0eb670154685591206b152fc004ce6c451fef9a943551fadcd3`  
		Last Modified: Wed, 20 Apr 2022 07:12:50 GMT  
		Size: 293.0 KB (292999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a2e12c8171ada18637a2283a72671a543337a37bbcf331b52278c4409757ec`  
		Last Modified: Wed, 20 Apr 2022 07:13:06 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a639ecaab8e86d7b523cf05522c1368c600adcc2062aad176ca5b33ab77a3300`  
		Last Modified: Wed, 20 Apr 2022 07:13:10 GMT  
		Size: 49.1 MB (49127269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74051b123e4939a6f3bc7c39cbd5375d52d623529e0f08613660a9f9cb0e49c`  
		Last Modified: Wed, 20 Apr 2022 07:13:03 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ce5af6c9b47c385cfac931450b252cb048e43cc36ea2ca931fffb8c0f32cf9`  
		Last Modified: Wed, 20 Apr 2022 07:13:03 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33cdb258daba32d5410b3bf8f776d939f04a73695db1e82e1c991cee7639cb6e`  
		Last Modified: Wed, 20 Apr 2022 07:13:04 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292ed1f8c554bf529de54064d74415a35f7086568a5d6d8c6018782bfcd126e4`  
		Last Modified: Wed, 20 Apr 2022 07:13:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:92e5b524b1215273cec9b7d952e01e5f3f1f1c2734a01d7394333ac6c5c8f31e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72526018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e35c2d9fe0697fc396bd4fd20cc54ff94766f709742995d1059b0232d413bc0a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:36 GMT
ADD file:5de4397c1295f7249c93907be599d96efbd9cd25909340d245ec8d1c9770f444 in / 
# Wed, 20 Apr 2022 04:29:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:03:39 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 20 Apr 2022 07:03:40 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 20 Apr 2022 07:03:48 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:03:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 20 Apr 2022 07:03:53 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 20 Apr 2022 07:04:00 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:04:41 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 20 Apr 2022 07:04:41 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 20 Apr 2022 07:04:59 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 20 Apr 2022 07:05:00 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 20 Apr 2022 07:05:01 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 20 Apr 2022 07:05:02 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 20 Apr 2022 07:05:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 20 Apr 2022 07:05:03 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 20 Apr 2022 07:05:04 GMT
VOLUME [/opt/couchdb/data]
# Wed, 20 Apr 2022 07:05:05 GMT
EXPOSE 4369 5984 9100
# Wed, 20 Apr 2022 07:05:06 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6c3e5b218d6477ff77053280968d5bdeaa5dcf16a803e917d98dd0ea8b93ac82`  
		Last Modified: Wed, 20 Apr 2022 04:36:38 GMT  
		Size: 25.9 MB (25908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15dfa2d73c72258f50f849a1f31a09fb838258553d12e341020e966370d0b858`  
		Last Modified: Wed, 20 Apr 2022 07:06:01 GMT  
		Size: 3.3 KB (3316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcdad7b881f9dd0b2907bb1dc0f751b78915b2de7b6ddc44cd02157372005dfd`  
		Last Modified: Wed, 20 Apr 2022 07:06:01 GMT  
		Size: 6.6 MB (6556359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2262e1b6750144c60a72a0ef3a2a8f8b12096df0ed32f784a1fd0b002e95bba1`  
		Last Modified: Wed, 20 Apr 2022 07:05:59 GMT  
		Size: 951.1 KB (951150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7d0666a4c86366363b1a4fcb9e452af0faa020dc867402e9b609b49fde965e`  
		Last Modified: Wed, 20 Apr 2022 07:05:59 GMT  
		Size: 79.9 KB (79922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe46b4b25438b885ee9c1fec6a6050ec924f6bc5952ebf6d7059afdc0008af78`  
		Last Modified: Wed, 20 Apr 2022 07:06:21 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3917d45454bb9c84ab2b897b3490ecac6432b87fa0464823f05a23b84dcf1ead`  
		Last Modified: Wed, 20 Apr 2022 07:06:23 GMT  
		Size: 39.0 MB (39023324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a7136770d795096863da4852e9df05db997c93b6ae2e0fe29bc6f6fe60e74a3`  
		Last Modified: Wed, 20 Apr 2022 07:06:19 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237c1405fed0ce55bcb0715c109ef8e4709dea268796aed7c16edb9fe091f7bf`  
		Last Modified: Wed, 20 Apr 2022 07:06:19 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5a4d4209b43365059e75cd2681333a4824abc4c903b8732b5401728b03c59a`  
		Last Modified: Wed, 20 Apr 2022 07:06:18 GMT  
		Size: 2.1 KB (2055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690005ade0aceb8251d459dcd83208087d6d57d7c11d4fee40f4d290fe3d7776`  
		Last Modified: Wed, 20 Apr 2022 07:06:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3.1`

```console
$ docker pull couchdb@sha256:3c83c1aa4eb6548948f1af9098feba08a3b4cf792880b3748b5a519d9ed6aed6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:c9959132c680bfc45b160e168d8af0773e70dcdc164202f128d6db3ddabf1107
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84524914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9efd7cbb09732e24bd26b3a1869601e84aafa300304e8b692ef909b15a6e559`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:11:10 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 20 Apr 2022 07:11:10 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 20 Apr 2022 07:11:17 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:11:21 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 20 Apr 2022 07:11:21 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 20 Apr 2022 07:11:28 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:11:50 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 20 Apr 2022 07:11:50 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 20 Apr 2022 07:12:07 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 20 Apr 2022 07:12:08 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 20 Apr 2022 07:12:08 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 20 Apr 2022 07:12:08 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 20 Apr 2022 07:12:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 20 Apr 2022 07:12:09 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 20 Apr 2022 07:12:09 GMT
VOLUME [/opt/couchdb/data]
# Wed, 20 Apr 2022 07:12:09 GMT
EXPOSE 4369 5984 9100
# Wed, 20 Apr 2022 07:12:09 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cda2a4a9a9c0972a269e783092de1ff725f53eb1d78a8fb9e9fc7edd249003e`  
		Last Modified: Wed, 20 Apr 2022 07:12:52 GMT  
		Size: 3.4 KB (3408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35595421e132bd4b6bbcb5ce7de4cab1b3e6166ff0310ec3a445baf267b0ee49`  
		Last Modified: Wed, 20 Apr 2022 07:12:51 GMT  
		Size: 6.7 MB (6698605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e21c134e694eaf537fbfa0a926df693f490ddccc20da9b4d1e1b72c3fa4415d`  
		Last Modified: Wed, 20 Apr 2022 07:12:50 GMT  
		Size: 1.3 MB (1258366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613f17690642b0eb670154685591206b152fc004ce6c451fef9a943551fadcd3`  
		Last Modified: Wed, 20 Apr 2022 07:12:50 GMT  
		Size: 293.0 KB (292999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a2e12c8171ada18637a2283a72671a543337a37bbcf331b52278c4409757ec`  
		Last Modified: Wed, 20 Apr 2022 07:13:06 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a639ecaab8e86d7b523cf05522c1368c600adcc2062aad176ca5b33ab77a3300`  
		Last Modified: Wed, 20 Apr 2022 07:13:10 GMT  
		Size: 49.1 MB (49127269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74051b123e4939a6f3bc7c39cbd5375d52d623529e0f08613660a9f9cb0e49c`  
		Last Modified: Wed, 20 Apr 2022 07:13:03 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ce5af6c9b47c385cfac931450b252cb048e43cc36ea2ca931fffb8c0f32cf9`  
		Last Modified: Wed, 20 Apr 2022 07:13:03 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33cdb258daba32d5410b3bf8f776d939f04a73695db1e82e1c991cee7639cb6e`  
		Last Modified: Wed, 20 Apr 2022 07:13:04 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292ed1f8c554bf529de54064d74415a35f7086568a5d6d8c6018782bfcd126e4`  
		Last Modified: Wed, 20 Apr 2022 07:13:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:92e5b524b1215273cec9b7d952e01e5f3f1f1c2734a01d7394333ac6c5c8f31e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72526018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e35c2d9fe0697fc396bd4fd20cc54ff94766f709742995d1059b0232d413bc0a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:36 GMT
ADD file:5de4397c1295f7249c93907be599d96efbd9cd25909340d245ec8d1c9770f444 in / 
# Wed, 20 Apr 2022 04:29:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:03:39 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 20 Apr 2022 07:03:40 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 20 Apr 2022 07:03:48 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:03:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 20 Apr 2022 07:03:53 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 20 Apr 2022 07:04:00 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:04:41 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 20 Apr 2022 07:04:41 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 20 Apr 2022 07:04:59 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 20 Apr 2022 07:05:00 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 20 Apr 2022 07:05:01 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 20 Apr 2022 07:05:02 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 20 Apr 2022 07:05:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 20 Apr 2022 07:05:03 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 20 Apr 2022 07:05:04 GMT
VOLUME [/opt/couchdb/data]
# Wed, 20 Apr 2022 07:05:05 GMT
EXPOSE 4369 5984 9100
# Wed, 20 Apr 2022 07:05:06 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6c3e5b218d6477ff77053280968d5bdeaa5dcf16a803e917d98dd0ea8b93ac82`  
		Last Modified: Wed, 20 Apr 2022 04:36:38 GMT  
		Size: 25.9 MB (25908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15dfa2d73c72258f50f849a1f31a09fb838258553d12e341020e966370d0b858`  
		Last Modified: Wed, 20 Apr 2022 07:06:01 GMT  
		Size: 3.3 KB (3316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcdad7b881f9dd0b2907bb1dc0f751b78915b2de7b6ddc44cd02157372005dfd`  
		Last Modified: Wed, 20 Apr 2022 07:06:01 GMT  
		Size: 6.6 MB (6556359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2262e1b6750144c60a72a0ef3a2a8f8b12096df0ed32f784a1fd0b002e95bba1`  
		Last Modified: Wed, 20 Apr 2022 07:05:59 GMT  
		Size: 951.1 KB (951150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7d0666a4c86366363b1a4fcb9e452af0faa020dc867402e9b609b49fde965e`  
		Last Modified: Wed, 20 Apr 2022 07:05:59 GMT  
		Size: 79.9 KB (79922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe46b4b25438b885ee9c1fec6a6050ec924f6bc5952ebf6d7059afdc0008af78`  
		Last Modified: Wed, 20 Apr 2022 07:06:21 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3917d45454bb9c84ab2b897b3490ecac6432b87fa0464823f05a23b84dcf1ead`  
		Last Modified: Wed, 20 Apr 2022 07:06:23 GMT  
		Size: 39.0 MB (39023324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a7136770d795096863da4852e9df05db997c93b6ae2e0fe29bc6f6fe60e74a3`  
		Last Modified: Wed, 20 Apr 2022 07:06:19 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237c1405fed0ce55bcb0715c109ef8e4709dea268796aed7c16edb9fe091f7bf`  
		Last Modified: Wed, 20 Apr 2022 07:06:19 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5a4d4209b43365059e75cd2681333a4824abc4c903b8732b5401728b03c59a`  
		Last Modified: Wed, 20 Apr 2022 07:06:18 GMT  
		Size: 2.1 KB (2055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690005ade0aceb8251d459dcd83208087d6d57d7c11d4fee40f4d290fe3d7776`  
		Last Modified: Wed, 20 Apr 2022 07:06:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3`

```console
$ docker pull couchdb@sha256:37a7a9aab050c8c376b012d9c52da58e2c94d221b0eb5567edb88d8ceca096ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3` - linux; amd64

```console
$ docker pull couchdb@sha256:2c96232290fe0414177909bdb8c30224af32c2f8f7031d868fb832ffaac6cc4f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87451684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b53c5467cf3ac9c9d94c8922a210bc132fa625e0059a48054a22a992881b1a8f`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:10:30 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 20 Apr 2022 07:10:30 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 20 Apr 2022 07:10:37 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:10:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 20 Apr 2022 07:10:41 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 20 Apr 2022 07:10:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:10:47 GMT
ENV COUCHDB_VERSION=3.2.1-1
# Wed, 20 Apr 2022 07:10:47 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 20 Apr 2022 07:11:00 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 20 Apr 2022 07:11:00 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 20 Apr 2022 07:11:01 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 20 Apr 2022 07:11:01 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 20 Apr 2022 07:11:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 20 Apr 2022 07:11:01 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 20 Apr 2022 07:11:01 GMT
VOLUME [/opt/couchdb/data]
# Wed, 20 Apr 2022 07:11:02 GMT
EXPOSE 4369 5984 9100
# Wed, 20 Apr 2022 07:11:02 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e4fb628d536f433a0a908e8e65812c407b41d7039fa72adc77277f091a8924`  
		Last Modified: Wed, 20 Apr 2022 07:12:30 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5ada74819f3e5a933ad7776886fd3b202f99653d68b746f8e1ca6bf158db5a`  
		Last Modified: Wed, 20 Apr 2022 07:12:29 GMT  
		Size: 5.2 MB (5223690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7d8f1aed9465ca9c4007a6277de02a53c60b7f77c8a0a6dca2a0fe064afa93`  
		Last Modified: Wed, 20 Apr 2022 07:12:29 GMT  
		Size: 1.6 MB (1553283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464d6b8b4bbbc83281231e89eac3d0d5d2142d261de2db10cc7f65167b545c77`  
		Last Modified: Wed, 20 Apr 2022 07:12:28 GMT  
		Size: 295.6 KB (295569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b71906ef4252c8d9093a53eaeae741462aed454881113137d2c5539a5b39cca`  
		Last Modified: Wed, 20 Apr 2022 07:12:28 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43f2ebb365be093fc6c10de52167a7915582ca0d80a1594fe31f74d652ec583`  
		Last Modified: Wed, 20 Apr 2022 07:12:32 GMT  
		Size: 49.0 MB (48993027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09b9610f19e31700a17b805c579fed67585d29389cd706ac975e38fe16967c3`  
		Last Modified: Wed, 20 Apr 2022 07:12:26 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad96a982041d41e0a94650bcac88201e50a18622c16b84db337c84799cbaadf2`  
		Last Modified: Wed, 20 Apr 2022 07:12:26 GMT  
		Size: 768.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9590c0cb12e900d1d82e53daf2bb099c6230b830cc3f3b72fd4455e2ff598306`  
		Last Modified: Wed, 20 Apr 2022 07:12:26 GMT  
		Size: 2.2 KB (2179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a01aac1048bee36c25c3b24ae92a24faf3c8418d592dbd209938398b439036`  
		Last Modified: Wed, 20 Apr 2022 07:12:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:b1ce2bd46ec5ea9656d89ee31fb5ddb80f5bbb18c24b38536eab91423bd75654
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.4 MB (85383029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72dd9a06ea5af54ebc9afe1b239f350e954ae38e39e75097dcbfba5ce977eb21`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:02:48 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 20 Apr 2022 07:02:48 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 20 Apr 2022 07:02:55 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:02:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 20 Apr 2022 07:03:00 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 20 Apr 2022 07:03:06 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:03:07 GMT
ENV COUCHDB_VERSION=3.2.1-1
# Wed, 20 Apr 2022 07:03:08 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 20 Apr 2022 07:03:26 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 20 Apr 2022 07:03:27 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 20 Apr 2022 07:03:28 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 20 Apr 2022 07:03:29 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 20 Apr 2022 07:03:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 20 Apr 2022 07:03:30 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 20 Apr 2022 07:03:31 GMT
VOLUME [/opt/couchdb/data]
# Wed, 20 Apr 2022 07:03:32 GMT
EXPOSE 4369 5984 9100
# Wed, 20 Apr 2022 07:03:33 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51cefb89564694ca915e167c405ee5881088311379fb87639609d213f6bb420`  
		Last Modified: Wed, 20 Apr 2022 07:05:36 GMT  
		Size: 3.3 KB (3319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ec39efab772ade8e91f1021e60940ff0365826df140afe1f51e150ceb0303b`  
		Last Modified: Wed, 20 Apr 2022 07:05:35 GMT  
		Size: 5.0 MB (5002920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b4d5c3bee5b8e99b3e70d3a88123a53caf0860986a9eb6e68d6c4ed7022533`  
		Last Modified: Wed, 20 Apr 2022 07:05:34 GMT  
		Size: 1.2 MB (1221077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6fb8160cb2a1f0d19dd386151a86a62c1e568354e1aac1a650c0d9fde62de7`  
		Last Modified: Wed, 20 Apr 2022 07:05:34 GMT  
		Size: 79.2 KB (79168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b99c7181f5a3992355deabe6e521d071029050e68f777a730b24dba5cf3a949`  
		Last Modified: Wed, 20 Apr 2022 07:05:34 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd1b9b51ff525d46c102aafe33ec2631c99218677d1fb9505db73af88f22380`  
		Last Modified: Wed, 20 Apr 2022 07:05:37 GMT  
		Size: 49.0 MB (49007026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf44f240a74efe39263490f22dbad69cb71869ee20eeeca196dc544cadaa1e26`  
		Last Modified: Wed, 20 Apr 2022 07:05:31 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dfe021f0efc89117bdd8aaf84ff80a530d7366daf172e2ce3aabb5b7d4c9ea7`  
		Last Modified: Wed, 20 Apr 2022 07:05:32 GMT  
		Size: 761.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03dfc4e590017fbe73692daf143f06beda0a5c608db21e54a1f335fe8a112c4`  
		Last Modified: Wed, 20 Apr 2022 07:05:31 GMT  
		Size: 2.2 KB (2182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726df3f6f358317ff48ad598cd6294cc97db9360f05674ad2b3251d7ec7c9cd4`  
		Last Modified: Wed, 20 Apr 2022 07:05:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; ppc64le

```console
$ docker pull couchdb@sha256:1c4f2cdf4fd85d3542f9d953a52e34ec350bdd9bdef6bc2319852c03a79ea3ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93170578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:687faa76badbcab293da87344a0728961f84a6dcc64c64b38adbc1e0e6962a71`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 20 Apr 2022 09:46:36 GMT
ADD file:8d406ebce4d9b0884d46ee25ec31fe7714726024b80aba9b408d81d39e2f6f8c in / 
# Wed, 20 Apr 2022 09:46:44 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 17:38:52 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 20 Apr 2022 17:39:03 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 20 Apr 2022 17:40:27 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 17:40:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 20 Apr 2022 17:40:45 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 20 Apr 2022 17:41:21 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 17:41:24 GMT
ENV COUCHDB_VERSION=3.2.1-1
# Wed, 20 Apr 2022 17:41:31 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 20 Apr 2022 17:42:11 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 20 Apr 2022 17:42:13 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 20 Apr 2022 17:42:14 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 20 Apr 2022 17:42:16 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 20 Apr 2022 17:42:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 20 Apr 2022 17:42:24 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 20 Apr 2022 17:42:26 GMT
VOLUME [/opt/couchdb/data]
# Wed, 20 Apr 2022 17:42:30 GMT
EXPOSE 4369 5984 9100
# Wed, 20 Apr 2022 17:42:32 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:5e0d035960b14409a1ddb839de80aa08677b71addd5e94264ff9ee89a2523e5b`  
		Last Modified: Wed, 20 Apr 2022 09:56:59 GMT  
		Size: 35.3 MB (35285249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188a5996a68176f11650fa0166342f84d30a315d76d4a70562defe4528ede8d2`  
		Last Modified: Wed, 20 Apr 2022 17:43:03 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c752a79eaca840a137608a3021b6cc666055ffb706a73ff54f5353c6ffd933`  
		Last Modified: Wed, 20 Apr 2022 17:43:01 GMT  
		Size: 6.0 MB (6043780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d488f2af80a56c0f11ddcdeaa3941cb822ae2cdc4bed7b5cee88f1cf382f6db0`  
		Last Modified: Wed, 20 Apr 2022 17:43:00 GMT  
		Size: 1.5 MB (1509335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b958f31aae831160c8329bdb19bcb57c1dbd219b156fdfce20bfe5c1e3bc72`  
		Last Modified: Wed, 20 Apr 2022 17:43:01 GMT  
		Size: 295.7 KB (295733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b45400e02e64efbce766c8a10cd174ed7902d081ca92b816d94a4e03375a95`  
		Last Modified: Wed, 20 Apr 2022 17:43:00 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1150f12eed05ab2096de0b9a91767e07ba799e2e58c52e9d0462f240ca1dc641`  
		Last Modified: Wed, 20 Apr 2022 17:43:05 GMT  
		Size: 50.0 MB (50029335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3ebde4b104f87037282a2dd623138620548ef9f0c7ec84acd4a357b16199c0`  
		Last Modified: Wed, 20 Apr 2022 17:42:57 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e3f2b1940560793ab014bc68027fdec22ac5bdd5ca38444da6df377e9df987`  
		Last Modified: Wed, 20 Apr 2022 17:42:57 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea19cadf45f2297795ff6894e7d3df3a91e166e71704d2c3eae94c4afbf9d0f9`  
		Last Modified: Wed, 20 Apr 2022 17:42:57 GMT  
		Size: 2.2 KB (2188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d70e2634cff623886f8a678fab41a5d4158a1bd6d6f4dcdc7ae82b4d0d3607`  
		Last Modified: Wed, 20 Apr 2022 17:42:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1`

```console
$ docker pull couchdb@sha256:a18e2e79817527719dc9af1f8c2cc67bab63e9a83dca164c3ac1d9b6c6157af6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:1327b4719a309eecd4737ce51506b867ad47d7040353c36d178b031f95c0a07e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80009876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a073ccc4150877efa603e9c3b799f7f2552153bf4f1c55f4d9e84c6a4b3cb7b3`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:11:10 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 20 Apr 2022 07:11:10 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 20 Apr 2022 07:11:17 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:11:21 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 20 Apr 2022 07:11:21 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 20 Apr 2022 07:11:28 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:11:28 GMT
ENV COUCHDB_VERSION=3.1.2
# Wed, 20 Apr 2022 07:11:28 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 20 Apr 2022 07:11:42 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 20 Apr 2022 07:11:42 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 20 Apr 2022 07:11:42 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 20 Apr 2022 07:11:42 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 20 Apr 2022 07:11:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 20 Apr 2022 07:11:43 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 20 Apr 2022 07:11:43 GMT
VOLUME [/opt/couchdb/data]
# Wed, 20 Apr 2022 07:11:43 GMT
EXPOSE 4369 5984 9100
# Wed, 20 Apr 2022 07:11:43 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cda2a4a9a9c0972a269e783092de1ff725f53eb1d78a8fb9e9fc7edd249003e`  
		Last Modified: Wed, 20 Apr 2022 07:12:52 GMT  
		Size: 3.4 KB (3408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35595421e132bd4b6bbcb5ce7de4cab1b3e6166ff0310ec3a445baf267b0ee49`  
		Last Modified: Wed, 20 Apr 2022 07:12:51 GMT  
		Size: 6.7 MB (6698605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e21c134e694eaf537fbfa0a926df693f490ddccc20da9b4d1e1b72c3fa4415d`  
		Last Modified: Wed, 20 Apr 2022 07:12:50 GMT  
		Size: 1.3 MB (1258366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613f17690642b0eb670154685591206b152fc004ce6c451fef9a943551fadcd3`  
		Last Modified: Wed, 20 Apr 2022 07:12:50 GMT  
		Size: 293.0 KB (292999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98f535ebc016d2e50cc212c899468dc5a16d41f10eab7fc5c6331a52888efa1d`  
		Last Modified: Wed, 20 Apr 2022 07:12:50 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ea72ee2cf4cb7497a97d20f65dea99c1708962f8eac376f9baa83e481f9abd`  
		Last Modified: Wed, 20 Apr 2022 07:12:53 GMT  
		Size: 44.6 MB (44612241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2751f3407a76c10f2f624f6496291f2cbb4bb1f8302d3dcce5931898ba7617`  
		Last Modified: Wed, 20 Apr 2022 07:12:48 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9905b54ec2a6b543273ff2135dd12a449ebd9101e7ec86c92e324b5c741bf189`  
		Last Modified: Wed, 20 Apr 2022 07:12:47 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20349b7cce82d73993ad9221569b8665490627b6979b590a1370da1eb32c61fc`  
		Last Modified: Wed, 20 Apr 2022 07:12:47 GMT  
		Size: 2.1 KB (2056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6789f6e6be0cc122e54512c9653ba927835e3d93ba4a43217da085ca293b670c`  
		Last Modified: Wed, 20 Apr 2022 07:12:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:f3908b181a74e95c54b42988e7852a301cdc432e96b9d743516fe11cb68c74b9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74615234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c756e28808c4459a6411688662f0a1da3ab8fda054ee87e9ebfde5f2b155ab5f`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:36 GMT
ADD file:5de4397c1295f7249c93907be599d96efbd9cd25909340d245ec8d1c9770f444 in / 
# Wed, 20 Apr 2022 04:29:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:03:39 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 20 Apr 2022 07:03:40 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 20 Apr 2022 07:03:48 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:03:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 20 Apr 2022 07:03:53 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 20 Apr 2022 07:04:00 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:04:00 GMT
ENV COUCHDB_VERSION=3.1.2
# Wed, 20 Apr 2022 07:04:01 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 20 Apr 2022 07:04:19 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 20 Apr 2022 07:04:21 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 20 Apr 2022 07:04:22 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 20 Apr 2022 07:04:23 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 20 Apr 2022 07:04:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 20 Apr 2022 07:04:24 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 20 Apr 2022 07:04:25 GMT
VOLUME [/opt/couchdb/data]
# Wed, 20 Apr 2022 07:04:26 GMT
EXPOSE 4369 5984 9100
# Wed, 20 Apr 2022 07:04:27 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6c3e5b218d6477ff77053280968d5bdeaa5dcf16a803e917d98dd0ea8b93ac82`  
		Last Modified: Wed, 20 Apr 2022 04:36:38 GMT  
		Size: 25.9 MB (25908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15dfa2d73c72258f50f849a1f31a09fb838258553d12e341020e966370d0b858`  
		Last Modified: Wed, 20 Apr 2022 07:06:01 GMT  
		Size: 3.3 KB (3316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcdad7b881f9dd0b2907bb1dc0f751b78915b2de7b6ddc44cd02157372005dfd`  
		Last Modified: Wed, 20 Apr 2022 07:06:01 GMT  
		Size: 6.6 MB (6556359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2262e1b6750144c60a72a0ef3a2a8f8b12096df0ed32f784a1fd0b002e95bba1`  
		Last Modified: Wed, 20 Apr 2022 07:05:59 GMT  
		Size: 951.1 KB (951150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7d0666a4c86366363b1a4fcb9e452af0faa020dc867402e9b609b49fde965e`  
		Last Modified: Wed, 20 Apr 2022 07:05:59 GMT  
		Size: 79.9 KB (79922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fe5c7236bf910b320f7095182b16d6250cb5028bb933ba74ce601554777673`  
		Last Modified: Wed, 20 Apr 2022 07:05:59 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb8867ec1107935115c1fb1eeca46dfb3b4d7b127cd3f24c7dfb5251e04a5af`  
		Last Modified: Wed, 20 Apr 2022 07:06:02 GMT  
		Size: 41.1 MB (41112540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953af7dec7b828efe5a6f93229ee11516acfd3061230552867a0734fa4478917`  
		Last Modified: Wed, 20 Apr 2022 07:05:57 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0e21c4295b22ca6079f7a475ab03bcdd7e979ed2ce3900be892a08151702c5`  
		Last Modified: Wed, 20 Apr 2022 07:05:57 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1347aa0b12961ab0309af180e4a4691dddec581f87aa3e147627925baa5bc161`  
		Last Modified: Wed, 20 Apr 2022 07:05:57 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3d40c189a512811b2a9ed3a1412449155bb1ae67f2865d5e325ba0fda20b44`  
		Last Modified: Wed, 20 Apr 2022 07:05:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1.2`

```console
$ docker pull couchdb@sha256:a18e2e79817527719dc9af1f8c2cc67bab63e9a83dca164c3ac1d9b6c6157af6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1.2` - linux; amd64

```console
$ docker pull couchdb@sha256:1327b4719a309eecd4737ce51506b867ad47d7040353c36d178b031f95c0a07e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80009876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a073ccc4150877efa603e9c3b799f7f2552153bf4f1c55f4d9e84c6a4b3cb7b3`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:48 GMT
ADD file:011a43ee23214c201afb7f3b5be592f374b89a4c71aea82ca66146bbbc31b959 in / 
# Wed, 20 Apr 2022 04:43:48 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:11:10 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 20 Apr 2022 07:11:10 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 20 Apr 2022 07:11:17 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:11:21 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 20 Apr 2022 07:11:21 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 20 Apr 2022 07:11:28 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:11:28 GMT
ENV COUCHDB_VERSION=3.1.2
# Wed, 20 Apr 2022 07:11:28 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 20 Apr 2022 07:11:42 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 20 Apr 2022 07:11:42 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 20 Apr 2022 07:11:42 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 20 Apr 2022 07:11:42 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 20 Apr 2022 07:11:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 20 Apr 2022 07:11:43 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 20 Apr 2022 07:11:43 GMT
VOLUME [/opt/couchdb/data]
# Wed, 20 Apr 2022 07:11:43 GMT
EXPOSE 4369 5984 9100
# Wed, 20 Apr 2022 07:11:43 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:4be315f6562fccf08fd6c749557e31e45ab6d987370e20e2c4933ddb04ddd5ff`  
		Last Modified: Wed, 20 Apr 2022 04:49:15 GMT  
		Size: 27.1 MB (27140664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cda2a4a9a9c0972a269e783092de1ff725f53eb1d78a8fb9e9fc7edd249003e`  
		Last Modified: Wed, 20 Apr 2022 07:12:52 GMT  
		Size: 3.4 KB (3408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35595421e132bd4b6bbcb5ce7de4cab1b3e6166ff0310ec3a445baf267b0ee49`  
		Last Modified: Wed, 20 Apr 2022 07:12:51 GMT  
		Size: 6.7 MB (6698605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e21c134e694eaf537fbfa0a926df693f490ddccc20da9b4d1e1b72c3fa4415d`  
		Last Modified: Wed, 20 Apr 2022 07:12:50 GMT  
		Size: 1.3 MB (1258366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613f17690642b0eb670154685591206b152fc004ce6c451fef9a943551fadcd3`  
		Last Modified: Wed, 20 Apr 2022 07:12:50 GMT  
		Size: 293.0 KB (292999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98f535ebc016d2e50cc212c899468dc5a16d41f10eab7fc5c6331a52888efa1d`  
		Last Modified: Wed, 20 Apr 2022 07:12:50 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ea72ee2cf4cb7497a97d20f65dea99c1708962f8eac376f9baa83e481f9abd`  
		Last Modified: Wed, 20 Apr 2022 07:12:53 GMT  
		Size: 44.6 MB (44612241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2751f3407a76c10f2f624f6496291f2cbb4bb1f8302d3dcce5931898ba7617`  
		Last Modified: Wed, 20 Apr 2022 07:12:48 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9905b54ec2a6b543273ff2135dd12a449ebd9101e7ec86c92e324b5c741bf189`  
		Last Modified: Wed, 20 Apr 2022 07:12:47 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20349b7cce82d73993ad9221569b8665490627b6979b590a1370da1eb32c61fc`  
		Last Modified: Wed, 20 Apr 2022 07:12:47 GMT  
		Size: 2.1 KB (2056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6789f6e6be0cc122e54512c9653ba927835e3d93ba4a43217da085ca293b670c`  
		Last Modified: Wed, 20 Apr 2022 07:12:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:f3908b181a74e95c54b42988e7852a301cdc432e96b9d743516fe11cb68c74b9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74615234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c756e28808c4459a6411688662f0a1da3ab8fda054ee87e9ebfde5f2b155ab5f`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:36 GMT
ADD file:5de4397c1295f7249c93907be599d96efbd9cd25909340d245ec8d1c9770f444 in / 
# Wed, 20 Apr 2022 04:29:37 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:03:39 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 20 Apr 2022 07:03:40 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 20 Apr 2022 07:03:48 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:03:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 20 Apr 2022 07:03:53 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 20 Apr 2022 07:04:00 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:04:00 GMT
ENV COUCHDB_VERSION=3.1.2
# Wed, 20 Apr 2022 07:04:01 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 20 Apr 2022 07:04:19 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 20 Apr 2022 07:04:21 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 20 Apr 2022 07:04:22 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 20 Apr 2022 07:04:23 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 20 Apr 2022 07:04:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 20 Apr 2022 07:04:24 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 20 Apr 2022 07:04:25 GMT
VOLUME [/opt/couchdb/data]
# Wed, 20 Apr 2022 07:04:26 GMT
EXPOSE 4369 5984 9100
# Wed, 20 Apr 2022 07:04:27 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6c3e5b218d6477ff77053280968d5bdeaa5dcf16a803e917d98dd0ea8b93ac82`  
		Last Modified: Wed, 20 Apr 2022 04:36:38 GMT  
		Size: 25.9 MB (25908349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15dfa2d73c72258f50f849a1f31a09fb838258553d12e341020e966370d0b858`  
		Last Modified: Wed, 20 Apr 2022 07:06:01 GMT  
		Size: 3.3 KB (3316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcdad7b881f9dd0b2907bb1dc0f751b78915b2de7b6ddc44cd02157372005dfd`  
		Last Modified: Wed, 20 Apr 2022 07:06:01 GMT  
		Size: 6.6 MB (6556359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2262e1b6750144c60a72a0ef3a2a8f8b12096df0ed32f784a1fd0b002e95bba1`  
		Last Modified: Wed, 20 Apr 2022 07:05:59 GMT  
		Size: 951.1 KB (951150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7d0666a4c86366363b1a4fcb9e452af0faa020dc867402e9b609b49fde965e`  
		Last Modified: Wed, 20 Apr 2022 07:05:59 GMT  
		Size: 79.9 KB (79922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fe5c7236bf910b320f7095182b16d6250cb5028bb933ba74ce601554777673`  
		Last Modified: Wed, 20 Apr 2022 07:05:59 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb8867ec1107935115c1fb1eeca46dfb3b4d7b127cd3f24c7dfb5251e04a5af`  
		Last Modified: Wed, 20 Apr 2022 07:06:02 GMT  
		Size: 41.1 MB (41112540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953af7dec7b828efe5a6f93229ee11516acfd3061230552867a0734fa4478917`  
		Last Modified: Wed, 20 Apr 2022 07:05:57 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0e21c4295b22ca6079f7a475ab03bcdd7e979ed2ce3900be892a08151702c5`  
		Last Modified: Wed, 20 Apr 2022 07:05:57 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1347aa0b12961ab0309af180e4a4691dddec581f87aa3e147627925baa5bc161`  
		Last Modified: Wed, 20 Apr 2022 07:05:57 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3d40c189a512811b2a9ed3a1412449155bb1ae67f2865d5e325ba0fda20b44`  
		Last Modified: Wed, 20 Apr 2022 07:05:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2`

```console
$ docker pull couchdb@sha256:37a7a9aab050c8c376b012d9c52da58e2c94d221b0eb5567edb88d8ceca096ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2` - linux; amd64

```console
$ docker pull couchdb@sha256:2c96232290fe0414177909bdb8c30224af32c2f8f7031d868fb832ffaac6cc4f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87451684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b53c5467cf3ac9c9d94c8922a210bc132fa625e0059a48054a22a992881b1a8f`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:10:30 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 20 Apr 2022 07:10:30 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 20 Apr 2022 07:10:37 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:10:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 20 Apr 2022 07:10:41 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 20 Apr 2022 07:10:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:10:47 GMT
ENV COUCHDB_VERSION=3.2.1-1
# Wed, 20 Apr 2022 07:10:47 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 20 Apr 2022 07:11:00 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 20 Apr 2022 07:11:00 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 20 Apr 2022 07:11:01 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 20 Apr 2022 07:11:01 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 20 Apr 2022 07:11:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 20 Apr 2022 07:11:01 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 20 Apr 2022 07:11:01 GMT
VOLUME [/opt/couchdb/data]
# Wed, 20 Apr 2022 07:11:02 GMT
EXPOSE 4369 5984 9100
# Wed, 20 Apr 2022 07:11:02 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e4fb628d536f433a0a908e8e65812c407b41d7039fa72adc77277f091a8924`  
		Last Modified: Wed, 20 Apr 2022 07:12:30 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5ada74819f3e5a933ad7776886fd3b202f99653d68b746f8e1ca6bf158db5a`  
		Last Modified: Wed, 20 Apr 2022 07:12:29 GMT  
		Size: 5.2 MB (5223690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7d8f1aed9465ca9c4007a6277de02a53c60b7f77c8a0a6dca2a0fe064afa93`  
		Last Modified: Wed, 20 Apr 2022 07:12:29 GMT  
		Size: 1.6 MB (1553283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464d6b8b4bbbc83281231e89eac3d0d5d2142d261de2db10cc7f65167b545c77`  
		Last Modified: Wed, 20 Apr 2022 07:12:28 GMT  
		Size: 295.6 KB (295569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b71906ef4252c8d9093a53eaeae741462aed454881113137d2c5539a5b39cca`  
		Last Modified: Wed, 20 Apr 2022 07:12:28 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43f2ebb365be093fc6c10de52167a7915582ca0d80a1594fe31f74d652ec583`  
		Last Modified: Wed, 20 Apr 2022 07:12:32 GMT  
		Size: 49.0 MB (48993027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09b9610f19e31700a17b805c579fed67585d29389cd706ac975e38fe16967c3`  
		Last Modified: Wed, 20 Apr 2022 07:12:26 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad96a982041d41e0a94650bcac88201e50a18622c16b84db337c84799cbaadf2`  
		Last Modified: Wed, 20 Apr 2022 07:12:26 GMT  
		Size: 768.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9590c0cb12e900d1d82e53daf2bb099c6230b830cc3f3b72fd4455e2ff598306`  
		Last Modified: Wed, 20 Apr 2022 07:12:26 GMT  
		Size: 2.2 KB (2179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a01aac1048bee36c25c3b24ae92a24faf3c8418d592dbd209938398b439036`  
		Last Modified: Wed, 20 Apr 2022 07:12:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:b1ce2bd46ec5ea9656d89ee31fb5ddb80f5bbb18c24b38536eab91423bd75654
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.4 MB (85383029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72dd9a06ea5af54ebc9afe1b239f350e954ae38e39e75097dcbfba5ce977eb21`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:02:48 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 20 Apr 2022 07:02:48 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 20 Apr 2022 07:02:55 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:02:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 20 Apr 2022 07:03:00 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 20 Apr 2022 07:03:06 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:03:07 GMT
ENV COUCHDB_VERSION=3.2.1-1
# Wed, 20 Apr 2022 07:03:08 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 20 Apr 2022 07:03:26 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 20 Apr 2022 07:03:27 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 20 Apr 2022 07:03:28 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 20 Apr 2022 07:03:29 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 20 Apr 2022 07:03:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 20 Apr 2022 07:03:30 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 20 Apr 2022 07:03:31 GMT
VOLUME [/opt/couchdb/data]
# Wed, 20 Apr 2022 07:03:32 GMT
EXPOSE 4369 5984 9100
# Wed, 20 Apr 2022 07:03:33 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51cefb89564694ca915e167c405ee5881088311379fb87639609d213f6bb420`  
		Last Modified: Wed, 20 Apr 2022 07:05:36 GMT  
		Size: 3.3 KB (3319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ec39efab772ade8e91f1021e60940ff0365826df140afe1f51e150ceb0303b`  
		Last Modified: Wed, 20 Apr 2022 07:05:35 GMT  
		Size: 5.0 MB (5002920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b4d5c3bee5b8e99b3e70d3a88123a53caf0860986a9eb6e68d6c4ed7022533`  
		Last Modified: Wed, 20 Apr 2022 07:05:34 GMT  
		Size: 1.2 MB (1221077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6fb8160cb2a1f0d19dd386151a86a62c1e568354e1aac1a650c0d9fde62de7`  
		Last Modified: Wed, 20 Apr 2022 07:05:34 GMT  
		Size: 79.2 KB (79168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b99c7181f5a3992355deabe6e521d071029050e68f777a730b24dba5cf3a949`  
		Last Modified: Wed, 20 Apr 2022 07:05:34 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd1b9b51ff525d46c102aafe33ec2631c99218677d1fb9505db73af88f22380`  
		Last Modified: Wed, 20 Apr 2022 07:05:37 GMT  
		Size: 49.0 MB (49007026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf44f240a74efe39263490f22dbad69cb71869ee20eeeca196dc544cadaa1e26`  
		Last Modified: Wed, 20 Apr 2022 07:05:31 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dfe021f0efc89117bdd8aaf84ff80a530d7366daf172e2ce3aabb5b7d4c9ea7`  
		Last Modified: Wed, 20 Apr 2022 07:05:32 GMT  
		Size: 761.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03dfc4e590017fbe73692daf143f06beda0a5c608db21e54a1f335fe8a112c4`  
		Last Modified: Wed, 20 Apr 2022 07:05:31 GMT  
		Size: 2.2 KB (2182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726df3f6f358317ff48ad598cd6294cc97db9360f05674ad2b3251d7ec7c9cd4`  
		Last Modified: Wed, 20 Apr 2022 07:05:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; ppc64le

```console
$ docker pull couchdb@sha256:1c4f2cdf4fd85d3542f9d953a52e34ec350bdd9bdef6bc2319852c03a79ea3ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93170578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:687faa76badbcab293da87344a0728961f84a6dcc64c64b38adbc1e0e6962a71`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 20 Apr 2022 09:46:36 GMT
ADD file:8d406ebce4d9b0884d46ee25ec31fe7714726024b80aba9b408d81d39e2f6f8c in / 
# Wed, 20 Apr 2022 09:46:44 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 17:38:52 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 20 Apr 2022 17:39:03 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 20 Apr 2022 17:40:27 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 17:40:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 20 Apr 2022 17:40:45 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 20 Apr 2022 17:41:21 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 17:41:24 GMT
ENV COUCHDB_VERSION=3.2.1-1
# Wed, 20 Apr 2022 17:41:31 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 20 Apr 2022 17:42:11 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 20 Apr 2022 17:42:13 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 20 Apr 2022 17:42:14 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 20 Apr 2022 17:42:16 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 20 Apr 2022 17:42:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 20 Apr 2022 17:42:24 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 20 Apr 2022 17:42:26 GMT
VOLUME [/opt/couchdb/data]
# Wed, 20 Apr 2022 17:42:30 GMT
EXPOSE 4369 5984 9100
# Wed, 20 Apr 2022 17:42:32 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:5e0d035960b14409a1ddb839de80aa08677b71addd5e94264ff9ee89a2523e5b`  
		Last Modified: Wed, 20 Apr 2022 09:56:59 GMT  
		Size: 35.3 MB (35285249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188a5996a68176f11650fa0166342f84d30a315d76d4a70562defe4528ede8d2`  
		Last Modified: Wed, 20 Apr 2022 17:43:03 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c752a79eaca840a137608a3021b6cc666055ffb706a73ff54f5353c6ffd933`  
		Last Modified: Wed, 20 Apr 2022 17:43:01 GMT  
		Size: 6.0 MB (6043780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d488f2af80a56c0f11ddcdeaa3941cb822ae2cdc4bed7b5cee88f1cf382f6db0`  
		Last Modified: Wed, 20 Apr 2022 17:43:00 GMT  
		Size: 1.5 MB (1509335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b958f31aae831160c8329bdb19bcb57c1dbd219b156fdfce20bfe5c1e3bc72`  
		Last Modified: Wed, 20 Apr 2022 17:43:01 GMT  
		Size: 295.7 KB (295733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b45400e02e64efbce766c8a10cd174ed7902d081ca92b816d94a4e03375a95`  
		Last Modified: Wed, 20 Apr 2022 17:43:00 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1150f12eed05ab2096de0b9a91767e07ba799e2e58c52e9d0462f240ca1dc641`  
		Last Modified: Wed, 20 Apr 2022 17:43:05 GMT  
		Size: 50.0 MB (50029335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3ebde4b104f87037282a2dd623138620548ef9f0c7ec84acd4a357b16199c0`  
		Last Modified: Wed, 20 Apr 2022 17:42:57 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e3f2b1940560793ab014bc68027fdec22ac5bdd5ca38444da6df377e9df987`  
		Last Modified: Wed, 20 Apr 2022 17:42:57 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea19cadf45f2297795ff6894e7d3df3a91e166e71704d2c3eae94c4afbf9d0f9`  
		Last Modified: Wed, 20 Apr 2022 17:42:57 GMT  
		Size: 2.2 KB (2188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d70e2634cff623886f8a678fab41a5d4158a1bd6d6f4dcdc7ae82b4d0d3607`  
		Last Modified: Wed, 20 Apr 2022 17:42:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2.2`

```console
$ docker pull couchdb@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `couchdb:latest`

```console
$ docker pull couchdb@sha256:37a7a9aab050c8c376b012d9c52da58e2c94d221b0eb5567edb88d8ceca096ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:2c96232290fe0414177909bdb8c30224af32c2f8f7031d868fb832ffaac6cc4f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87451684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b53c5467cf3ac9c9d94c8922a210bc132fa625e0059a48054a22a992881b1a8f`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:10:30 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 20 Apr 2022 07:10:30 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 20 Apr 2022 07:10:37 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:10:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 20 Apr 2022 07:10:41 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 20 Apr 2022 07:10:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:10:47 GMT
ENV COUCHDB_VERSION=3.2.1-1
# Wed, 20 Apr 2022 07:10:47 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 20 Apr 2022 07:11:00 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 20 Apr 2022 07:11:00 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 20 Apr 2022 07:11:01 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 20 Apr 2022 07:11:01 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 20 Apr 2022 07:11:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 20 Apr 2022 07:11:01 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 20 Apr 2022 07:11:01 GMT
VOLUME [/opt/couchdb/data]
# Wed, 20 Apr 2022 07:11:02 GMT
EXPOSE 4369 5984 9100
# Wed, 20 Apr 2022 07:11:02 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e4fb628d536f433a0a908e8e65812c407b41d7039fa72adc77277f091a8924`  
		Last Modified: Wed, 20 Apr 2022 07:12:30 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5ada74819f3e5a933ad7776886fd3b202f99653d68b746f8e1ca6bf158db5a`  
		Last Modified: Wed, 20 Apr 2022 07:12:29 GMT  
		Size: 5.2 MB (5223690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7d8f1aed9465ca9c4007a6277de02a53c60b7f77c8a0a6dca2a0fe064afa93`  
		Last Modified: Wed, 20 Apr 2022 07:12:29 GMT  
		Size: 1.6 MB (1553283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464d6b8b4bbbc83281231e89eac3d0d5d2142d261de2db10cc7f65167b545c77`  
		Last Modified: Wed, 20 Apr 2022 07:12:28 GMT  
		Size: 295.6 KB (295569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b71906ef4252c8d9093a53eaeae741462aed454881113137d2c5539a5b39cca`  
		Last Modified: Wed, 20 Apr 2022 07:12:28 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43f2ebb365be093fc6c10de52167a7915582ca0d80a1594fe31f74d652ec583`  
		Last Modified: Wed, 20 Apr 2022 07:12:32 GMT  
		Size: 49.0 MB (48993027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09b9610f19e31700a17b805c579fed67585d29389cd706ac975e38fe16967c3`  
		Last Modified: Wed, 20 Apr 2022 07:12:26 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad96a982041d41e0a94650bcac88201e50a18622c16b84db337c84799cbaadf2`  
		Last Modified: Wed, 20 Apr 2022 07:12:26 GMT  
		Size: 768.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9590c0cb12e900d1d82e53daf2bb099c6230b830cc3f3b72fd4455e2ff598306`  
		Last Modified: Wed, 20 Apr 2022 07:12:26 GMT  
		Size: 2.2 KB (2179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a01aac1048bee36c25c3b24ae92a24faf3c8418d592dbd209938398b439036`  
		Last Modified: Wed, 20 Apr 2022 07:12:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:b1ce2bd46ec5ea9656d89ee31fb5ddb80f5bbb18c24b38536eab91423bd75654
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.4 MB (85383029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72dd9a06ea5af54ebc9afe1b239f350e954ae38e39e75097dcbfba5ce977eb21`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:02:48 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 20 Apr 2022 07:02:48 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 20 Apr 2022 07:02:55 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:02:59 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 20 Apr 2022 07:03:00 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 20 Apr 2022 07:03:06 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:03:07 GMT
ENV COUCHDB_VERSION=3.2.1-1
# Wed, 20 Apr 2022 07:03:08 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 20 Apr 2022 07:03:26 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 20 Apr 2022 07:03:27 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 20 Apr 2022 07:03:28 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 20 Apr 2022 07:03:29 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 20 Apr 2022 07:03:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 20 Apr 2022 07:03:30 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 20 Apr 2022 07:03:31 GMT
VOLUME [/opt/couchdb/data]
# Wed, 20 Apr 2022 07:03:32 GMT
EXPOSE 4369 5984 9100
# Wed, 20 Apr 2022 07:03:33 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51cefb89564694ca915e167c405ee5881088311379fb87639609d213f6bb420`  
		Last Modified: Wed, 20 Apr 2022 07:05:36 GMT  
		Size: 3.3 KB (3319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ec39efab772ade8e91f1021e60940ff0365826df140afe1f51e150ceb0303b`  
		Last Modified: Wed, 20 Apr 2022 07:05:35 GMT  
		Size: 5.0 MB (5002920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b4d5c3bee5b8e99b3e70d3a88123a53caf0860986a9eb6e68d6c4ed7022533`  
		Last Modified: Wed, 20 Apr 2022 07:05:34 GMT  
		Size: 1.2 MB (1221077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6fb8160cb2a1f0d19dd386151a86a62c1e568354e1aac1a650c0d9fde62de7`  
		Last Modified: Wed, 20 Apr 2022 07:05:34 GMT  
		Size: 79.2 KB (79168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b99c7181f5a3992355deabe6e521d071029050e68f777a730b24dba5cf3a949`  
		Last Modified: Wed, 20 Apr 2022 07:05:34 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd1b9b51ff525d46c102aafe33ec2631c99218677d1fb9505db73af88f22380`  
		Last Modified: Wed, 20 Apr 2022 07:05:37 GMT  
		Size: 49.0 MB (49007026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf44f240a74efe39263490f22dbad69cb71869ee20eeeca196dc544cadaa1e26`  
		Last Modified: Wed, 20 Apr 2022 07:05:31 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dfe021f0efc89117bdd8aaf84ff80a530d7366daf172e2ce3aabb5b7d4c9ea7`  
		Last Modified: Wed, 20 Apr 2022 07:05:32 GMT  
		Size: 761.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03dfc4e590017fbe73692daf143f06beda0a5c608db21e54a1f335fe8a112c4`  
		Last Modified: Wed, 20 Apr 2022 07:05:31 GMT  
		Size: 2.2 KB (2182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726df3f6f358317ff48ad598cd6294cc97db9360f05674ad2b3251d7ec7c9cd4`  
		Last Modified: Wed, 20 Apr 2022 07:05:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; ppc64le

```console
$ docker pull couchdb@sha256:1c4f2cdf4fd85d3542f9d953a52e34ec350bdd9bdef6bc2319852c03a79ea3ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93170578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:687faa76badbcab293da87344a0728961f84a6dcc64c64b38adbc1e0e6962a71`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 20 Apr 2022 09:46:36 GMT
ADD file:8d406ebce4d9b0884d46ee25ec31fe7714726024b80aba9b408d81d39e2f6f8c in / 
# Wed, 20 Apr 2022 09:46:44 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 17:38:52 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 20 Apr 2022 17:39:03 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 20 Apr 2022 17:40:27 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 17:40:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 20 Apr 2022 17:40:45 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 20 Apr 2022 17:41:21 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 17:41:24 GMT
ENV COUCHDB_VERSION=3.2.1-1
# Wed, 20 Apr 2022 17:41:31 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 20 Apr 2022 17:42:11 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 20 Apr 2022 17:42:13 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 20 Apr 2022 17:42:14 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 20 Apr 2022 17:42:16 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 20 Apr 2022 17:42:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 20 Apr 2022 17:42:24 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 20 Apr 2022 17:42:26 GMT
VOLUME [/opt/couchdb/data]
# Wed, 20 Apr 2022 17:42:30 GMT
EXPOSE 4369 5984 9100
# Wed, 20 Apr 2022 17:42:32 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:5e0d035960b14409a1ddb839de80aa08677b71addd5e94264ff9ee89a2523e5b`  
		Last Modified: Wed, 20 Apr 2022 09:56:59 GMT  
		Size: 35.3 MB (35285249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188a5996a68176f11650fa0166342f84d30a315d76d4a70562defe4528ede8d2`  
		Last Modified: Wed, 20 Apr 2022 17:43:03 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c752a79eaca840a137608a3021b6cc666055ffb706a73ff54f5353c6ffd933`  
		Last Modified: Wed, 20 Apr 2022 17:43:01 GMT  
		Size: 6.0 MB (6043780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d488f2af80a56c0f11ddcdeaa3941cb822ae2cdc4bed7b5cee88f1cf382f6db0`  
		Last Modified: Wed, 20 Apr 2022 17:43:00 GMT  
		Size: 1.5 MB (1509335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b958f31aae831160c8329bdb19bcb57c1dbd219b156fdfce20bfe5c1e3bc72`  
		Last Modified: Wed, 20 Apr 2022 17:43:01 GMT  
		Size: 295.7 KB (295733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b45400e02e64efbce766c8a10cd174ed7902d081ca92b816d94a4e03375a95`  
		Last Modified: Wed, 20 Apr 2022 17:43:00 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1150f12eed05ab2096de0b9a91767e07ba799e2e58c52e9d0462f240ca1dc641`  
		Last Modified: Wed, 20 Apr 2022 17:43:05 GMT  
		Size: 50.0 MB (50029335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3ebde4b104f87037282a2dd623138620548ef9f0c7ec84acd4a357b16199c0`  
		Last Modified: Wed, 20 Apr 2022 17:42:57 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e3f2b1940560793ab014bc68027fdec22ac5bdd5ca38444da6df377e9df987`  
		Last Modified: Wed, 20 Apr 2022 17:42:57 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea19cadf45f2297795ff6894e7d3df3a91e166e71704d2c3eae94c4afbf9d0f9`  
		Last Modified: Wed, 20 Apr 2022 17:42:57 GMT  
		Size: 2.2 KB (2188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d70e2634cff623886f8a678fab41a5d4158a1bd6d6f4dcdc7ae82b4d0d3607`  
		Last Modified: Wed, 20 Apr 2022 17:42:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
