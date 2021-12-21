<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `couchdb`

-	[`couchdb:2`](#couchdb2)
-	[`couchdb:2.3`](#couchdb23)
-	[`couchdb:2.3.1`](#couchdb231)
-	[`couchdb:3`](#couchdb3)
-	[`couchdb:3.1`](#couchdb31)
-	[`couchdb:3.1.2`](#couchdb312)
-	[`couchdb:3.2`](#couchdb32)
-	[`couchdb:3.2.0`](#couchdb320)
-	[`couchdb:latest`](#couchdblatest)

## `couchdb:2`

```console
$ docker pull couchdb@sha256:3e80462285b5ae54c5200e4bbf07b6a0e2076238b41f0c409706943f0ced5bd4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2` - linux; amd64

```console
$ docker pull couchdb@sha256:03775cf875992a4d4c2ecc960a3ad993ce75d1e253052d6a97a1b5f35d703373
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84517207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4eeb2fa8b5b9ce75c02a424d5d37dd3f2a515c2d5a0360dd625644e0dd84b71`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:09:14 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Dec 2021 02:09:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Dec 2021 02:09:22 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:09:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 21 Dec 2021 02:09:27 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Dec 2021 02:09:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:10:13 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 21 Dec 2021 02:10:14 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Dec 2021 02:10:32 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Dec 2021 02:10:33 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Dec 2021 02:10:33 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 21 Dec 2021 02:10:33 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 21 Dec 2021 02:10:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Dec 2021 02:10:34 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Dec 2021 02:10:34 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Dec 2021 02:10:35 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Dec 2021 02:10:35 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430d6c754b31c32dd1a76de01ad3420033c05661c724b97d708362a8ec139d42`  
		Last Modified: Tue, 21 Dec 2021 02:10:58 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3227820103030b5232e32ba7e76de56823a61d47245d450403c0040933f6aebd`  
		Last Modified: Tue, 21 Dec 2021 02:10:58 GMT  
		Size: 6.7 MB (6691223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454611cf9dafef09164a7f64cb967a12ab5d1549d70599c56b74a2c283ae8ef1`  
		Last Modified: Tue, 21 Dec 2021 02:10:56 GMT  
		Size: 1.3 MB (1258346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5993063a8d6d688f066b9d8208c98f7d0dd3d78e7076cbc7a132ab98a975dece`  
		Last Modified: Tue, 21 Dec 2021 02:10:56 GMT  
		Size: 293.0 KB (293029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1637f5ce62470caf7b07bea4f8d9390cbc4b7d4d0327077ff7dc0a6945d1c7e1`  
		Last Modified: Tue, 21 Dec 2021 02:11:33 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94c9d9a9a8f2c85a319528cd13d772ff89bec2ee8a63c3f44f29146f33381ae`  
		Last Modified: Tue, 21 Dec 2021 02:11:38 GMT  
		Size: 49.1 MB (49113865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5c1ae4a87ec62883c2b6cdecdcbd87b2b45770266482f2affe0e987595c1fd`  
		Last Modified: Tue, 21 Dec 2021 02:11:31 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca940117ded324a7613aec69d0a872122475b20d28490cc85075417bc2e1c14b`  
		Last Modified: Tue, 21 Dec 2021 02:11:31 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8b1e22e3198e344c657e9b7e16d7a102e3f9be9c43e64e085f782600ca1627`  
		Last Modified: Tue, 21 Dec 2021 02:11:31 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f074cac28bde7e408bfeaf9dbc7076e5376ff6197806fc282ef88f12967f2230`  
		Last Modified: Tue, 21 Dec 2021 02:11:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:8756f44be2a37e374b5c03a908af5791d6fece92059f73e60a0ce736f76c0568
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72522897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3349cfde297fc5d02e0373c189ba970a79b47d61bb3ea4d20a7964a6c597f907`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:46:04 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 02 Dec 2021 17:46:05 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 02 Dec 2021 17:46:13 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 17:46:17 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 02 Dec 2021 17:46:18 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 02 Dec 2021 17:46:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 17:47:36 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Thu, 02 Dec 2021 17:47:37 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 02 Dec 2021 17:47:55 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 02 Dec 2021 17:47:56 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Thu, 02 Dec 2021 17:47:57 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 02 Dec 2021 17:47:58 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Thu, 02 Dec 2021 17:47:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 02 Dec 2021 17:47:59 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 02 Dec 2021 17:48:00 GMT
VOLUME [/opt/couchdb/data]
# Thu, 02 Dec 2021 17:48:01 GMT
EXPOSE 4369 5984 9100
# Thu, 02 Dec 2021 17:48:02 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5791b8b3b4e5d779c522c8017cee4a5f7c64f62d1208f4d56d084e1d27362c98`  
		Last Modified: Thu, 02 Dec 2021 17:48:32 GMT  
		Size: 3.3 KB (3321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba826eb9f904f9937112e4e7500b42b85d35917d8458e9127896ac660ca0ffa5`  
		Last Modified: Thu, 02 Dec 2021 17:48:33 GMT  
		Size: 6.5 MB (6549971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d876e68b2d02a750e6cedd22e42c92932d962bdd0b252c5c0f3019749066899b`  
		Last Modified: Thu, 02 Dec 2021 17:48:30 GMT  
		Size: 951.2 KB (951153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24f278b93ab8d00de4ac6464e2204e283e60aedfcce676149a9d2400fdca51c`  
		Last Modified: Thu, 02 Dec 2021 17:48:30 GMT  
		Size: 79.9 KB (79917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9faeac5439f1e45b6a44899ff7690d83836e5467b6b55a005d3d7e331217cb87`  
		Last Modified: Thu, 02 Dec 2021 17:49:10 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8cf3ef078c338285580f2bde933050d99147ed85c1a488d4123e559eebca367`  
		Last Modified: Thu, 02 Dec 2021 17:49:12 GMT  
		Size: 39.0 MB (39011789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7665658769b023926c69a9257d2ffbb5c3e691bd956add0e73c55c561d8ceeb`  
		Last Modified: Thu, 02 Dec 2021 17:49:08 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d8bf7691dbfe3e5e3cd600230e010f36861a55b5e7203f54baaeff0d306552`  
		Last Modified: Thu, 02 Dec 2021 17:49:08 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3c6b538a67d78b6909ff1fa1a069c5c6eff6adaa549af8637fb52a7e75be51`  
		Last Modified: Thu, 02 Dec 2021 17:49:08 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb5cce696776e910dbce75e70d3f9a1e94d2d87cfbce70858e02dafb701acbd`  
		Last Modified: Thu, 02 Dec 2021 17:49:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3`

```console
$ docker pull couchdb@sha256:3e80462285b5ae54c5200e4bbf07b6a0e2076238b41f0c409706943f0ced5bd4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:03775cf875992a4d4c2ecc960a3ad993ce75d1e253052d6a97a1b5f35d703373
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84517207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4eeb2fa8b5b9ce75c02a424d5d37dd3f2a515c2d5a0360dd625644e0dd84b71`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:09:14 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Dec 2021 02:09:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Dec 2021 02:09:22 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:09:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 21 Dec 2021 02:09:27 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Dec 2021 02:09:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:10:13 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 21 Dec 2021 02:10:14 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Dec 2021 02:10:32 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Dec 2021 02:10:33 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Dec 2021 02:10:33 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 21 Dec 2021 02:10:33 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 21 Dec 2021 02:10:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Dec 2021 02:10:34 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Dec 2021 02:10:34 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Dec 2021 02:10:35 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Dec 2021 02:10:35 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430d6c754b31c32dd1a76de01ad3420033c05661c724b97d708362a8ec139d42`  
		Last Modified: Tue, 21 Dec 2021 02:10:58 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3227820103030b5232e32ba7e76de56823a61d47245d450403c0040933f6aebd`  
		Last Modified: Tue, 21 Dec 2021 02:10:58 GMT  
		Size: 6.7 MB (6691223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454611cf9dafef09164a7f64cb967a12ab5d1549d70599c56b74a2c283ae8ef1`  
		Last Modified: Tue, 21 Dec 2021 02:10:56 GMT  
		Size: 1.3 MB (1258346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5993063a8d6d688f066b9d8208c98f7d0dd3d78e7076cbc7a132ab98a975dece`  
		Last Modified: Tue, 21 Dec 2021 02:10:56 GMT  
		Size: 293.0 KB (293029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1637f5ce62470caf7b07bea4f8d9390cbc4b7d4d0327077ff7dc0a6945d1c7e1`  
		Last Modified: Tue, 21 Dec 2021 02:11:33 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94c9d9a9a8f2c85a319528cd13d772ff89bec2ee8a63c3f44f29146f33381ae`  
		Last Modified: Tue, 21 Dec 2021 02:11:38 GMT  
		Size: 49.1 MB (49113865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5c1ae4a87ec62883c2b6cdecdcbd87b2b45770266482f2affe0e987595c1fd`  
		Last Modified: Tue, 21 Dec 2021 02:11:31 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca940117ded324a7613aec69d0a872122475b20d28490cc85075417bc2e1c14b`  
		Last Modified: Tue, 21 Dec 2021 02:11:31 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8b1e22e3198e344c657e9b7e16d7a102e3f9be9c43e64e085f782600ca1627`  
		Last Modified: Tue, 21 Dec 2021 02:11:31 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f074cac28bde7e408bfeaf9dbc7076e5376ff6197806fc282ef88f12967f2230`  
		Last Modified: Tue, 21 Dec 2021 02:11:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:8756f44be2a37e374b5c03a908af5791d6fece92059f73e60a0ce736f76c0568
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72522897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3349cfde297fc5d02e0373c189ba970a79b47d61bb3ea4d20a7964a6c597f907`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:46:04 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 02 Dec 2021 17:46:05 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 02 Dec 2021 17:46:13 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 17:46:17 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 02 Dec 2021 17:46:18 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 02 Dec 2021 17:46:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 17:47:36 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Thu, 02 Dec 2021 17:47:37 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 02 Dec 2021 17:47:55 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 02 Dec 2021 17:47:56 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Thu, 02 Dec 2021 17:47:57 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 02 Dec 2021 17:47:58 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Thu, 02 Dec 2021 17:47:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 02 Dec 2021 17:47:59 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 02 Dec 2021 17:48:00 GMT
VOLUME [/opt/couchdb/data]
# Thu, 02 Dec 2021 17:48:01 GMT
EXPOSE 4369 5984 9100
# Thu, 02 Dec 2021 17:48:02 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5791b8b3b4e5d779c522c8017cee4a5f7c64f62d1208f4d56d084e1d27362c98`  
		Last Modified: Thu, 02 Dec 2021 17:48:32 GMT  
		Size: 3.3 KB (3321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba826eb9f904f9937112e4e7500b42b85d35917d8458e9127896ac660ca0ffa5`  
		Last Modified: Thu, 02 Dec 2021 17:48:33 GMT  
		Size: 6.5 MB (6549971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d876e68b2d02a750e6cedd22e42c92932d962bdd0b252c5c0f3019749066899b`  
		Last Modified: Thu, 02 Dec 2021 17:48:30 GMT  
		Size: 951.2 KB (951153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24f278b93ab8d00de4ac6464e2204e283e60aedfcce676149a9d2400fdca51c`  
		Last Modified: Thu, 02 Dec 2021 17:48:30 GMT  
		Size: 79.9 KB (79917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9faeac5439f1e45b6a44899ff7690d83836e5467b6b55a005d3d7e331217cb87`  
		Last Modified: Thu, 02 Dec 2021 17:49:10 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8cf3ef078c338285580f2bde933050d99147ed85c1a488d4123e559eebca367`  
		Last Modified: Thu, 02 Dec 2021 17:49:12 GMT  
		Size: 39.0 MB (39011789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7665658769b023926c69a9257d2ffbb5c3e691bd956add0e73c55c561d8ceeb`  
		Last Modified: Thu, 02 Dec 2021 17:49:08 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d8bf7691dbfe3e5e3cd600230e010f36861a55b5e7203f54baaeff0d306552`  
		Last Modified: Thu, 02 Dec 2021 17:49:08 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3c6b538a67d78b6909ff1fa1a069c5c6eff6adaa549af8637fb52a7e75be51`  
		Last Modified: Thu, 02 Dec 2021 17:49:08 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb5cce696776e910dbce75e70d3f9a1e94d2d87cfbce70858e02dafb701acbd`  
		Last Modified: Thu, 02 Dec 2021 17:49:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3.1`

```console
$ docker pull couchdb@sha256:3e80462285b5ae54c5200e4bbf07b6a0e2076238b41f0c409706943f0ced5bd4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:03775cf875992a4d4c2ecc960a3ad993ce75d1e253052d6a97a1b5f35d703373
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84517207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4eeb2fa8b5b9ce75c02a424d5d37dd3f2a515c2d5a0360dd625644e0dd84b71`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:09:14 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Dec 2021 02:09:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Dec 2021 02:09:22 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:09:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 21 Dec 2021 02:09:27 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Dec 2021 02:09:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:10:13 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 21 Dec 2021 02:10:14 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Dec 2021 02:10:32 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Dec 2021 02:10:33 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Dec 2021 02:10:33 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 21 Dec 2021 02:10:33 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 21 Dec 2021 02:10:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Dec 2021 02:10:34 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Dec 2021 02:10:34 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Dec 2021 02:10:35 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Dec 2021 02:10:35 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430d6c754b31c32dd1a76de01ad3420033c05661c724b97d708362a8ec139d42`  
		Last Modified: Tue, 21 Dec 2021 02:10:58 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3227820103030b5232e32ba7e76de56823a61d47245d450403c0040933f6aebd`  
		Last Modified: Tue, 21 Dec 2021 02:10:58 GMT  
		Size: 6.7 MB (6691223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454611cf9dafef09164a7f64cb967a12ab5d1549d70599c56b74a2c283ae8ef1`  
		Last Modified: Tue, 21 Dec 2021 02:10:56 GMT  
		Size: 1.3 MB (1258346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5993063a8d6d688f066b9d8208c98f7d0dd3d78e7076cbc7a132ab98a975dece`  
		Last Modified: Tue, 21 Dec 2021 02:10:56 GMT  
		Size: 293.0 KB (293029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1637f5ce62470caf7b07bea4f8d9390cbc4b7d4d0327077ff7dc0a6945d1c7e1`  
		Last Modified: Tue, 21 Dec 2021 02:11:33 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94c9d9a9a8f2c85a319528cd13d772ff89bec2ee8a63c3f44f29146f33381ae`  
		Last Modified: Tue, 21 Dec 2021 02:11:38 GMT  
		Size: 49.1 MB (49113865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5c1ae4a87ec62883c2b6cdecdcbd87b2b45770266482f2affe0e987595c1fd`  
		Last Modified: Tue, 21 Dec 2021 02:11:31 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca940117ded324a7613aec69d0a872122475b20d28490cc85075417bc2e1c14b`  
		Last Modified: Tue, 21 Dec 2021 02:11:31 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8b1e22e3198e344c657e9b7e16d7a102e3f9be9c43e64e085f782600ca1627`  
		Last Modified: Tue, 21 Dec 2021 02:11:31 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f074cac28bde7e408bfeaf9dbc7076e5376ff6197806fc282ef88f12967f2230`  
		Last Modified: Tue, 21 Dec 2021 02:11:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:8756f44be2a37e374b5c03a908af5791d6fece92059f73e60a0ce736f76c0568
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72522897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3349cfde297fc5d02e0373c189ba970a79b47d61bb3ea4d20a7964a6c597f907`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:46:04 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 02 Dec 2021 17:46:05 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 02 Dec 2021 17:46:13 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 17:46:17 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 02 Dec 2021 17:46:18 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 02 Dec 2021 17:46:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 17:47:36 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Thu, 02 Dec 2021 17:47:37 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 02 Dec 2021 17:47:55 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 02 Dec 2021 17:47:56 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Thu, 02 Dec 2021 17:47:57 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 02 Dec 2021 17:47:58 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Thu, 02 Dec 2021 17:47:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 02 Dec 2021 17:47:59 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 02 Dec 2021 17:48:00 GMT
VOLUME [/opt/couchdb/data]
# Thu, 02 Dec 2021 17:48:01 GMT
EXPOSE 4369 5984 9100
# Thu, 02 Dec 2021 17:48:02 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5791b8b3b4e5d779c522c8017cee4a5f7c64f62d1208f4d56d084e1d27362c98`  
		Last Modified: Thu, 02 Dec 2021 17:48:32 GMT  
		Size: 3.3 KB (3321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba826eb9f904f9937112e4e7500b42b85d35917d8458e9127896ac660ca0ffa5`  
		Last Modified: Thu, 02 Dec 2021 17:48:33 GMT  
		Size: 6.5 MB (6549971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d876e68b2d02a750e6cedd22e42c92932d962bdd0b252c5c0f3019749066899b`  
		Last Modified: Thu, 02 Dec 2021 17:48:30 GMT  
		Size: 951.2 KB (951153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24f278b93ab8d00de4ac6464e2204e283e60aedfcce676149a9d2400fdca51c`  
		Last Modified: Thu, 02 Dec 2021 17:48:30 GMT  
		Size: 79.9 KB (79917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9faeac5439f1e45b6a44899ff7690d83836e5467b6b55a005d3d7e331217cb87`  
		Last Modified: Thu, 02 Dec 2021 17:49:10 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8cf3ef078c338285580f2bde933050d99147ed85c1a488d4123e559eebca367`  
		Last Modified: Thu, 02 Dec 2021 17:49:12 GMT  
		Size: 39.0 MB (39011789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7665658769b023926c69a9257d2ffbb5c3e691bd956add0e73c55c561d8ceeb`  
		Last Modified: Thu, 02 Dec 2021 17:49:08 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d8bf7691dbfe3e5e3cd600230e010f36861a55b5e7203f54baaeff0d306552`  
		Last Modified: Thu, 02 Dec 2021 17:49:08 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3c6b538a67d78b6909ff1fa1a069c5c6eff6adaa549af8637fb52a7e75be51`  
		Last Modified: Thu, 02 Dec 2021 17:49:08 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb5cce696776e910dbce75e70d3f9a1e94d2d87cfbce70858e02dafb701acbd`  
		Last Modified: Thu, 02 Dec 2021 17:49:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3`

```console
$ docker pull couchdb@sha256:25c0c045a616e9a3a95adbafba306f33e622bd582ed4e988968dbc5d3e3384d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3` - linux; amd64

```console
$ docker pull couchdb@sha256:658ef40b47f068cdbc8e8a069d18e72df1a37c38f26890e7e2543decc24246fe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.6 MB (80555365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ac41a5539f547e479507d3cefa4a9b2a7250cbf6fd0660fbeedd8fee65f9234`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:09:14 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Dec 2021 02:09:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Dec 2021 02:09:22 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:09:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 21 Dec 2021 02:09:27 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Dec 2021 02:09:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:09:33 GMT
ENV COUCHDB_VERSION=3.2.0
# Tue, 21 Dec 2021 02:09:34 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Dec 2021 02:09:48 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Dec 2021 02:09:49 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Dec 2021 02:09:49 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 21 Dec 2021 02:09:49 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 21 Dec 2021 02:09:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Dec 2021 02:09:50 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Dec 2021 02:09:51 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Dec 2021 02:09:51 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Dec 2021 02:09:51 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430d6c754b31c32dd1a76de01ad3420033c05661c724b97d708362a8ec139d42`  
		Last Modified: Tue, 21 Dec 2021 02:10:58 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3227820103030b5232e32ba7e76de56823a61d47245d450403c0040933f6aebd`  
		Last Modified: Tue, 21 Dec 2021 02:10:58 GMT  
		Size: 6.7 MB (6691223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454611cf9dafef09164a7f64cb967a12ab5d1549d70599c56b74a2c283ae8ef1`  
		Last Modified: Tue, 21 Dec 2021 02:10:56 GMT  
		Size: 1.3 MB (1258346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5993063a8d6d688f066b9d8208c98f7d0dd3d78e7076cbc7a132ab98a975dece`  
		Last Modified: Tue, 21 Dec 2021 02:10:56 GMT  
		Size: 293.0 KB (293029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e1a5cbb187a2701cb1f4f219e175d4903fc4ef19eecfbafaa89efecfe9f350`  
		Last Modified: Tue, 21 Dec 2021 02:10:56 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf5b3b5a34ef74b2afa7c1ab7adc5957d6def0d5cb372796cadbc953023f76e`  
		Last Modified: Tue, 21 Dec 2021 02:10:59 GMT  
		Size: 45.2 MB (45152027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67b48a446b521e34ad7bbbb9989e634a2a7e726f24df622bc933d81cf8c45a7`  
		Last Modified: Tue, 21 Dec 2021 02:10:54 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd626acdd610cc57988f501ff79961f1428c576461bebd4231e6ea26986e247c`  
		Last Modified: Tue, 21 Dec 2021 02:10:54 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c823a8f47edfaf32b423082634aea86cdb7addaf551842be131974000268d72f`  
		Last Modified: Tue, 21 Dec 2021 02:10:54 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920494c25accb2e7113ebc8561d68c1b875ce9ea97b254e7f0b1859d0c42fb85`  
		Last Modified: Tue, 21 Dec 2021 02:10:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:c4f98f6c041d1a644f87f94d4ced314735a53c1e0c8f2de992d1fbffddffa7dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75231372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d86dc6b9ce7bf172eb8c3368116868a18d3a8be8d321e3ecb2340618a5c73e70`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:46:04 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 02 Dec 2021 17:46:05 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 02 Dec 2021 17:46:13 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 17:46:17 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 02 Dec 2021 17:46:18 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 02 Dec 2021 17:46:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 17:46:26 GMT
ENV COUCHDB_VERSION=3.2.0
# Thu, 02 Dec 2021 17:46:27 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 02 Dec 2021 17:46:45 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 02 Dec 2021 17:46:46 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 02 Dec 2021 17:46:47 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 02 Dec 2021 17:46:48 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Thu, 02 Dec 2021 17:46:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 02 Dec 2021 17:46:49 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 02 Dec 2021 17:46:50 GMT
VOLUME [/opt/couchdb/data]
# Thu, 02 Dec 2021 17:46:51 GMT
EXPOSE 4369 5984 9100
# Thu, 02 Dec 2021 17:46:52 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5791b8b3b4e5d779c522c8017cee4a5f7c64f62d1208f4d56d084e1d27362c98`  
		Last Modified: Thu, 02 Dec 2021 17:48:32 GMT  
		Size: 3.3 KB (3321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba826eb9f904f9937112e4e7500b42b85d35917d8458e9127896ac660ca0ffa5`  
		Last Modified: Thu, 02 Dec 2021 17:48:33 GMT  
		Size: 6.5 MB (6549971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d876e68b2d02a750e6cedd22e42c92932d962bdd0b252c5c0f3019749066899b`  
		Last Modified: Thu, 02 Dec 2021 17:48:30 GMT  
		Size: 951.2 KB (951153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24f278b93ab8d00de4ac6464e2204e283e60aedfcce676149a9d2400fdca51c`  
		Last Modified: Thu, 02 Dec 2021 17:48:30 GMT  
		Size: 79.9 KB (79917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac3b2f61e998178b0a54e61bb8e0fe4126d024e34a6622640eba070494f852b`  
		Last Modified: Thu, 02 Dec 2021 17:48:29 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a68d218c1a237e1012401f3320ea8480b0a0135bd33bc344f6bc6aea0e196a`  
		Last Modified: Thu, 02 Dec 2021 17:48:33 GMT  
		Size: 41.7 MB (41720266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2716d6980e4f68c66a5d1eb51b4b8a7829b37b1eaaa0e5b19e4129a1eeaabe90`  
		Last Modified: Thu, 02 Dec 2021 17:48:27 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3176fd224bda6fbb6eb05b200170a46812b47f6c166a192178adc23fa7d8c93e`  
		Last Modified: Thu, 02 Dec 2021 17:48:27 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d25e3e16593c30e1a87464ddc82826b223969bd3648da3dfba982543686dcb`  
		Last Modified: Thu, 02 Dec 2021 17:48:27 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e92b81d67f590094639906ed6702448501b657c6ce10d2b6a6b0838b15dee6`  
		Last Modified: Thu, 02 Dec 2021 17:48:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1`

```console
$ docker pull couchdb@sha256:42f3ad83cf10c800813f14665367773cea398b872b88609dbcd58e9322e0c1df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:2e06818b7a3fa8ae48f4e3bf7ca82db67de0d1f6bfe3c70e8a68d0d8170cfa53
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80002622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87828b0a612a59cc70d4a823c78f2a891faeb5ed9ed02814966fc51ff27a45b9`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:09:14 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Dec 2021 02:09:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Dec 2021 02:09:22 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:09:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 21 Dec 2021 02:09:27 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Dec 2021 02:09:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:09:54 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 21 Dec 2021 02:09:55 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Dec 2021 02:10:08 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Dec 2021 02:10:09 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Dec 2021 02:10:09 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 21 Dec 2021 02:10:09 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 21 Dec 2021 02:10:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Dec 2021 02:10:10 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Dec 2021 02:10:11 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Dec 2021 02:10:11 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Dec 2021 02:10:11 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430d6c754b31c32dd1a76de01ad3420033c05661c724b97d708362a8ec139d42`  
		Last Modified: Tue, 21 Dec 2021 02:10:58 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3227820103030b5232e32ba7e76de56823a61d47245d450403c0040933f6aebd`  
		Last Modified: Tue, 21 Dec 2021 02:10:58 GMT  
		Size: 6.7 MB (6691223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454611cf9dafef09164a7f64cb967a12ab5d1549d70599c56b74a2c283ae8ef1`  
		Last Modified: Tue, 21 Dec 2021 02:10:56 GMT  
		Size: 1.3 MB (1258346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5993063a8d6d688f066b9d8208c98f7d0dd3d78e7076cbc7a132ab98a975dece`  
		Last Modified: Tue, 21 Dec 2021 02:10:56 GMT  
		Size: 293.0 KB (293029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae5e24fa47c4d07d685f4da7933c29053e805916adbc1f25a32b18431a019ab`  
		Last Modified: Tue, 21 Dec 2021 02:11:18 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aed3be65c5381338c3823426cd0d147ee4e6645dda931266529c35bb7cc38e1`  
		Last Modified: Tue, 21 Dec 2021 02:11:21 GMT  
		Size: 44.6 MB (44599286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83197b74e0dd7dbea62a348f70081bcc753e1e46abaf13c5b2a2ed0db63df8dc`  
		Last Modified: Tue, 21 Dec 2021 02:11:16 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa83aca7b989869c6bb1bab2377fc32570122aaba095a35659beba6b38bf12d`  
		Last Modified: Tue, 21 Dec 2021 02:11:16 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49a58d05524c9278149f90a1238c117f9169d6db7ff90351e62dba516890192`  
		Last Modified: Tue, 21 Dec 2021 02:11:16 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953b11a446c19d551e48a794270efad862132626a6a1e382b3245cd202fbfe7e`  
		Last Modified: Tue, 21 Dec 2021 02:11:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:089e86895becf9656e72481a9d21e84003db62fce29899ff729916d8a11c3c85
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74612410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46edae94926687ea407cbaaab05dda9a9d8fb1fd47c87f8af412e7b7b889c0f0`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:46:04 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 02 Dec 2021 17:46:05 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 02 Dec 2021 17:46:13 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 17:46:17 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 02 Dec 2021 17:46:18 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 02 Dec 2021 17:46:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 17:47:05 GMT
ENV COUCHDB_VERSION=3.1.2
# Thu, 02 Dec 2021 17:47:05 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 02 Dec 2021 17:47:22 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 02 Dec 2021 17:47:23 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 02 Dec 2021 17:47:24 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 02 Dec 2021 17:47:25 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Thu, 02 Dec 2021 17:47:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 02 Dec 2021 17:47:26 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 02 Dec 2021 17:47:27 GMT
VOLUME [/opt/couchdb/data]
# Thu, 02 Dec 2021 17:47:28 GMT
EXPOSE 4369 5984 9100
# Thu, 02 Dec 2021 17:47:29 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5791b8b3b4e5d779c522c8017cee4a5f7c64f62d1208f4d56d084e1d27362c98`  
		Last Modified: Thu, 02 Dec 2021 17:48:32 GMT  
		Size: 3.3 KB (3321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba826eb9f904f9937112e4e7500b42b85d35917d8458e9127896ac660ca0ffa5`  
		Last Modified: Thu, 02 Dec 2021 17:48:33 GMT  
		Size: 6.5 MB (6549971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d876e68b2d02a750e6cedd22e42c92932d962bdd0b252c5c0f3019749066899b`  
		Last Modified: Thu, 02 Dec 2021 17:48:30 GMT  
		Size: 951.2 KB (951153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24f278b93ab8d00de4ac6464e2204e283e60aedfcce676149a9d2400fdca51c`  
		Last Modified: Thu, 02 Dec 2021 17:48:30 GMT  
		Size: 79.9 KB (79917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ac196808071a5dd615704005eb1eefb4e97ac383b08360d62aefbb9f587c78c`  
		Last Modified: Thu, 02 Dec 2021 17:48:53 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4d603c1d1929f5509fac2f61dd21c2fd25408b38a61c81735b3a7acbc210f9`  
		Last Modified: Thu, 02 Dec 2021 17:48:56 GMT  
		Size: 41.1 MB (41101310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12d4e71c3e2dc457947adc5490f6d9ad5ffcdb005d59c34cf77c7cd5a5bf577`  
		Last Modified: Thu, 02 Dec 2021 17:48:51 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73704288d866fac4f92b2e3c6e2506b96544c80cfa59996a6048e4e6f6cb4c7`  
		Last Modified: Thu, 02 Dec 2021 17:48:51 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5e60e5f5ef0ef59e1eec9a235544dc817bcd481b360bc83f3f9ff518c727df`  
		Last Modified: Thu, 02 Dec 2021 17:48:51 GMT  
		Size: 2.1 KB (2055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6793806d8196ff92b34438e18cb3ef9df49a72accd43d25e1415ecd023311c`  
		Last Modified: Thu, 02 Dec 2021 17:48:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1.2`

```console
$ docker pull couchdb@sha256:42f3ad83cf10c800813f14665367773cea398b872b88609dbcd58e9322e0c1df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1.2` - linux; amd64

```console
$ docker pull couchdb@sha256:2e06818b7a3fa8ae48f4e3bf7ca82db67de0d1f6bfe3c70e8a68d0d8170cfa53
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80002622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87828b0a612a59cc70d4a823c78f2a891faeb5ed9ed02814966fc51ff27a45b9`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:09:14 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Dec 2021 02:09:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Dec 2021 02:09:22 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:09:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 21 Dec 2021 02:09:27 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Dec 2021 02:09:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:09:54 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 21 Dec 2021 02:09:55 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Dec 2021 02:10:08 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Dec 2021 02:10:09 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Dec 2021 02:10:09 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 21 Dec 2021 02:10:09 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 21 Dec 2021 02:10:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Dec 2021 02:10:10 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Dec 2021 02:10:11 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Dec 2021 02:10:11 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Dec 2021 02:10:11 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430d6c754b31c32dd1a76de01ad3420033c05661c724b97d708362a8ec139d42`  
		Last Modified: Tue, 21 Dec 2021 02:10:58 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3227820103030b5232e32ba7e76de56823a61d47245d450403c0040933f6aebd`  
		Last Modified: Tue, 21 Dec 2021 02:10:58 GMT  
		Size: 6.7 MB (6691223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454611cf9dafef09164a7f64cb967a12ab5d1549d70599c56b74a2c283ae8ef1`  
		Last Modified: Tue, 21 Dec 2021 02:10:56 GMT  
		Size: 1.3 MB (1258346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5993063a8d6d688f066b9d8208c98f7d0dd3d78e7076cbc7a132ab98a975dece`  
		Last Modified: Tue, 21 Dec 2021 02:10:56 GMT  
		Size: 293.0 KB (293029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae5e24fa47c4d07d685f4da7933c29053e805916adbc1f25a32b18431a019ab`  
		Last Modified: Tue, 21 Dec 2021 02:11:18 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aed3be65c5381338c3823426cd0d147ee4e6645dda931266529c35bb7cc38e1`  
		Last Modified: Tue, 21 Dec 2021 02:11:21 GMT  
		Size: 44.6 MB (44599286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83197b74e0dd7dbea62a348f70081bcc753e1e46abaf13c5b2a2ed0db63df8dc`  
		Last Modified: Tue, 21 Dec 2021 02:11:16 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa83aca7b989869c6bb1bab2377fc32570122aaba095a35659beba6b38bf12d`  
		Last Modified: Tue, 21 Dec 2021 02:11:16 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49a58d05524c9278149f90a1238c117f9169d6db7ff90351e62dba516890192`  
		Last Modified: Tue, 21 Dec 2021 02:11:16 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953b11a446c19d551e48a794270efad862132626a6a1e382b3245cd202fbfe7e`  
		Last Modified: Tue, 21 Dec 2021 02:11:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:089e86895becf9656e72481a9d21e84003db62fce29899ff729916d8a11c3c85
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74612410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46edae94926687ea407cbaaab05dda9a9d8fb1fd47c87f8af412e7b7b889c0f0`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:46:04 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 02 Dec 2021 17:46:05 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 02 Dec 2021 17:46:13 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 17:46:17 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 02 Dec 2021 17:46:18 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 02 Dec 2021 17:46:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 17:47:05 GMT
ENV COUCHDB_VERSION=3.1.2
# Thu, 02 Dec 2021 17:47:05 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 02 Dec 2021 17:47:22 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 02 Dec 2021 17:47:23 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 02 Dec 2021 17:47:24 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 02 Dec 2021 17:47:25 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Thu, 02 Dec 2021 17:47:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 02 Dec 2021 17:47:26 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 02 Dec 2021 17:47:27 GMT
VOLUME [/opt/couchdb/data]
# Thu, 02 Dec 2021 17:47:28 GMT
EXPOSE 4369 5984 9100
# Thu, 02 Dec 2021 17:47:29 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5791b8b3b4e5d779c522c8017cee4a5f7c64f62d1208f4d56d084e1d27362c98`  
		Last Modified: Thu, 02 Dec 2021 17:48:32 GMT  
		Size: 3.3 KB (3321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba826eb9f904f9937112e4e7500b42b85d35917d8458e9127896ac660ca0ffa5`  
		Last Modified: Thu, 02 Dec 2021 17:48:33 GMT  
		Size: 6.5 MB (6549971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d876e68b2d02a750e6cedd22e42c92932d962bdd0b252c5c0f3019749066899b`  
		Last Modified: Thu, 02 Dec 2021 17:48:30 GMT  
		Size: 951.2 KB (951153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24f278b93ab8d00de4ac6464e2204e283e60aedfcce676149a9d2400fdca51c`  
		Last Modified: Thu, 02 Dec 2021 17:48:30 GMT  
		Size: 79.9 KB (79917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ac196808071a5dd615704005eb1eefb4e97ac383b08360d62aefbb9f587c78c`  
		Last Modified: Thu, 02 Dec 2021 17:48:53 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4d603c1d1929f5509fac2f61dd21c2fd25408b38a61c81735b3a7acbc210f9`  
		Last Modified: Thu, 02 Dec 2021 17:48:56 GMT  
		Size: 41.1 MB (41101310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12d4e71c3e2dc457947adc5490f6d9ad5ffcdb005d59c34cf77c7cd5a5bf577`  
		Last Modified: Thu, 02 Dec 2021 17:48:51 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73704288d866fac4f92b2e3c6e2506b96544c80cfa59996a6048e4e6f6cb4c7`  
		Last Modified: Thu, 02 Dec 2021 17:48:51 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5e60e5f5ef0ef59e1eec9a235544dc817bcd481b360bc83f3f9ff518c727df`  
		Last Modified: Thu, 02 Dec 2021 17:48:51 GMT  
		Size: 2.1 KB (2055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6793806d8196ff92b34438e18cb3ef9df49a72accd43d25e1415ecd023311c`  
		Last Modified: Thu, 02 Dec 2021 17:48:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2`

```console
$ docker pull couchdb@sha256:25c0c045a616e9a3a95adbafba306f33e622bd582ed4e988968dbc5d3e3384d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.2` - linux; amd64

```console
$ docker pull couchdb@sha256:658ef40b47f068cdbc8e8a069d18e72df1a37c38f26890e7e2543decc24246fe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.6 MB (80555365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ac41a5539f547e479507d3cefa4a9b2a7250cbf6fd0660fbeedd8fee65f9234`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:09:14 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Dec 2021 02:09:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Dec 2021 02:09:22 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:09:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 21 Dec 2021 02:09:27 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Dec 2021 02:09:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:09:33 GMT
ENV COUCHDB_VERSION=3.2.0
# Tue, 21 Dec 2021 02:09:34 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Dec 2021 02:09:48 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Dec 2021 02:09:49 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Dec 2021 02:09:49 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 21 Dec 2021 02:09:49 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 21 Dec 2021 02:09:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Dec 2021 02:09:50 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Dec 2021 02:09:51 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Dec 2021 02:09:51 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Dec 2021 02:09:51 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430d6c754b31c32dd1a76de01ad3420033c05661c724b97d708362a8ec139d42`  
		Last Modified: Tue, 21 Dec 2021 02:10:58 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3227820103030b5232e32ba7e76de56823a61d47245d450403c0040933f6aebd`  
		Last Modified: Tue, 21 Dec 2021 02:10:58 GMT  
		Size: 6.7 MB (6691223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454611cf9dafef09164a7f64cb967a12ab5d1549d70599c56b74a2c283ae8ef1`  
		Last Modified: Tue, 21 Dec 2021 02:10:56 GMT  
		Size: 1.3 MB (1258346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5993063a8d6d688f066b9d8208c98f7d0dd3d78e7076cbc7a132ab98a975dece`  
		Last Modified: Tue, 21 Dec 2021 02:10:56 GMT  
		Size: 293.0 KB (293029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e1a5cbb187a2701cb1f4f219e175d4903fc4ef19eecfbafaa89efecfe9f350`  
		Last Modified: Tue, 21 Dec 2021 02:10:56 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf5b3b5a34ef74b2afa7c1ab7adc5957d6def0d5cb372796cadbc953023f76e`  
		Last Modified: Tue, 21 Dec 2021 02:10:59 GMT  
		Size: 45.2 MB (45152027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67b48a446b521e34ad7bbbb9989e634a2a7e726f24df622bc933d81cf8c45a7`  
		Last Modified: Tue, 21 Dec 2021 02:10:54 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd626acdd610cc57988f501ff79961f1428c576461bebd4231e6ea26986e247c`  
		Last Modified: Tue, 21 Dec 2021 02:10:54 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c823a8f47edfaf32b423082634aea86cdb7addaf551842be131974000268d72f`  
		Last Modified: Tue, 21 Dec 2021 02:10:54 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920494c25accb2e7113ebc8561d68c1b875ce9ea97b254e7f0b1859d0c42fb85`  
		Last Modified: Tue, 21 Dec 2021 02:10:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:c4f98f6c041d1a644f87f94d4ced314735a53c1e0c8f2de992d1fbffddffa7dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75231372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d86dc6b9ce7bf172eb8c3368116868a18d3a8be8d321e3ecb2340618a5c73e70`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:46:04 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 02 Dec 2021 17:46:05 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 02 Dec 2021 17:46:13 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 17:46:17 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 02 Dec 2021 17:46:18 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 02 Dec 2021 17:46:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 17:46:26 GMT
ENV COUCHDB_VERSION=3.2.0
# Thu, 02 Dec 2021 17:46:27 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 02 Dec 2021 17:46:45 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 02 Dec 2021 17:46:46 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 02 Dec 2021 17:46:47 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 02 Dec 2021 17:46:48 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Thu, 02 Dec 2021 17:46:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 02 Dec 2021 17:46:49 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 02 Dec 2021 17:46:50 GMT
VOLUME [/opt/couchdb/data]
# Thu, 02 Dec 2021 17:46:51 GMT
EXPOSE 4369 5984 9100
# Thu, 02 Dec 2021 17:46:52 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5791b8b3b4e5d779c522c8017cee4a5f7c64f62d1208f4d56d084e1d27362c98`  
		Last Modified: Thu, 02 Dec 2021 17:48:32 GMT  
		Size: 3.3 KB (3321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba826eb9f904f9937112e4e7500b42b85d35917d8458e9127896ac660ca0ffa5`  
		Last Modified: Thu, 02 Dec 2021 17:48:33 GMT  
		Size: 6.5 MB (6549971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d876e68b2d02a750e6cedd22e42c92932d962bdd0b252c5c0f3019749066899b`  
		Last Modified: Thu, 02 Dec 2021 17:48:30 GMT  
		Size: 951.2 KB (951153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24f278b93ab8d00de4ac6464e2204e283e60aedfcce676149a9d2400fdca51c`  
		Last Modified: Thu, 02 Dec 2021 17:48:30 GMT  
		Size: 79.9 KB (79917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac3b2f61e998178b0a54e61bb8e0fe4126d024e34a6622640eba070494f852b`  
		Last Modified: Thu, 02 Dec 2021 17:48:29 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a68d218c1a237e1012401f3320ea8480b0a0135bd33bc344f6bc6aea0e196a`  
		Last Modified: Thu, 02 Dec 2021 17:48:33 GMT  
		Size: 41.7 MB (41720266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2716d6980e4f68c66a5d1eb51b4b8a7829b37b1eaaa0e5b19e4129a1eeaabe90`  
		Last Modified: Thu, 02 Dec 2021 17:48:27 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3176fd224bda6fbb6eb05b200170a46812b47f6c166a192178adc23fa7d8c93e`  
		Last Modified: Thu, 02 Dec 2021 17:48:27 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d25e3e16593c30e1a87464ddc82826b223969bd3648da3dfba982543686dcb`  
		Last Modified: Thu, 02 Dec 2021 17:48:27 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e92b81d67f590094639906ed6702448501b657c6ce10d2b6a6b0838b15dee6`  
		Last Modified: Thu, 02 Dec 2021 17:48:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2.0`

```console
$ docker pull couchdb@sha256:25c0c045a616e9a3a95adbafba306f33e622bd582ed4e988968dbc5d3e3384d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.2.0` - linux; amd64

```console
$ docker pull couchdb@sha256:658ef40b47f068cdbc8e8a069d18e72df1a37c38f26890e7e2543decc24246fe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.6 MB (80555365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ac41a5539f547e479507d3cefa4a9b2a7250cbf6fd0660fbeedd8fee65f9234`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:09:14 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Dec 2021 02:09:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Dec 2021 02:09:22 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:09:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 21 Dec 2021 02:09:27 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Dec 2021 02:09:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:09:33 GMT
ENV COUCHDB_VERSION=3.2.0
# Tue, 21 Dec 2021 02:09:34 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Dec 2021 02:09:48 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Dec 2021 02:09:49 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Dec 2021 02:09:49 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 21 Dec 2021 02:09:49 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 21 Dec 2021 02:09:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Dec 2021 02:09:50 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Dec 2021 02:09:51 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Dec 2021 02:09:51 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Dec 2021 02:09:51 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430d6c754b31c32dd1a76de01ad3420033c05661c724b97d708362a8ec139d42`  
		Last Modified: Tue, 21 Dec 2021 02:10:58 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3227820103030b5232e32ba7e76de56823a61d47245d450403c0040933f6aebd`  
		Last Modified: Tue, 21 Dec 2021 02:10:58 GMT  
		Size: 6.7 MB (6691223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454611cf9dafef09164a7f64cb967a12ab5d1549d70599c56b74a2c283ae8ef1`  
		Last Modified: Tue, 21 Dec 2021 02:10:56 GMT  
		Size: 1.3 MB (1258346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5993063a8d6d688f066b9d8208c98f7d0dd3d78e7076cbc7a132ab98a975dece`  
		Last Modified: Tue, 21 Dec 2021 02:10:56 GMT  
		Size: 293.0 KB (293029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e1a5cbb187a2701cb1f4f219e175d4903fc4ef19eecfbafaa89efecfe9f350`  
		Last Modified: Tue, 21 Dec 2021 02:10:56 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf5b3b5a34ef74b2afa7c1ab7adc5957d6def0d5cb372796cadbc953023f76e`  
		Last Modified: Tue, 21 Dec 2021 02:10:59 GMT  
		Size: 45.2 MB (45152027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67b48a446b521e34ad7bbbb9989e634a2a7e726f24df622bc933d81cf8c45a7`  
		Last Modified: Tue, 21 Dec 2021 02:10:54 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd626acdd610cc57988f501ff79961f1428c576461bebd4231e6ea26986e247c`  
		Last Modified: Tue, 21 Dec 2021 02:10:54 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c823a8f47edfaf32b423082634aea86cdb7addaf551842be131974000268d72f`  
		Last Modified: Tue, 21 Dec 2021 02:10:54 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920494c25accb2e7113ebc8561d68c1b875ce9ea97b254e7f0b1859d0c42fb85`  
		Last Modified: Tue, 21 Dec 2021 02:10:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2.0` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:c4f98f6c041d1a644f87f94d4ced314735a53c1e0c8f2de992d1fbffddffa7dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75231372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d86dc6b9ce7bf172eb8c3368116868a18d3a8be8d321e3ecb2340618a5c73e70`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:46:04 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 02 Dec 2021 17:46:05 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 02 Dec 2021 17:46:13 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 17:46:17 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 02 Dec 2021 17:46:18 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 02 Dec 2021 17:46:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 17:46:26 GMT
ENV COUCHDB_VERSION=3.2.0
# Thu, 02 Dec 2021 17:46:27 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 02 Dec 2021 17:46:45 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 02 Dec 2021 17:46:46 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 02 Dec 2021 17:46:47 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 02 Dec 2021 17:46:48 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Thu, 02 Dec 2021 17:46:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 02 Dec 2021 17:46:49 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 02 Dec 2021 17:46:50 GMT
VOLUME [/opt/couchdb/data]
# Thu, 02 Dec 2021 17:46:51 GMT
EXPOSE 4369 5984 9100
# Thu, 02 Dec 2021 17:46:52 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5791b8b3b4e5d779c522c8017cee4a5f7c64f62d1208f4d56d084e1d27362c98`  
		Last Modified: Thu, 02 Dec 2021 17:48:32 GMT  
		Size: 3.3 KB (3321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba826eb9f904f9937112e4e7500b42b85d35917d8458e9127896ac660ca0ffa5`  
		Last Modified: Thu, 02 Dec 2021 17:48:33 GMT  
		Size: 6.5 MB (6549971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d876e68b2d02a750e6cedd22e42c92932d962bdd0b252c5c0f3019749066899b`  
		Last Modified: Thu, 02 Dec 2021 17:48:30 GMT  
		Size: 951.2 KB (951153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24f278b93ab8d00de4ac6464e2204e283e60aedfcce676149a9d2400fdca51c`  
		Last Modified: Thu, 02 Dec 2021 17:48:30 GMT  
		Size: 79.9 KB (79917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac3b2f61e998178b0a54e61bb8e0fe4126d024e34a6622640eba070494f852b`  
		Last Modified: Thu, 02 Dec 2021 17:48:29 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a68d218c1a237e1012401f3320ea8480b0a0135bd33bc344f6bc6aea0e196a`  
		Last Modified: Thu, 02 Dec 2021 17:48:33 GMT  
		Size: 41.7 MB (41720266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2716d6980e4f68c66a5d1eb51b4b8a7829b37b1eaaa0e5b19e4129a1eeaabe90`  
		Last Modified: Thu, 02 Dec 2021 17:48:27 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3176fd224bda6fbb6eb05b200170a46812b47f6c166a192178adc23fa7d8c93e`  
		Last Modified: Thu, 02 Dec 2021 17:48:27 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d25e3e16593c30e1a87464ddc82826b223969bd3648da3dfba982543686dcb`  
		Last Modified: Thu, 02 Dec 2021 17:48:27 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e92b81d67f590094639906ed6702448501b657c6ce10d2b6a6b0838b15dee6`  
		Last Modified: Thu, 02 Dec 2021 17:48:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:latest`

```console
$ docker pull couchdb@sha256:25c0c045a616e9a3a95adbafba306f33e622bd582ed4e988968dbc5d3e3384d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:658ef40b47f068cdbc8e8a069d18e72df1a37c38f26890e7e2543decc24246fe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.6 MB (80555365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ac41a5539f547e479507d3cefa4a9b2a7250cbf6fd0660fbeedd8fee65f9234`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:09:14 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Dec 2021 02:09:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Dec 2021 02:09:22 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:09:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 21 Dec 2021 02:09:27 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Dec 2021 02:09:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:09:33 GMT
ENV COUCHDB_VERSION=3.2.0
# Tue, 21 Dec 2021 02:09:34 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Dec 2021 02:09:48 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Dec 2021 02:09:49 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Dec 2021 02:09:49 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 21 Dec 2021 02:09:49 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 21 Dec 2021 02:09:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Dec 2021 02:09:50 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Dec 2021 02:09:51 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Dec 2021 02:09:51 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Dec 2021 02:09:51 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430d6c754b31c32dd1a76de01ad3420033c05661c724b97d708362a8ec139d42`  
		Last Modified: Tue, 21 Dec 2021 02:10:58 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3227820103030b5232e32ba7e76de56823a61d47245d450403c0040933f6aebd`  
		Last Modified: Tue, 21 Dec 2021 02:10:58 GMT  
		Size: 6.7 MB (6691223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454611cf9dafef09164a7f64cb967a12ab5d1549d70599c56b74a2c283ae8ef1`  
		Last Modified: Tue, 21 Dec 2021 02:10:56 GMT  
		Size: 1.3 MB (1258346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5993063a8d6d688f066b9d8208c98f7d0dd3d78e7076cbc7a132ab98a975dece`  
		Last Modified: Tue, 21 Dec 2021 02:10:56 GMT  
		Size: 293.0 KB (293029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e1a5cbb187a2701cb1f4f219e175d4903fc4ef19eecfbafaa89efecfe9f350`  
		Last Modified: Tue, 21 Dec 2021 02:10:56 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf5b3b5a34ef74b2afa7c1ab7adc5957d6def0d5cb372796cadbc953023f76e`  
		Last Modified: Tue, 21 Dec 2021 02:10:59 GMT  
		Size: 45.2 MB (45152027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67b48a446b521e34ad7bbbb9989e634a2a7e726f24df622bc933d81cf8c45a7`  
		Last Modified: Tue, 21 Dec 2021 02:10:54 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd626acdd610cc57988f501ff79961f1428c576461bebd4231e6ea26986e247c`  
		Last Modified: Tue, 21 Dec 2021 02:10:54 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c823a8f47edfaf32b423082634aea86cdb7addaf551842be131974000268d72f`  
		Last Modified: Tue, 21 Dec 2021 02:10:54 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920494c25accb2e7113ebc8561d68c1b875ce9ea97b254e7f0b1859d0c42fb85`  
		Last Modified: Tue, 21 Dec 2021 02:10:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:c4f98f6c041d1a644f87f94d4ced314735a53c1e0c8f2de992d1fbffddffa7dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75231372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d86dc6b9ce7bf172eb8c3368116868a18d3a8be8d321e3ecb2340618a5c73e70`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:34 GMT
ADD file:83d9e760a84be2bd8754e31e33b3f782b44f6e7b7e02c156f519715c88c40615 in / 
# Thu, 02 Dec 2021 08:08:35 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 17:46:04 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 02 Dec 2021 17:46:05 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 02 Dec 2021 17:46:13 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 17:46:17 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 02 Dec 2021 17:46:18 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 02 Dec 2021 17:46:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 17:46:26 GMT
ENV COUCHDB_VERSION=3.2.0
# Thu, 02 Dec 2021 17:46:27 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 02 Dec 2021 17:46:45 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 02 Dec 2021 17:46:46 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 02 Dec 2021 17:46:47 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 02 Dec 2021 17:46:48 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Thu, 02 Dec 2021 17:46:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 02 Dec 2021 17:46:49 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 02 Dec 2021 17:46:50 GMT
VOLUME [/opt/couchdb/data]
# Thu, 02 Dec 2021 17:46:51 GMT
EXPOSE 4369 5984 9100
# Thu, 02 Dec 2021 17:46:52 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:2a37a2e6ba8cbf21e3950cf7b2455f0af054667b6a35719fb2bd6070973bfa76`  
		Last Modified: Thu, 02 Dec 2021 08:41:37 GMT  
		Size: 25.9 MB (25923144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5791b8b3b4e5d779c522c8017cee4a5f7c64f62d1208f4d56d084e1d27362c98`  
		Last Modified: Thu, 02 Dec 2021 17:48:32 GMT  
		Size: 3.3 KB (3321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba826eb9f904f9937112e4e7500b42b85d35917d8458e9127896ac660ca0ffa5`  
		Last Modified: Thu, 02 Dec 2021 17:48:33 GMT  
		Size: 6.5 MB (6549971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d876e68b2d02a750e6cedd22e42c92932d962bdd0b252c5c0f3019749066899b`  
		Last Modified: Thu, 02 Dec 2021 17:48:30 GMT  
		Size: 951.2 KB (951153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24f278b93ab8d00de4ac6464e2204e283e60aedfcce676149a9d2400fdca51c`  
		Last Modified: Thu, 02 Dec 2021 17:48:30 GMT  
		Size: 79.9 KB (79917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac3b2f61e998178b0a54e61bb8e0fe4126d024e34a6622640eba070494f852b`  
		Last Modified: Thu, 02 Dec 2021 17:48:29 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a68d218c1a237e1012401f3320ea8480b0a0135bd33bc344f6bc6aea0e196a`  
		Last Modified: Thu, 02 Dec 2021 17:48:33 GMT  
		Size: 41.7 MB (41720266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2716d6980e4f68c66a5d1eb51b4b8a7829b37b1eaaa0e5b19e4129a1eeaabe90`  
		Last Modified: Thu, 02 Dec 2021 17:48:27 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3176fd224bda6fbb6eb05b200170a46812b47f6c166a192178adc23fa7d8c93e`  
		Last Modified: Thu, 02 Dec 2021 17:48:27 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d25e3e16593c30e1a87464ddc82826b223969bd3648da3dfba982543686dcb`  
		Last Modified: Thu, 02 Dec 2021 17:48:27 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e92b81d67f590094639906ed6702448501b657c6ce10d2b6a6b0838b15dee6`  
		Last Modified: Thu, 02 Dec 2021 17:48:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
