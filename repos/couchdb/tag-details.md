<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `couchdb`

-	[`couchdb:2`](#couchdb2)
-	[`couchdb:2.3`](#couchdb23)
-	[`couchdb:2.3.1`](#couchdb231)
-	[`couchdb:3`](#couchdb3)
-	[`couchdb:3.1`](#couchdb31)
-	[`couchdb:3.1.1`](#couchdb311)
-	[`couchdb:latest`](#couchdblatest)

## `couchdb:2`

```console
$ docker pull couchdb@sha256:b0aecbda87e687ab60da8b6c096853196d05f8ee212341e100095ea8a6d4cd20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2` - linux; amd64

```console
$ docker pull couchdb@sha256:e1132082541e4450a6885f3669a6e3a84d502ca82457d1f24802e184f9549b44
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84509203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5acc0a1b103e16a37ea2e0d157085679900fe0dd0b260fca875ff2a1e601718f`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:15:37 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 03 Sep 2021 06:15:39 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 03 Sep 2021 06:15:51 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:15:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Fri, 03 Sep 2021 06:15:56 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Fri, 03 Sep 2021 06:16:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:16:26 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Fri, 03 Sep 2021 06:16:27 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Fri, 03 Sep 2021 06:16:47 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 03 Sep 2021 06:16:47 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Fri, 03 Sep 2021 06:16:47 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 03 Sep 2021 06:16:48 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Fri, 03 Sep 2021 06:16:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 06:16:49 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 03 Sep 2021 06:16:49 GMT
VOLUME [/opt/couchdb/data]
# Fri, 03 Sep 2021 06:16:49 GMT
EXPOSE 4369 5984 9100
# Fri, 03 Sep 2021 06:16:49 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffb8269f3cb958b6df784b131310249635f0c725b445d8f0e87b0ead49ada9f`  
		Last Modified: Fri, 03 Sep 2021 06:17:09 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840bf77d4fc471ec5858c07cf9912695d13473e04ae907919ee1509eb8f7921f`  
		Last Modified: Fri, 03 Sep 2021 06:17:08 GMT  
		Size: 6.7 MB (6691209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e219a2ce8909fbc38343906eb23b70d86ea9d3e6143247c74112de1f8bc4fa4`  
		Last Modified: Fri, 03 Sep 2021 06:17:07 GMT  
		Size: 1.3 MB (1258358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0a480c76cb4a0c3785d4a1ea6713048f3018eb8313103dd4287d9448b334aa`  
		Last Modified: Fri, 03 Sep 2021 06:17:06 GMT  
		Size: 293.0 KB (293028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f97259cb1075ecb7d853ba8da4da380bdcae86381a2bee3b85375aae2295b9d`  
		Last Modified: Fri, 03 Sep 2021 06:17:31 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a1ed1c5711d1dad25e873c4414a2703792129dd561a623ee644fe679c79de9`  
		Last Modified: Fri, 03 Sep 2021 06:17:36 GMT  
		Size: 49.1 MB (49113753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b53b9a481c785beb979805b58003aa05db414b60002170997a89167760eb69`  
		Last Modified: Fri, 03 Sep 2021 06:17:28 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717988e2febf27029da4a1b991c82b9f53ad6c015b8103b7f4c9d8bea1c900a4`  
		Last Modified: Fri, 03 Sep 2021 06:17:28 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a26787e90886418814487a4f195d4c9ea6a5a4f19392ad81e4127579d0df15`  
		Last Modified: Fri, 03 Sep 2021 06:17:28 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33533f4754363740142204bab54242e97156e519abfb1aaaa5bac520aaba3d46`  
		Last Modified: Fri, 03 Sep 2021 06:17:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:657fc9b6e80ec6bb2ec0de15149946bb1cc1e83b7ac82456b1042a17913af030
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72941323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b06b091a87d0b61e7ed5aa848df0f2097c16830e908d450f95e2945e9e76f4c`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:58 GMT
ADD file:4a1d7f2d989aee6bd83da076b6e9dd3da2da97cf5654bd37568e9baec30ac4b1 in / 
# Fri, 03 Sep 2021 00:40:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:20:38 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 03 Sep 2021 02:20:39 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 03 Sep 2021 02:20:46 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:20:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Fri, 03 Sep 2021 02:20:51 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Fri, 03 Sep 2021 02:20:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:21:22 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Fri, 03 Sep 2021 02:21:23 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Fri, 03 Sep 2021 02:21:37 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 03 Sep 2021 02:21:37 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Fri, 03 Sep 2021 02:21:37 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 03 Sep 2021 02:21:37 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Fri, 03 Sep 2021 02:21:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 02:21:38 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 03 Sep 2021 02:21:38 GMT
VOLUME [/opt/couchdb/data]
# Fri, 03 Sep 2021 02:21:39 GMT
EXPOSE 4369 5984 9100
# Fri, 03 Sep 2021 02:21:39 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:d10c227306ce3db344a8399cbc02bbf0dcb36519318efbde3c6027c00be8b40e`  
		Last Modified: Fri, 03 Sep 2021 00:49:47 GMT  
		Size: 25.9 MB (25914860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99e79104d74eff69e54fc43ab54d6de030dd137c9e5bce2ffab52a9f05d15c1`  
		Last Modified: Fri, 03 Sep 2021 02:22:07 GMT  
		Size: 3.4 KB (3436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f67a48a613d6afa25a640af5edb573fbd0bd6d0277ff9ac7f49585509ec56e7`  
		Last Modified: Fri, 03 Sep 2021 02:22:06 GMT  
		Size: 6.6 MB (6550707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d09704c92c5208d2688917e5a7b0035964c24c408ac214f76a6029354f08ed`  
		Last Modified: Fri, 03 Sep 2021 02:22:05 GMT  
		Size: 1.2 MB (1163437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358dd0bf58fd7721bd227efacff5d5ffa69f48d47f62fbc43e4ce34337b182d3`  
		Last Modified: Fri, 03 Sep 2021 02:22:05 GMT  
		Size: 292.8 KB (292801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f26dd20ba9faa43ae3b8c0cac43ea3bc8def10641ab4df1c0b080e36f01afa`  
		Last Modified: Fri, 03 Sep 2021 02:22:31 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c34880ec7f86e6b4f2f08e581deabe6897676a324073f1720f1c31a8101aae`  
		Last Modified: Fri, 03 Sep 2021 02:22:34 GMT  
		Size: 39.0 MB (39012488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd833be5b59232692050a135241dac37cf394a072a2563fbb0aaf8168023a912`  
		Last Modified: Fri, 03 Sep 2021 02:22:29 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53ba676c3ffde7334574b6fb8804e65440b7f513a4b553b9784bbdaa60812dc`  
		Last Modified: Fri, 03 Sep 2021 02:22:28 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e289128d57c31b0c784853a411c2f004a43123d632d09a0bee7f1b542402f369`  
		Last Modified: Fri, 03 Sep 2021 02:22:29 GMT  
		Size: 2.0 KB (2050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891129364ea0461f72fb2a1aed097d4ceb2e409c91e50eaba79249b75f1c0c66`  
		Last Modified: Fri, 03 Sep 2021 02:22:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3`

```console
$ docker pull couchdb@sha256:b0aecbda87e687ab60da8b6c096853196d05f8ee212341e100095ea8a6d4cd20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:e1132082541e4450a6885f3669a6e3a84d502ca82457d1f24802e184f9549b44
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84509203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5acc0a1b103e16a37ea2e0d157085679900fe0dd0b260fca875ff2a1e601718f`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:15:37 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 03 Sep 2021 06:15:39 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 03 Sep 2021 06:15:51 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:15:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Fri, 03 Sep 2021 06:15:56 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Fri, 03 Sep 2021 06:16:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:16:26 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Fri, 03 Sep 2021 06:16:27 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Fri, 03 Sep 2021 06:16:47 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 03 Sep 2021 06:16:47 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Fri, 03 Sep 2021 06:16:47 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 03 Sep 2021 06:16:48 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Fri, 03 Sep 2021 06:16:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 06:16:49 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 03 Sep 2021 06:16:49 GMT
VOLUME [/opt/couchdb/data]
# Fri, 03 Sep 2021 06:16:49 GMT
EXPOSE 4369 5984 9100
# Fri, 03 Sep 2021 06:16:49 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffb8269f3cb958b6df784b131310249635f0c725b445d8f0e87b0ead49ada9f`  
		Last Modified: Fri, 03 Sep 2021 06:17:09 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840bf77d4fc471ec5858c07cf9912695d13473e04ae907919ee1509eb8f7921f`  
		Last Modified: Fri, 03 Sep 2021 06:17:08 GMT  
		Size: 6.7 MB (6691209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e219a2ce8909fbc38343906eb23b70d86ea9d3e6143247c74112de1f8bc4fa4`  
		Last Modified: Fri, 03 Sep 2021 06:17:07 GMT  
		Size: 1.3 MB (1258358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0a480c76cb4a0c3785d4a1ea6713048f3018eb8313103dd4287d9448b334aa`  
		Last Modified: Fri, 03 Sep 2021 06:17:06 GMT  
		Size: 293.0 KB (293028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f97259cb1075ecb7d853ba8da4da380bdcae86381a2bee3b85375aae2295b9d`  
		Last Modified: Fri, 03 Sep 2021 06:17:31 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a1ed1c5711d1dad25e873c4414a2703792129dd561a623ee644fe679c79de9`  
		Last Modified: Fri, 03 Sep 2021 06:17:36 GMT  
		Size: 49.1 MB (49113753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b53b9a481c785beb979805b58003aa05db414b60002170997a89167760eb69`  
		Last Modified: Fri, 03 Sep 2021 06:17:28 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717988e2febf27029da4a1b991c82b9f53ad6c015b8103b7f4c9d8bea1c900a4`  
		Last Modified: Fri, 03 Sep 2021 06:17:28 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a26787e90886418814487a4f195d4c9ea6a5a4f19392ad81e4127579d0df15`  
		Last Modified: Fri, 03 Sep 2021 06:17:28 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33533f4754363740142204bab54242e97156e519abfb1aaaa5bac520aaba3d46`  
		Last Modified: Fri, 03 Sep 2021 06:17:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:657fc9b6e80ec6bb2ec0de15149946bb1cc1e83b7ac82456b1042a17913af030
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72941323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b06b091a87d0b61e7ed5aa848df0f2097c16830e908d450f95e2945e9e76f4c`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:58 GMT
ADD file:4a1d7f2d989aee6bd83da076b6e9dd3da2da97cf5654bd37568e9baec30ac4b1 in / 
# Fri, 03 Sep 2021 00:40:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:20:38 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 03 Sep 2021 02:20:39 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 03 Sep 2021 02:20:46 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:20:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Fri, 03 Sep 2021 02:20:51 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Fri, 03 Sep 2021 02:20:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:21:22 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Fri, 03 Sep 2021 02:21:23 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Fri, 03 Sep 2021 02:21:37 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 03 Sep 2021 02:21:37 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Fri, 03 Sep 2021 02:21:37 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 03 Sep 2021 02:21:37 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Fri, 03 Sep 2021 02:21:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 02:21:38 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 03 Sep 2021 02:21:38 GMT
VOLUME [/opt/couchdb/data]
# Fri, 03 Sep 2021 02:21:39 GMT
EXPOSE 4369 5984 9100
# Fri, 03 Sep 2021 02:21:39 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:d10c227306ce3db344a8399cbc02bbf0dcb36519318efbde3c6027c00be8b40e`  
		Last Modified: Fri, 03 Sep 2021 00:49:47 GMT  
		Size: 25.9 MB (25914860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99e79104d74eff69e54fc43ab54d6de030dd137c9e5bce2ffab52a9f05d15c1`  
		Last Modified: Fri, 03 Sep 2021 02:22:07 GMT  
		Size: 3.4 KB (3436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f67a48a613d6afa25a640af5edb573fbd0bd6d0277ff9ac7f49585509ec56e7`  
		Last Modified: Fri, 03 Sep 2021 02:22:06 GMT  
		Size: 6.6 MB (6550707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d09704c92c5208d2688917e5a7b0035964c24c408ac214f76a6029354f08ed`  
		Last Modified: Fri, 03 Sep 2021 02:22:05 GMT  
		Size: 1.2 MB (1163437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358dd0bf58fd7721bd227efacff5d5ffa69f48d47f62fbc43e4ce34337b182d3`  
		Last Modified: Fri, 03 Sep 2021 02:22:05 GMT  
		Size: 292.8 KB (292801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f26dd20ba9faa43ae3b8c0cac43ea3bc8def10641ab4df1c0b080e36f01afa`  
		Last Modified: Fri, 03 Sep 2021 02:22:31 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c34880ec7f86e6b4f2f08e581deabe6897676a324073f1720f1c31a8101aae`  
		Last Modified: Fri, 03 Sep 2021 02:22:34 GMT  
		Size: 39.0 MB (39012488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd833be5b59232692050a135241dac37cf394a072a2563fbb0aaf8168023a912`  
		Last Modified: Fri, 03 Sep 2021 02:22:29 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53ba676c3ffde7334574b6fb8804e65440b7f513a4b553b9784bbdaa60812dc`  
		Last Modified: Fri, 03 Sep 2021 02:22:28 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e289128d57c31b0c784853a411c2f004a43123d632d09a0bee7f1b542402f369`  
		Last Modified: Fri, 03 Sep 2021 02:22:29 GMT  
		Size: 2.0 KB (2050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891129364ea0461f72fb2a1aed097d4ceb2e409c91e50eaba79249b75f1c0c66`  
		Last Modified: Fri, 03 Sep 2021 02:22:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3.1`

```console
$ docker pull couchdb@sha256:b0aecbda87e687ab60da8b6c096853196d05f8ee212341e100095ea8a6d4cd20
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:e1132082541e4450a6885f3669a6e3a84d502ca82457d1f24802e184f9549b44
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84509203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5acc0a1b103e16a37ea2e0d157085679900fe0dd0b260fca875ff2a1e601718f`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:15:37 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 03 Sep 2021 06:15:39 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 03 Sep 2021 06:15:51 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:15:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Fri, 03 Sep 2021 06:15:56 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Fri, 03 Sep 2021 06:16:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:16:26 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Fri, 03 Sep 2021 06:16:27 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Fri, 03 Sep 2021 06:16:47 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 03 Sep 2021 06:16:47 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Fri, 03 Sep 2021 06:16:47 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 03 Sep 2021 06:16:48 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Fri, 03 Sep 2021 06:16:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 06:16:49 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 03 Sep 2021 06:16:49 GMT
VOLUME [/opt/couchdb/data]
# Fri, 03 Sep 2021 06:16:49 GMT
EXPOSE 4369 5984 9100
# Fri, 03 Sep 2021 06:16:49 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffb8269f3cb958b6df784b131310249635f0c725b445d8f0e87b0ead49ada9f`  
		Last Modified: Fri, 03 Sep 2021 06:17:09 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840bf77d4fc471ec5858c07cf9912695d13473e04ae907919ee1509eb8f7921f`  
		Last Modified: Fri, 03 Sep 2021 06:17:08 GMT  
		Size: 6.7 MB (6691209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e219a2ce8909fbc38343906eb23b70d86ea9d3e6143247c74112de1f8bc4fa4`  
		Last Modified: Fri, 03 Sep 2021 06:17:07 GMT  
		Size: 1.3 MB (1258358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0a480c76cb4a0c3785d4a1ea6713048f3018eb8313103dd4287d9448b334aa`  
		Last Modified: Fri, 03 Sep 2021 06:17:06 GMT  
		Size: 293.0 KB (293028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f97259cb1075ecb7d853ba8da4da380bdcae86381a2bee3b85375aae2295b9d`  
		Last Modified: Fri, 03 Sep 2021 06:17:31 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a1ed1c5711d1dad25e873c4414a2703792129dd561a623ee644fe679c79de9`  
		Last Modified: Fri, 03 Sep 2021 06:17:36 GMT  
		Size: 49.1 MB (49113753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b53b9a481c785beb979805b58003aa05db414b60002170997a89167760eb69`  
		Last Modified: Fri, 03 Sep 2021 06:17:28 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717988e2febf27029da4a1b991c82b9f53ad6c015b8103b7f4c9d8bea1c900a4`  
		Last Modified: Fri, 03 Sep 2021 06:17:28 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a26787e90886418814487a4f195d4c9ea6a5a4f19392ad81e4127579d0df15`  
		Last Modified: Fri, 03 Sep 2021 06:17:28 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33533f4754363740142204bab54242e97156e519abfb1aaaa5bac520aaba3d46`  
		Last Modified: Fri, 03 Sep 2021 06:17:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:657fc9b6e80ec6bb2ec0de15149946bb1cc1e83b7ac82456b1042a17913af030
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72941323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b06b091a87d0b61e7ed5aa848df0f2097c16830e908d450f95e2945e9e76f4c`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:58 GMT
ADD file:4a1d7f2d989aee6bd83da076b6e9dd3da2da97cf5654bd37568e9baec30ac4b1 in / 
# Fri, 03 Sep 2021 00:40:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:20:38 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 03 Sep 2021 02:20:39 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 03 Sep 2021 02:20:46 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:20:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Fri, 03 Sep 2021 02:20:51 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Fri, 03 Sep 2021 02:20:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:21:22 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Fri, 03 Sep 2021 02:21:23 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Fri, 03 Sep 2021 02:21:37 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 03 Sep 2021 02:21:37 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Fri, 03 Sep 2021 02:21:37 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 03 Sep 2021 02:21:37 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Fri, 03 Sep 2021 02:21:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 02:21:38 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 03 Sep 2021 02:21:38 GMT
VOLUME [/opt/couchdb/data]
# Fri, 03 Sep 2021 02:21:39 GMT
EXPOSE 4369 5984 9100
# Fri, 03 Sep 2021 02:21:39 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:d10c227306ce3db344a8399cbc02bbf0dcb36519318efbde3c6027c00be8b40e`  
		Last Modified: Fri, 03 Sep 2021 00:49:47 GMT  
		Size: 25.9 MB (25914860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99e79104d74eff69e54fc43ab54d6de030dd137c9e5bce2ffab52a9f05d15c1`  
		Last Modified: Fri, 03 Sep 2021 02:22:07 GMT  
		Size: 3.4 KB (3436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f67a48a613d6afa25a640af5edb573fbd0bd6d0277ff9ac7f49585509ec56e7`  
		Last Modified: Fri, 03 Sep 2021 02:22:06 GMT  
		Size: 6.6 MB (6550707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d09704c92c5208d2688917e5a7b0035964c24c408ac214f76a6029354f08ed`  
		Last Modified: Fri, 03 Sep 2021 02:22:05 GMT  
		Size: 1.2 MB (1163437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358dd0bf58fd7721bd227efacff5d5ffa69f48d47f62fbc43e4ce34337b182d3`  
		Last Modified: Fri, 03 Sep 2021 02:22:05 GMT  
		Size: 292.8 KB (292801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f26dd20ba9faa43ae3b8c0cac43ea3bc8def10641ab4df1c0b080e36f01afa`  
		Last Modified: Fri, 03 Sep 2021 02:22:31 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c34880ec7f86e6b4f2f08e581deabe6897676a324073f1720f1c31a8101aae`  
		Last Modified: Fri, 03 Sep 2021 02:22:34 GMT  
		Size: 39.0 MB (39012488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd833be5b59232692050a135241dac37cf394a072a2563fbb0aaf8168023a912`  
		Last Modified: Fri, 03 Sep 2021 02:22:29 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53ba676c3ffde7334574b6fb8804e65440b7f513a4b553b9784bbdaa60812dc`  
		Last Modified: Fri, 03 Sep 2021 02:22:28 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e289128d57c31b0c784853a411c2f004a43123d632d09a0bee7f1b542402f369`  
		Last Modified: Fri, 03 Sep 2021 02:22:29 GMT  
		Size: 2.0 KB (2050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891129364ea0461f72fb2a1aed097d4ceb2e409c91e50eaba79249b75f1c0c66`  
		Last Modified: Fri, 03 Sep 2021 02:22:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3`

```console
$ docker pull couchdb@sha256:d9941894f83b00ecbd5b62f1f01100daf4185c8bba85fa0241da369a7e346808
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3` - linux; amd64

```console
$ docker pull couchdb@sha256:02accfec9a2611e4ba7b52c2b766bd5a488d715b794a692e888a29a724470f16
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.8 MB (83771652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90b214af24368244615835a40997fa9a8498d177d633c6987a88052dfda63a78`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:15:37 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 03 Sep 2021 06:15:39 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 03 Sep 2021 06:15:51 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:15:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Fri, 03 Sep 2021 06:15:56 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Fri, 03 Sep 2021 06:16:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:16:04 GMT
ENV COUCHDB_VERSION=3.1.1
# Fri, 03 Sep 2021 06:16:04 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Fri, 03 Sep 2021 06:16:20 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 03 Sep 2021 06:16:20 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 03 Sep 2021 06:16:20 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 03 Sep 2021 06:16:20 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Fri, 03 Sep 2021 06:16:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 06:16:22 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 03 Sep 2021 06:16:22 GMT
VOLUME [/opt/couchdb/data]
# Fri, 03 Sep 2021 06:16:22 GMT
EXPOSE 4369 5984 9100
# Fri, 03 Sep 2021 06:16:22 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffb8269f3cb958b6df784b131310249635f0c725b445d8f0e87b0ead49ada9f`  
		Last Modified: Fri, 03 Sep 2021 06:17:09 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840bf77d4fc471ec5858c07cf9912695d13473e04ae907919ee1509eb8f7921f`  
		Last Modified: Fri, 03 Sep 2021 06:17:08 GMT  
		Size: 6.7 MB (6691209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e219a2ce8909fbc38343906eb23b70d86ea9d3e6143247c74112de1f8bc4fa4`  
		Last Modified: Fri, 03 Sep 2021 06:17:07 GMT  
		Size: 1.3 MB (1258358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0a480c76cb4a0c3785d4a1ea6713048f3018eb8313103dd4287d9448b334aa`  
		Last Modified: Fri, 03 Sep 2021 06:17:06 GMT  
		Size: 293.0 KB (293028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec685daee3580a0d619710b817f227d060c7e66b606a5092cef2fe6d3838a82`  
		Last Modified: Fri, 03 Sep 2021 06:17:06 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf44c3c081b641bad70d5036131805d279524a5de0fb7f9c55414699565d932`  
		Last Modified: Fri, 03 Sep 2021 06:17:10 GMT  
		Size: 48.4 MB (48376212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68d8065f543726fb1d74a4e653624cb45b32639e61a709941e2f42d4b9a268ad`  
		Last Modified: Fri, 03 Sep 2021 06:17:04 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2c3bd35e7d6fea081925fa6f3b2c45ebfa4fe9b7b0792da7a411325fe22b2d`  
		Last Modified: Fri, 03 Sep 2021 06:17:04 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c223d4eab0ff83a54123851e578fec5b44dd03e9b2398e7194ae465385a7d27`  
		Last Modified: Fri, 03 Sep 2021 06:17:04 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5045900fbfc2ffb196e6b9cdda9b54c26dc48e9a562954f76fa0917675d250`  
		Last Modified: Fri, 03 Sep 2021 06:17:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:da7714793e1a514a6cde341ced81c8d3d2f36b82cbad5a35858b1df47db601a1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.8 MB (78787152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbe184b5bb1122b33a5b9a8acd8dc10fc6323503d1c3a988e7d8b8a841aadd8e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:58 GMT
ADD file:4a1d7f2d989aee6bd83da076b6e9dd3da2da97cf5654bd37568e9baec30ac4b1 in / 
# Fri, 03 Sep 2021 00:40:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:20:38 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 03 Sep 2021 02:20:39 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 03 Sep 2021 02:20:46 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:20:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Fri, 03 Sep 2021 02:20:51 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Fri, 03 Sep 2021 02:20:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:20:57 GMT
ENV COUCHDB_VERSION=3.1.1
# Fri, 03 Sep 2021 02:20:58 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Fri, 03 Sep 2021 02:21:11 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 03 Sep 2021 02:21:11 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 03 Sep 2021 02:21:12 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 03 Sep 2021 02:21:12 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Fri, 03 Sep 2021 02:21:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 02:21:13 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 03 Sep 2021 02:21:13 GMT
VOLUME [/opt/couchdb/data]
# Fri, 03 Sep 2021 02:21:13 GMT
EXPOSE 4369 5984 9100
# Fri, 03 Sep 2021 02:21:13 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:d10c227306ce3db344a8399cbc02bbf0dcb36519318efbde3c6027c00be8b40e`  
		Last Modified: Fri, 03 Sep 2021 00:49:47 GMT  
		Size: 25.9 MB (25914860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99e79104d74eff69e54fc43ab54d6de030dd137c9e5bce2ffab52a9f05d15c1`  
		Last Modified: Fri, 03 Sep 2021 02:22:07 GMT  
		Size: 3.4 KB (3436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f67a48a613d6afa25a640af5edb573fbd0bd6d0277ff9ac7f49585509ec56e7`  
		Last Modified: Fri, 03 Sep 2021 02:22:06 GMT  
		Size: 6.6 MB (6550707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d09704c92c5208d2688917e5a7b0035964c24c408ac214f76a6029354f08ed`  
		Last Modified: Fri, 03 Sep 2021 02:22:05 GMT  
		Size: 1.2 MB (1163437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358dd0bf58fd7721bd227efacff5d5ffa69f48d47f62fbc43e4ce34337b182d3`  
		Last Modified: Fri, 03 Sep 2021 02:22:05 GMT  
		Size: 292.8 KB (292801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e826e67cc2cc559691eea2e09255171bfb03bc505091027760ca1bc53016aed`  
		Last Modified: Fri, 03 Sep 2021 02:22:05 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3acd258899d95e5989c5f18bc51acca5778073963e64860451aa216fafb8a7`  
		Last Modified: Fri, 03 Sep 2021 02:22:08 GMT  
		Size: 44.9 MB (44858319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70341c1a388088f9228570d5e7d453e69f0fe7b8186b7988399d36434cfd53d0`  
		Last Modified: Fri, 03 Sep 2021 02:22:02 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f4bbbbb9b7cc4f667867e423e1282d5f860f0a5b5a327dca8fbba8cf3372fe`  
		Last Modified: Fri, 03 Sep 2021 02:22:03 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18adfc31069aa5ae63f462cc40cbea13df82317ccca7bc8afd4bc6e9beb9efc`  
		Last Modified: Fri, 03 Sep 2021 02:22:02 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6eea9622d25cfda9c178422b431c157302385677ffc93b03c20ce148dd3b4ec`  
		Last Modified: Fri, 03 Sep 2021 02:22:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1`

```console
$ docker pull couchdb@sha256:d9941894f83b00ecbd5b62f1f01100daf4185c8bba85fa0241da369a7e346808
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:02accfec9a2611e4ba7b52c2b766bd5a488d715b794a692e888a29a724470f16
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.8 MB (83771652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90b214af24368244615835a40997fa9a8498d177d633c6987a88052dfda63a78`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:15:37 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 03 Sep 2021 06:15:39 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 03 Sep 2021 06:15:51 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:15:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Fri, 03 Sep 2021 06:15:56 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Fri, 03 Sep 2021 06:16:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:16:04 GMT
ENV COUCHDB_VERSION=3.1.1
# Fri, 03 Sep 2021 06:16:04 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Fri, 03 Sep 2021 06:16:20 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 03 Sep 2021 06:16:20 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 03 Sep 2021 06:16:20 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 03 Sep 2021 06:16:20 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Fri, 03 Sep 2021 06:16:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 06:16:22 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 03 Sep 2021 06:16:22 GMT
VOLUME [/opt/couchdb/data]
# Fri, 03 Sep 2021 06:16:22 GMT
EXPOSE 4369 5984 9100
# Fri, 03 Sep 2021 06:16:22 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffb8269f3cb958b6df784b131310249635f0c725b445d8f0e87b0ead49ada9f`  
		Last Modified: Fri, 03 Sep 2021 06:17:09 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840bf77d4fc471ec5858c07cf9912695d13473e04ae907919ee1509eb8f7921f`  
		Last Modified: Fri, 03 Sep 2021 06:17:08 GMT  
		Size: 6.7 MB (6691209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e219a2ce8909fbc38343906eb23b70d86ea9d3e6143247c74112de1f8bc4fa4`  
		Last Modified: Fri, 03 Sep 2021 06:17:07 GMT  
		Size: 1.3 MB (1258358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0a480c76cb4a0c3785d4a1ea6713048f3018eb8313103dd4287d9448b334aa`  
		Last Modified: Fri, 03 Sep 2021 06:17:06 GMT  
		Size: 293.0 KB (293028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec685daee3580a0d619710b817f227d060c7e66b606a5092cef2fe6d3838a82`  
		Last Modified: Fri, 03 Sep 2021 06:17:06 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf44c3c081b641bad70d5036131805d279524a5de0fb7f9c55414699565d932`  
		Last Modified: Fri, 03 Sep 2021 06:17:10 GMT  
		Size: 48.4 MB (48376212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68d8065f543726fb1d74a4e653624cb45b32639e61a709941e2f42d4b9a268ad`  
		Last Modified: Fri, 03 Sep 2021 06:17:04 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2c3bd35e7d6fea081925fa6f3b2c45ebfa4fe9b7b0792da7a411325fe22b2d`  
		Last Modified: Fri, 03 Sep 2021 06:17:04 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c223d4eab0ff83a54123851e578fec5b44dd03e9b2398e7194ae465385a7d27`  
		Last Modified: Fri, 03 Sep 2021 06:17:04 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5045900fbfc2ffb196e6b9cdda9b54c26dc48e9a562954f76fa0917675d250`  
		Last Modified: Fri, 03 Sep 2021 06:17:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:da7714793e1a514a6cde341ced81c8d3d2f36b82cbad5a35858b1df47db601a1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.8 MB (78787152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbe184b5bb1122b33a5b9a8acd8dc10fc6323503d1c3a988e7d8b8a841aadd8e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:58 GMT
ADD file:4a1d7f2d989aee6bd83da076b6e9dd3da2da97cf5654bd37568e9baec30ac4b1 in / 
# Fri, 03 Sep 2021 00:40:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:20:38 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 03 Sep 2021 02:20:39 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 03 Sep 2021 02:20:46 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:20:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Fri, 03 Sep 2021 02:20:51 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Fri, 03 Sep 2021 02:20:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:20:57 GMT
ENV COUCHDB_VERSION=3.1.1
# Fri, 03 Sep 2021 02:20:58 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Fri, 03 Sep 2021 02:21:11 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 03 Sep 2021 02:21:11 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 03 Sep 2021 02:21:12 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 03 Sep 2021 02:21:12 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Fri, 03 Sep 2021 02:21:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 02:21:13 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 03 Sep 2021 02:21:13 GMT
VOLUME [/opt/couchdb/data]
# Fri, 03 Sep 2021 02:21:13 GMT
EXPOSE 4369 5984 9100
# Fri, 03 Sep 2021 02:21:13 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:d10c227306ce3db344a8399cbc02bbf0dcb36519318efbde3c6027c00be8b40e`  
		Last Modified: Fri, 03 Sep 2021 00:49:47 GMT  
		Size: 25.9 MB (25914860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99e79104d74eff69e54fc43ab54d6de030dd137c9e5bce2ffab52a9f05d15c1`  
		Last Modified: Fri, 03 Sep 2021 02:22:07 GMT  
		Size: 3.4 KB (3436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f67a48a613d6afa25a640af5edb573fbd0bd6d0277ff9ac7f49585509ec56e7`  
		Last Modified: Fri, 03 Sep 2021 02:22:06 GMT  
		Size: 6.6 MB (6550707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d09704c92c5208d2688917e5a7b0035964c24c408ac214f76a6029354f08ed`  
		Last Modified: Fri, 03 Sep 2021 02:22:05 GMT  
		Size: 1.2 MB (1163437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358dd0bf58fd7721bd227efacff5d5ffa69f48d47f62fbc43e4ce34337b182d3`  
		Last Modified: Fri, 03 Sep 2021 02:22:05 GMT  
		Size: 292.8 KB (292801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e826e67cc2cc559691eea2e09255171bfb03bc505091027760ca1bc53016aed`  
		Last Modified: Fri, 03 Sep 2021 02:22:05 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3acd258899d95e5989c5f18bc51acca5778073963e64860451aa216fafb8a7`  
		Last Modified: Fri, 03 Sep 2021 02:22:08 GMT  
		Size: 44.9 MB (44858319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70341c1a388088f9228570d5e7d453e69f0fe7b8186b7988399d36434cfd53d0`  
		Last Modified: Fri, 03 Sep 2021 02:22:02 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f4bbbbb9b7cc4f667867e423e1282d5f860f0a5b5a327dca8fbba8cf3372fe`  
		Last Modified: Fri, 03 Sep 2021 02:22:03 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18adfc31069aa5ae63f462cc40cbea13df82317ccca7bc8afd4bc6e9beb9efc`  
		Last Modified: Fri, 03 Sep 2021 02:22:02 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6eea9622d25cfda9c178422b431c157302385677ffc93b03c20ce148dd3b4ec`  
		Last Modified: Fri, 03 Sep 2021 02:22:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1.1`

```console
$ docker pull couchdb@sha256:d9941894f83b00ecbd5b62f1f01100daf4185c8bba85fa0241da369a7e346808
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1.1` - linux; amd64

```console
$ docker pull couchdb@sha256:02accfec9a2611e4ba7b52c2b766bd5a488d715b794a692e888a29a724470f16
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.8 MB (83771652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90b214af24368244615835a40997fa9a8498d177d633c6987a88052dfda63a78`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:15:37 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 03 Sep 2021 06:15:39 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 03 Sep 2021 06:15:51 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:15:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Fri, 03 Sep 2021 06:15:56 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Fri, 03 Sep 2021 06:16:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:16:04 GMT
ENV COUCHDB_VERSION=3.1.1
# Fri, 03 Sep 2021 06:16:04 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Fri, 03 Sep 2021 06:16:20 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 03 Sep 2021 06:16:20 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 03 Sep 2021 06:16:20 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 03 Sep 2021 06:16:20 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Fri, 03 Sep 2021 06:16:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 06:16:22 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 03 Sep 2021 06:16:22 GMT
VOLUME [/opt/couchdb/data]
# Fri, 03 Sep 2021 06:16:22 GMT
EXPOSE 4369 5984 9100
# Fri, 03 Sep 2021 06:16:22 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffb8269f3cb958b6df784b131310249635f0c725b445d8f0e87b0ead49ada9f`  
		Last Modified: Fri, 03 Sep 2021 06:17:09 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840bf77d4fc471ec5858c07cf9912695d13473e04ae907919ee1509eb8f7921f`  
		Last Modified: Fri, 03 Sep 2021 06:17:08 GMT  
		Size: 6.7 MB (6691209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e219a2ce8909fbc38343906eb23b70d86ea9d3e6143247c74112de1f8bc4fa4`  
		Last Modified: Fri, 03 Sep 2021 06:17:07 GMT  
		Size: 1.3 MB (1258358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0a480c76cb4a0c3785d4a1ea6713048f3018eb8313103dd4287d9448b334aa`  
		Last Modified: Fri, 03 Sep 2021 06:17:06 GMT  
		Size: 293.0 KB (293028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec685daee3580a0d619710b817f227d060c7e66b606a5092cef2fe6d3838a82`  
		Last Modified: Fri, 03 Sep 2021 06:17:06 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf44c3c081b641bad70d5036131805d279524a5de0fb7f9c55414699565d932`  
		Last Modified: Fri, 03 Sep 2021 06:17:10 GMT  
		Size: 48.4 MB (48376212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68d8065f543726fb1d74a4e653624cb45b32639e61a709941e2f42d4b9a268ad`  
		Last Modified: Fri, 03 Sep 2021 06:17:04 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2c3bd35e7d6fea081925fa6f3b2c45ebfa4fe9b7b0792da7a411325fe22b2d`  
		Last Modified: Fri, 03 Sep 2021 06:17:04 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c223d4eab0ff83a54123851e578fec5b44dd03e9b2398e7194ae465385a7d27`  
		Last Modified: Fri, 03 Sep 2021 06:17:04 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5045900fbfc2ffb196e6b9cdda9b54c26dc48e9a562954f76fa0917675d250`  
		Last Modified: Fri, 03 Sep 2021 06:17:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:da7714793e1a514a6cde341ced81c8d3d2f36b82cbad5a35858b1df47db601a1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.8 MB (78787152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbe184b5bb1122b33a5b9a8acd8dc10fc6323503d1c3a988e7d8b8a841aadd8e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:58 GMT
ADD file:4a1d7f2d989aee6bd83da076b6e9dd3da2da97cf5654bd37568e9baec30ac4b1 in / 
# Fri, 03 Sep 2021 00:40:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:20:38 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 03 Sep 2021 02:20:39 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 03 Sep 2021 02:20:46 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:20:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Fri, 03 Sep 2021 02:20:51 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Fri, 03 Sep 2021 02:20:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:20:57 GMT
ENV COUCHDB_VERSION=3.1.1
# Fri, 03 Sep 2021 02:20:58 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Fri, 03 Sep 2021 02:21:11 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 03 Sep 2021 02:21:11 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 03 Sep 2021 02:21:12 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 03 Sep 2021 02:21:12 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Fri, 03 Sep 2021 02:21:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 02:21:13 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 03 Sep 2021 02:21:13 GMT
VOLUME [/opt/couchdb/data]
# Fri, 03 Sep 2021 02:21:13 GMT
EXPOSE 4369 5984 9100
# Fri, 03 Sep 2021 02:21:13 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:d10c227306ce3db344a8399cbc02bbf0dcb36519318efbde3c6027c00be8b40e`  
		Last Modified: Fri, 03 Sep 2021 00:49:47 GMT  
		Size: 25.9 MB (25914860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99e79104d74eff69e54fc43ab54d6de030dd137c9e5bce2ffab52a9f05d15c1`  
		Last Modified: Fri, 03 Sep 2021 02:22:07 GMT  
		Size: 3.4 KB (3436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f67a48a613d6afa25a640af5edb573fbd0bd6d0277ff9ac7f49585509ec56e7`  
		Last Modified: Fri, 03 Sep 2021 02:22:06 GMT  
		Size: 6.6 MB (6550707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d09704c92c5208d2688917e5a7b0035964c24c408ac214f76a6029354f08ed`  
		Last Modified: Fri, 03 Sep 2021 02:22:05 GMT  
		Size: 1.2 MB (1163437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358dd0bf58fd7721bd227efacff5d5ffa69f48d47f62fbc43e4ce34337b182d3`  
		Last Modified: Fri, 03 Sep 2021 02:22:05 GMT  
		Size: 292.8 KB (292801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e826e67cc2cc559691eea2e09255171bfb03bc505091027760ca1bc53016aed`  
		Last Modified: Fri, 03 Sep 2021 02:22:05 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3acd258899d95e5989c5f18bc51acca5778073963e64860451aa216fafb8a7`  
		Last Modified: Fri, 03 Sep 2021 02:22:08 GMT  
		Size: 44.9 MB (44858319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70341c1a388088f9228570d5e7d453e69f0fe7b8186b7988399d36434cfd53d0`  
		Last Modified: Fri, 03 Sep 2021 02:22:02 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f4bbbbb9b7cc4f667867e423e1282d5f860f0a5b5a327dca8fbba8cf3372fe`  
		Last Modified: Fri, 03 Sep 2021 02:22:03 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18adfc31069aa5ae63f462cc40cbea13df82317ccca7bc8afd4bc6e9beb9efc`  
		Last Modified: Fri, 03 Sep 2021 02:22:02 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6eea9622d25cfda9c178422b431c157302385677ffc93b03c20ce148dd3b4ec`  
		Last Modified: Fri, 03 Sep 2021 02:22:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:latest`

```console
$ docker pull couchdb@sha256:d9941894f83b00ecbd5b62f1f01100daf4185c8bba85fa0241da369a7e346808
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:02accfec9a2611e4ba7b52c2b766bd5a488d715b794a692e888a29a724470f16
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.8 MB (83771652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90b214af24368244615835a40997fa9a8498d177d633c6987a88052dfda63a78`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 03 Sep 2021 01:21:46 GMT
ADD file:4ff85d9f6aa246746912db62dea02eb71750474bb29611e770516a1fcd217add in / 
# Fri, 03 Sep 2021 01:21:46 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 06:15:37 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 03 Sep 2021 06:15:39 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 03 Sep 2021 06:15:51 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:15:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Fri, 03 Sep 2021 06:15:56 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Fri, 03 Sep 2021 06:16:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 06:16:04 GMT
ENV COUCHDB_VERSION=3.1.1
# Fri, 03 Sep 2021 06:16:04 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Fri, 03 Sep 2021 06:16:20 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 03 Sep 2021 06:16:20 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 03 Sep 2021 06:16:20 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 03 Sep 2021 06:16:20 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Fri, 03 Sep 2021 06:16:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 06:16:22 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 03 Sep 2021 06:16:22 GMT
VOLUME [/opt/couchdb/data]
# Fri, 03 Sep 2021 06:16:22 GMT
EXPOSE 4369 5984 9100
# Fri, 03 Sep 2021 06:16:22 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:a330b6cecb98cd2425fd25fce36669073f593b3176b4ee14731e48c05d678cdd`  
		Last Modified: Fri, 03 Sep 2021 01:28:19 GMT  
		Size: 27.1 MB (27145844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffb8269f3cb958b6df784b131310249635f0c725b445d8f0e87b0ead49ada9f`  
		Last Modified: Fri, 03 Sep 2021 06:17:09 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840bf77d4fc471ec5858c07cf9912695d13473e04ae907919ee1509eb8f7921f`  
		Last Modified: Fri, 03 Sep 2021 06:17:08 GMT  
		Size: 6.7 MB (6691209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e219a2ce8909fbc38343906eb23b70d86ea9d3e6143247c74112de1f8bc4fa4`  
		Last Modified: Fri, 03 Sep 2021 06:17:07 GMT  
		Size: 1.3 MB (1258358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0a480c76cb4a0c3785d4a1ea6713048f3018eb8313103dd4287d9448b334aa`  
		Last Modified: Fri, 03 Sep 2021 06:17:06 GMT  
		Size: 293.0 KB (293028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec685daee3580a0d619710b817f227d060c7e66b606a5092cef2fe6d3838a82`  
		Last Modified: Fri, 03 Sep 2021 06:17:06 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf44c3c081b641bad70d5036131805d279524a5de0fb7f9c55414699565d932`  
		Last Modified: Fri, 03 Sep 2021 06:17:10 GMT  
		Size: 48.4 MB (48376212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68d8065f543726fb1d74a4e653624cb45b32639e61a709941e2f42d4b9a268ad`  
		Last Modified: Fri, 03 Sep 2021 06:17:04 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2c3bd35e7d6fea081925fa6f3b2c45ebfa4fe9b7b0792da7a411325fe22b2d`  
		Last Modified: Fri, 03 Sep 2021 06:17:04 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c223d4eab0ff83a54123851e578fec5b44dd03e9b2398e7194ae465385a7d27`  
		Last Modified: Fri, 03 Sep 2021 06:17:04 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5045900fbfc2ffb196e6b9cdda9b54c26dc48e9a562954f76fa0917675d250`  
		Last Modified: Fri, 03 Sep 2021 06:17:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:da7714793e1a514a6cde341ced81c8d3d2f36b82cbad5a35858b1df47db601a1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.8 MB (78787152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbe184b5bb1122b33a5b9a8acd8dc10fc6323503d1c3a988e7d8b8a841aadd8e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:58 GMT
ADD file:4a1d7f2d989aee6bd83da076b6e9dd3da2da97cf5654bd37568e9baec30ac4b1 in / 
# Fri, 03 Sep 2021 00:40:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 02:20:38 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 03 Sep 2021 02:20:39 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 03 Sep 2021 02:20:46 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:20:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Fri, 03 Sep 2021 02:20:51 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Fri, 03 Sep 2021 02:20:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 02:20:57 GMT
ENV COUCHDB_VERSION=3.1.1
# Fri, 03 Sep 2021 02:20:58 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Fri, 03 Sep 2021 02:21:11 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 03 Sep 2021 02:21:11 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 03 Sep 2021 02:21:12 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 03 Sep 2021 02:21:12 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Fri, 03 Sep 2021 02:21:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 03 Sep 2021 02:21:13 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 03 Sep 2021 02:21:13 GMT
VOLUME [/opt/couchdb/data]
# Fri, 03 Sep 2021 02:21:13 GMT
EXPOSE 4369 5984 9100
# Fri, 03 Sep 2021 02:21:13 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:d10c227306ce3db344a8399cbc02bbf0dcb36519318efbde3c6027c00be8b40e`  
		Last Modified: Fri, 03 Sep 2021 00:49:47 GMT  
		Size: 25.9 MB (25914860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99e79104d74eff69e54fc43ab54d6de030dd137c9e5bce2ffab52a9f05d15c1`  
		Last Modified: Fri, 03 Sep 2021 02:22:07 GMT  
		Size: 3.4 KB (3436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f67a48a613d6afa25a640af5edb573fbd0bd6d0277ff9ac7f49585509ec56e7`  
		Last Modified: Fri, 03 Sep 2021 02:22:06 GMT  
		Size: 6.6 MB (6550707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d09704c92c5208d2688917e5a7b0035964c24c408ac214f76a6029354f08ed`  
		Last Modified: Fri, 03 Sep 2021 02:22:05 GMT  
		Size: 1.2 MB (1163437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358dd0bf58fd7721bd227efacff5d5ffa69f48d47f62fbc43e4ce34337b182d3`  
		Last Modified: Fri, 03 Sep 2021 02:22:05 GMT  
		Size: 292.8 KB (292801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e826e67cc2cc559691eea2e09255171bfb03bc505091027760ca1bc53016aed`  
		Last Modified: Fri, 03 Sep 2021 02:22:05 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3acd258899d95e5989c5f18bc51acca5778073963e64860451aa216fafb8a7`  
		Last Modified: Fri, 03 Sep 2021 02:22:08 GMT  
		Size: 44.9 MB (44858319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70341c1a388088f9228570d5e7d453e69f0fe7b8186b7988399d36434cfd53d0`  
		Last Modified: Fri, 03 Sep 2021 02:22:02 GMT  
		Size: 378.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f4bbbbb9b7cc4f667867e423e1282d5f860f0a5b5a327dca8fbba8cf3372fe`  
		Last Modified: Fri, 03 Sep 2021 02:22:03 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18adfc31069aa5ae63f462cc40cbea13df82317ccca7bc8afd4bc6e9beb9efc`  
		Last Modified: Fri, 03 Sep 2021 02:22:02 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6eea9622d25cfda9c178422b431c157302385677ffc93b03c20ce148dd3b4ec`  
		Last Modified: Fri, 03 Sep 2021 02:22:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
