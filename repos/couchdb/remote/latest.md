## `couchdb:latest`

```console
$ docker pull couchdb@sha256:f00e527a2396094e356e2b95d869c918e95641de8b57a34c2eb3498719464c61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:ac5c57c4df9f9d0129390f652b62dfa348a1b383c458841010ad52abbb6c8f0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87530196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9292db79eb5d3107963496f664c9764d4974a423cff1612702d8ca782a888f5`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:29 GMT
ADD file:5bd53bff884e470b3c12425132975ab9c6f99002c62c43bca1ff5cde9d863b92 in / 
# Tue, 13 Sep 2022 00:56:29 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:53:59 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Sep 2022 03:54:00 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Sep 2022 03:54:07 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:54:10 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 13 Sep 2022 03:54:10 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Sep 2022 03:54:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:54:16 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 13 Sep 2022 03:54:16 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Sep 2022 03:54:29 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Sep 2022 03:54:30 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Sep 2022 03:54:30 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 13 Sep 2022 03:54:30 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 13 Sep 2022 03:54:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 03:54:30 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Sep 2022 03:54:31 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Sep 2022 03:54:31 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Sep 2022 03:54:31 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:31b3f1ad4ce1f369084d0f959813c51df0ca17d9877d5ee88c2db6ff88341430`  
		Last Modified: Tue, 13 Sep 2022 01:00:29 GMT  
		Size: 31.4 MB (31404121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9775a4fbb4b5564bbc1ec8e077d317b8745a7598e059365241ddc1a9766c129c`  
		Last Modified: Tue, 13 Sep 2022 03:55:55 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d707a0a4de816f6a35046bed27c3bd025081394b651fd4b339188a4e19967c4`  
		Last Modified: Tue, 13 Sep 2022 03:55:54 GMT  
		Size: 5.2 MB (5224215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c15634eb84187cbacfe864298c664c5eb740aa1a455a39e64f4f6a94c0f07a14`  
		Last Modified: Tue, 13 Sep 2022 03:55:53 GMT  
		Size: 1.6 MB (1553277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59f0fe4ba863352dbd7372301d2eae5be8cd69838e66876a65c5c0b1666de8c`  
		Last Modified: Tue, 13 Sep 2022 03:55:53 GMT  
		Size: 295.6 KB (295573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f507b233637bff8bdab3e80909e9dcdcc02a11efcca3f242c4ae8bf410296bbe`  
		Last Modified: Tue, 13 Sep 2022 03:55:53 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a76624d812c6c764f46d961f80510fa92e7512419c528ba6ab86e250d365d8`  
		Last Modified: Tue, 13 Sep 2022 03:55:56 GMT  
		Size: 49.0 MB (49045868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6166f23a925f2a6a18aa9efa186271f01020d8fd5d40d7a307cb02d6172974`  
		Last Modified: Tue, 13 Sep 2022 03:55:50 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc867e39bf60d67febf095d33500f8b30b51f6edbef26bd9d37b7a38a9bfaebc`  
		Last Modified: Tue, 13 Sep 2022 03:55:50 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5bc74ba5f149b1005fb23f07d5b84e4946fc31381d124892f99322b8c9a202`  
		Last Modified: Tue, 13 Sep 2022 03:55:50 GMT  
		Size: 2.2 KB (2187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7ff75922f5a116b20c00eabe11b5280455fc7c77595f4ae03ed74a4e45ffb41`  
		Last Modified: Tue, 13 Sep 2022 03:55:50 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:8ab6f02f40e97fea4c834a90934e56fe7850abce916702b11a4b5d6740d161fc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.6 MB (85626156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb4d1c6ffd6d7f1bf64a2744e7edea3ba1e5f129d6b1ecd81cb0f2b55aaada31`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:56 GMT
ADD file:e8f00260a993aacae732bef51e6074b6c064d50a8ce1f0c44d53fe9e3c868e43 in / 
# Tue, 13 Sep 2022 02:10:56 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 13:43:41 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Sep 2022 13:43:42 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Sep 2022 13:43:50 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 13:43:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 13 Sep 2022 13:43:54 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Sep 2022 13:44:00 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 13:44:01 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 13 Sep 2022 13:44:02 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Sep 2022 13:44:21 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Sep 2022 13:44:22 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Sep 2022 13:44:23 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 13 Sep 2022 13:44:24 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 13 Sep 2022 13:44:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 13:44:25 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Sep 2022 13:44:26 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Sep 2022 13:44:27 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Sep 2022 13:44:28 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:3d898485473e3507374cea2e09f019c2ff5728f0911aa36c70b7a7235e9bc8ac`  
		Last Modified: Tue, 13 Sep 2022 02:16:19 GMT  
		Size: 30.1 MB (30054239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df4be65845e06938882e60b2adaaaa4f5af8dad0485a86f9b391d3a89e0dc476`  
		Last Modified: Tue, 13 Sep 2022 13:46:28 GMT  
		Size: 3.3 KB (3321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c57696a64df0068d00c4b40c44347727692e96f1b9628b60acbe09a292f8b163`  
		Last Modified: Tue, 13 Sep 2022 13:46:26 GMT  
		Size: 5.2 MB (5207937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1124b5a50be1aa76caeed0e8df5b91708dae04bf90bf0924c9195debdaef7f84`  
		Last Modified: Tue, 13 Sep 2022 13:46:25 GMT  
		Size: 1.2 MB (1221121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a0dfbbe063cc9c5bb129c2a32ae2a437375da28a080bd9ebbb7caa572c9e94`  
		Last Modified: Tue, 13 Sep 2022 13:46:25 GMT  
		Size: 79.2 KB (79231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6953c42d9f58c5776a6ac1943540c187223cabce11ccc121116607149a50721f`  
		Last Modified: Tue, 13 Sep 2022 13:46:25 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a525805cfb803ec268f9fef2f85948356175ae8d5ea356e9d632c9061a8784b0`  
		Last Modified: Tue, 13 Sep 2022 13:46:29 GMT  
		Size: 49.1 MB (49056583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff8c6a3aab4679325554887946af400c1a4634d83e25d392c576d2c0e72b7e3`  
		Last Modified: Tue, 13 Sep 2022 13:46:23 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8daf3297e98d68337a84abdf40fdeaa8e000944f140a208ef7eb145f92b97e22`  
		Last Modified: Tue, 13 Sep 2022 13:46:23 GMT  
		Size: 762.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1196ff1efc04714eeed6a1fd68b5dd42c135f8f8414d8c79f39cf2f66ccd0ca7`  
		Last Modified: Tue, 13 Sep 2022 13:46:23 GMT  
		Size: 2.2 KB (2185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14da08c81908c7e967ae2363d02e1540977885675c86246a1aa915f47eb9bfad`  
		Last Modified: Tue, 13 Sep 2022 13:46:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; ppc64le

```console
$ docker pull couchdb@sha256:521fb0e82f3368e3fe7da98ec7f58e57c7ef55af2b13573ca6295f353b661644
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93218160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7df38e26c1b01270057c94a8a17d39b3a4b5a5e414ad649479d1886ee838b38f`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 13 Sep 2022 02:07:56 GMT
ADD file:8b05dcf5f16a2ae9169b27aa848b812e07cd30414e51e4d53df9a5f01cd4c1a4 in / 
# Tue, 13 Sep 2022 02:07:58 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 05:28:59 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 13 Sep 2022 05:29:00 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 13 Sep 2022 05:29:14 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 05:29:21 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 13 Sep 2022 05:29:21 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 13 Sep 2022 05:29:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 05:29:34 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 13 Sep 2022 05:29:35 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 13 Sep 2022 05:29:57 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 13 Sep 2022 05:29:59 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 13 Sep 2022 05:30:00 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 13 Sep 2022 05:30:00 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 13 Sep 2022 05:30:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 05:30:01 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 13 Sep 2022 05:30:02 GMT
VOLUME [/opt/couchdb/data]
# Tue, 13 Sep 2022 05:30:02 GMT
EXPOSE 4369 5984 9100
# Tue, 13 Sep 2022 05:30:02 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:9716ed411387b5ba1ec8278e9fb108a44d8a09ffbbbfd1639f06c63f20364b45`  
		Last Modified: Tue, 13 Sep 2022 02:13:40 GMT  
		Size: 35.3 MB (35277392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d43f2bb2e2de6f6b1f08bd3f7a2709e6c761c74eee7671b41ea40cab1610501`  
		Last Modified: Tue, 13 Sep 2022 05:30:26 GMT  
		Size: 3.4 KB (3410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391586b0a120d8818bdf70c22c5f8c6d4e5b761f9f38a512ed57f61e398af755`  
		Last Modified: Tue, 13 Sep 2022 05:30:25 GMT  
		Size: 6.0 MB (6043732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd86580ba66721f3987a3b59b6d0744c3b98d33da0bdc936251964b4aa4f538c`  
		Last Modified: Tue, 13 Sep 2022 05:30:24 GMT  
		Size: 1.5 MB (1509157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ec816b1ffced464580155415e10f538a59d71bf4de6d72a2b317193b0f1d5e`  
		Last Modified: Tue, 13 Sep 2022 05:30:24 GMT  
		Size: 295.5 KB (295523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbaf5276605d31d34be219fed245d433add9c7a2504d065e0d1941d1e54bef4d`  
		Last Modified: Tue, 13 Sep 2022 05:30:24 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a05e74bbd7bffd25c59b82d4f5cd99beeace738e91dbf6031c7996ae53c85cf`  
		Last Modified: Tue, 13 Sep 2022 05:30:31 GMT  
		Size: 50.1 MB (50085213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01207b543dae2d302ebffc5ed1717e86985f71ff665a782e72db3466320b042`  
		Last Modified: Tue, 13 Sep 2022 05:30:21 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43de669bd6602f9f4052ff576e68160523fd062ee7c9314d23c9308ca44f2b40`  
		Last Modified: Tue, 13 Sep 2022 05:30:21 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ae3c6e9b7e4bf652090555957aa2f2942a67945febfd0a073e3061d761fa22`  
		Last Modified: Tue, 13 Sep 2022 05:30:21 GMT  
		Size: 2.2 KB (2188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21da6a4761ece80a750ae0df3baef58f53e3a2fb009b1c693e63f5a2d671971`  
		Last Modified: Tue, 13 Sep 2022 05:30:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
