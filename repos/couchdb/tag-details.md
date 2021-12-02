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
$ docker pull couchdb@sha256:28b57a6b8678e7406921635fe46d1c32fa4882ff80938b6056a9583004468442
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2` - linux; amd64

```console
$ docker pull couchdb@sha256:202c00e38dab9e0a1b4576057e8570b7767ff8768d95c76153b0e33e1790dbf6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84517462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67111255e70659562b908fda3c157b78e1d5b2f4b928ba9646559ef128ef8e59`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:43 GMT
ADD file:70f893355b4ecf317b289874ea624aa52c30735086e26de45bad73f57d16757b in / 
# Thu, 02 Dec 2021 02:48:43 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:58:30 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 02 Dec 2021 03:58:31 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 02 Dec 2021 03:58:44 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:58:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 02 Dec 2021 03:58:50 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 02 Dec 2021 03:59:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:59:52 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Thu, 02 Dec 2021 03:59:53 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 02 Dec 2021 04:00:16 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 02 Dec 2021 04:00:17 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Thu, 02 Dec 2021 04:00:17 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 02 Dec 2021 04:00:17 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Thu, 02 Dec 2021 04:00:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 02 Dec 2021 04:00:19 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 02 Dec 2021 04:00:19 GMT
VOLUME [/opt/couchdb/data]
# Thu, 02 Dec 2021 04:00:19 GMT
EXPOSE 4369 5984 9100
# Thu, 02 Dec 2021 04:00:19 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ffbb094f4f9e7c61d97c2b409f3e8154e2621a5074a0087d35f1849e665d0d34`  
		Last Modified: Thu, 02 Dec 2021 02:54:33 GMT  
		Size: 27.2 MB (27153729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc792cd9b52792ad0938a5e388d9be2fc702025774b84de794a632c3e0fc02f0`  
		Last Modified: Thu, 02 Dec 2021 04:00:48 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f87e7045bce9bef72fd9b5bce42edd9ce50aef6775f3694194a1a82c18bf70`  
		Last Modified: Thu, 02 Dec 2021 04:00:47 GMT  
		Size: 6.7 MB (6691479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf38738ecf8be506b95c3b574b38b0c85c9a3cb22aeaac83ebd8440141cc1f82`  
		Last Modified: Thu, 02 Dec 2021 04:00:46 GMT  
		Size: 1.3 MB (1258356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff34fe25c165c10968d4888c5428741e30d459237de0007534284fa46f4577d`  
		Last Modified: Thu, 02 Dec 2021 04:00:45 GMT  
		Size: 293.1 KB (293059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ee2a6c6321bb98473070bf36746a5fe84f1903e1c3ecd9b2ff1c20bf3775e3`  
		Last Modified: Thu, 02 Dec 2021 04:01:26 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bf68be8d4c0978b1d50f1b5876c649d686317a6049080faef114dffbd0c2bc`  
		Last Modified: Thu, 02 Dec 2021 04:01:31 GMT  
		Size: 49.1 MB (49113821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e0472396d00fc8494998a67c99dcf52be7733e2f046cb500c15e16d8612f2e`  
		Last Modified: Thu, 02 Dec 2021 04:01:23 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cccf5364c7e42615110763f6b626b006bfefd5e43bb3bad9707b0b95fece955b`  
		Last Modified: Thu, 02 Dec 2021 04:01:24 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4719d0f7cd526efec2ba629e4734529cef44a2af61f50529d1bd376db11b2a51`  
		Last Modified: Thu, 02 Dec 2021 04:01:23 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be803775575ea7160cc895f602a77188a1a25e91d4ee10df4bd2511431566a4a`  
		Last Modified: Thu, 02 Dec 2021 04:01:23 GMT  
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
$ docker pull couchdb@sha256:28b57a6b8678e7406921635fe46d1c32fa4882ff80938b6056a9583004468442
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:202c00e38dab9e0a1b4576057e8570b7767ff8768d95c76153b0e33e1790dbf6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84517462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67111255e70659562b908fda3c157b78e1d5b2f4b928ba9646559ef128ef8e59`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:43 GMT
ADD file:70f893355b4ecf317b289874ea624aa52c30735086e26de45bad73f57d16757b in / 
# Thu, 02 Dec 2021 02:48:43 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:58:30 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 02 Dec 2021 03:58:31 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 02 Dec 2021 03:58:44 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:58:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 02 Dec 2021 03:58:50 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 02 Dec 2021 03:59:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:59:52 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Thu, 02 Dec 2021 03:59:53 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 02 Dec 2021 04:00:16 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 02 Dec 2021 04:00:17 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Thu, 02 Dec 2021 04:00:17 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 02 Dec 2021 04:00:17 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Thu, 02 Dec 2021 04:00:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 02 Dec 2021 04:00:19 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 02 Dec 2021 04:00:19 GMT
VOLUME [/opt/couchdb/data]
# Thu, 02 Dec 2021 04:00:19 GMT
EXPOSE 4369 5984 9100
# Thu, 02 Dec 2021 04:00:19 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ffbb094f4f9e7c61d97c2b409f3e8154e2621a5074a0087d35f1849e665d0d34`  
		Last Modified: Thu, 02 Dec 2021 02:54:33 GMT  
		Size: 27.2 MB (27153729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc792cd9b52792ad0938a5e388d9be2fc702025774b84de794a632c3e0fc02f0`  
		Last Modified: Thu, 02 Dec 2021 04:00:48 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f87e7045bce9bef72fd9b5bce42edd9ce50aef6775f3694194a1a82c18bf70`  
		Last Modified: Thu, 02 Dec 2021 04:00:47 GMT  
		Size: 6.7 MB (6691479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf38738ecf8be506b95c3b574b38b0c85c9a3cb22aeaac83ebd8440141cc1f82`  
		Last Modified: Thu, 02 Dec 2021 04:00:46 GMT  
		Size: 1.3 MB (1258356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff34fe25c165c10968d4888c5428741e30d459237de0007534284fa46f4577d`  
		Last Modified: Thu, 02 Dec 2021 04:00:45 GMT  
		Size: 293.1 KB (293059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ee2a6c6321bb98473070bf36746a5fe84f1903e1c3ecd9b2ff1c20bf3775e3`  
		Last Modified: Thu, 02 Dec 2021 04:01:26 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bf68be8d4c0978b1d50f1b5876c649d686317a6049080faef114dffbd0c2bc`  
		Last Modified: Thu, 02 Dec 2021 04:01:31 GMT  
		Size: 49.1 MB (49113821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e0472396d00fc8494998a67c99dcf52be7733e2f046cb500c15e16d8612f2e`  
		Last Modified: Thu, 02 Dec 2021 04:01:23 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cccf5364c7e42615110763f6b626b006bfefd5e43bb3bad9707b0b95fece955b`  
		Last Modified: Thu, 02 Dec 2021 04:01:24 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4719d0f7cd526efec2ba629e4734529cef44a2af61f50529d1bd376db11b2a51`  
		Last Modified: Thu, 02 Dec 2021 04:01:23 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be803775575ea7160cc895f602a77188a1a25e91d4ee10df4bd2511431566a4a`  
		Last Modified: Thu, 02 Dec 2021 04:01:23 GMT  
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
$ docker pull couchdb@sha256:28b57a6b8678e7406921635fe46d1c32fa4882ff80938b6056a9583004468442
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:202c00e38dab9e0a1b4576057e8570b7767ff8768d95c76153b0e33e1790dbf6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84517462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67111255e70659562b908fda3c157b78e1d5b2f4b928ba9646559ef128ef8e59`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:43 GMT
ADD file:70f893355b4ecf317b289874ea624aa52c30735086e26de45bad73f57d16757b in / 
# Thu, 02 Dec 2021 02:48:43 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:58:30 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 02 Dec 2021 03:58:31 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 02 Dec 2021 03:58:44 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:58:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 02 Dec 2021 03:58:50 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 02 Dec 2021 03:59:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:59:52 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Thu, 02 Dec 2021 03:59:53 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 02 Dec 2021 04:00:16 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 02 Dec 2021 04:00:17 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Thu, 02 Dec 2021 04:00:17 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 02 Dec 2021 04:00:17 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Thu, 02 Dec 2021 04:00:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 02 Dec 2021 04:00:19 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 02 Dec 2021 04:00:19 GMT
VOLUME [/opt/couchdb/data]
# Thu, 02 Dec 2021 04:00:19 GMT
EXPOSE 4369 5984 9100
# Thu, 02 Dec 2021 04:00:19 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ffbb094f4f9e7c61d97c2b409f3e8154e2621a5074a0087d35f1849e665d0d34`  
		Last Modified: Thu, 02 Dec 2021 02:54:33 GMT  
		Size: 27.2 MB (27153729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc792cd9b52792ad0938a5e388d9be2fc702025774b84de794a632c3e0fc02f0`  
		Last Modified: Thu, 02 Dec 2021 04:00:48 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f87e7045bce9bef72fd9b5bce42edd9ce50aef6775f3694194a1a82c18bf70`  
		Last Modified: Thu, 02 Dec 2021 04:00:47 GMT  
		Size: 6.7 MB (6691479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf38738ecf8be506b95c3b574b38b0c85c9a3cb22aeaac83ebd8440141cc1f82`  
		Last Modified: Thu, 02 Dec 2021 04:00:46 GMT  
		Size: 1.3 MB (1258356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff34fe25c165c10968d4888c5428741e30d459237de0007534284fa46f4577d`  
		Last Modified: Thu, 02 Dec 2021 04:00:45 GMT  
		Size: 293.1 KB (293059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ee2a6c6321bb98473070bf36746a5fe84f1903e1c3ecd9b2ff1c20bf3775e3`  
		Last Modified: Thu, 02 Dec 2021 04:01:26 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bf68be8d4c0978b1d50f1b5876c649d686317a6049080faef114dffbd0c2bc`  
		Last Modified: Thu, 02 Dec 2021 04:01:31 GMT  
		Size: 49.1 MB (49113821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e0472396d00fc8494998a67c99dcf52be7733e2f046cb500c15e16d8612f2e`  
		Last Modified: Thu, 02 Dec 2021 04:01:23 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cccf5364c7e42615110763f6b626b006bfefd5e43bb3bad9707b0b95fece955b`  
		Last Modified: Thu, 02 Dec 2021 04:01:24 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4719d0f7cd526efec2ba629e4734529cef44a2af61f50529d1bd376db11b2a51`  
		Last Modified: Thu, 02 Dec 2021 04:01:23 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be803775575ea7160cc895f602a77188a1a25e91d4ee10df4bd2511431566a4a`  
		Last Modified: Thu, 02 Dec 2021 04:01:23 GMT  
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
$ docker pull couchdb@sha256:12a26ccb78ebcff517252bf4581f0189ac22c667459f8bb5e0113ff181fe96bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3` - linux; amd64

```console
$ docker pull couchdb@sha256:f9233a3c37fc3a10a128c63ee24d6d710ecb256efcea6470cf1481a88497c14f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.6 MB (80555600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c54858da96e40fd74eb5ba582c8555ce4d7e6a8d1680922378e6ee368ea7116`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:43 GMT
ADD file:70f893355b4ecf317b289874ea624aa52c30735086e26de45bad73f57d16757b in / 
# Thu, 02 Dec 2021 02:48:43 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:58:30 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 02 Dec 2021 03:58:31 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 02 Dec 2021 03:58:44 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:58:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 02 Dec 2021 03:58:50 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 02 Dec 2021 03:59:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:59:01 GMT
ENV COUCHDB_VERSION=3.2.0
# Thu, 02 Dec 2021 03:59:03 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 02 Dec 2021 03:59:20 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 02 Dec 2021 03:59:20 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 02 Dec 2021 03:59:20 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 02 Dec 2021 03:59:21 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Thu, 02 Dec 2021 03:59:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 02 Dec 2021 03:59:22 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 02 Dec 2021 03:59:22 GMT
VOLUME [/opt/couchdb/data]
# Thu, 02 Dec 2021 03:59:22 GMT
EXPOSE 4369 5984 9100
# Thu, 02 Dec 2021 03:59:22 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ffbb094f4f9e7c61d97c2b409f3e8154e2621a5074a0087d35f1849e665d0d34`  
		Last Modified: Thu, 02 Dec 2021 02:54:33 GMT  
		Size: 27.2 MB (27153729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc792cd9b52792ad0938a5e388d9be2fc702025774b84de794a632c3e0fc02f0`  
		Last Modified: Thu, 02 Dec 2021 04:00:48 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f87e7045bce9bef72fd9b5bce42edd9ce50aef6775f3694194a1a82c18bf70`  
		Last Modified: Thu, 02 Dec 2021 04:00:47 GMT  
		Size: 6.7 MB (6691479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf38738ecf8be506b95c3b574b38b0c85c9a3cb22aeaac83ebd8440141cc1f82`  
		Last Modified: Thu, 02 Dec 2021 04:00:46 GMT  
		Size: 1.3 MB (1258356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff34fe25c165c10968d4888c5428741e30d459237de0007534284fa46f4577d`  
		Last Modified: Thu, 02 Dec 2021 04:00:45 GMT  
		Size: 293.1 KB (293059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c15fe4082d8bc4ffe30e811af7011a5a2d3838d55adb4e8ed5726d005543a34`  
		Last Modified: Thu, 02 Dec 2021 04:00:45 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb97c47e07838a0f160aebf72818bc31d97a769d7ccd3e7cee6e376abeacf70`  
		Last Modified: Thu, 02 Dec 2021 04:00:49 GMT  
		Size: 45.2 MB (45151962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314989771b01cbcd55238bde9274da680acf89f4af915d1afec64fcf4c34caec`  
		Last Modified: Thu, 02 Dec 2021 04:00:42 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7045cb60dfcd780b48dce1b614f91f784c903bbe054158c9a06884aa16273e`  
		Last Modified: Thu, 02 Dec 2021 04:00:42 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f478ee4109a6eb9fde5f2cb0044c0f3b29b4b7b0a5c2f4f8143f23f65c27d64f`  
		Last Modified: Thu, 02 Dec 2021 04:00:42 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097296e42e603863e72b649d7e75e356ff483c5062c9438e8022dd6bab7fe6f6`  
		Last Modified: Thu, 02 Dec 2021 04:00:43 GMT  
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
$ docker pull couchdb@sha256:49179c053bc64007387af80305e16a932d9eda7828bbd8543018461bb2204e33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:fdb62ff5ce4d44a880046e0ac30933889b4f260236caf923ad945cac941eafbc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80003666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57ff697fa5558306b2afa4e682d4b6380a9738cdbc5d9a2b014c7a0fc241a91f`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:43 GMT
ADD file:70f893355b4ecf317b289874ea624aa52c30735086e26de45bad73f57d16757b in / 
# Thu, 02 Dec 2021 02:48:43 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:58:30 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 02 Dec 2021 03:58:31 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 02 Dec 2021 03:58:44 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:58:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 02 Dec 2021 03:58:50 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 02 Dec 2021 03:59:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:59:27 GMT
ENV COUCHDB_VERSION=3.1.2
# Thu, 02 Dec 2021 03:59:28 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 02 Dec 2021 03:59:43 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 02 Dec 2021 03:59:44 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 02 Dec 2021 03:59:44 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 02 Dec 2021 03:59:45 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Thu, 02 Dec 2021 03:59:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 02 Dec 2021 03:59:46 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 02 Dec 2021 03:59:46 GMT
VOLUME [/opt/couchdb/data]
# Thu, 02 Dec 2021 03:59:47 GMT
EXPOSE 4369 5984 9100
# Thu, 02 Dec 2021 03:59:47 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ffbb094f4f9e7c61d97c2b409f3e8154e2621a5074a0087d35f1849e665d0d34`  
		Last Modified: Thu, 02 Dec 2021 02:54:33 GMT  
		Size: 27.2 MB (27153729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc792cd9b52792ad0938a5e388d9be2fc702025774b84de794a632c3e0fc02f0`  
		Last Modified: Thu, 02 Dec 2021 04:00:48 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f87e7045bce9bef72fd9b5bce42edd9ce50aef6775f3694194a1a82c18bf70`  
		Last Modified: Thu, 02 Dec 2021 04:00:47 GMT  
		Size: 6.7 MB (6691479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf38738ecf8be506b95c3b574b38b0c85c9a3cb22aeaac83ebd8440141cc1f82`  
		Last Modified: Thu, 02 Dec 2021 04:00:46 GMT  
		Size: 1.3 MB (1258356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff34fe25c165c10968d4888c5428741e30d459237de0007534284fa46f4577d`  
		Last Modified: Thu, 02 Dec 2021 04:00:45 GMT  
		Size: 293.1 KB (293059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee142f85ca1332628ddc4730e56d9a9ffeb106490c130516755dd1fe0667b80`  
		Last Modified: Thu, 02 Dec 2021 04:01:09 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b4c913cc766f03be3365121cd0b59e89c01ee7ecdce226860f56e74e5c64a1`  
		Last Modified: Thu, 02 Dec 2021 04:01:13 GMT  
		Size: 44.6 MB (44600031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f7c0c283a9da41259c0ea6a5279ffebabc10018e320e1c71a3e5dbdb197791`  
		Last Modified: Thu, 02 Dec 2021 04:01:07 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b090f6094bb41cf4a08e9288fd6812b8adb0644e5d793f7c1e6568ef2e97ee0`  
		Last Modified: Thu, 02 Dec 2021 04:01:07 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2edb36e304a7ada2e1f1b37b3db3c65eff8b1b14000581ef64cb4419daa603e`  
		Last Modified: Thu, 02 Dec 2021 04:01:07 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c8efda332d8c32ebbcbc7df3b733e6caba419dc9d2f73cbf3214314a38610c`  
		Last Modified: Thu, 02 Dec 2021 04:01:07 GMT  
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
$ docker pull couchdb@sha256:49179c053bc64007387af80305e16a932d9eda7828bbd8543018461bb2204e33
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1.2` - linux; amd64

```console
$ docker pull couchdb@sha256:fdb62ff5ce4d44a880046e0ac30933889b4f260236caf923ad945cac941eafbc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80003666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57ff697fa5558306b2afa4e682d4b6380a9738cdbc5d9a2b014c7a0fc241a91f`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:43 GMT
ADD file:70f893355b4ecf317b289874ea624aa52c30735086e26de45bad73f57d16757b in / 
# Thu, 02 Dec 2021 02:48:43 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:58:30 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 02 Dec 2021 03:58:31 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 02 Dec 2021 03:58:44 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:58:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 02 Dec 2021 03:58:50 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 02 Dec 2021 03:59:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:59:27 GMT
ENV COUCHDB_VERSION=3.1.2
# Thu, 02 Dec 2021 03:59:28 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 02 Dec 2021 03:59:43 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 02 Dec 2021 03:59:44 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 02 Dec 2021 03:59:44 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 02 Dec 2021 03:59:45 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Thu, 02 Dec 2021 03:59:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 02 Dec 2021 03:59:46 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 02 Dec 2021 03:59:46 GMT
VOLUME [/opt/couchdb/data]
# Thu, 02 Dec 2021 03:59:47 GMT
EXPOSE 4369 5984 9100
# Thu, 02 Dec 2021 03:59:47 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ffbb094f4f9e7c61d97c2b409f3e8154e2621a5074a0087d35f1849e665d0d34`  
		Last Modified: Thu, 02 Dec 2021 02:54:33 GMT  
		Size: 27.2 MB (27153729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc792cd9b52792ad0938a5e388d9be2fc702025774b84de794a632c3e0fc02f0`  
		Last Modified: Thu, 02 Dec 2021 04:00:48 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f87e7045bce9bef72fd9b5bce42edd9ce50aef6775f3694194a1a82c18bf70`  
		Last Modified: Thu, 02 Dec 2021 04:00:47 GMT  
		Size: 6.7 MB (6691479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf38738ecf8be506b95c3b574b38b0c85c9a3cb22aeaac83ebd8440141cc1f82`  
		Last Modified: Thu, 02 Dec 2021 04:00:46 GMT  
		Size: 1.3 MB (1258356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff34fe25c165c10968d4888c5428741e30d459237de0007534284fa46f4577d`  
		Last Modified: Thu, 02 Dec 2021 04:00:45 GMT  
		Size: 293.1 KB (293059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee142f85ca1332628ddc4730e56d9a9ffeb106490c130516755dd1fe0667b80`  
		Last Modified: Thu, 02 Dec 2021 04:01:09 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b4c913cc766f03be3365121cd0b59e89c01ee7ecdce226860f56e74e5c64a1`  
		Last Modified: Thu, 02 Dec 2021 04:01:13 GMT  
		Size: 44.6 MB (44600031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f7c0c283a9da41259c0ea6a5279ffebabc10018e320e1c71a3e5dbdb197791`  
		Last Modified: Thu, 02 Dec 2021 04:01:07 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b090f6094bb41cf4a08e9288fd6812b8adb0644e5d793f7c1e6568ef2e97ee0`  
		Last Modified: Thu, 02 Dec 2021 04:01:07 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2edb36e304a7ada2e1f1b37b3db3c65eff8b1b14000581ef64cb4419daa603e`  
		Last Modified: Thu, 02 Dec 2021 04:01:07 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c8efda332d8c32ebbcbc7df3b733e6caba419dc9d2f73cbf3214314a38610c`  
		Last Modified: Thu, 02 Dec 2021 04:01:07 GMT  
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
$ docker pull couchdb@sha256:12a26ccb78ebcff517252bf4581f0189ac22c667459f8bb5e0113ff181fe96bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.2` - linux; amd64

```console
$ docker pull couchdb@sha256:f9233a3c37fc3a10a128c63ee24d6d710ecb256efcea6470cf1481a88497c14f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.6 MB (80555600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c54858da96e40fd74eb5ba582c8555ce4d7e6a8d1680922378e6ee368ea7116`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:43 GMT
ADD file:70f893355b4ecf317b289874ea624aa52c30735086e26de45bad73f57d16757b in / 
# Thu, 02 Dec 2021 02:48:43 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:58:30 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 02 Dec 2021 03:58:31 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 02 Dec 2021 03:58:44 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:58:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 02 Dec 2021 03:58:50 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 02 Dec 2021 03:59:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:59:01 GMT
ENV COUCHDB_VERSION=3.2.0
# Thu, 02 Dec 2021 03:59:03 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 02 Dec 2021 03:59:20 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 02 Dec 2021 03:59:20 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 02 Dec 2021 03:59:20 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 02 Dec 2021 03:59:21 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Thu, 02 Dec 2021 03:59:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 02 Dec 2021 03:59:22 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 02 Dec 2021 03:59:22 GMT
VOLUME [/opt/couchdb/data]
# Thu, 02 Dec 2021 03:59:22 GMT
EXPOSE 4369 5984 9100
# Thu, 02 Dec 2021 03:59:22 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ffbb094f4f9e7c61d97c2b409f3e8154e2621a5074a0087d35f1849e665d0d34`  
		Last Modified: Thu, 02 Dec 2021 02:54:33 GMT  
		Size: 27.2 MB (27153729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc792cd9b52792ad0938a5e388d9be2fc702025774b84de794a632c3e0fc02f0`  
		Last Modified: Thu, 02 Dec 2021 04:00:48 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f87e7045bce9bef72fd9b5bce42edd9ce50aef6775f3694194a1a82c18bf70`  
		Last Modified: Thu, 02 Dec 2021 04:00:47 GMT  
		Size: 6.7 MB (6691479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf38738ecf8be506b95c3b574b38b0c85c9a3cb22aeaac83ebd8440141cc1f82`  
		Last Modified: Thu, 02 Dec 2021 04:00:46 GMT  
		Size: 1.3 MB (1258356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff34fe25c165c10968d4888c5428741e30d459237de0007534284fa46f4577d`  
		Last Modified: Thu, 02 Dec 2021 04:00:45 GMT  
		Size: 293.1 KB (293059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c15fe4082d8bc4ffe30e811af7011a5a2d3838d55adb4e8ed5726d005543a34`  
		Last Modified: Thu, 02 Dec 2021 04:00:45 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb97c47e07838a0f160aebf72818bc31d97a769d7ccd3e7cee6e376abeacf70`  
		Last Modified: Thu, 02 Dec 2021 04:00:49 GMT  
		Size: 45.2 MB (45151962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314989771b01cbcd55238bde9274da680acf89f4af915d1afec64fcf4c34caec`  
		Last Modified: Thu, 02 Dec 2021 04:00:42 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7045cb60dfcd780b48dce1b614f91f784c903bbe054158c9a06884aa16273e`  
		Last Modified: Thu, 02 Dec 2021 04:00:42 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f478ee4109a6eb9fde5f2cb0044c0f3b29b4b7b0a5c2f4f8143f23f65c27d64f`  
		Last Modified: Thu, 02 Dec 2021 04:00:42 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097296e42e603863e72b649d7e75e356ff483c5062c9438e8022dd6bab7fe6f6`  
		Last Modified: Thu, 02 Dec 2021 04:00:43 GMT  
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
$ docker pull couchdb@sha256:12a26ccb78ebcff517252bf4581f0189ac22c667459f8bb5e0113ff181fe96bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.2.0` - linux; amd64

```console
$ docker pull couchdb@sha256:f9233a3c37fc3a10a128c63ee24d6d710ecb256efcea6470cf1481a88497c14f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.6 MB (80555600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c54858da96e40fd74eb5ba582c8555ce4d7e6a8d1680922378e6ee368ea7116`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:43 GMT
ADD file:70f893355b4ecf317b289874ea624aa52c30735086e26de45bad73f57d16757b in / 
# Thu, 02 Dec 2021 02:48:43 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:58:30 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 02 Dec 2021 03:58:31 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 02 Dec 2021 03:58:44 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:58:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 02 Dec 2021 03:58:50 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 02 Dec 2021 03:59:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:59:01 GMT
ENV COUCHDB_VERSION=3.2.0
# Thu, 02 Dec 2021 03:59:03 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 02 Dec 2021 03:59:20 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 02 Dec 2021 03:59:20 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 02 Dec 2021 03:59:20 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 02 Dec 2021 03:59:21 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Thu, 02 Dec 2021 03:59:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 02 Dec 2021 03:59:22 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 02 Dec 2021 03:59:22 GMT
VOLUME [/opt/couchdb/data]
# Thu, 02 Dec 2021 03:59:22 GMT
EXPOSE 4369 5984 9100
# Thu, 02 Dec 2021 03:59:22 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ffbb094f4f9e7c61d97c2b409f3e8154e2621a5074a0087d35f1849e665d0d34`  
		Last Modified: Thu, 02 Dec 2021 02:54:33 GMT  
		Size: 27.2 MB (27153729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc792cd9b52792ad0938a5e388d9be2fc702025774b84de794a632c3e0fc02f0`  
		Last Modified: Thu, 02 Dec 2021 04:00:48 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f87e7045bce9bef72fd9b5bce42edd9ce50aef6775f3694194a1a82c18bf70`  
		Last Modified: Thu, 02 Dec 2021 04:00:47 GMT  
		Size: 6.7 MB (6691479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf38738ecf8be506b95c3b574b38b0c85c9a3cb22aeaac83ebd8440141cc1f82`  
		Last Modified: Thu, 02 Dec 2021 04:00:46 GMT  
		Size: 1.3 MB (1258356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff34fe25c165c10968d4888c5428741e30d459237de0007534284fa46f4577d`  
		Last Modified: Thu, 02 Dec 2021 04:00:45 GMT  
		Size: 293.1 KB (293059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c15fe4082d8bc4ffe30e811af7011a5a2d3838d55adb4e8ed5726d005543a34`  
		Last Modified: Thu, 02 Dec 2021 04:00:45 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb97c47e07838a0f160aebf72818bc31d97a769d7ccd3e7cee6e376abeacf70`  
		Last Modified: Thu, 02 Dec 2021 04:00:49 GMT  
		Size: 45.2 MB (45151962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314989771b01cbcd55238bde9274da680acf89f4af915d1afec64fcf4c34caec`  
		Last Modified: Thu, 02 Dec 2021 04:00:42 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7045cb60dfcd780b48dce1b614f91f784c903bbe054158c9a06884aa16273e`  
		Last Modified: Thu, 02 Dec 2021 04:00:42 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f478ee4109a6eb9fde5f2cb0044c0f3b29b4b7b0a5c2f4f8143f23f65c27d64f`  
		Last Modified: Thu, 02 Dec 2021 04:00:42 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097296e42e603863e72b649d7e75e356ff483c5062c9438e8022dd6bab7fe6f6`  
		Last Modified: Thu, 02 Dec 2021 04:00:43 GMT  
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
$ docker pull couchdb@sha256:12a26ccb78ebcff517252bf4581f0189ac22c667459f8bb5e0113ff181fe96bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:f9233a3c37fc3a10a128c63ee24d6d710ecb256efcea6470cf1481a88497c14f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.6 MB (80555600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c54858da96e40fd74eb5ba582c8555ce4d7e6a8d1680922378e6ee368ea7116`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:43 GMT
ADD file:70f893355b4ecf317b289874ea624aa52c30735086e26de45bad73f57d16757b in / 
# Thu, 02 Dec 2021 02:48:43 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:58:30 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 02 Dec 2021 03:58:31 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 02 Dec 2021 03:58:44 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:58:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 02 Dec 2021 03:58:50 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 02 Dec 2021 03:59:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 03:59:01 GMT
ENV COUCHDB_VERSION=3.2.0
# Thu, 02 Dec 2021 03:59:03 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 02 Dec 2021 03:59:20 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 02 Dec 2021 03:59:20 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 02 Dec 2021 03:59:20 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 02 Dec 2021 03:59:21 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Thu, 02 Dec 2021 03:59:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 02 Dec 2021 03:59:22 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 02 Dec 2021 03:59:22 GMT
VOLUME [/opt/couchdb/data]
# Thu, 02 Dec 2021 03:59:22 GMT
EXPOSE 4369 5984 9100
# Thu, 02 Dec 2021 03:59:22 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ffbb094f4f9e7c61d97c2b409f3e8154e2621a5074a0087d35f1849e665d0d34`  
		Last Modified: Thu, 02 Dec 2021 02:54:33 GMT  
		Size: 27.2 MB (27153729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc792cd9b52792ad0938a5e388d9be2fc702025774b84de794a632c3e0fc02f0`  
		Last Modified: Thu, 02 Dec 2021 04:00:48 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f87e7045bce9bef72fd9b5bce42edd9ce50aef6775f3694194a1a82c18bf70`  
		Last Modified: Thu, 02 Dec 2021 04:00:47 GMT  
		Size: 6.7 MB (6691479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf38738ecf8be506b95c3b574b38b0c85c9a3cb22aeaac83ebd8440141cc1f82`  
		Last Modified: Thu, 02 Dec 2021 04:00:46 GMT  
		Size: 1.3 MB (1258356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff34fe25c165c10968d4888c5428741e30d459237de0007534284fa46f4577d`  
		Last Modified: Thu, 02 Dec 2021 04:00:45 GMT  
		Size: 293.1 KB (293059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c15fe4082d8bc4ffe30e811af7011a5a2d3838d55adb4e8ed5726d005543a34`  
		Last Modified: Thu, 02 Dec 2021 04:00:45 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb97c47e07838a0f160aebf72818bc31d97a769d7ccd3e7cee6e376abeacf70`  
		Last Modified: Thu, 02 Dec 2021 04:00:49 GMT  
		Size: 45.2 MB (45151962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314989771b01cbcd55238bde9274da680acf89f4af915d1afec64fcf4c34caec`  
		Last Modified: Thu, 02 Dec 2021 04:00:42 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7045cb60dfcd780b48dce1b614f91f784c903bbe054158c9a06884aa16273e`  
		Last Modified: Thu, 02 Dec 2021 04:00:42 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f478ee4109a6eb9fde5f2cb0044c0f3b29b4b7b0a5c2f4f8143f23f65c27d64f`  
		Last Modified: Thu, 02 Dec 2021 04:00:42 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097296e42e603863e72b649d7e75e356ff483c5062c9438e8022dd6bab7fe6f6`  
		Last Modified: Thu, 02 Dec 2021 04:00:43 GMT  
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
