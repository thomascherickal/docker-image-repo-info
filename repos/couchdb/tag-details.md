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
$ docker pull couchdb@sha256:38b645be402d16d36b8e6c79832e0d43115b320ca9eee4d5ded31e8ee08b8ec3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2` - linux; amd64

```console
$ docker pull couchdb@sha256:2ae35f05964d869e9e0a91a4439e9bd2f221ab7a55c805f9506c508ee88300a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84537227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1ccfdedceb663e349949001f3c5f441c074ad46d5a85ae709bfe812a49391da`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Sat, 04 Feb 2023 06:52:07 GMT
ADD file:4fbe1e3712cf37c85529cc81e0d03c82085203de00d64b0d669b5996e975925a in / 
# Sat, 04 Feb 2023 06:52:07 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:17:39 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 04 Feb 2023 07:17:40 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 04 Feb 2023 07:17:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:17:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Sat, 04 Feb 2023 07:17:53 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Sat, 04 Feb 2023 07:18:00 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:18:20 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Sat, 04 Feb 2023 07:18:21 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Sat, 04 Feb 2023 07:18:40 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 04 Feb 2023 07:18:40 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Sat, 04 Feb 2023 07:18:40 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 04 Feb 2023 07:18:40 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Sat, 04 Feb 2023 07:18:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 04 Feb 2023 07:18:41 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 07:18:41 GMT
VOLUME [/opt/couchdb/data]
# Sat, 04 Feb 2023 07:18:41 GMT
EXPOSE 4369 5984 9100
# Sat, 04 Feb 2023 07:18:41 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:0cf508b37688dca559387b506062329202aaf08b48be5f55f9278b2a818ad2c9`  
		Last Modified: Sat, 04 Feb 2023 06:56:58 GMT  
		Size: 27.1 MB (27140353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2077aca956be48413850558c99aed2abe9648b6f9b9426c1135e15b89dc335ca`  
		Last Modified: Sat, 04 Feb 2023 07:19:33 GMT  
		Size: 3.4 KB (3410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7242eb760000d68511583e5224849d57fcf7a36c0e53982efab6da6ed3e8760b`  
		Last Modified: Sat, 04 Feb 2023 07:19:32 GMT  
		Size: 6.7 MB (6703784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7226bb128a799d16fae1c3ca8f2cc831f56e1a799146562752f3665a224983e6`  
		Last Modified: Sat, 04 Feb 2023 07:19:31 GMT  
		Size: 1.3 MB (1259577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bbbd4823cbeb627c5529042b3857b765bfed971236216aea4249a891e32b90`  
		Last Modified: Sat, 04 Feb 2023 07:19:31 GMT  
		Size: 294.3 KB (294296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0068092afc5d3cde2f17a4f5152fc93ef48bb689d1bc10d8bbc66d18366d992d`  
		Last Modified: Sat, 04 Feb 2023 07:19:45 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ac500017a4fd00865fee794536ce43a2dd246477176f3a4ea1eba2f15c61d3`  
		Last Modified: Sat, 04 Feb 2023 07:19:49 GMT  
		Size: 49.1 MB (49132205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9992ec80c106f5db7bebac91263b1f1a873ca656352d1b3c3e874d168fac5cef`  
		Last Modified: Sat, 04 Feb 2023 07:19:43 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:687a2cb80cde226d4d1bef9e0f91be6fd273a6e39da85339a87728a19384bde7`  
		Last Modified: Sat, 04 Feb 2023 07:19:43 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2434c1b2ac9467a54b63ce080c730ae0872966330badc4b3bd8963373b8aa5`  
		Last Modified: Sat, 04 Feb 2023 07:19:43 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf3ce40c4c2e027fcfb04f5c173fe8fe34d0fae4e1306d670143b3acd88883c2`  
		Last Modified: Sat, 04 Feb 2023 07:19:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:1cb5a3e7aef4e216952743c76b29c4eb88b1a578b5f9d6d4162e0cd95ad4ac7a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72987090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec2f7d541e92b28205022f9b17a0e8569566b08eebda8395c320798bf3e97b02`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:52 GMT
ADD file:08addf73dde8bf5ac64e0d9bdd1997ce5f406976c19da431616783c14fdb36ac in / 
# Wed, 11 Jan 2023 02:57:52 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:58:25 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 Jan 2023 03:58:25 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 Jan 2023 03:58:32 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:58:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 Jan 2023 03:58:36 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 Jan 2023 03:58:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:58:58 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 11 Jan 2023 03:58:59 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 Jan 2023 03:59:10 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 Jan 2023 03:59:10 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 11 Jan 2023 03:59:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 Jan 2023 03:59:10 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 11 Jan 2023 03:59:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 Jan 2023 03:59:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 Jan 2023 03:59:11 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 Jan 2023 03:59:11 GMT
EXPOSE 4369 5984 9100
# Wed, 11 Jan 2023 03:59:11 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:7fac02f4cd2bcf681b9e156a67009cf4609f45447818b52327d93553bfeb2965`  
		Last Modified: Wed, 11 Jan 2023 03:01:58 GMT  
		Size: 25.9 MB (25914925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49c2ee40908e629f9af8a7cab6dd0cd3837146e1417c5687ea458a09e766135`  
		Last Modified: Wed, 11 Jan 2023 04:00:06 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c510231b78ec40191b73fcf37265b834eb84575e8e9e59214e699e0fb2443f23`  
		Last Modified: Wed, 11 Jan 2023 04:00:06 GMT  
		Size: 6.6 MB (6577083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7fa713a90ae4df09d27f1f23a63a2a6e7df1f68b7907280efb3d944b8bd006`  
		Last Modified: Wed, 11 Jan 2023 04:00:05 GMT  
		Size: 1.2 MB (1164501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c83d395471dc77d8f630b48a40ec852957fdb479ef92505965c06a0297d3c0f`  
		Last Modified: Wed, 11 Jan 2023 04:00:04 GMT  
		Size: 294.1 KB (294133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1efd60f371e1e52363f272f85918ac4387fdaef6f0ac760cf27a1a129cdd7ca`  
		Last Modified: Wed, 11 Jan 2023 04:00:19 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df5cd36bc757fedbf7593edbc3ebb33dec27a4bfc364586b6194fe45a759650`  
		Last Modified: Wed, 11 Jan 2023 04:00:21 GMT  
		Size: 39.0 MB (39029409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812d9c58c0bb5f21046fa51f640b0fc96b54baf6d6fbbc87e2f9e46ccc35642d`  
		Last Modified: Wed, 11 Jan 2023 04:00:17 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6606db77f6e9fa1b66078936a6df4c5140f5803969ea6ab782d53cc730c71274`  
		Last Modified: Wed, 11 Jan 2023 04:00:17 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aee9ecdb2af156a7acbd8dbb24a7e6612149aa1d96568b0ad1ab1d637ec113b`  
		Last Modified: Wed, 11 Jan 2023 04:00:17 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e477447789dc28dd2ba5c7c08e7e4c96f84786e0cee41c144091143c345c7f`  
		Last Modified: Wed, 11 Jan 2023 04:00:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3`

```console
$ docker pull couchdb@sha256:38b645be402d16d36b8e6c79832e0d43115b320ca9eee4d5ded31e8ee08b8ec3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:2ae35f05964d869e9e0a91a4439e9bd2f221ab7a55c805f9506c508ee88300a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84537227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1ccfdedceb663e349949001f3c5f441c074ad46d5a85ae709bfe812a49391da`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Sat, 04 Feb 2023 06:52:07 GMT
ADD file:4fbe1e3712cf37c85529cc81e0d03c82085203de00d64b0d669b5996e975925a in / 
# Sat, 04 Feb 2023 06:52:07 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:17:39 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 04 Feb 2023 07:17:40 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 04 Feb 2023 07:17:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:17:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Sat, 04 Feb 2023 07:17:53 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Sat, 04 Feb 2023 07:18:00 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:18:20 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Sat, 04 Feb 2023 07:18:21 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Sat, 04 Feb 2023 07:18:40 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 04 Feb 2023 07:18:40 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Sat, 04 Feb 2023 07:18:40 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 04 Feb 2023 07:18:40 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Sat, 04 Feb 2023 07:18:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 04 Feb 2023 07:18:41 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 07:18:41 GMT
VOLUME [/opt/couchdb/data]
# Sat, 04 Feb 2023 07:18:41 GMT
EXPOSE 4369 5984 9100
# Sat, 04 Feb 2023 07:18:41 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:0cf508b37688dca559387b506062329202aaf08b48be5f55f9278b2a818ad2c9`  
		Last Modified: Sat, 04 Feb 2023 06:56:58 GMT  
		Size: 27.1 MB (27140353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2077aca956be48413850558c99aed2abe9648b6f9b9426c1135e15b89dc335ca`  
		Last Modified: Sat, 04 Feb 2023 07:19:33 GMT  
		Size: 3.4 KB (3410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7242eb760000d68511583e5224849d57fcf7a36c0e53982efab6da6ed3e8760b`  
		Last Modified: Sat, 04 Feb 2023 07:19:32 GMT  
		Size: 6.7 MB (6703784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7226bb128a799d16fae1c3ca8f2cc831f56e1a799146562752f3665a224983e6`  
		Last Modified: Sat, 04 Feb 2023 07:19:31 GMT  
		Size: 1.3 MB (1259577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bbbd4823cbeb627c5529042b3857b765bfed971236216aea4249a891e32b90`  
		Last Modified: Sat, 04 Feb 2023 07:19:31 GMT  
		Size: 294.3 KB (294296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0068092afc5d3cde2f17a4f5152fc93ef48bb689d1bc10d8bbc66d18366d992d`  
		Last Modified: Sat, 04 Feb 2023 07:19:45 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ac500017a4fd00865fee794536ce43a2dd246477176f3a4ea1eba2f15c61d3`  
		Last Modified: Sat, 04 Feb 2023 07:19:49 GMT  
		Size: 49.1 MB (49132205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9992ec80c106f5db7bebac91263b1f1a873ca656352d1b3c3e874d168fac5cef`  
		Last Modified: Sat, 04 Feb 2023 07:19:43 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:687a2cb80cde226d4d1bef9e0f91be6fd273a6e39da85339a87728a19384bde7`  
		Last Modified: Sat, 04 Feb 2023 07:19:43 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2434c1b2ac9467a54b63ce080c730ae0872966330badc4b3bd8963373b8aa5`  
		Last Modified: Sat, 04 Feb 2023 07:19:43 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf3ce40c4c2e027fcfb04f5c173fe8fe34d0fae4e1306d670143b3acd88883c2`  
		Last Modified: Sat, 04 Feb 2023 07:19:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:1cb5a3e7aef4e216952743c76b29c4eb88b1a578b5f9d6d4162e0cd95ad4ac7a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72987090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec2f7d541e92b28205022f9b17a0e8569566b08eebda8395c320798bf3e97b02`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:52 GMT
ADD file:08addf73dde8bf5ac64e0d9bdd1997ce5f406976c19da431616783c14fdb36ac in / 
# Wed, 11 Jan 2023 02:57:52 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:58:25 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 Jan 2023 03:58:25 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 Jan 2023 03:58:32 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:58:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 Jan 2023 03:58:36 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 Jan 2023 03:58:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:58:58 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 11 Jan 2023 03:58:59 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 Jan 2023 03:59:10 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 Jan 2023 03:59:10 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 11 Jan 2023 03:59:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 Jan 2023 03:59:10 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 11 Jan 2023 03:59:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 Jan 2023 03:59:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 Jan 2023 03:59:11 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 Jan 2023 03:59:11 GMT
EXPOSE 4369 5984 9100
# Wed, 11 Jan 2023 03:59:11 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:7fac02f4cd2bcf681b9e156a67009cf4609f45447818b52327d93553bfeb2965`  
		Last Modified: Wed, 11 Jan 2023 03:01:58 GMT  
		Size: 25.9 MB (25914925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49c2ee40908e629f9af8a7cab6dd0cd3837146e1417c5687ea458a09e766135`  
		Last Modified: Wed, 11 Jan 2023 04:00:06 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c510231b78ec40191b73fcf37265b834eb84575e8e9e59214e699e0fb2443f23`  
		Last Modified: Wed, 11 Jan 2023 04:00:06 GMT  
		Size: 6.6 MB (6577083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7fa713a90ae4df09d27f1f23a63a2a6e7df1f68b7907280efb3d944b8bd006`  
		Last Modified: Wed, 11 Jan 2023 04:00:05 GMT  
		Size: 1.2 MB (1164501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c83d395471dc77d8f630b48a40ec852957fdb479ef92505965c06a0297d3c0f`  
		Last Modified: Wed, 11 Jan 2023 04:00:04 GMT  
		Size: 294.1 KB (294133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1efd60f371e1e52363f272f85918ac4387fdaef6f0ac760cf27a1a129cdd7ca`  
		Last Modified: Wed, 11 Jan 2023 04:00:19 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df5cd36bc757fedbf7593edbc3ebb33dec27a4bfc364586b6194fe45a759650`  
		Last Modified: Wed, 11 Jan 2023 04:00:21 GMT  
		Size: 39.0 MB (39029409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812d9c58c0bb5f21046fa51f640b0fc96b54baf6d6fbbc87e2f9e46ccc35642d`  
		Last Modified: Wed, 11 Jan 2023 04:00:17 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6606db77f6e9fa1b66078936a6df4c5140f5803969ea6ab782d53cc730c71274`  
		Last Modified: Wed, 11 Jan 2023 04:00:17 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aee9ecdb2af156a7acbd8dbb24a7e6612149aa1d96568b0ad1ab1d637ec113b`  
		Last Modified: Wed, 11 Jan 2023 04:00:17 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e477447789dc28dd2ba5c7c08e7e4c96f84786e0cee41c144091143c345c7f`  
		Last Modified: Wed, 11 Jan 2023 04:00:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3.1`

```console
$ docker pull couchdb@sha256:38b645be402d16d36b8e6c79832e0d43115b320ca9eee4d5ded31e8ee08b8ec3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:2ae35f05964d869e9e0a91a4439e9bd2f221ab7a55c805f9506c508ee88300a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84537227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1ccfdedceb663e349949001f3c5f441c074ad46d5a85ae709bfe812a49391da`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Sat, 04 Feb 2023 06:52:07 GMT
ADD file:4fbe1e3712cf37c85529cc81e0d03c82085203de00d64b0d669b5996e975925a in / 
# Sat, 04 Feb 2023 06:52:07 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:17:39 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 04 Feb 2023 07:17:40 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 04 Feb 2023 07:17:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:17:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Sat, 04 Feb 2023 07:17:53 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Sat, 04 Feb 2023 07:18:00 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:18:20 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Sat, 04 Feb 2023 07:18:21 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Sat, 04 Feb 2023 07:18:40 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 04 Feb 2023 07:18:40 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Sat, 04 Feb 2023 07:18:40 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 04 Feb 2023 07:18:40 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Sat, 04 Feb 2023 07:18:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 04 Feb 2023 07:18:41 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 07:18:41 GMT
VOLUME [/opt/couchdb/data]
# Sat, 04 Feb 2023 07:18:41 GMT
EXPOSE 4369 5984 9100
# Sat, 04 Feb 2023 07:18:41 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:0cf508b37688dca559387b506062329202aaf08b48be5f55f9278b2a818ad2c9`  
		Last Modified: Sat, 04 Feb 2023 06:56:58 GMT  
		Size: 27.1 MB (27140353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2077aca956be48413850558c99aed2abe9648b6f9b9426c1135e15b89dc335ca`  
		Last Modified: Sat, 04 Feb 2023 07:19:33 GMT  
		Size: 3.4 KB (3410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7242eb760000d68511583e5224849d57fcf7a36c0e53982efab6da6ed3e8760b`  
		Last Modified: Sat, 04 Feb 2023 07:19:32 GMT  
		Size: 6.7 MB (6703784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7226bb128a799d16fae1c3ca8f2cc831f56e1a799146562752f3665a224983e6`  
		Last Modified: Sat, 04 Feb 2023 07:19:31 GMT  
		Size: 1.3 MB (1259577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bbbd4823cbeb627c5529042b3857b765bfed971236216aea4249a891e32b90`  
		Last Modified: Sat, 04 Feb 2023 07:19:31 GMT  
		Size: 294.3 KB (294296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0068092afc5d3cde2f17a4f5152fc93ef48bb689d1bc10d8bbc66d18366d992d`  
		Last Modified: Sat, 04 Feb 2023 07:19:45 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ac500017a4fd00865fee794536ce43a2dd246477176f3a4ea1eba2f15c61d3`  
		Last Modified: Sat, 04 Feb 2023 07:19:49 GMT  
		Size: 49.1 MB (49132205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9992ec80c106f5db7bebac91263b1f1a873ca656352d1b3c3e874d168fac5cef`  
		Last Modified: Sat, 04 Feb 2023 07:19:43 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:687a2cb80cde226d4d1bef9e0f91be6fd273a6e39da85339a87728a19384bde7`  
		Last Modified: Sat, 04 Feb 2023 07:19:43 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2434c1b2ac9467a54b63ce080c730ae0872966330badc4b3bd8963373b8aa5`  
		Last Modified: Sat, 04 Feb 2023 07:19:43 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf3ce40c4c2e027fcfb04f5c173fe8fe34d0fae4e1306d670143b3acd88883c2`  
		Last Modified: Sat, 04 Feb 2023 07:19:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:1cb5a3e7aef4e216952743c76b29c4eb88b1a578b5f9d6d4162e0cd95ad4ac7a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72987090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec2f7d541e92b28205022f9b17a0e8569566b08eebda8395c320798bf3e97b02`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:52 GMT
ADD file:08addf73dde8bf5ac64e0d9bdd1997ce5f406976c19da431616783c14fdb36ac in / 
# Wed, 11 Jan 2023 02:57:52 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:58:25 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 Jan 2023 03:58:25 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 Jan 2023 03:58:32 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:58:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 Jan 2023 03:58:36 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 Jan 2023 03:58:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:58:58 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 11 Jan 2023 03:58:59 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 Jan 2023 03:59:10 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 Jan 2023 03:59:10 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 11 Jan 2023 03:59:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 Jan 2023 03:59:10 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 11 Jan 2023 03:59:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 Jan 2023 03:59:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 Jan 2023 03:59:11 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 Jan 2023 03:59:11 GMT
EXPOSE 4369 5984 9100
# Wed, 11 Jan 2023 03:59:11 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:7fac02f4cd2bcf681b9e156a67009cf4609f45447818b52327d93553bfeb2965`  
		Last Modified: Wed, 11 Jan 2023 03:01:58 GMT  
		Size: 25.9 MB (25914925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49c2ee40908e629f9af8a7cab6dd0cd3837146e1417c5687ea458a09e766135`  
		Last Modified: Wed, 11 Jan 2023 04:00:06 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c510231b78ec40191b73fcf37265b834eb84575e8e9e59214e699e0fb2443f23`  
		Last Modified: Wed, 11 Jan 2023 04:00:06 GMT  
		Size: 6.6 MB (6577083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7fa713a90ae4df09d27f1f23a63a2a6e7df1f68b7907280efb3d944b8bd006`  
		Last Modified: Wed, 11 Jan 2023 04:00:05 GMT  
		Size: 1.2 MB (1164501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c83d395471dc77d8f630b48a40ec852957fdb479ef92505965c06a0297d3c0f`  
		Last Modified: Wed, 11 Jan 2023 04:00:04 GMT  
		Size: 294.1 KB (294133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1efd60f371e1e52363f272f85918ac4387fdaef6f0ac760cf27a1a129cdd7ca`  
		Last Modified: Wed, 11 Jan 2023 04:00:19 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df5cd36bc757fedbf7593edbc3ebb33dec27a4bfc364586b6194fe45a759650`  
		Last Modified: Wed, 11 Jan 2023 04:00:21 GMT  
		Size: 39.0 MB (39029409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812d9c58c0bb5f21046fa51f640b0fc96b54baf6d6fbbc87e2f9e46ccc35642d`  
		Last Modified: Wed, 11 Jan 2023 04:00:17 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6606db77f6e9fa1b66078936a6df4c5140f5803969ea6ab782d53cc730c71274`  
		Last Modified: Wed, 11 Jan 2023 04:00:17 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aee9ecdb2af156a7acbd8dbb24a7e6612149aa1d96568b0ad1ab1d637ec113b`  
		Last Modified: Wed, 11 Jan 2023 04:00:17 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e477447789dc28dd2ba5c7c08e7e4c96f84786e0cee41c144091143c345c7f`  
		Last Modified: Wed, 11 Jan 2023 04:00:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3`

```console
$ docker pull couchdb@sha256:6e4b8553339e200f346fdf8308a4b03d37ebe449bd96c7c3e8c1cfbcdcd7eb73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3` - linux; amd64

```console
$ docker pull couchdb@sha256:6d588a96a550033c02f45a4ce38c296cbe08f9ec14cdd4f5ca4320d8af8eb00b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91153896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1274dd1bda729da68f2c64f847a63ec5d6634042dbe09ee8fb9ee1810b35493a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:16:45 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 04 Feb 2023 07:16:46 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 04 Feb 2023 07:16:53 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:16:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Sat, 04 Feb 2023 07:16:57 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Sat, 04 Feb 2023 07:17:02 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:17:02 GMT
ENV COUCHDB_VERSION=3.3.1
# Sat, 04 Feb 2023 07:17:03 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Sat, 04 Feb 2023 07:17:15 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 04 Feb 2023 07:17:16 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 04 Feb 2023 07:17:16 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Sat, 04 Feb 2023 07:17:16 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Sat, 04 Feb 2023 07:17:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 04 Feb 2023 07:17:17 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 07:17:17 GMT
VOLUME [/opt/couchdb/data]
# Sat, 04 Feb 2023 07:17:17 GMT
EXPOSE 4369 5984 9100
# Sat, 04 Feb 2023 07:17:17 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77476cf11acd0f8081beb4a23efc99a2652c66cabe691898d51dd54b7a973967`  
		Last Modified: Sat, 04 Feb 2023 07:19:00 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e5ab1e54fdd1586bf4c41713f66e3c3dd536afdf177ab750bac5420e11af8b`  
		Last Modified: Sat, 04 Feb 2023 07:18:59 GMT  
		Size: 5.2 MB (5224338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aea5b54023137f626790058724f9349eb5aece02da7ca2ec80ff98cbb34df42`  
		Last Modified: Sat, 04 Feb 2023 07:18:59 GMT  
		Size: 1.6 MB (1553311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd561fdfab9d1eed8c99fefa269d1b26ceae1633127918de8c9bba901cd8642e`  
		Last Modified: Sat, 04 Feb 2023 07:18:59 GMT  
		Size: 295.6 KB (295625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e24cec0cc44eeb1e0f1880275166759ac0aab64b4dcca3410a217f78fe5e2a`  
		Last Modified: Sat, 04 Feb 2023 07:18:58 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3132b1e018f6c5014588752194c7ac7ffabf8e0eec4b3528ff1fce2b24a6df5`  
		Last Modified: Sat, 04 Feb 2023 07:19:02 GMT  
		Size: 52.7 MB (52676329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768bc1a4f6854d19062811091a6930b6efd398b9dd84643f35bc1ced44ea5bba`  
		Last Modified: Sat, 04 Feb 2023 07:18:57 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c6b69d74d3c03eb77600518b7afdc0ed80493cd272bfc1c2c664656cf195381`  
		Last Modified: Sat, 04 Feb 2023 07:18:57 GMT  
		Size: 998.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e138b051b652e40f53e6ace489845ca2a92f430f592f5112730c8b2bce6866aa`  
		Last Modified: Sat, 04 Feb 2023 07:18:57 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3809ab88d6017f3f38fea418f135f4f8c181568eb8302a3bc9b42f69eea21122`  
		Last Modified: Sat, 04 Feb 2023 07:18:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:ed00ba73f951d5f496355f043a50b0c1d28169ff66e1383605c87cd5b26c6144
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.5 MB (89524742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b855eaae40b75dc29eb937b8f1d1a345f679ef01cbf689fa45b0637fa2e139c9`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:57:35 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 Jan 2023 03:57:36 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 Jan 2023 03:57:42 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:57:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 Jan 2023 03:57:45 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 Jan 2023 03:57:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 22:08:39 GMT
ENV COUCHDB_VERSION=3.3.1
# Wed, 11 Jan 2023 22:08:40 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 Jan 2023 22:08:52 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 Jan 2023 22:08:52 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 11 Jan 2023 22:08:52 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 11 Jan 2023 22:08:53 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 11 Jan 2023 22:08:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 Jan 2023 22:08:53 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 Jan 2023 22:08:53 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 Jan 2023 22:08:53 GMT
EXPOSE 4369 5984 9100
# Wed, 11 Jan 2023 22:08:53 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961831464917d8a5133f3840f3e3d15b6bb840593a5cbb857f67c46f39d73546`  
		Last Modified: Wed, 11 Jan 2023 03:59:34 GMT  
		Size: 3.4 KB (3436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ba419ee6c06e64643e7104acf6aaa7133d872e801ba6d5559cf58a005e1d13`  
		Last Modified: Wed, 11 Jan 2023 03:59:33 GMT  
		Size: 5.2 MB (5209470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2fd7db3c36ccb6f388d0be04337eaf1c4c0b32352e9a7d95b4ae708024cdbd`  
		Last Modified: Wed, 11 Jan 2023 03:59:32 GMT  
		Size: 1.4 MB (1435925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7fbb1ce521b1b1a114c87f3991a7a9de1562c8be484357ddc8d03f2f2c1404`  
		Last Modified: Wed, 11 Jan 2023 03:59:32 GMT  
		Size: 295.5 KB (295517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5bcd70f03fefccc3314c5bd804107f5ca7ec891100c2e85d481e9b84f377c3`  
		Last Modified: Wed, 11 Jan 2023 22:09:15 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a54b1952a30cff448a907d4f82fbbac930beeb1bc452c05e9270fef7a3b056e`  
		Last Modified: Wed, 11 Jan 2023 22:09:18 GMT  
		Size: 52.5 MB (52531616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0782ea0b803ce74bf6e5d05e1a11776e25001beb73576a0c42faa330c238eda0`  
		Last Modified: Wed, 11 Jan 2023 22:09:13 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d347329aa65d9c4b005d93d848c27e025f14d6cb638099fafbecd04dbd43c4f7`  
		Last Modified: Wed, 11 Jan 2023 22:09:13 GMT  
		Size: 998.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0736c691206ce54706b7761f838f3cedd9a8c8f72b933d6ee58c55070659bfb5`  
		Last Modified: Wed, 11 Jan 2023 22:09:14 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b0d0ee154aca0d4270a4eced51b0e6de35a1d7336bb1dc51549889432ea5afc`  
		Last Modified: Wed, 11 Jan 2023 22:09:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; ppc64le

```console
$ docker pull couchdb@sha256:3dbe27c0954f5bc9b14c9addd991ccbc014bf2a1f4208be2ac38945d575fc7e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.7 MB (96659339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71245c02d57bea6de896825db5b96fc126473b2cc688ae84d4c67d18f26645b1`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 Jan 2023 03:49:30 GMT
ADD file:3c7553fb5eda606d574ff6c08bc2213f9e6a68910043fe3087e4c1a04b65a18e in / 
# Wed, 11 Jan 2023 03:49:32 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 04:17:48 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 Jan 2023 04:17:49 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 Jan 2023 04:18:03 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 04:18:11 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 Jan 2023 04:18:11 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 Jan 2023 04:18:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 00:33:57 GMT
ENV COUCHDB_VERSION=3.3.1
# Thu, 12 Jan 2023 00:33:59 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 12 Jan 2023 00:34:21 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 12 Jan 2023 00:34:23 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 12 Jan 2023 00:34:23 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Thu, 12 Jan 2023 00:34:24 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Thu, 12 Jan 2023 00:34:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 12 Jan 2023 00:34:26 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 12 Jan 2023 00:34:26 GMT
VOLUME [/opt/couchdb/data]
# Thu, 12 Jan 2023 00:34:27 GMT
EXPOSE 4369 5984 9100
# Thu, 12 Jan 2023 00:34:27 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:bbf81328aca90b7ddb122fc175443f5323674a9e51bbb00d5b1d683ef0b858f4`  
		Last Modified: Wed, 11 Jan 2023 03:55:33 GMT  
		Size: 35.3 MB (35268773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d4b7dfde57dc3b711e2273da5a61a5829a57b9d58474f1d5ffd21634458f5e`  
		Last Modified: Wed, 11 Jan 2023 04:19:54 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e0b83a7c039dc80fa7b1d8424d0c1a059fbd972e127d4bb4845181526ca907`  
		Last Modified: Wed, 11 Jan 2023 04:19:54 GMT  
		Size: 6.0 MB (6043874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2673661962247aa7e2f981fd8bfb91ba790a2cf92ab3c5c63e6e1340e5f5bc5b`  
		Last Modified: Wed, 11 Jan 2023 04:19:52 GMT  
		Size: 1.5 MB (1509211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c497897d6b3b0e80026e3b729b1d0d01cb112a46c93249841c7394cb4930e3`  
		Last Modified: Wed, 11 Jan 2023 04:19:52 GMT  
		Size: 295.5 KB (295534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9403f4fb1966638fa28ea0a446b686e49577dbfd672df1c2fc26adc93e2723d3`  
		Last Modified: Thu, 12 Jan 2023 00:34:54 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237e765bcf056085764037f970126bbcc67ba3b2f2dde82444c2e655f8d1861c`  
		Last Modified: Thu, 12 Jan 2023 00:35:02 GMT  
		Size: 53.5 MB (53534567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1aae2f6ff7bde8cf74ca73321c82a6189d241ccbc9052c71a2407faac1aefa`  
		Last Modified: Thu, 12 Jan 2023 00:34:52 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002f4c990614acc994cd24eecdeafacfef50d95b0b818ccb9490e1790166836f`  
		Last Modified: Thu, 12 Jan 2023 00:34:52 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b190d63784e2313a291d286c994d2f03ec625274dd5376ae377e89d0181d414f`  
		Last Modified: Thu, 12 Jan 2023 00:34:52 GMT  
		Size: 2.2 KB (2187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c9cd39999ec300f570c4b8cc5ad8af05fd227d5efbb382c416c3fb0d301c89`  
		Last Modified: Thu, 12 Jan 2023 00:34:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1`

```console
$ docker pull couchdb@sha256:53b39fbb73a3a209e52e39a9c8c3af93a03cc9de1b69fec9f2a9a55c00abb9b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:46064776b5eea6b9723add4a461249ba4867495d368173e1212fe38db00dfce5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80024635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:411ed82dfe5a9675836b6d38656c85b281f0ac052ed41230354dcfe828f66c9f`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Sat, 04 Feb 2023 06:52:07 GMT
ADD file:4fbe1e3712cf37c85529cc81e0d03c82085203de00d64b0d669b5996e975925a in / 
# Sat, 04 Feb 2023 06:52:07 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:17:39 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 04 Feb 2023 07:17:40 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 04 Feb 2023 07:17:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:17:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Sat, 04 Feb 2023 07:17:53 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Sat, 04 Feb 2023 07:18:00 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:18:00 GMT
ENV COUCHDB_VERSION=3.1.2
# Sat, 04 Feb 2023 07:18:00 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Sat, 04 Feb 2023 07:18:14 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 04 Feb 2023 07:18:15 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 04 Feb 2023 07:18:15 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 04 Feb 2023 07:18:15 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Sat, 04 Feb 2023 07:18:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 04 Feb 2023 07:18:16 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 07:18:16 GMT
VOLUME [/opt/couchdb/data]
# Sat, 04 Feb 2023 07:18:16 GMT
EXPOSE 4369 5984 9100
# Sat, 04 Feb 2023 07:18:16 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:0cf508b37688dca559387b506062329202aaf08b48be5f55f9278b2a818ad2c9`  
		Last Modified: Sat, 04 Feb 2023 06:56:58 GMT  
		Size: 27.1 MB (27140353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2077aca956be48413850558c99aed2abe9648b6f9b9426c1135e15b89dc335ca`  
		Last Modified: Sat, 04 Feb 2023 07:19:33 GMT  
		Size: 3.4 KB (3410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7242eb760000d68511583e5224849d57fcf7a36c0e53982efab6da6ed3e8760b`  
		Last Modified: Sat, 04 Feb 2023 07:19:32 GMT  
		Size: 6.7 MB (6703784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7226bb128a799d16fae1c3ca8f2cc831f56e1a799146562752f3665a224983e6`  
		Last Modified: Sat, 04 Feb 2023 07:19:31 GMT  
		Size: 1.3 MB (1259577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bbbd4823cbeb627c5529042b3857b765bfed971236216aea4249a891e32b90`  
		Last Modified: Sat, 04 Feb 2023 07:19:31 GMT  
		Size: 294.3 KB (294296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8e0827227c253602e25bf3924aed5af3a9d145ac6600ee8c455029b9fb5b5c`  
		Last Modified: Sat, 04 Feb 2023 07:19:31 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e164a9e3abf791c0eeac9d02c8a6eec719f121a806f747749981c78ac8bb00`  
		Last Modified: Sat, 04 Feb 2023 07:19:34 GMT  
		Size: 44.6 MB (44619618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38d19f05fce411a5c7d03595278edfff9be5e29c76b73ea0239127d9eb51f38`  
		Last Modified: Sat, 04 Feb 2023 07:19:29 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b79dd7eab7bbe21605e7417f3abbe77a6a43bdf6308771b35e69baf0f65434`  
		Last Modified: Sat, 04 Feb 2023 07:19:29 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e3617cd28cde174c912e6e888307d690517dfdd8aa29382578018a337832ef`  
		Last Modified: Sat, 04 Feb 2023 07:19:29 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:986e56bb9a0dd25a27c5132c564191e0d145018fef2c9ea4830232820aa46b93`  
		Last Modified: Sat, 04 Feb 2023 07:19:29 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:068cf4b3782452a97c9347f5f7cf97018cf85c390cf250738baf218100b7999e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75079572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f730d0ebb1efe32b4c88aeae93dc6b4773ff70b50b38e9c75d2a0231a773f47d`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:52 GMT
ADD file:08addf73dde8bf5ac64e0d9bdd1997ce5f406976c19da431616783c14fdb36ac in / 
# Wed, 11 Jan 2023 02:57:52 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:58:25 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 Jan 2023 03:58:25 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 Jan 2023 03:58:32 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:58:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 Jan 2023 03:58:36 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 Jan 2023 03:58:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:58:42 GMT
ENV COUCHDB_VERSION=3.1.2
# Wed, 11 Jan 2023 03:58:43 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 Jan 2023 03:58:54 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 Jan 2023 03:58:54 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 11 Jan 2023 03:58:54 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 Jan 2023 03:58:54 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 11 Jan 2023 03:58:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 Jan 2023 03:58:55 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 Jan 2023 03:58:55 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 Jan 2023 03:58:55 GMT
EXPOSE 4369 5984 9100
# Wed, 11 Jan 2023 03:58:55 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:7fac02f4cd2bcf681b9e156a67009cf4609f45447818b52327d93553bfeb2965`  
		Last Modified: Wed, 11 Jan 2023 03:01:58 GMT  
		Size: 25.9 MB (25914925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49c2ee40908e629f9af8a7cab6dd0cd3837146e1417c5687ea458a09e766135`  
		Last Modified: Wed, 11 Jan 2023 04:00:06 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c510231b78ec40191b73fcf37265b834eb84575e8e9e59214e699e0fb2443f23`  
		Last Modified: Wed, 11 Jan 2023 04:00:06 GMT  
		Size: 6.6 MB (6577083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7fa713a90ae4df09d27f1f23a63a2a6e7df1f68b7907280efb3d944b8bd006`  
		Last Modified: Wed, 11 Jan 2023 04:00:05 GMT  
		Size: 1.2 MB (1164501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c83d395471dc77d8f630b48a40ec852957fdb479ef92505965c06a0297d3c0f`  
		Last Modified: Wed, 11 Jan 2023 04:00:04 GMT  
		Size: 294.1 KB (294133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2ea83fca2dabeb73ea6c9b6afe718c85e6cf1fbe99a4a2ea231b2e08bbada8`  
		Last Modified: Wed, 11 Jan 2023 04:00:04 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639e30434c64b9391fcc739fc0e4f5a3fc0405b0fdb1e52addfbce2802c5fd14`  
		Last Modified: Wed, 11 Jan 2023 04:00:06 GMT  
		Size: 41.1 MB (41121896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6265546072ca4d14a307205cad17f850ca4ed021860e18a8fe246b9997bcdda6`  
		Last Modified: Wed, 11 Jan 2023 04:00:02 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a782805964de8364f24425f37c312a88327e815dcefbe8b00d7913483ca1cf45`  
		Last Modified: Wed, 11 Jan 2023 04:00:02 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c69755a439c0f644c08edfed09861b37c19b50a581ba984ae38399d7f8f8e1a`  
		Last Modified: Wed, 11 Jan 2023 04:00:02 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da7ca01a16a2f7d15cd4d9a6365a8fb58bc7414b6a675688eda576855fd9285`  
		Last Modified: Wed, 11 Jan 2023 04:00:01 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1.2`

```console
$ docker pull couchdb@sha256:53b39fbb73a3a209e52e39a9c8c3af93a03cc9de1b69fec9f2a9a55c00abb9b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1.2` - linux; amd64

```console
$ docker pull couchdb@sha256:46064776b5eea6b9723add4a461249ba4867495d368173e1212fe38db00dfce5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80024635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:411ed82dfe5a9675836b6d38656c85b281f0ac052ed41230354dcfe828f66c9f`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Sat, 04 Feb 2023 06:52:07 GMT
ADD file:4fbe1e3712cf37c85529cc81e0d03c82085203de00d64b0d669b5996e975925a in / 
# Sat, 04 Feb 2023 06:52:07 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:17:39 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 04 Feb 2023 07:17:40 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 04 Feb 2023 07:17:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:17:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Sat, 04 Feb 2023 07:17:53 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Sat, 04 Feb 2023 07:18:00 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:18:00 GMT
ENV COUCHDB_VERSION=3.1.2
# Sat, 04 Feb 2023 07:18:00 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Sat, 04 Feb 2023 07:18:14 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 04 Feb 2023 07:18:15 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 04 Feb 2023 07:18:15 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 04 Feb 2023 07:18:15 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Sat, 04 Feb 2023 07:18:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 04 Feb 2023 07:18:16 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 07:18:16 GMT
VOLUME [/opt/couchdb/data]
# Sat, 04 Feb 2023 07:18:16 GMT
EXPOSE 4369 5984 9100
# Sat, 04 Feb 2023 07:18:16 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:0cf508b37688dca559387b506062329202aaf08b48be5f55f9278b2a818ad2c9`  
		Last Modified: Sat, 04 Feb 2023 06:56:58 GMT  
		Size: 27.1 MB (27140353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2077aca956be48413850558c99aed2abe9648b6f9b9426c1135e15b89dc335ca`  
		Last Modified: Sat, 04 Feb 2023 07:19:33 GMT  
		Size: 3.4 KB (3410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7242eb760000d68511583e5224849d57fcf7a36c0e53982efab6da6ed3e8760b`  
		Last Modified: Sat, 04 Feb 2023 07:19:32 GMT  
		Size: 6.7 MB (6703784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7226bb128a799d16fae1c3ca8f2cc831f56e1a799146562752f3665a224983e6`  
		Last Modified: Sat, 04 Feb 2023 07:19:31 GMT  
		Size: 1.3 MB (1259577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bbbd4823cbeb627c5529042b3857b765bfed971236216aea4249a891e32b90`  
		Last Modified: Sat, 04 Feb 2023 07:19:31 GMT  
		Size: 294.3 KB (294296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8e0827227c253602e25bf3924aed5af3a9d145ac6600ee8c455029b9fb5b5c`  
		Last Modified: Sat, 04 Feb 2023 07:19:31 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e164a9e3abf791c0eeac9d02c8a6eec719f121a806f747749981c78ac8bb00`  
		Last Modified: Sat, 04 Feb 2023 07:19:34 GMT  
		Size: 44.6 MB (44619618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38d19f05fce411a5c7d03595278edfff9be5e29c76b73ea0239127d9eb51f38`  
		Last Modified: Sat, 04 Feb 2023 07:19:29 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b79dd7eab7bbe21605e7417f3abbe77a6a43bdf6308771b35e69baf0f65434`  
		Last Modified: Sat, 04 Feb 2023 07:19:29 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e3617cd28cde174c912e6e888307d690517dfdd8aa29382578018a337832ef`  
		Last Modified: Sat, 04 Feb 2023 07:19:29 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:986e56bb9a0dd25a27c5132c564191e0d145018fef2c9ea4830232820aa46b93`  
		Last Modified: Sat, 04 Feb 2023 07:19:29 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:068cf4b3782452a97c9347f5f7cf97018cf85c390cf250738baf218100b7999e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75079572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f730d0ebb1efe32b4c88aeae93dc6b4773ff70b50b38e9c75d2a0231a773f47d`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:52 GMT
ADD file:08addf73dde8bf5ac64e0d9bdd1997ce5f406976c19da431616783c14fdb36ac in / 
# Wed, 11 Jan 2023 02:57:52 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:58:25 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 Jan 2023 03:58:25 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 Jan 2023 03:58:32 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:58:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 Jan 2023 03:58:36 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 Jan 2023 03:58:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:58:42 GMT
ENV COUCHDB_VERSION=3.1.2
# Wed, 11 Jan 2023 03:58:43 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 Jan 2023 03:58:54 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 Jan 2023 03:58:54 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 11 Jan 2023 03:58:54 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 Jan 2023 03:58:54 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 11 Jan 2023 03:58:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 Jan 2023 03:58:55 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 Jan 2023 03:58:55 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 Jan 2023 03:58:55 GMT
EXPOSE 4369 5984 9100
# Wed, 11 Jan 2023 03:58:55 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:7fac02f4cd2bcf681b9e156a67009cf4609f45447818b52327d93553bfeb2965`  
		Last Modified: Wed, 11 Jan 2023 03:01:58 GMT  
		Size: 25.9 MB (25914925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49c2ee40908e629f9af8a7cab6dd0cd3837146e1417c5687ea458a09e766135`  
		Last Modified: Wed, 11 Jan 2023 04:00:06 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c510231b78ec40191b73fcf37265b834eb84575e8e9e59214e699e0fb2443f23`  
		Last Modified: Wed, 11 Jan 2023 04:00:06 GMT  
		Size: 6.6 MB (6577083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7fa713a90ae4df09d27f1f23a63a2a6e7df1f68b7907280efb3d944b8bd006`  
		Last Modified: Wed, 11 Jan 2023 04:00:05 GMT  
		Size: 1.2 MB (1164501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c83d395471dc77d8f630b48a40ec852957fdb479ef92505965c06a0297d3c0f`  
		Last Modified: Wed, 11 Jan 2023 04:00:04 GMT  
		Size: 294.1 KB (294133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2ea83fca2dabeb73ea6c9b6afe718c85e6cf1fbe99a4a2ea231b2e08bbada8`  
		Last Modified: Wed, 11 Jan 2023 04:00:04 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639e30434c64b9391fcc739fc0e4f5a3fc0405b0fdb1e52addfbce2802c5fd14`  
		Last Modified: Wed, 11 Jan 2023 04:00:06 GMT  
		Size: 41.1 MB (41121896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6265546072ca4d14a307205cad17f850ca4ed021860e18a8fe246b9997bcdda6`  
		Last Modified: Wed, 11 Jan 2023 04:00:02 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a782805964de8364f24425f37c312a88327e815dcefbe8b00d7913483ca1cf45`  
		Last Modified: Wed, 11 Jan 2023 04:00:02 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c69755a439c0f644c08edfed09861b37c19b50a581ba984ae38399d7f8f8e1a`  
		Last Modified: Wed, 11 Jan 2023 04:00:02 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da7ca01a16a2f7d15cd4d9a6365a8fb58bc7414b6a675688eda576855fd9285`  
		Last Modified: Wed, 11 Jan 2023 04:00:01 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2`

```console
$ docker pull couchdb@sha256:f64fb1df2970e9ce03a513037128d0b92199976ee3c338ce928c7d8f4a1ba6d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2` - linux; amd64

```console
$ docker pull couchdb@sha256:eef425ab2025c66119f83c8678dda3e8c9708a8c7e63ac983c3f8e7c61f0bcd4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87524351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba914f3f7e2c0514b7d64342ffa01ff61acf217303426fa0cf49bca6c1e16c0d`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:16:45 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 04 Feb 2023 07:16:46 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 04 Feb 2023 07:16:53 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:16:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Sat, 04 Feb 2023 07:16:57 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Sat, 04 Feb 2023 07:17:02 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:17:19 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Sat, 04 Feb 2023 07:17:20 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Sat, 04 Feb 2023 07:17:33 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 04 Feb 2023 07:17:33 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 04 Feb 2023 07:17:33 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 04 Feb 2023 07:17:34 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Sat, 04 Feb 2023 07:17:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 04 Feb 2023 07:17:34 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 07:17:34 GMT
VOLUME [/opt/couchdb/data]
# Sat, 04 Feb 2023 07:17:34 GMT
EXPOSE 4369 5984 9100
# Sat, 04 Feb 2023 07:17:35 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77476cf11acd0f8081beb4a23efc99a2652c66cabe691898d51dd54b7a973967`  
		Last Modified: Sat, 04 Feb 2023 07:19:00 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e5ab1e54fdd1586bf4c41713f66e3c3dd536afdf177ab750bac5420e11af8b`  
		Last Modified: Sat, 04 Feb 2023 07:18:59 GMT  
		Size: 5.2 MB (5224338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aea5b54023137f626790058724f9349eb5aece02da7ca2ec80ff98cbb34df42`  
		Last Modified: Sat, 04 Feb 2023 07:18:59 GMT  
		Size: 1.6 MB (1553311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd561fdfab9d1eed8c99fefa269d1b26ceae1633127918de8c9bba901cd8642e`  
		Last Modified: Sat, 04 Feb 2023 07:18:59 GMT  
		Size: 295.6 KB (295625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b17ebcb880f4550003dc3fbf095b2c8ce01f10dc3361a34e678cd2c558165e`  
		Last Modified: Sat, 04 Feb 2023 07:19:17 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de52ef5c29d0fd49050c902d5b9148547baf472c5bdadb0055df8b3ed007b13f`  
		Last Modified: Sat, 04 Feb 2023 07:19:21 GMT  
		Size: 49.0 MB (49047011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5c1db9cc13ba70b8e1acb5074418aad0a2ee7b06788162c2f224e4e6762e89`  
		Last Modified: Sat, 04 Feb 2023 07:19:16 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f266404a325e853abdf4d88321bec76e5820faacfaf74c0f11eedf25681b4e82`  
		Last Modified: Sat, 04 Feb 2023 07:19:16 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4701880f67dd8c277b4992810ee8dd33b9905d7ced59409d0691a302ff0b7ac5`  
		Last Modified: Sat, 04 Feb 2023 07:19:15 GMT  
		Size: 2.2 KB (2187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e680e922d77deb270acb9558b2d619a99fd2c1682bd663e7aaa6af801ad65bbe`  
		Last Modified: Sat, 04 Feb 2023 07:19:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:95d32b3ab15184cc130539fe8ba4899ebe65ff946b14787fd836c8944bf47936
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.1 MB (86058193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f789ec44b9bb25bf5e2cef5452bc852089f29219c41c03c3334a31ece6d2e329`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:57:35 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 Jan 2023 03:57:36 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 Jan 2023 03:57:42 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:57:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 Jan 2023 03:57:45 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 Jan 2023 03:57:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:58:09 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Wed, 11 Jan 2023 03:58:09 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 Jan 2023 03:58:20 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 Jan 2023 03:58:20 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 11 Jan 2023 03:58:21 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 Jan 2023 03:58:21 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 11 Jan 2023 03:58:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 Jan 2023 03:58:21 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 Jan 2023 03:58:21 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 Jan 2023 03:58:21 GMT
EXPOSE 4369 5984 9100
# Wed, 11 Jan 2023 03:58:21 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961831464917d8a5133f3840f3e3d15b6bb840593a5cbb857f67c46f39d73546`  
		Last Modified: Wed, 11 Jan 2023 03:59:34 GMT  
		Size: 3.4 KB (3436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ba419ee6c06e64643e7104acf6aaa7133d872e801ba6d5559cf58a005e1d13`  
		Last Modified: Wed, 11 Jan 2023 03:59:33 GMT  
		Size: 5.2 MB (5209470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2fd7db3c36ccb6f388d0be04337eaf1c4c0b32352e9a7d95b4ae708024cdbd`  
		Last Modified: Wed, 11 Jan 2023 03:59:32 GMT  
		Size: 1.4 MB (1435925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7fbb1ce521b1b1a114c87f3991a7a9de1562c8be484357ddc8d03f2f2c1404`  
		Last Modified: Wed, 11 Jan 2023 03:59:32 GMT  
		Size: 295.5 KB (295517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6dad358ded8610705f625cdcdfcd647d3f5283af0c801fc763ff03a180a30c8`  
		Last Modified: Wed, 11 Jan 2023 03:59:50 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636d0283b23cdce42cee7bab78df338a1faad0c50cf95b85f98d05bd9390f25f`  
		Last Modified: Wed, 11 Jan 2023 03:59:53 GMT  
		Size: 49.1 MB (49065304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061db316aa0197baafc1ae6f4dee4bc7911a786207b26ea775ceb430f284b12a`  
		Last Modified: Wed, 11 Jan 2023 03:59:48 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7725be66e477a0f061abf8cafd5a073b4a5c9186d6bfad8a8d205156a3a3f3a`  
		Last Modified: Wed, 11 Jan 2023 03:59:48 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa56978aa2219eda9723688003514b9007bbc67dc17d4b2caa3ee2c3b5716fb`  
		Last Modified: Wed, 11 Jan 2023 03:59:48 GMT  
		Size: 2.2 KB (2185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29f7134d9aaf45c7033d01d8ecacef1f33b44dbe22ee7b250a37e621c8559ea`  
		Last Modified: Wed, 11 Jan 2023 03:59:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; ppc64le

```console
$ docker pull couchdb@sha256:75850eff81cebbc5c66f290d5fbc8deb6a39d8f6d5a753c2bb54efb9f68a0d2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93210528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d908496914c04ea5ed686a19445d87e37784ee7173c3fe8aa1580049b2132764`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 Jan 2023 03:49:30 GMT
ADD file:3c7553fb5eda606d574ff6c08bc2213f9e6a68910043fe3087e4c1a04b65a18e in / 
# Wed, 11 Jan 2023 03:49:32 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 04:17:48 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 Jan 2023 04:17:49 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 Jan 2023 04:18:03 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 04:18:11 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 Jan 2023 04:18:11 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 Jan 2023 04:18:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 04:18:58 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Wed, 11 Jan 2023 04:18:59 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 Jan 2023 04:19:21 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 Jan 2023 04:19:23 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 11 Jan 2023 04:19:23 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 Jan 2023 04:19:23 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 11 Jan 2023 04:19:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 Jan 2023 04:19:25 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 Jan 2023 04:19:25 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 Jan 2023 04:19:25 GMT
EXPOSE 4369 5984 9100
# Wed, 11 Jan 2023 04:19:26 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:bbf81328aca90b7ddb122fc175443f5323674a9e51bbb00d5b1d683ef0b858f4`  
		Last Modified: Wed, 11 Jan 2023 03:55:33 GMT  
		Size: 35.3 MB (35268773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d4b7dfde57dc3b711e2273da5a61a5829a57b9d58474f1d5ffd21634458f5e`  
		Last Modified: Wed, 11 Jan 2023 04:19:54 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e0b83a7c039dc80fa7b1d8424d0c1a059fbd972e127d4bb4845181526ca907`  
		Last Modified: Wed, 11 Jan 2023 04:19:54 GMT  
		Size: 6.0 MB (6043874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2673661962247aa7e2f981fd8bfb91ba790a2cf92ab3c5c63e6e1340e5f5bc5b`  
		Last Modified: Wed, 11 Jan 2023 04:19:52 GMT  
		Size: 1.5 MB (1509211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c497897d6b3b0e80026e3b729b1d0d01cb112a46c93249841c7394cb4930e3`  
		Last Modified: Wed, 11 Jan 2023 04:19:52 GMT  
		Size: 295.5 KB (295534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28015fe227fccfe108c2228326f4f86acd95b321c246ce68385f84a2f69e08d8`  
		Last Modified: Wed, 11 Jan 2023 04:20:22 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2673c190fd453dfabe57ebbb3fc2961eec3153ad007a5e2cd2ccff212f3a0c8e`  
		Last Modified: Wed, 11 Jan 2023 04:20:28 GMT  
		Size: 50.1 MB (50085993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b8a5b0bbdbf782871d7299c9ee8863978972dc8a210da3afd21174370d7ece`  
		Last Modified: Wed, 11 Jan 2023 04:20:19 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c7768733a08358b7de0ddb016dc8fa2d6a97ae2bc6180368a1cf92a9abeb3a`  
		Last Modified: Wed, 11 Jan 2023 04:20:19 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89dd72912ecd2d2693913736074f5afb3d88884d8ed648fdb300ee9d9e0f2a8`  
		Last Modified: Wed, 11 Jan 2023 04:20:19 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527e2ed4a1ec1d9cba539192afdceb7781d11860ea43646355685c8796a6221c`  
		Last Modified: Wed, 11 Jan 2023 04:20:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2.2`

```console
$ docker pull couchdb@sha256:f64fb1df2970e9ce03a513037128d0b92199976ee3c338ce928c7d8f4a1ba6d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2.2` - linux; amd64

```console
$ docker pull couchdb@sha256:eef425ab2025c66119f83c8678dda3e8c9708a8c7e63ac983c3f8e7c61f0bcd4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87524351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba914f3f7e2c0514b7d64342ffa01ff61acf217303426fa0cf49bca6c1e16c0d`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:16:45 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 04 Feb 2023 07:16:46 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 04 Feb 2023 07:16:53 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:16:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Sat, 04 Feb 2023 07:16:57 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Sat, 04 Feb 2023 07:17:02 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:17:19 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Sat, 04 Feb 2023 07:17:20 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Sat, 04 Feb 2023 07:17:33 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 04 Feb 2023 07:17:33 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 04 Feb 2023 07:17:33 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 04 Feb 2023 07:17:34 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Sat, 04 Feb 2023 07:17:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 04 Feb 2023 07:17:34 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 07:17:34 GMT
VOLUME [/opt/couchdb/data]
# Sat, 04 Feb 2023 07:17:34 GMT
EXPOSE 4369 5984 9100
# Sat, 04 Feb 2023 07:17:35 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77476cf11acd0f8081beb4a23efc99a2652c66cabe691898d51dd54b7a973967`  
		Last Modified: Sat, 04 Feb 2023 07:19:00 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e5ab1e54fdd1586bf4c41713f66e3c3dd536afdf177ab750bac5420e11af8b`  
		Last Modified: Sat, 04 Feb 2023 07:18:59 GMT  
		Size: 5.2 MB (5224338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aea5b54023137f626790058724f9349eb5aece02da7ca2ec80ff98cbb34df42`  
		Last Modified: Sat, 04 Feb 2023 07:18:59 GMT  
		Size: 1.6 MB (1553311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd561fdfab9d1eed8c99fefa269d1b26ceae1633127918de8c9bba901cd8642e`  
		Last Modified: Sat, 04 Feb 2023 07:18:59 GMT  
		Size: 295.6 KB (295625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b17ebcb880f4550003dc3fbf095b2c8ce01f10dc3361a34e678cd2c558165e`  
		Last Modified: Sat, 04 Feb 2023 07:19:17 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de52ef5c29d0fd49050c902d5b9148547baf472c5bdadb0055df8b3ed007b13f`  
		Last Modified: Sat, 04 Feb 2023 07:19:21 GMT  
		Size: 49.0 MB (49047011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5c1db9cc13ba70b8e1acb5074418aad0a2ee7b06788162c2f224e4e6762e89`  
		Last Modified: Sat, 04 Feb 2023 07:19:16 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f266404a325e853abdf4d88321bec76e5820faacfaf74c0f11eedf25681b4e82`  
		Last Modified: Sat, 04 Feb 2023 07:19:16 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4701880f67dd8c277b4992810ee8dd33b9905d7ced59409d0691a302ff0b7ac5`  
		Last Modified: Sat, 04 Feb 2023 07:19:15 GMT  
		Size: 2.2 KB (2187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e680e922d77deb270acb9558b2d619a99fd2c1682bd663e7aaa6af801ad65bbe`  
		Last Modified: Sat, 04 Feb 2023 07:19:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:95d32b3ab15184cc130539fe8ba4899ebe65ff946b14787fd836c8944bf47936
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.1 MB (86058193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f789ec44b9bb25bf5e2cef5452bc852089f29219c41c03c3334a31ece6d2e329`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:57:35 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 Jan 2023 03:57:36 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 Jan 2023 03:57:42 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:57:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 Jan 2023 03:57:45 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 Jan 2023 03:57:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:58:09 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Wed, 11 Jan 2023 03:58:09 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 Jan 2023 03:58:20 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 Jan 2023 03:58:20 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 11 Jan 2023 03:58:21 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 Jan 2023 03:58:21 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 11 Jan 2023 03:58:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 Jan 2023 03:58:21 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 Jan 2023 03:58:21 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 Jan 2023 03:58:21 GMT
EXPOSE 4369 5984 9100
# Wed, 11 Jan 2023 03:58:21 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961831464917d8a5133f3840f3e3d15b6bb840593a5cbb857f67c46f39d73546`  
		Last Modified: Wed, 11 Jan 2023 03:59:34 GMT  
		Size: 3.4 KB (3436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ba419ee6c06e64643e7104acf6aaa7133d872e801ba6d5559cf58a005e1d13`  
		Last Modified: Wed, 11 Jan 2023 03:59:33 GMT  
		Size: 5.2 MB (5209470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2fd7db3c36ccb6f388d0be04337eaf1c4c0b32352e9a7d95b4ae708024cdbd`  
		Last Modified: Wed, 11 Jan 2023 03:59:32 GMT  
		Size: 1.4 MB (1435925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7fbb1ce521b1b1a114c87f3991a7a9de1562c8be484357ddc8d03f2f2c1404`  
		Last Modified: Wed, 11 Jan 2023 03:59:32 GMT  
		Size: 295.5 KB (295517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6dad358ded8610705f625cdcdfcd647d3f5283af0c801fc763ff03a180a30c8`  
		Last Modified: Wed, 11 Jan 2023 03:59:50 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636d0283b23cdce42cee7bab78df338a1faad0c50cf95b85f98d05bd9390f25f`  
		Last Modified: Wed, 11 Jan 2023 03:59:53 GMT  
		Size: 49.1 MB (49065304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061db316aa0197baafc1ae6f4dee4bc7911a786207b26ea775ceb430f284b12a`  
		Last Modified: Wed, 11 Jan 2023 03:59:48 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7725be66e477a0f061abf8cafd5a073b4a5c9186d6bfad8a8d205156a3a3f3a`  
		Last Modified: Wed, 11 Jan 2023 03:59:48 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa56978aa2219eda9723688003514b9007bbc67dc17d4b2caa3ee2c3b5716fb`  
		Last Modified: Wed, 11 Jan 2023 03:59:48 GMT  
		Size: 2.2 KB (2185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29f7134d9aaf45c7033d01d8ecacef1f33b44dbe22ee7b250a37e621c8559ea`  
		Last Modified: Wed, 11 Jan 2023 03:59:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2.2` - linux; ppc64le

```console
$ docker pull couchdb@sha256:75850eff81cebbc5c66f290d5fbc8deb6a39d8f6d5a753c2bb54efb9f68a0d2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93210528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d908496914c04ea5ed686a19445d87e37784ee7173c3fe8aa1580049b2132764`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 Jan 2023 03:49:30 GMT
ADD file:3c7553fb5eda606d574ff6c08bc2213f9e6a68910043fe3087e4c1a04b65a18e in / 
# Wed, 11 Jan 2023 03:49:32 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 04:17:48 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 Jan 2023 04:17:49 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 Jan 2023 04:18:03 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 04:18:11 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 Jan 2023 04:18:11 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 Jan 2023 04:18:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 04:18:58 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Wed, 11 Jan 2023 04:18:59 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 Jan 2023 04:19:21 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 Jan 2023 04:19:23 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 11 Jan 2023 04:19:23 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 11 Jan 2023 04:19:23 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 11 Jan 2023 04:19:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 Jan 2023 04:19:25 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 Jan 2023 04:19:25 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 Jan 2023 04:19:25 GMT
EXPOSE 4369 5984 9100
# Wed, 11 Jan 2023 04:19:26 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:bbf81328aca90b7ddb122fc175443f5323674a9e51bbb00d5b1d683ef0b858f4`  
		Last Modified: Wed, 11 Jan 2023 03:55:33 GMT  
		Size: 35.3 MB (35268773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d4b7dfde57dc3b711e2273da5a61a5829a57b9d58474f1d5ffd21634458f5e`  
		Last Modified: Wed, 11 Jan 2023 04:19:54 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e0b83a7c039dc80fa7b1d8424d0c1a059fbd972e127d4bb4845181526ca907`  
		Last Modified: Wed, 11 Jan 2023 04:19:54 GMT  
		Size: 6.0 MB (6043874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2673661962247aa7e2f981fd8bfb91ba790a2cf92ab3c5c63e6e1340e5f5bc5b`  
		Last Modified: Wed, 11 Jan 2023 04:19:52 GMT  
		Size: 1.5 MB (1509211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c497897d6b3b0e80026e3b729b1d0d01cb112a46c93249841c7394cb4930e3`  
		Last Modified: Wed, 11 Jan 2023 04:19:52 GMT  
		Size: 295.5 KB (295534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28015fe227fccfe108c2228326f4f86acd95b321c246ce68385f84a2f69e08d8`  
		Last Modified: Wed, 11 Jan 2023 04:20:22 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2673c190fd453dfabe57ebbb3fc2961eec3153ad007a5e2cd2ccff212f3a0c8e`  
		Last Modified: Wed, 11 Jan 2023 04:20:28 GMT  
		Size: 50.1 MB (50085993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b8a5b0bbdbf782871d7299c9ee8863978972dc8a210da3afd21174370d7ece`  
		Last Modified: Wed, 11 Jan 2023 04:20:19 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c7768733a08358b7de0ddb016dc8fa2d6a97ae2bc6180368a1cf92a9abeb3a`  
		Last Modified: Wed, 11 Jan 2023 04:20:19 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89dd72912ecd2d2693913736074f5afb3d88884d8ed648fdb300ee9d9e0f2a8`  
		Last Modified: Wed, 11 Jan 2023 04:20:19 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527e2ed4a1ec1d9cba539192afdceb7781d11860ea43646355685c8796a6221c`  
		Last Modified: Wed, 11 Jan 2023 04:20:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.3`

```console
$ docker pull couchdb@sha256:6e4b8553339e200f346fdf8308a4b03d37ebe449bd96c7c3e8c1cfbcdcd7eb73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.3` - linux; amd64

```console
$ docker pull couchdb@sha256:6d588a96a550033c02f45a4ce38c296cbe08f9ec14cdd4f5ca4320d8af8eb00b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91153896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1274dd1bda729da68f2c64f847a63ec5d6634042dbe09ee8fb9ee1810b35493a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:16:45 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 04 Feb 2023 07:16:46 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 04 Feb 2023 07:16:53 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:16:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Sat, 04 Feb 2023 07:16:57 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Sat, 04 Feb 2023 07:17:02 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:17:02 GMT
ENV COUCHDB_VERSION=3.3.1
# Sat, 04 Feb 2023 07:17:03 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Sat, 04 Feb 2023 07:17:15 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 04 Feb 2023 07:17:16 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 04 Feb 2023 07:17:16 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Sat, 04 Feb 2023 07:17:16 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Sat, 04 Feb 2023 07:17:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 04 Feb 2023 07:17:17 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 07:17:17 GMT
VOLUME [/opt/couchdb/data]
# Sat, 04 Feb 2023 07:17:17 GMT
EXPOSE 4369 5984 9100
# Sat, 04 Feb 2023 07:17:17 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77476cf11acd0f8081beb4a23efc99a2652c66cabe691898d51dd54b7a973967`  
		Last Modified: Sat, 04 Feb 2023 07:19:00 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e5ab1e54fdd1586bf4c41713f66e3c3dd536afdf177ab750bac5420e11af8b`  
		Last Modified: Sat, 04 Feb 2023 07:18:59 GMT  
		Size: 5.2 MB (5224338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aea5b54023137f626790058724f9349eb5aece02da7ca2ec80ff98cbb34df42`  
		Last Modified: Sat, 04 Feb 2023 07:18:59 GMT  
		Size: 1.6 MB (1553311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd561fdfab9d1eed8c99fefa269d1b26ceae1633127918de8c9bba901cd8642e`  
		Last Modified: Sat, 04 Feb 2023 07:18:59 GMT  
		Size: 295.6 KB (295625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e24cec0cc44eeb1e0f1880275166759ac0aab64b4dcca3410a217f78fe5e2a`  
		Last Modified: Sat, 04 Feb 2023 07:18:58 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3132b1e018f6c5014588752194c7ac7ffabf8e0eec4b3528ff1fce2b24a6df5`  
		Last Modified: Sat, 04 Feb 2023 07:19:02 GMT  
		Size: 52.7 MB (52676329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768bc1a4f6854d19062811091a6930b6efd398b9dd84643f35bc1ced44ea5bba`  
		Last Modified: Sat, 04 Feb 2023 07:18:57 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c6b69d74d3c03eb77600518b7afdc0ed80493cd272bfc1c2c664656cf195381`  
		Last Modified: Sat, 04 Feb 2023 07:18:57 GMT  
		Size: 998.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e138b051b652e40f53e6ace489845ca2a92f430f592f5112730c8b2bce6866aa`  
		Last Modified: Sat, 04 Feb 2023 07:18:57 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3809ab88d6017f3f38fea418f135f4f8c181568eb8302a3bc9b42f69eea21122`  
		Last Modified: Sat, 04 Feb 2023 07:18:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:ed00ba73f951d5f496355f043a50b0c1d28169ff66e1383605c87cd5b26c6144
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.5 MB (89524742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b855eaae40b75dc29eb937b8f1d1a345f679ef01cbf689fa45b0637fa2e139c9`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:57:35 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 Jan 2023 03:57:36 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 Jan 2023 03:57:42 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:57:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 Jan 2023 03:57:45 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 Jan 2023 03:57:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 22:08:39 GMT
ENV COUCHDB_VERSION=3.3.1
# Wed, 11 Jan 2023 22:08:40 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 Jan 2023 22:08:52 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 Jan 2023 22:08:52 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 11 Jan 2023 22:08:52 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 11 Jan 2023 22:08:53 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 11 Jan 2023 22:08:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 Jan 2023 22:08:53 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 Jan 2023 22:08:53 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 Jan 2023 22:08:53 GMT
EXPOSE 4369 5984 9100
# Wed, 11 Jan 2023 22:08:53 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961831464917d8a5133f3840f3e3d15b6bb840593a5cbb857f67c46f39d73546`  
		Last Modified: Wed, 11 Jan 2023 03:59:34 GMT  
		Size: 3.4 KB (3436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ba419ee6c06e64643e7104acf6aaa7133d872e801ba6d5559cf58a005e1d13`  
		Last Modified: Wed, 11 Jan 2023 03:59:33 GMT  
		Size: 5.2 MB (5209470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2fd7db3c36ccb6f388d0be04337eaf1c4c0b32352e9a7d95b4ae708024cdbd`  
		Last Modified: Wed, 11 Jan 2023 03:59:32 GMT  
		Size: 1.4 MB (1435925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7fbb1ce521b1b1a114c87f3991a7a9de1562c8be484357ddc8d03f2f2c1404`  
		Last Modified: Wed, 11 Jan 2023 03:59:32 GMT  
		Size: 295.5 KB (295517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5bcd70f03fefccc3314c5bd804107f5ca7ec891100c2e85d481e9b84f377c3`  
		Last Modified: Wed, 11 Jan 2023 22:09:15 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a54b1952a30cff448a907d4f82fbbac930beeb1bc452c05e9270fef7a3b056e`  
		Last Modified: Wed, 11 Jan 2023 22:09:18 GMT  
		Size: 52.5 MB (52531616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0782ea0b803ce74bf6e5d05e1a11776e25001beb73576a0c42faa330c238eda0`  
		Last Modified: Wed, 11 Jan 2023 22:09:13 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d347329aa65d9c4b005d93d848c27e025f14d6cb638099fafbecd04dbd43c4f7`  
		Last Modified: Wed, 11 Jan 2023 22:09:13 GMT  
		Size: 998.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0736c691206ce54706b7761f838f3cedd9a8c8f72b933d6ee58c55070659bfb5`  
		Last Modified: Wed, 11 Jan 2023 22:09:14 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b0d0ee154aca0d4270a4eced51b0e6de35a1d7336bb1dc51549889432ea5afc`  
		Last Modified: Wed, 11 Jan 2023 22:09:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3` - linux; ppc64le

```console
$ docker pull couchdb@sha256:3dbe27c0954f5bc9b14c9addd991ccbc014bf2a1f4208be2ac38945d575fc7e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.7 MB (96659339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71245c02d57bea6de896825db5b96fc126473b2cc688ae84d4c67d18f26645b1`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 Jan 2023 03:49:30 GMT
ADD file:3c7553fb5eda606d574ff6c08bc2213f9e6a68910043fe3087e4c1a04b65a18e in / 
# Wed, 11 Jan 2023 03:49:32 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 04:17:48 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 Jan 2023 04:17:49 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 Jan 2023 04:18:03 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 04:18:11 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 Jan 2023 04:18:11 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 Jan 2023 04:18:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 00:33:57 GMT
ENV COUCHDB_VERSION=3.3.1
# Thu, 12 Jan 2023 00:33:59 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 12 Jan 2023 00:34:21 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 12 Jan 2023 00:34:23 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 12 Jan 2023 00:34:23 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Thu, 12 Jan 2023 00:34:24 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Thu, 12 Jan 2023 00:34:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 12 Jan 2023 00:34:26 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 12 Jan 2023 00:34:26 GMT
VOLUME [/opt/couchdb/data]
# Thu, 12 Jan 2023 00:34:27 GMT
EXPOSE 4369 5984 9100
# Thu, 12 Jan 2023 00:34:27 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:bbf81328aca90b7ddb122fc175443f5323674a9e51bbb00d5b1d683ef0b858f4`  
		Last Modified: Wed, 11 Jan 2023 03:55:33 GMT  
		Size: 35.3 MB (35268773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d4b7dfde57dc3b711e2273da5a61a5829a57b9d58474f1d5ffd21634458f5e`  
		Last Modified: Wed, 11 Jan 2023 04:19:54 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e0b83a7c039dc80fa7b1d8424d0c1a059fbd972e127d4bb4845181526ca907`  
		Last Modified: Wed, 11 Jan 2023 04:19:54 GMT  
		Size: 6.0 MB (6043874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2673661962247aa7e2f981fd8bfb91ba790a2cf92ab3c5c63e6e1340e5f5bc5b`  
		Last Modified: Wed, 11 Jan 2023 04:19:52 GMT  
		Size: 1.5 MB (1509211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c497897d6b3b0e80026e3b729b1d0d01cb112a46c93249841c7394cb4930e3`  
		Last Modified: Wed, 11 Jan 2023 04:19:52 GMT  
		Size: 295.5 KB (295534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9403f4fb1966638fa28ea0a446b686e49577dbfd672df1c2fc26adc93e2723d3`  
		Last Modified: Thu, 12 Jan 2023 00:34:54 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237e765bcf056085764037f970126bbcc67ba3b2f2dde82444c2e655f8d1861c`  
		Last Modified: Thu, 12 Jan 2023 00:35:02 GMT  
		Size: 53.5 MB (53534567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1aae2f6ff7bde8cf74ca73321c82a6189d241ccbc9052c71a2407faac1aefa`  
		Last Modified: Thu, 12 Jan 2023 00:34:52 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002f4c990614acc994cd24eecdeafacfef50d95b0b818ccb9490e1790166836f`  
		Last Modified: Thu, 12 Jan 2023 00:34:52 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b190d63784e2313a291d286c994d2f03ec625274dd5376ae377e89d0181d414f`  
		Last Modified: Thu, 12 Jan 2023 00:34:52 GMT  
		Size: 2.2 KB (2187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c9cd39999ec300f570c4b8cc5ad8af05fd227d5efbb382c416c3fb0d301c89`  
		Last Modified: Thu, 12 Jan 2023 00:34:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.3.1`

```console
$ docker pull couchdb@sha256:6e4b8553339e200f346fdf8308a4b03d37ebe449bd96c7c3e8c1cfbcdcd7eb73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:6d588a96a550033c02f45a4ce38c296cbe08f9ec14cdd4f5ca4320d8af8eb00b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91153896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1274dd1bda729da68f2c64f847a63ec5d6634042dbe09ee8fb9ee1810b35493a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:16:45 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 04 Feb 2023 07:16:46 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 04 Feb 2023 07:16:53 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:16:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Sat, 04 Feb 2023 07:16:57 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Sat, 04 Feb 2023 07:17:02 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:17:02 GMT
ENV COUCHDB_VERSION=3.3.1
# Sat, 04 Feb 2023 07:17:03 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Sat, 04 Feb 2023 07:17:15 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 04 Feb 2023 07:17:16 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 04 Feb 2023 07:17:16 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Sat, 04 Feb 2023 07:17:16 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Sat, 04 Feb 2023 07:17:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 04 Feb 2023 07:17:17 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 07:17:17 GMT
VOLUME [/opt/couchdb/data]
# Sat, 04 Feb 2023 07:17:17 GMT
EXPOSE 4369 5984 9100
# Sat, 04 Feb 2023 07:17:17 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77476cf11acd0f8081beb4a23efc99a2652c66cabe691898d51dd54b7a973967`  
		Last Modified: Sat, 04 Feb 2023 07:19:00 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e5ab1e54fdd1586bf4c41713f66e3c3dd536afdf177ab750bac5420e11af8b`  
		Last Modified: Sat, 04 Feb 2023 07:18:59 GMT  
		Size: 5.2 MB (5224338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aea5b54023137f626790058724f9349eb5aece02da7ca2ec80ff98cbb34df42`  
		Last Modified: Sat, 04 Feb 2023 07:18:59 GMT  
		Size: 1.6 MB (1553311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd561fdfab9d1eed8c99fefa269d1b26ceae1633127918de8c9bba901cd8642e`  
		Last Modified: Sat, 04 Feb 2023 07:18:59 GMT  
		Size: 295.6 KB (295625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e24cec0cc44eeb1e0f1880275166759ac0aab64b4dcca3410a217f78fe5e2a`  
		Last Modified: Sat, 04 Feb 2023 07:18:58 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3132b1e018f6c5014588752194c7ac7ffabf8e0eec4b3528ff1fce2b24a6df5`  
		Last Modified: Sat, 04 Feb 2023 07:19:02 GMT  
		Size: 52.7 MB (52676329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768bc1a4f6854d19062811091a6930b6efd398b9dd84643f35bc1ced44ea5bba`  
		Last Modified: Sat, 04 Feb 2023 07:18:57 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c6b69d74d3c03eb77600518b7afdc0ed80493cd272bfc1c2c664656cf195381`  
		Last Modified: Sat, 04 Feb 2023 07:18:57 GMT  
		Size: 998.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e138b051b652e40f53e6ace489845ca2a92f430f592f5112730c8b2bce6866aa`  
		Last Modified: Sat, 04 Feb 2023 07:18:57 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3809ab88d6017f3f38fea418f135f4f8c181568eb8302a3bc9b42f69eea21122`  
		Last Modified: Sat, 04 Feb 2023 07:18:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:ed00ba73f951d5f496355f043a50b0c1d28169ff66e1383605c87cd5b26c6144
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.5 MB (89524742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b855eaae40b75dc29eb937b8f1d1a345f679ef01cbf689fa45b0637fa2e139c9`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:57:35 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 Jan 2023 03:57:36 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 Jan 2023 03:57:42 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:57:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 Jan 2023 03:57:45 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 Jan 2023 03:57:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 22:08:39 GMT
ENV COUCHDB_VERSION=3.3.1
# Wed, 11 Jan 2023 22:08:40 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 Jan 2023 22:08:52 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 Jan 2023 22:08:52 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 11 Jan 2023 22:08:52 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 11 Jan 2023 22:08:53 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 11 Jan 2023 22:08:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 Jan 2023 22:08:53 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 Jan 2023 22:08:53 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 Jan 2023 22:08:53 GMT
EXPOSE 4369 5984 9100
# Wed, 11 Jan 2023 22:08:53 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961831464917d8a5133f3840f3e3d15b6bb840593a5cbb857f67c46f39d73546`  
		Last Modified: Wed, 11 Jan 2023 03:59:34 GMT  
		Size: 3.4 KB (3436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ba419ee6c06e64643e7104acf6aaa7133d872e801ba6d5559cf58a005e1d13`  
		Last Modified: Wed, 11 Jan 2023 03:59:33 GMT  
		Size: 5.2 MB (5209470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2fd7db3c36ccb6f388d0be04337eaf1c4c0b32352e9a7d95b4ae708024cdbd`  
		Last Modified: Wed, 11 Jan 2023 03:59:32 GMT  
		Size: 1.4 MB (1435925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7fbb1ce521b1b1a114c87f3991a7a9de1562c8be484357ddc8d03f2f2c1404`  
		Last Modified: Wed, 11 Jan 2023 03:59:32 GMT  
		Size: 295.5 KB (295517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5bcd70f03fefccc3314c5bd804107f5ca7ec891100c2e85d481e9b84f377c3`  
		Last Modified: Wed, 11 Jan 2023 22:09:15 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a54b1952a30cff448a907d4f82fbbac930beeb1bc452c05e9270fef7a3b056e`  
		Last Modified: Wed, 11 Jan 2023 22:09:18 GMT  
		Size: 52.5 MB (52531616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0782ea0b803ce74bf6e5d05e1a11776e25001beb73576a0c42faa330c238eda0`  
		Last Modified: Wed, 11 Jan 2023 22:09:13 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d347329aa65d9c4b005d93d848c27e025f14d6cb638099fafbecd04dbd43c4f7`  
		Last Modified: Wed, 11 Jan 2023 22:09:13 GMT  
		Size: 998.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0736c691206ce54706b7761f838f3cedd9a8c8f72b933d6ee58c55070659bfb5`  
		Last Modified: Wed, 11 Jan 2023 22:09:14 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b0d0ee154aca0d4270a4eced51b0e6de35a1d7336bb1dc51549889432ea5afc`  
		Last Modified: Wed, 11 Jan 2023 22:09:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3.1` - linux; ppc64le

```console
$ docker pull couchdb@sha256:3dbe27c0954f5bc9b14c9addd991ccbc014bf2a1f4208be2ac38945d575fc7e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.7 MB (96659339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71245c02d57bea6de896825db5b96fc126473b2cc688ae84d4c67d18f26645b1`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 Jan 2023 03:49:30 GMT
ADD file:3c7553fb5eda606d574ff6c08bc2213f9e6a68910043fe3087e4c1a04b65a18e in / 
# Wed, 11 Jan 2023 03:49:32 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 04:17:48 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 Jan 2023 04:17:49 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 Jan 2023 04:18:03 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 04:18:11 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 Jan 2023 04:18:11 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 Jan 2023 04:18:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 00:33:57 GMT
ENV COUCHDB_VERSION=3.3.1
# Thu, 12 Jan 2023 00:33:59 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 12 Jan 2023 00:34:21 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 12 Jan 2023 00:34:23 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 12 Jan 2023 00:34:23 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Thu, 12 Jan 2023 00:34:24 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Thu, 12 Jan 2023 00:34:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 12 Jan 2023 00:34:26 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 12 Jan 2023 00:34:26 GMT
VOLUME [/opt/couchdb/data]
# Thu, 12 Jan 2023 00:34:27 GMT
EXPOSE 4369 5984 9100
# Thu, 12 Jan 2023 00:34:27 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:bbf81328aca90b7ddb122fc175443f5323674a9e51bbb00d5b1d683ef0b858f4`  
		Last Modified: Wed, 11 Jan 2023 03:55:33 GMT  
		Size: 35.3 MB (35268773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d4b7dfde57dc3b711e2273da5a61a5829a57b9d58474f1d5ffd21634458f5e`  
		Last Modified: Wed, 11 Jan 2023 04:19:54 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e0b83a7c039dc80fa7b1d8424d0c1a059fbd972e127d4bb4845181526ca907`  
		Last Modified: Wed, 11 Jan 2023 04:19:54 GMT  
		Size: 6.0 MB (6043874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2673661962247aa7e2f981fd8bfb91ba790a2cf92ab3c5c63e6e1340e5f5bc5b`  
		Last Modified: Wed, 11 Jan 2023 04:19:52 GMT  
		Size: 1.5 MB (1509211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c497897d6b3b0e80026e3b729b1d0d01cb112a46c93249841c7394cb4930e3`  
		Last Modified: Wed, 11 Jan 2023 04:19:52 GMT  
		Size: 295.5 KB (295534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9403f4fb1966638fa28ea0a446b686e49577dbfd672df1c2fc26adc93e2723d3`  
		Last Modified: Thu, 12 Jan 2023 00:34:54 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237e765bcf056085764037f970126bbcc67ba3b2f2dde82444c2e655f8d1861c`  
		Last Modified: Thu, 12 Jan 2023 00:35:02 GMT  
		Size: 53.5 MB (53534567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1aae2f6ff7bde8cf74ca73321c82a6189d241ccbc9052c71a2407faac1aefa`  
		Last Modified: Thu, 12 Jan 2023 00:34:52 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002f4c990614acc994cd24eecdeafacfef50d95b0b818ccb9490e1790166836f`  
		Last Modified: Thu, 12 Jan 2023 00:34:52 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b190d63784e2313a291d286c994d2f03ec625274dd5376ae377e89d0181d414f`  
		Last Modified: Thu, 12 Jan 2023 00:34:52 GMT  
		Size: 2.2 KB (2187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c9cd39999ec300f570c4b8cc5ad8af05fd227d5efbb382c416c3fb0d301c89`  
		Last Modified: Thu, 12 Jan 2023 00:34:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:latest`

```console
$ docker pull couchdb@sha256:6e4b8553339e200f346fdf8308a4b03d37ebe449bd96c7c3e8c1cfbcdcd7eb73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:6d588a96a550033c02f45a4ce38c296cbe08f9ec14cdd4f5ca4320d8af8eb00b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91153896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1274dd1bda729da68f2c64f847a63ec5d6634042dbe09ee8fb9ee1810b35493a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:16:45 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 04 Feb 2023 07:16:46 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 04 Feb 2023 07:16:53 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:16:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Sat, 04 Feb 2023 07:16:57 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Sat, 04 Feb 2023 07:17:02 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:17:02 GMT
ENV COUCHDB_VERSION=3.3.1
# Sat, 04 Feb 2023 07:17:03 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Sat, 04 Feb 2023 07:17:15 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 04 Feb 2023 07:17:16 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 04 Feb 2023 07:17:16 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Sat, 04 Feb 2023 07:17:16 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Sat, 04 Feb 2023 07:17:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 04 Feb 2023 07:17:17 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 07:17:17 GMT
VOLUME [/opt/couchdb/data]
# Sat, 04 Feb 2023 07:17:17 GMT
EXPOSE 4369 5984 9100
# Sat, 04 Feb 2023 07:17:17 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77476cf11acd0f8081beb4a23efc99a2652c66cabe691898d51dd54b7a973967`  
		Last Modified: Sat, 04 Feb 2023 07:19:00 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e5ab1e54fdd1586bf4c41713f66e3c3dd536afdf177ab750bac5420e11af8b`  
		Last Modified: Sat, 04 Feb 2023 07:18:59 GMT  
		Size: 5.2 MB (5224338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aea5b54023137f626790058724f9349eb5aece02da7ca2ec80ff98cbb34df42`  
		Last Modified: Sat, 04 Feb 2023 07:18:59 GMT  
		Size: 1.6 MB (1553311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd561fdfab9d1eed8c99fefa269d1b26ceae1633127918de8c9bba901cd8642e`  
		Last Modified: Sat, 04 Feb 2023 07:18:59 GMT  
		Size: 295.6 KB (295625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e24cec0cc44eeb1e0f1880275166759ac0aab64b4dcca3410a217f78fe5e2a`  
		Last Modified: Sat, 04 Feb 2023 07:18:58 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3132b1e018f6c5014588752194c7ac7ffabf8e0eec4b3528ff1fce2b24a6df5`  
		Last Modified: Sat, 04 Feb 2023 07:19:02 GMT  
		Size: 52.7 MB (52676329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768bc1a4f6854d19062811091a6930b6efd398b9dd84643f35bc1ced44ea5bba`  
		Last Modified: Sat, 04 Feb 2023 07:18:57 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c6b69d74d3c03eb77600518b7afdc0ed80493cd272bfc1c2c664656cf195381`  
		Last Modified: Sat, 04 Feb 2023 07:18:57 GMT  
		Size: 998.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e138b051b652e40f53e6ace489845ca2a92f430f592f5112730c8b2bce6866aa`  
		Last Modified: Sat, 04 Feb 2023 07:18:57 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3809ab88d6017f3f38fea418f135f4f8c181568eb8302a3bc9b42f69eea21122`  
		Last Modified: Sat, 04 Feb 2023 07:18:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:ed00ba73f951d5f496355f043a50b0c1d28169ff66e1383605c87cd5b26c6144
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.5 MB (89524742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b855eaae40b75dc29eb937b8f1d1a345f679ef01cbf689fa45b0637fa2e139c9`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 Jan 2023 02:57:34 GMT
ADD file:92cf2c9ffaaea1a6bc1baa7b681303b1029dfd6ddbfef1792be8b21aaf09235c in / 
# Wed, 11 Jan 2023 02:57:35 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:57:35 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 Jan 2023 03:57:36 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 Jan 2023 03:57:42 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:57:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 Jan 2023 03:57:45 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 Jan 2023 03:57:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 22:08:39 GMT
ENV COUCHDB_VERSION=3.3.1
# Wed, 11 Jan 2023 22:08:40 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 11 Jan 2023 22:08:52 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 11 Jan 2023 22:08:52 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 11 Jan 2023 22:08:52 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 11 Jan 2023 22:08:53 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 11 Jan 2023 22:08:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 11 Jan 2023 22:08:53 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 11 Jan 2023 22:08:53 GMT
VOLUME [/opt/couchdb/data]
# Wed, 11 Jan 2023 22:08:53 GMT
EXPOSE 4369 5984 9100
# Wed, 11 Jan 2023 22:08:53 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:934ce60d1040c5d4922bae5879321a398777457b7514de02ef69ece49e6aa907`  
		Last Modified: Wed, 11 Jan 2023 03:01:19 GMT  
		Size: 30.0 MB (30044814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961831464917d8a5133f3840f3e3d15b6bb840593a5cbb857f67c46f39d73546`  
		Last Modified: Wed, 11 Jan 2023 03:59:34 GMT  
		Size: 3.4 KB (3436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ba419ee6c06e64643e7104acf6aaa7133d872e801ba6d5559cf58a005e1d13`  
		Last Modified: Wed, 11 Jan 2023 03:59:33 GMT  
		Size: 5.2 MB (5209470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2fd7db3c36ccb6f388d0be04337eaf1c4c0b32352e9a7d95b4ae708024cdbd`  
		Last Modified: Wed, 11 Jan 2023 03:59:32 GMT  
		Size: 1.4 MB (1435925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7fbb1ce521b1b1a114c87f3991a7a9de1562c8be484357ddc8d03f2f2c1404`  
		Last Modified: Wed, 11 Jan 2023 03:59:32 GMT  
		Size: 295.5 KB (295517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5bcd70f03fefccc3314c5bd804107f5ca7ec891100c2e85d481e9b84f377c3`  
		Last Modified: Wed, 11 Jan 2023 22:09:15 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a54b1952a30cff448a907d4f82fbbac930beeb1bc452c05e9270fef7a3b056e`  
		Last Modified: Wed, 11 Jan 2023 22:09:18 GMT  
		Size: 52.5 MB (52531616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0782ea0b803ce74bf6e5d05e1a11776e25001beb73576a0c42faa330c238eda0`  
		Last Modified: Wed, 11 Jan 2023 22:09:13 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d347329aa65d9c4b005d93d848c27e025f14d6cb638099fafbecd04dbd43c4f7`  
		Last Modified: Wed, 11 Jan 2023 22:09:13 GMT  
		Size: 998.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0736c691206ce54706b7761f838f3cedd9a8c8f72b933d6ee58c55070659bfb5`  
		Last Modified: Wed, 11 Jan 2023 22:09:14 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b0d0ee154aca0d4270a4eced51b0e6de35a1d7336bb1dc51549889432ea5afc`  
		Last Modified: Wed, 11 Jan 2023 22:09:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; ppc64le

```console
$ docker pull couchdb@sha256:3dbe27c0954f5bc9b14c9addd991ccbc014bf2a1f4208be2ac38945d575fc7e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.7 MB (96659339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71245c02d57bea6de896825db5b96fc126473b2cc688ae84d4c67d18f26645b1`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 11 Jan 2023 03:49:30 GMT
ADD file:3c7553fb5eda606d574ff6c08bc2213f9e6a68910043fe3087e4c1a04b65a18e in / 
# Wed, 11 Jan 2023 03:49:32 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 04:17:48 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 11 Jan 2023 04:17:49 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 11 Jan 2023 04:18:03 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 04:18:11 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 11 Jan 2023 04:18:11 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 11 Jan 2023 04:18:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 00:33:57 GMT
ENV COUCHDB_VERSION=3.3.1
# Thu, 12 Jan 2023 00:33:59 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 12 Jan 2023 00:34:21 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 12 Jan 2023 00:34:23 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 12 Jan 2023 00:34:23 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Thu, 12 Jan 2023 00:34:24 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Thu, 12 Jan 2023 00:34:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 12 Jan 2023 00:34:26 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 12 Jan 2023 00:34:26 GMT
VOLUME [/opt/couchdb/data]
# Thu, 12 Jan 2023 00:34:27 GMT
EXPOSE 4369 5984 9100
# Thu, 12 Jan 2023 00:34:27 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:bbf81328aca90b7ddb122fc175443f5323674a9e51bbb00d5b1d683ef0b858f4`  
		Last Modified: Wed, 11 Jan 2023 03:55:33 GMT  
		Size: 35.3 MB (35268773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d4b7dfde57dc3b711e2273da5a61a5829a57b9d58474f1d5ffd21634458f5e`  
		Last Modified: Wed, 11 Jan 2023 04:19:54 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e0b83a7c039dc80fa7b1d8424d0c1a059fbd972e127d4bb4845181526ca907`  
		Last Modified: Wed, 11 Jan 2023 04:19:54 GMT  
		Size: 6.0 MB (6043874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2673661962247aa7e2f981fd8bfb91ba790a2cf92ab3c5c63e6e1340e5f5bc5b`  
		Last Modified: Wed, 11 Jan 2023 04:19:52 GMT  
		Size: 1.5 MB (1509211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c497897d6b3b0e80026e3b729b1d0d01cb112a46c93249841c7394cb4930e3`  
		Last Modified: Wed, 11 Jan 2023 04:19:52 GMT  
		Size: 295.5 KB (295534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9403f4fb1966638fa28ea0a446b686e49577dbfd672df1c2fc26adc93e2723d3`  
		Last Modified: Thu, 12 Jan 2023 00:34:54 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237e765bcf056085764037f970126bbcc67ba3b2f2dde82444c2e655f8d1861c`  
		Last Modified: Thu, 12 Jan 2023 00:35:02 GMT  
		Size: 53.5 MB (53534567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1aae2f6ff7bde8cf74ca73321c82a6189d241ccbc9052c71a2407faac1aefa`  
		Last Modified: Thu, 12 Jan 2023 00:34:52 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002f4c990614acc994cd24eecdeafacfef50d95b0b818ccb9490e1790166836f`  
		Last Modified: Thu, 12 Jan 2023 00:34:52 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b190d63784e2313a291d286c994d2f03ec625274dd5376ae377e89d0181d414f`  
		Last Modified: Thu, 12 Jan 2023 00:34:52 GMT  
		Size: 2.2 KB (2187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c9cd39999ec300f570c4b8cc5ad8af05fd227d5efbb382c416c3fb0d301c89`  
		Last Modified: Thu, 12 Jan 2023 00:34:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
