## `couchdb:latest`

```console
$ docker pull couchdb@sha256:89ff9e8b82080a0a09367c7781d82e93caf789002a40d82f47324289e7565dfc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:f842b081d584a9cebd2c7e9236cf83573dd709d8536f134c25748bd2db6f8f15
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.8 MB (83771505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14502741b94c59331f032467a706322ac7a366d8803179a8a59a52ccafb41a96`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:38:17 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 17 Aug 2021 09:38:18 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 17 Aug 2021 09:38:39 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:38:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 17 Aug 2021 09:38:45 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 17 Aug 2021 09:38:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:38:52 GMT
ENV COUCHDB_VERSION=3.1.1
# Tue, 17 Aug 2021 09:38:53 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 17 Aug 2021 09:39:09 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 17 Aug 2021 09:39:10 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 17 Aug 2021 09:39:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 17 Aug 2021 09:39:11 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 17 Aug 2021 09:39:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 17 Aug 2021 09:39:13 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 09:39:13 GMT
VOLUME [/opt/couchdb/data]
# Tue, 17 Aug 2021 09:39:13 GMT
EXPOSE 4369 5984 9100
# Tue, 17 Aug 2021 09:39:13 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f42f4d38cbf31bed3f27b58346190ea29ee14cec152ad44f07ef55175d9c055`  
		Last Modified: Tue, 17 Aug 2021 09:40:15 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b8216568b0598794cab6ed82a1c24c039865819e4ac0cdf2b871a943ac813b`  
		Last Modified: Tue, 17 Aug 2021 09:40:15 GMT  
		Size: 6.7 MB (6690783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eed64046c4dd433adb7d77997f00edb049f5d6cbc3fc5ddf3d61527741be6db`  
		Last Modified: Tue, 17 Aug 2021 09:40:13 GMT  
		Size: 1.3 MB (1258341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cba51966f0872e9bd9dac956ed819756d7b3b7c6f039ab31be7c8c9e8baa1ce`  
		Last Modified: Tue, 17 Aug 2021 09:40:13 GMT  
		Size: 293.0 KB (292974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d65e3faec249f895849040e0b4aaf63cf54c47334b53be172b175e58814491`  
		Last Modified: Tue, 17 Aug 2021 09:40:12 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86d59f14c279a50719e39dfbe41a4f9faf00faf4a49d3dc7dd7e473013f8870`  
		Last Modified: Tue, 17 Aug 2021 09:40:18 GMT  
		Size: 48.4 MB (48376415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2b701d40adb5e7ed270dbd7ee811b24742e501179af04ad97e09590c3cca1`  
		Last Modified: Tue, 17 Aug 2021 09:40:10 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c6100ff07eaad02be6c5725c74f06ac475ec795b8abce0132ab4735b859cb0`  
		Last Modified: Tue, 17 Aug 2021 09:40:10 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17fbd510ecd6db8e961e87596cf295bce60babe8836c36a8c9e7d975733c9521`  
		Last Modified: Tue, 17 Aug 2021 09:40:10 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90225c0f1a6a0dd6719927c561d22e407323fe15e377723415fe6fc58bbb2daa`  
		Last Modified: Tue, 17 Aug 2021 09:40:10 GMT  
		Size: 118.0 B  
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
