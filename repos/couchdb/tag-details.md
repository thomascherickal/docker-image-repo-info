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
$ docker pull couchdb@sha256:8046799d478ea8bcb70567b31797217e979c9dd061e9117255babc9414d9e5e7
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
$ docker pull couchdb@sha256:a3d10d9247c7752e14634448ace11aa91234bda900dadd8fc2e3e4ba14692cb6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72522958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:154bfb5a3405c061d262397e60860c9e021f37a6b315cb6364d78e2bec56190c`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:48 GMT
ADD file:9810440ab841e71bd153282c21cfcd46d3f40bd5099e60c332e05bf066e390ac in / 
# Tue, 21 Dec 2021 01:42:49 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:44:40 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Dec 2021 10:44:41 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Dec 2021 10:44:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:44:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 21 Dec 2021 10:44:54 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Dec 2021 10:45:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:46:18 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 21 Dec 2021 10:46:18 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Dec 2021 10:46:38 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Dec 2021 10:46:39 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Dec 2021 10:46:40 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 21 Dec 2021 10:46:41 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 21 Dec 2021 10:46:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Dec 2021 10:46:42 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Dec 2021 10:46:43 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Dec 2021 10:46:44 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Dec 2021 10:46:45 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:753408153c81560bc4244b14524c404cbf483c8afa8ac924272545400536a9d8`  
		Last Modified: Tue, 21 Dec 2021 01:49:44 GMT  
		Size: 25.9 MB (25923149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589f1cb358d3e3a123049341ce44cdc00d6c6484a66c1169425711e3d4e5ef61`  
		Last Modified: Tue, 21 Dec 2021 10:47:20 GMT  
		Size: 3.3 KB (3322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519ca2948856ed69aa492a4294b0510bcc03616eceac737dd2fe13ddbdad889d`  
		Last Modified: Tue, 21 Dec 2021 10:47:19 GMT  
		Size: 6.5 MB (6549891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41232c99e6d3b4632a28126c15a9405dac5ec12ef1c3e71b47f7e455ed8bef7`  
		Last Modified: Tue, 21 Dec 2021 10:47:18 GMT  
		Size: 951.2 KB (951161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8413befe0746257456c09468b422890a186a8cf1a2868f008b8d56de24a7d815`  
		Last Modified: Tue, 21 Dec 2021 10:47:18 GMT  
		Size: 79.9 KB (79896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a6d094941ef8631acb8e5ee45fec2ede42e4bd34bd72487780d761a035d1c1`  
		Last Modified: Tue, 21 Dec 2021 10:48:07 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078d27380f72f29462473356c0b6ff2dd60b35664262a9837de59e80206d3ae4`  
		Last Modified: Tue, 21 Dec 2021 10:48:10 GMT  
		Size: 39.0 MB (39011935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9872b9e69dc520883ed7cf3d38d40f9562fdc9f921724a31f44513c172574bd0`  
		Last Modified: Tue, 21 Dec 2021 10:48:05 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60556cedd8f948beaed3ce12465b77400d7837624f2fb1d442631e6762cb356a`  
		Last Modified: Tue, 21 Dec 2021 10:48:05 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddc0d47de849ca62541cfade6c36dce399d20b240dda62ac32e7cc9362226ca`  
		Last Modified: Tue, 21 Dec 2021 10:48:05 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341aab2940e95718a85811ebfa73c3fb3c39b91aecf6e2e1e42f34f657e27e7e`  
		Last Modified: Tue, 21 Dec 2021 10:48:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3`

```console
$ docker pull couchdb@sha256:8046799d478ea8bcb70567b31797217e979c9dd061e9117255babc9414d9e5e7
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
$ docker pull couchdb@sha256:a3d10d9247c7752e14634448ace11aa91234bda900dadd8fc2e3e4ba14692cb6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72522958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:154bfb5a3405c061d262397e60860c9e021f37a6b315cb6364d78e2bec56190c`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:48 GMT
ADD file:9810440ab841e71bd153282c21cfcd46d3f40bd5099e60c332e05bf066e390ac in / 
# Tue, 21 Dec 2021 01:42:49 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:44:40 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Dec 2021 10:44:41 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Dec 2021 10:44:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:44:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 21 Dec 2021 10:44:54 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Dec 2021 10:45:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:46:18 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 21 Dec 2021 10:46:18 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Dec 2021 10:46:38 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Dec 2021 10:46:39 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Dec 2021 10:46:40 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 21 Dec 2021 10:46:41 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 21 Dec 2021 10:46:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Dec 2021 10:46:42 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Dec 2021 10:46:43 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Dec 2021 10:46:44 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Dec 2021 10:46:45 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:753408153c81560bc4244b14524c404cbf483c8afa8ac924272545400536a9d8`  
		Last Modified: Tue, 21 Dec 2021 01:49:44 GMT  
		Size: 25.9 MB (25923149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589f1cb358d3e3a123049341ce44cdc00d6c6484a66c1169425711e3d4e5ef61`  
		Last Modified: Tue, 21 Dec 2021 10:47:20 GMT  
		Size: 3.3 KB (3322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519ca2948856ed69aa492a4294b0510bcc03616eceac737dd2fe13ddbdad889d`  
		Last Modified: Tue, 21 Dec 2021 10:47:19 GMT  
		Size: 6.5 MB (6549891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41232c99e6d3b4632a28126c15a9405dac5ec12ef1c3e71b47f7e455ed8bef7`  
		Last Modified: Tue, 21 Dec 2021 10:47:18 GMT  
		Size: 951.2 KB (951161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8413befe0746257456c09468b422890a186a8cf1a2868f008b8d56de24a7d815`  
		Last Modified: Tue, 21 Dec 2021 10:47:18 GMT  
		Size: 79.9 KB (79896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a6d094941ef8631acb8e5ee45fec2ede42e4bd34bd72487780d761a035d1c1`  
		Last Modified: Tue, 21 Dec 2021 10:48:07 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078d27380f72f29462473356c0b6ff2dd60b35664262a9837de59e80206d3ae4`  
		Last Modified: Tue, 21 Dec 2021 10:48:10 GMT  
		Size: 39.0 MB (39011935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9872b9e69dc520883ed7cf3d38d40f9562fdc9f921724a31f44513c172574bd0`  
		Last Modified: Tue, 21 Dec 2021 10:48:05 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60556cedd8f948beaed3ce12465b77400d7837624f2fb1d442631e6762cb356a`  
		Last Modified: Tue, 21 Dec 2021 10:48:05 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddc0d47de849ca62541cfade6c36dce399d20b240dda62ac32e7cc9362226ca`  
		Last Modified: Tue, 21 Dec 2021 10:48:05 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341aab2940e95718a85811ebfa73c3fb3c39b91aecf6e2e1e42f34f657e27e7e`  
		Last Modified: Tue, 21 Dec 2021 10:48:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3.1`

```console
$ docker pull couchdb@sha256:8046799d478ea8bcb70567b31797217e979c9dd061e9117255babc9414d9e5e7
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
$ docker pull couchdb@sha256:a3d10d9247c7752e14634448ace11aa91234bda900dadd8fc2e3e4ba14692cb6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72522958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:154bfb5a3405c061d262397e60860c9e021f37a6b315cb6364d78e2bec56190c`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:48 GMT
ADD file:9810440ab841e71bd153282c21cfcd46d3f40bd5099e60c332e05bf066e390ac in / 
# Tue, 21 Dec 2021 01:42:49 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:44:40 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Dec 2021 10:44:41 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Dec 2021 10:44:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:44:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 21 Dec 2021 10:44:54 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Dec 2021 10:45:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:46:18 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 21 Dec 2021 10:46:18 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Dec 2021 10:46:38 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Dec 2021 10:46:39 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Dec 2021 10:46:40 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 21 Dec 2021 10:46:41 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 21 Dec 2021 10:46:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Dec 2021 10:46:42 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Dec 2021 10:46:43 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Dec 2021 10:46:44 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Dec 2021 10:46:45 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:753408153c81560bc4244b14524c404cbf483c8afa8ac924272545400536a9d8`  
		Last Modified: Tue, 21 Dec 2021 01:49:44 GMT  
		Size: 25.9 MB (25923149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589f1cb358d3e3a123049341ce44cdc00d6c6484a66c1169425711e3d4e5ef61`  
		Last Modified: Tue, 21 Dec 2021 10:47:20 GMT  
		Size: 3.3 KB (3322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519ca2948856ed69aa492a4294b0510bcc03616eceac737dd2fe13ddbdad889d`  
		Last Modified: Tue, 21 Dec 2021 10:47:19 GMT  
		Size: 6.5 MB (6549891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41232c99e6d3b4632a28126c15a9405dac5ec12ef1c3e71b47f7e455ed8bef7`  
		Last Modified: Tue, 21 Dec 2021 10:47:18 GMT  
		Size: 951.2 KB (951161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8413befe0746257456c09468b422890a186a8cf1a2868f008b8d56de24a7d815`  
		Last Modified: Tue, 21 Dec 2021 10:47:18 GMT  
		Size: 79.9 KB (79896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a6d094941ef8631acb8e5ee45fec2ede42e4bd34bd72487780d761a035d1c1`  
		Last Modified: Tue, 21 Dec 2021 10:48:07 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078d27380f72f29462473356c0b6ff2dd60b35664262a9837de59e80206d3ae4`  
		Last Modified: Tue, 21 Dec 2021 10:48:10 GMT  
		Size: 39.0 MB (39011935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9872b9e69dc520883ed7cf3d38d40f9562fdc9f921724a31f44513c172574bd0`  
		Last Modified: Tue, 21 Dec 2021 10:48:05 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60556cedd8f948beaed3ce12465b77400d7837624f2fb1d442631e6762cb356a`  
		Last Modified: Tue, 21 Dec 2021 10:48:05 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddc0d47de849ca62541cfade6c36dce399d20b240dda62ac32e7cc9362226ca`  
		Last Modified: Tue, 21 Dec 2021 10:48:05 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341aab2940e95718a85811ebfa73c3fb3c39b91aecf6e2e1e42f34f657e27e7e`  
		Last Modified: Tue, 21 Dec 2021 10:48:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3`

```console
$ docker pull couchdb@sha256:721df2c2a5da1b477e3976f3f10c3d1f015ba3c0101fb49efdcb7062b695a32c
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
$ docker pull couchdb@sha256:869f47e225975cb48c3eb1031664774c529080c0d6f9a71f3fcb404a698d4a6d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75231146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80c4d8555edeeddd256bfc90afd27fe69187e5be6505a8bfb08ea1bbe088a957`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:48 GMT
ADD file:9810440ab841e71bd153282c21cfcd46d3f40bd5099e60c332e05bf066e390ac in / 
# Tue, 21 Dec 2021 01:42:49 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:44:40 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Dec 2021 10:44:41 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Dec 2021 10:44:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:44:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 21 Dec 2021 10:44:54 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Dec 2021 10:45:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:45:02 GMT
ENV COUCHDB_VERSION=3.2.0
# Tue, 21 Dec 2021 10:45:03 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Dec 2021 10:45:21 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Dec 2021 10:45:22 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Dec 2021 10:45:23 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 21 Dec 2021 10:45:24 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 21 Dec 2021 10:45:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Dec 2021 10:45:25 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Dec 2021 10:45:26 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Dec 2021 10:45:27 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Dec 2021 10:45:28 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:753408153c81560bc4244b14524c404cbf483c8afa8ac924272545400536a9d8`  
		Last Modified: Tue, 21 Dec 2021 01:49:44 GMT  
		Size: 25.9 MB (25923149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589f1cb358d3e3a123049341ce44cdc00d6c6484a66c1169425711e3d4e5ef61`  
		Last Modified: Tue, 21 Dec 2021 10:47:20 GMT  
		Size: 3.3 KB (3322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519ca2948856ed69aa492a4294b0510bcc03616eceac737dd2fe13ddbdad889d`  
		Last Modified: Tue, 21 Dec 2021 10:47:19 GMT  
		Size: 6.5 MB (6549891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41232c99e6d3b4632a28126c15a9405dac5ec12ef1c3e71b47f7e455ed8bef7`  
		Last Modified: Tue, 21 Dec 2021 10:47:18 GMT  
		Size: 951.2 KB (951161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8413befe0746257456c09468b422890a186a8cf1a2868f008b8d56de24a7d815`  
		Last Modified: Tue, 21 Dec 2021 10:47:18 GMT  
		Size: 79.9 KB (79896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881e0db5b966260ec8900a1ed3580e995a95c4dc5080c6211050dfc9860f3d1c`  
		Last Modified: Tue, 21 Dec 2021 10:47:17 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025e09f93807f170da42d5be112a4f23ef5ac902b0beaa78c11c915805f0b1a9`  
		Last Modified: Tue, 21 Dec 2021 10:47:20 GMT  
		Size: 41.7 MB (41720123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde0b26399669e31d67674d81e379abf8ef313266494a9d475260b6a335625f3`  
		Last Modified: Tue, 21 Dec 2021 10:47:15 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402ec3e16c1dc98710c921b298b4ca7ca394a2dc0ca520cdd1c43ff281cc4957`  
		Last Modified: Tue, 21 Dec 2021 10:47:15 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc3cb611309b8ca0f28d85184acf44654e779f0bdddbc37dad0c41ad52adf34`  
		Last Modified: Tue, 21 Dec 2021 10:47:16 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3fdf7e2f3ce2dfd9e73da1db5bc4e20a67e2b21d05258e4ef11b690129988fa`  
		Last Modified: Tue, 21 Dec 2021 10:47:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1`

```console
$ docker pull couchdb@sha256:f394b5efef2c7847717f1b19e8dfad21e7ee8549cd3a1c80bb4754a3b0b0c8e5
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
$ docker pull couchdb@sha256:f988ebabdab088013e6ed91095e50319a6fd01c2eb1b7700ef91b01b7c699808
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74612501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6219f3f786f9d20c8771d747f90937559c8dbfe4247d20f513ec8bff4aca885`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:48 GMT
ADD file:9810440ab841e71bd153282c21cfcd46d3f40bd5099e60c332e05bf066e390ac in / 
# Tue, 21 Dec 2021 01:42:49 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:44:40 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Dec 2021 10:44:41 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Dec 2021 10:44:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:44:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 21 Dec 2021 10:44:54 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Dec 2021 10:45:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:45:41 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 21 Dec 2021 10:45:42 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Dec 2021 10:46:02 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Dec 2021 10:46:03 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Dec 2021 10:46:04 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 21 Dec 2021 10:46:05 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 21 Dec 2021 10:46:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Dec 2021 10:46:06 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Dec 2021 10:46:07 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Dec 2021 10:46:08 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Dec 2021 10:46:09 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:753408153c81560bc4244b14524c404cbf483c8afa8ac924272545400536a9d8`  
		Last Modified: Tue, 21 Dec 2021 01:49:44 GMT  
		Size: 25.9 MB (25923149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589f1cb358d3e3a123049341ce44cdc00d6c6484a66c1169425711e3d4e5ef61`  
		Last Modified: Tue, 21 Dec 2021 10:47:20 GMT  
		Size: 3.3 KB (3322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519ca2948856ed69aa492a4294b0510bcc03616eceac737dd2fe13ddbdad889d`  
		Last Modified: Tue, 21 Dec 2021 10:47:19 GMT  
		Size: 6.5 MB (6549891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41232c99e6d3b4632a28126c15a9405dac5ec12ef1c3e71b47f7e455ed8bef7`  
		Last Modified: Tue, 21 Dec 2021 10:47:18 GMT  
		Size: 951.2 KB (951161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8413befe0746257456c09468b422890a186a8cf1a2868f008b8d56de24a7d815`  
		Last Modified: Tue, 21 Dec 2021 10:47:18 GMT  
		Size: 79.9 KB (79896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e08a629b29d021aa7226c26fefa17d5eace42fdaa6b6d956df056bf48eaf77`  
		Last Modified: Tue, 21 Dec 2021 10:47:51 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c222a0edd71310ef39bdb1dc12359794f490d9a23be86329fddf10d79845daf`  
		Last Modified: Tue, 21 Dec 2021 10:47:54 GMT  
		Size: 41.1 MB (41101483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162b8bee104f638573a4cd9b8c16469ec14e1f09cf944d0b7d43ac4651a579ce`  
		Last Modified: Tue, 21 Dec 2021 10:47:49 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4987da0c177b4aa3945ef21699e453608ae10613a07ecb18f25c710857b61b`  
		Last Modified: Tue, 21 Dec 2021 10:47:49 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5d9540ea59c3e148a1b9a953f5eb3f9258a504165f8704eaf6e70b3a0f0acb`  
		Last Modified: Tue, 21 Dec 2021 10:47:49 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f657d8e28bae029f16c56ff6924e32764aba83819311f13114c37ec665f63f`  
		Last Modified: Tue, 21 Dec 2021 10:47:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1.2`

```console
$ docker pull couchdb@sha256:f394b5efef2c7847717f1b19e8dfad21e7ee8549cd3a1c80bb4754a3b0b0c8e5
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
$ docker pull couchdb@sha256:f988ebabdab088013e6ed91095e50319a6fd01c2eb1b7700ef91b01b7c699808
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74612501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6219f3f786f9d20c8771d747f90937559c8dbfe4247d20f513ec8bff4aca885`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:48 GMT
ADD file:9810440ab841e71bd153282c21cfcd46d3f40bd5099e60c332e05bf066e390ac in / 
# Tue, 21 Dec 2021 01:42:49 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:44:40 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Dec 2021 10:44:41 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Dec 2021 10:44:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:44:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 21 Dec 2021 10:44:54 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Dec 2021 10:45:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:45:41 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 21 Dec 2021 10:45:42 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Dec 2021 10:46:02 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Dec 2021 10:46:03 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Dec 2021 10:46:04 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 21 Dec 2021 10:46:05 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 21 Dec 2021 10:46:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Dec 2021 10:46:06 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Dec 2021 10:46:07 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Dec 2021 10:46:08 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Dec 2021 10:46:09 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:753408153c81560bc4244b14524c404cbf483c8afa8ac924272545400536a9d8`  
		Last Modified: Tue, 21 Dec 2021 01:49:44 GMT  
		Size: 25.9 MB (25923149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589f1cb358d3e3a123049341ce44cdc00d6c6484a66c1169425711e3d4e5ef61`  
		Last Modified: Tue, 21 Dec 2021 10:47:20 GMT  
		Size: 3.3 KB (3322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519ca2948856ed69aa492a4294b0510bcc03616eceac737dd2fe13ddbdad889d`  
		Last Modified: Tue, 21 Dec 2021 10:47:19 GMT  
		Size: 6.5 MB (6549891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41232c99e6d3b4632a28126c15a9405dac5ec12ef1c3e71b47f7e455ed8bef7`  
		Last Modified: Tue, 21 Dec 2021 10:47:18 GMT  
		Size: 951.2 KB (951161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8413befe0746257456c09468b422890a186a8cf1a2868f008b8d56de24a7d815`  
		Last Modified: Tue, 21 Dec 2021 10:47:18 GMT  
		Size: 79.9 KB (79896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e08a629b29d021aa7226c26fefa17d5eace42fdaa6b6d956df056bf48eaf77`  
		Last Modified: Tue, 21 Dec 2021 10:47:51 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c222a0edd71310ef39bdb1dc12359794f490d9a23be86329fddf10d79845daf`  
		Last Modified: Tue, 21 Dec 2021 10:47:54 GMT  
		Size: 41.1 MB (41101483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162b8bee104f638573a4cd9b8c16469ec14e1f09cf944d0b7d43ac4651a579ce`  
		Last Modified: Tue, 21 Dec 2021 10:47:49 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4987da0c177b4aa3945ef21699e453608ae10613a07ecb18f25c710857b61b`  
		Last Modified: Tue, 21 Dec 2021 10:47:49 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5d9540ea59c3e148a1b9a953f5eb3f9258a504165f8704eaf6e70b3a0f0acb`  
		Last Modified: Tue, 21 Dec 2021 10:47:49 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f657d8e28bae029f16c56ff6924e32764aba83819311f13114c37ec665f63f`  
		Last Modified: Tue, 21 Dec 2021 10:47:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2`

```console
$ docker pull couchdb@sha256:721df2c2a5da1b477e3976f3f10c3d1f015ba3c0101fb49efdcb7062b695a32c
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
$ docker pull couchdb@sha256:869f47e225975cb48c3eb1031664774c529080c0d6f9a71f3fcb404a698d4a6d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75231146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80c4d8555edeeddd256bfc90afd27fe69187e5be6505a8bfb08ea1bbe088a957`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:48 GMT
ADD file:9810440ab841e71bd153282c21cfcd46d3f40bd5099e60c332e05bf066e390ac in / 
# Tue, 21 Dec 2021 01:42:49 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:44:40 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Dec 2021 10:44:41 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Dec 2021 10:44:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:44:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 21 Dec 2021 10:44:54 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Dec 2021 10:45:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:45:02 GMT
ENV COUCHDB_VERSION=3.2.0
# Tue, 21 Dec 2021 10:45:03 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Dec 2021 10:45:21 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Dec 2021 10:45:22 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Dec 2021 10:45:23 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 21 Dec 2021 10:45:24 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 21 Dec 2021 10:45:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Dec 2021 10:45:25 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Dec 2021 10:45:26 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Dec 2021 10:45:27 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Dec 2021 10:45:28 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:753408153c81560bc4244b14524c404cbf483c8afa8ac924272545400536a9d8`  
		Last Modified: Tue, 21 Dec 2021 01:49:44 GMT  
		Size: 25.9 MB (25923149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589f1cb358d3e3a123049341ce44cdc00d6c6484a66c1169425711e3d4e5ef61`  
		Last Modified: Tue, 21 Dec 2021 10:47:20 GMT  
		Size: 3.3 KB (3322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519ca2948856ed69aa492a4294b0510bcc03616eceac737dd2fe13ddbdad889d`  
		Last Modified: Tue, 21 Dec 2021 10:47:19 GMT  
		Size: 6.5 MB (6549891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41232c99e6d3b4632a28126c15a9405dac5ec12ef1c3e71b47f7e455ed8bef7`  
		Last Modified: Tue, 21 Dec 2021 10:47:18 GMT  
		Size: 951.2 KB (951161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8413befe0746257456c09468b422890a186a8cf1a2868f008b8d56de24a7d815`  
		Last Modified: Tue, 21 Dec 2021 10:47:18 GMT  
		Size: 79.9 KB (79896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881e0db5b966260ec8900a1ed3580e995a95c4dc5080c6211050dfc9860f3d1c`  
		Last Modified: Tue, 21 Dec 2021 10:47:17 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025e09f93807f170da42d5be112a4f23ef5ac902b0beaa78c11c915805f0b1a9`  
		Last Modified: Tue, 21 Dec 2021 10:47:20 GMT  
		Size: 41.7 MB (41720123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde0b26399669e31d67674d81e379abf8ef313266494a9d475260b6a335625f3`  
		Last Modified: Tue, 21 Dec 2021 10:47:15 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402ec3e16c1dc98710c921b298b4ca7ca394a2dc0ca520cdd1c43ff281cc4957`  
		Last Modified: Tue, 21 Dec 2021 10:47:15 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc3cb611309b8ca0f28d85184acf44654e779f0bdddbc37dad0c41ad52adf34`  
		Last Modified: Tue, 21 Dec 2021 10:47:16 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3fdf7e2f3ce2dfd9e73da1db5bc4e20a67e2b21d05258e4ef11b690129988fa`  
		Last Modified: Tue, 21 Dec 2021 10:47:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2.0`

```console
$ docker pull couchdb@sha256:721df2c2a5da1b477e3976f3f10c3d1f015ba3c0101fb49efdcb7062b695a32c
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
$ docker pull couchdb@sha256:869f47e225975cb48c3eb1031664774c529080c0d6f9a71f3fcb404a698d4a6d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75231146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80c4d8555edeeddd256bfc90afd27fe69187e5be6505a8bfb08ea1bbe088a957`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:48 GMT
ADD file:9810440ab841e71bd153282c21cfcd46d3f40bd5099e60c332e05bf066e390ac in / 
# Tue, 21 Dec 2021 01:42:49 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:44:40 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Dec 2021 10:44:41 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Dec 2021 10:44:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:44:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 21 Dec 2021 10:44:54 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Dec 2021 10:45:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:45:02 GMT
ENV COUCHDB_VERSION=3.2.0
# Tue, 21 Dec 2021 10:45:03 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Dec 2021 10:45:21 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Dec 2021 10:45:22 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Dec 2021 10:45:23 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 21 Dec 2021 10:45:24 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 21 Dec 2021 10:45:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Dec 2021 10:45:25 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Dec 2021 10:45:26 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Dec 2021 10:45:27 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Dec 2021 10:45:28 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:753408153c81560bc4244b14524c404cbf483c8afa8ac924272545400536a9d8`  
		Last Modified: Tue, 21 Dec 2021 01:49:44 GMT  
		Size: 25.9 MB (25923149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589f1cb358d3e3a123049341ce44cdc00d6c6484a66c1169425711e3d4e5ef61`  
		Last Modified: Tue, 21 Dec 2021 10:47:20 GMT  
		Size: 3.3 KB (3322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519ca2948856ed69aa492a4294b0510bcc03616eceac737dd2fe13ddbdad889d`  
		Last Modified: Tue, 21 Dec 2021 10:47:19 GMT  
		Size: 6.5 MB (6549891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41232c99e6d3b4632a28126c15a9405dac5ec12ef1c3e71b47f7e455ed8bef7`  
		Last Modified: Tue, 21 Dec 2021 10:47:18 GMT  
		Size: 951.2 KB (951161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8413befe0746257456c09468b422890a186a8cf1a2868f008b8d56de24a7d815`  
		Last Modified: Tue, 21 Dec 2021 10:47:18 GMT  
		Size: 79.9 KB (79896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881e0db5b966260ec8900a1ed3580e995a95c4dc5080c6211050dfc9860f3d1c`  
		Last Modified: Tue, 21 Dec 2021 10:47:17 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025e09f93807f170da42d5be112a4f23ef5ac902b0beaa78c11c915805f0b1a9`  
		Last Modified: Tue, 21 Dec 2021 10:47:20 GMT  
		Size: 41.7 MB (41720123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde0b26399669e31d67674d81e379abf8ef313266494a9d475260b6a335625f3`  
		Last Modified: Tue, 21 Dec 2021 10:47:15 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402ec3e16c1dc98710c921b298b4ca7ca394a2dc0ca520cdd1c43ff281cc4957`  
		Last Modified: Tue, 21 Dec 2021 10:47:15 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc3cb611309b8ca0f28d85184acf44654e779f0bdddbc37dad0c41ad52adf34`  
		Last Modified: Tue, 21 Dec 2021 10:47:16 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3fdf7e2f3ce2dfd9e73da1db5bc4e20a67e2b21d05258e4ef11b690129988fa`  
		Last Modified: Tue, 21 Dec 2021 10:47:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:latest`

```console
$ docker pull couchdb@sha256:721df2c2a5da1b477e3976f3f10c3d1f015ba3c0101fb49efdcb7062b695a32c
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
$ docker pull couchdb@sha256:869f47e225975cb48c3eb1031664774c529080c0d6f9a71f3fcb404a698d4a6d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75231146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80c4d8555edeeddd256bfc90afd27fe69187e5be6505a8bfb08ea1bbe088a957`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:48 GMT
ADD file:9810440ab841e71bd153282c21cfcd46d3f40bd5099e60c332e05bf066e390ac in / 
# Tue, 21 Dec 2021 01:42:49 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:44:40 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Dec 2021 10:44:41 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Dec 2021 10:44:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:44:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 21 Dec 2021 10:44:54 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Dec 2021 10:45:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:45:02 GMT
ENV COUCHDB_VERSION=3.2.0
# Tue, 21 Dec 2021 10:45:03 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Dec 2021 10:45:21 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Dec 2021 10:45:22 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Dec 2021 10:45:23 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 21 Dec 2021 10:45:24 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 21 Dec 2021 10:45:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Dec 2021 10:45:25 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Dec 2021 10:45:26 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Dec 2021 10:45:27 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Dec 2021 10:45:28 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:753408153c81560bc4244b14524c404cbf483c8afa8ac924272545400536a9d8`  
		Last Modified: Tue, 21 Dec 2021 01:49:44 GMT  
		Size: 25.9 MB (25923149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589f1cb358d3e3a123049341ce44cdc00d6c6484a66c1169425711e3d4e5ef61`  
		Last Modified: Tue, 21 Dec 2021 10:47:20 GMT  
		Size: 3.3 KB (3322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519ca2948856ed69aa492a4294b0510bcc03616eceac737dd2fe13ddbdad889d`  
		Last Modified: Tue, 21 Dec 2021 10:47:19 GMT  
		Size: 6.5 MB (6549891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41232c99e6d3b4632a28126c15a9405dac5ec12ef1c3e71b47f7e455ed8bef7`  
		Last Modified: Tue, 21 Dec 2021 10:47:18 GMT  
		Size: 951.2 KB (951161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8413befe0746257456c09468b422890a186a8cf1a2868f008b8d56de24a7d815`  
		Last Modified: Tue, 21 Dec 2021 10:47:18 GMT  
		Size: 79.9 KB (79896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881e0db5b966260ec8900a1ed3580e995a95c4dc5080c6211050dfc9860f3d1c`  
		Last Modified: Tue, 21 Dec 2021 10:47:17 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025e09f93807f170da42d5be112a4f23ef5ac902b0beaa78c11c915805f0b1a9`  
		Last Modified: Tue, 21 Dec 2021 10:47:20 GMT  
		Size: 41.7 MB (41720123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde0b26399669e31d67674d81e379abf8ef313266494a9d475260b6a335625f3`  
		Last Modified: Tue, 21 Dec 2021 10:47:15 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402ec3e16c1dc98710c921b298b4ca7ca394a2dc0ca520cdd1c43ff281cc4957`  
		Last Modified: Tue, 21 Dec 2021 10:47:15 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc3cb611309b8ca0f28d85184acf44654e779f0bdddbc37dad0c41ad52adf34`  
		Last Modified: Tue, 21 Dec 2021 10:47:16 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3fdf7e2f3ce2dfd9e73da1db5bc4e20a67e2b21d05258e4ef11b690129988fa`  
		Last Modified: Tue, 21 Dec 2021 10:47:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
