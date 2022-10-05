## `couchdb:latest`

```console
$ docker pull couchdb@sha256:56a4221d164353188dfa070af3daaa4a098908956f17a191c5341746e19781ec
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
$ docker pull couchdb@sha256:143e3cd2945cb48d796d2278db9557504a800c77299549c9ac183576f1b6c918
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93229895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7711c8b3c5ab31870f4215b49471ddd8fa0a590d524a9b20be6af5f450232aa`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 04 Oct 2022 23:18:04 GMT
ADD file:66a0f55a4b4dfbb5d64082ffdb24751f20c5773039277ba278fdb4ce4a538c33 in / 
# Tue, 04 Oct 2022 23:18:06 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:08:24 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 05 Oct 2022 00:08:26 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 05 Oct 2022 00:08:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:08:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 05 Oct 2022 00:08:50 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 05 Oct 2022 00:09:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:09:02 GMT
ENV COUCHDB_VERSION=3.2.2
# Wed, 05 Oct 2022 00:09:03 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 05 Oct 2022 00:09:26 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 05 Oct 2022 00:09:28 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 05 Oct 2022 00:09:28 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 05 Oct 2022 00:09:29 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 05 Oct 2022 00:09:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 00:09:30 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 00:09:31 GMT
VOLUME [/opt/couchdb/data]
# Wed, 05 Oct 2022 00:09:31 GMT
EXPOSE 4369 5984 9100
# Wed, 05 Oct 2022 00:09:31 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:4e001127162dd884a6f7bd2e6f74215816d325bebb3a374ae9fcee9f038f99b8`  
		Last Modified: Tue, 04 Oct 2022 23:24:13 GMT  
		Size: 35.3 MB (35290584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381109cbfbaaa798f564a18947f6c0f1dd5910da0234beab17bd5819ea39399d`  
		Last Modified: Wed, 05 Oct 2022 00:09:54 GMT  
		Size: 3.4 KB (3410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395cceb53989fdd5e1a8a72b46ca77b7d6663f50db82d16939a22fc6bc490b0d`  
		Last Modified: Wed, 05 Oct 2022 00:09:54 GMT  
		Size: 6.0 MB (6043722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c601f28412075f4767666bf160d562b535fd07b9fb959ef7ff65f470e5554bb`  
		Last Modified: Wed, 05 Oct 2022 00:09:52 GMT  
		Size: 1.5 MB (1509160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908145ec6ae093dd2fcc342bd38df282b5851f529d6b3a835ac93d69aaa33424`  
		Last Modified: Wed, 05 Oct 2022 00:09:52 GMT  
		Size: 295.5 KB (295506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f5839c8ec51b87036b5260c4c50c7b68102134e73a620710ba0c6c551e02cc`  
		Last Modified: Wed, 05 Oct 2022 00:09:52 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf4fabbea2bc9c827bf92aa5c2f2d24249508e1f71a1228e328d2611e0d899c`  
		Last Modified: Wed, 05 Oct 2022 00:09:59 GMT  
		Size: 50.1 MB (50083786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:435f63e26726324a42486d58656d232b9a7a902119575252fbd7326ff3e78f12`  
		Last Modified: Wed, 05 Oct 2022 00:09:50 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d3b1210769a993aa36f893916060dffb032025964550b36c01181138dc64f74`  
		Last Modified: Wed, 05 Oct 2022 00:09:49 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ab88b6abdfeff6d61bc12392dd5649756851f5b7dda2e77bea1bbea2f90038`  
		Last Modified: Wed, 05 Oct 2022 00:09:50 GMT  
		Size: 2.2 KB (2187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2fcd7203df115c27ce9f60eea1502476c8d59cc71edf4c6f0994b0a78b200c`  
		Last Modified: Wed, 05 Oct 2022 00:09:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
