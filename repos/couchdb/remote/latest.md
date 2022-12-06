## `couchdb:latest`

```console
$ docker pull couchdb@sha256:d3346c205f96be4ce36c245ff08e44331115437ff8760cccb685df64e4470434
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:18b447eb4aa7371763ad1e65fb21b89e867e4e38fbaf87340e401c0d2b48672d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87542993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86d51a034b33057b01caf54d400a6f527ce26b7894ee8d93ea5e8c478307c77e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:35:14 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 15 Nov 2022 10:35:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 15 Nov 2022 10:35:22 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:35:26 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 15 Nov 2022 10:35:26 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 15 Nov 2022 10:35:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:35:32 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 15 Nov 2022 10:35:33 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 15 Nov 2022 10:35:46 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 15 Nov 2022 10:35:47 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 15 Nov 2022 10:35:47 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 15 Nov 2022 10:35:47 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 15 Nov 2022 10:35:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 15 Nov 2022 10:35:48 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 15 Nov 2022 10:35:48 GMT
VOLUME [/opt/couchdb/data]
# Tue, 15 Nov 2022 10:35:48 GMT
EXPOSE 4369 5984 9100
# Tue, 15 Nov 2022 10:35:48 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ac309e879645bf78b5b51a81163cbbaec1a07acab50160803d720a2cd20faa`  
		Last Modified: Tue, 15 Nov 2022 10:37:15 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49844afe089a8ae2b28167131e091ee4187c088c6a872e9325c1d31958cb820e`  
		Last Modified: Tue, 15 Nov 2022 10:37:14 GMT  
		Size: 5.2 MB (5225827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8627dd11a7afca5ddbc0d10ad202fc8c0cc3f7b4e616c5aa496ece15c69c41`  
		Last Modified: Tue, 15 Nov 2022 10:37:13 GMT  
		Size: 1.6 MB (1554043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74501422620a7da2c637583baba5da1d30f26f6914e9904901fe2d1fbcbd0e76`  
		Last Modified: Tue, 15 Nov 2022 10:37:13 GMT  
		Size: 296.3 KB (296279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36940d23f9815532c5e6f5ac48eac39ee6851584fad38d584af6e2d7e08868f8`  
		Last Modified: Tue, 15 Nov 2022 10:37:13 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc41a6e08f50ee957aa8bbdc82b5d63ec2c6070b39131eb7294753615a8a4525`  
		Last Modified: Tue, 15 Nov 2022 10:37:16 GMT  
		Size: 49.0 MB (49047070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64abb1d4412cba2191e7a32e467c78dcc0dc5f66248b85909e2585fcf9da9e6e`  
		Last Modified: Tue, 15 Nov 2022 10:37:11 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c470c6cf30f98b8c7dedcfbb51c7d3b31e28b9b4b054fc28defbc4b849a7c24d`  
		Last Modified: Tue, 15 Nov 2022 10:37:11 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28986f7c1a1bb4a3100d2af60b12e1819fff375e5ffd528ef2e948d4d9606a6b`  
		Last Modified: Tue, 15 Nov 2022 10:37:11 GMT  
		Size: 2.2 KB (2188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2411adc92296964132673b2cbd12ace5e926c6baf3d7f381e7475258440563`  
		Last Modified: Tue, 15 Nov 2022 10:37:11 GMT  
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
$ docker pull couchdb@sha256:c4d14a5a09618880cab6e3e8433192d8281e0e97346b7600fe82eb20867bd44d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93230341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49c2d3582f74ff15b8a063817e6cb657a7861160f88cbc16e1bacb2a4f494cee`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 06 Dec 2022 01:18:04 GMT
ADD file:2231a44ea52d93df58e23883ba6b6911d4c554f4c1d172d80fb21c751ddcbbfc in / 
# Tue, 06 Dec 2022 01:18:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:43:09 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 06 Dec 2022 01:43:11 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 06 Dec 2022 01:43:26 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 01:43:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 06 Dec 2022 01:43:33 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 06 Dec 2022 01:43:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 01:43:45 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 06 Dec 2022 01:43:47 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 06 Dec 2022 01:44:08 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 06 Dec 2022 01:44:10 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 06 Dec 2022 01:44:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 06 Dec 2022 01:44:11 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 06 Dec 2022 01:44:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 06 Dec 2022 01:44:12 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 01:44:13 GMT
VOLUME [/opt/couchdb/data]
# Tue, 06 Dec 2022 01:44:13 GMT
EXPOSE 4369 5984 9100
# Tue, 06 Dec 2022 01:44:14 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:1f72e1168976861c676bf86a6c149129baba7e13200e8b70e6f24dc2ac2797df`  
		Last Modified: Tue, 06 Dec 2022 01:24:18 GMT  
		Size: 35.3 MB (35285293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9651219ecb35e4178b548721d7d579b5bcad3527e218e212f22f49f1d0e737d`  
		Last Modified: Tue, 06 Dec 2022 01:44:37 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a6ae87d9066bfad2d47cacfb42b74ac3ea08ac23f95401d3ead11129b183e6`  
		Last Modified: Tue, 06 Dec 2022 01:44:37 GMT  
		Size: 6.0 MB (6045482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12bc23b90a71bd7b552b15d2eaebdada16d19778cb84909bcdf0a765b1c9e2c`  
		Last Modified: Tue, 06 Dec 2022 01:44:35 GMT  
		Size: 1.5 MB (1509788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b816512cc9ab4899e2488ff00e7575bcc5bf658ead8cfa8a385b8cdc2d69c89`  
		Last Modified: Tue, 06 Dec 2022 01:44:35 GMT  
		Size: 296.2 KB (296210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e052f116409b694b5f652845866ef6a296c7402a169355d9e101b62d4c4aa94`  
		Last Modified: Tue, 06 Dec 2022 01:44:35 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f424b3f99465a604107ba0d3286aebb6515a17c8d01c2b29a6ead5e6b46714`  
		Last Modified: Tue, 06 Dec 2022 01:44:42 GMT  
		Size: 50.1 MB (50086420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b0bb886f364f867efe9470c1cc85dcb481b9ab2b447cf42306ce8676d09dee`  
		Last Modified: Tue, 06 Dec 2022 01:44:33 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073409bf834d911edf2a2911adc4caef2428d48e577c9ae57fa86c4cb5c6eecb`  
		Last Modified: Tue, 06 Dec 2022 01:44:33 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b7c8a9cef21a2d437cbb4d2236784a5d38e6bc56e563908c03f8a3cb10c66ce`  
		Last Modified: Tue, 06 Dec 2022 01:44:33 GMT  
		Size: 2.2 KB (2187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b3e69b9284e828a40354df4b63224c55b3b9413b6592e7e6659599846c75db`  
		Last Modified: Tue, 06 Dec 2022 01:44:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
