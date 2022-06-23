## `couchdb:latest`

```console
$ docker pull couchdb@sha256:fac1dafe010ce15c56f967c6fe9cb26fa3be8032ce9cea433265d7b00af63c11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:3ea7f178b119a1bbd2adbec78486241a087ba35d1d3ec9128a3ada704d55ec97
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87498751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ee9d2dcf03aa6b53788baca7b138c9069926ce70119f77c999d0e2d0858e21d`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:27 GMT
ADD file:8adbbab04d6f84cd83b5f4205b89b0acb7ecbf27a1bb2dc181d0a629479039fe in / 
# Thu, 23 Jun 2022 00:20:27 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:06:19 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 23 Jun 2022 01:06:19 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 23 Jun 2022 01:06:26 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:06:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 23 Jun 2022 01:06:30 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 23 Jun 2022 01:06:35 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:06:35 GMT
ENV COUCHDB_VERSION=3.2.2
# Thu, 23 Jun 2022 01:06:36 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 23 Jun 2022 01:06:48 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 23 Jun 2022 01:06:49 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 23 Jun 2022 01:06:49 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 23 Jun 2022 01:06:49 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Thu, 23 Jun 2022 01:06:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 01:06:50 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 23 Jun 2022 01:06:50 GMT
VOLUME [/opt/couchdb/data]
# Thu, 23 Jun 2022 01:06:50 GMT
EXPOSE 4369 5984 9100
# Thu, 23 Jun 2022 01:06:50 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b85a868b505ffd0342a37e6a3b1c49f7c71878afe569a807e6238ef08252fcb7`  
		Last Modified: Thu, 23 Jun 2022 00:25:18 GMT  
		Size: 31.4 MB (31379408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4b67ef10ab3031244bf995ed483d30c4423feb9f42f12d55c8511d7497c931`  
		Last Modified: Thu, 23 Jun 2022 01:08:14 GMT  
		Size: 3.4 KB (3410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd945ed68b3fecb83857780d70642d81019952136407b87a9f4b6b94711e7dda`  
		Last Modified: Thu, 23 Jun 2022 01:08:13 GMT  
		Size: 5.2 MB (5224047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1d67ad9668554764252390c4e5b06fb0f33517e33a831601a00c10a05cfbe7`  
		Last Modified: Thu, 23 Jun 2022 01:08:13 GMT  
		Size: 1.6 MB (1553288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b56aaaffae17f3010ab5ba52d88e22126a8b18f5f8fd49ea4a01655c55e20b`  
		Last Modified: Thu, 23 Jun 2022 01:08:12 GMT  
		Size: 295.6 KB (295555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e601de752a6ea7ddb9a0b7201437219d647dd0a6555b1d9f48ae8d94004f40`  
		Last Modified: Thu, 23 Jun 2022 01:08:12 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbd769730295be73a2aae5a0882ad80bb9284ad34c68bff96c93ccd15f3cc73`  
		Last Modified: Thu, 23 Jun 2022 01:08:15 GMT  
		Size: 49.0 MB (49039317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec0fe21a89a509108c6d599b399458e374353649854cc07814e901deb7030198`  
		Last Modified: Thu, 23 Jun 2022 01:08:10 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9700366d2b2b831d620b0ee23a1b1ed39c86a91aa69aaad560465e5dd33889`  
		Last Modified: Thu, 23 Jun 2022 01:08:10 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd356f58092365eb5086db70cc449f1fce114ea73ac0ee9bc18298ac6c579120`  
		Last Modified: Thu, 23 Jun 2022 01:08:10 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f797d1e3134f5eda53222acba18a0644f920f20c2431b5b3604ab90b7d882c09`  
		Last Modified: Thu, 23 Jun 2022 01:08:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:963c6bdce2865332088af6db49b38fa74bf976524a961428a7f9722bc9eef2d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.4 MB (85427248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97a3f9bc4086335eba387e8861b885c1c1dc01693341c683f8bd6a301930b7c1`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:30:26 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 23 Jun 2022 01:30:27 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 23 Jun 2022 01:30:35 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:30:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 23 Jun 2022 01:30:39 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 23 Jun 2022 01:30:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:30:46 GMT
ENV COUCHDB_VERSION=3.2.2
# Thu, 23 Jun 2022 01:30:47 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 23 Jun 2022 01:31:05 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 23 Jun 2022 01:31:06 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 23 Jun 2022 01:31:07 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 23 Jun 2022 01:31:08 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Thu, 23 Jun 2022 01:31:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 23 Jun 2022 01:31:09 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 23 Jun 2022 01:31:10 GMT
VOLUME [/opt/couchdb/data]
# Thu, 23 Jun 2022 01:31:11 GMT
EXPOSE 4369 5984 9100
# Thu, 23 Jun 2022 01:31:12 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382e4beb83730624f8bcf51b1774b4100e1e412f82bf7581c2102c32d21babc2`  
		Last Modified: Thu, 23 Jun 2022 01:33:14 GMT  
		Size: 3.3 KB (3319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e72f96be5467954693838bc974a9b240de99dc781c890b8854a9b72ffe7810`  
		Last Modified: Thu, 23 Jun 2022 01:33:12 GMT  
		Size: 5.0 MB (5003043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1fe9d6128b137e4021863af326262d53382dc923b8253440d8c35dca9346dc`  
		Last Modified: Thu, 23 Jun 2022 01:33:12 GMT  
		Size: 1.2 MB (1221097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8033bc1cbfbb70b4bd70c8b6b05f4b51d787550ec906faaf7058fc28d2e0d541`  
		Last Modified: Thu, 23 Jun 2022 01:33:11 GMT  
		Size: 79.2 KB (79250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a155e5dda342d8db092d0838f17a385cac7c9e6b675c52aa622eab8691e9d436`  
		Last Modified: Thu, 23 Jun 2022 01:33:11 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060f539b2f3aceca17ca461e400c845f07355901db19b62abd957e9f73637648`  
		Last Modified: Thu, 23 Jun 2022 01:33:15 GMT  
		Size: 49.1 MB (49051089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8329e9015b73d2e5486a08a39b87b23aed1ec9c1ab1e696789f89e27827f751`  
		Last Modified: Thu, 23 Jun 2022 01:33:09 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d30a74bb6d8fc4574cf72fe64367d6ad19cd0054333a0910265d35011060b0c1`  
		Last Modified: Thu, 23 Jun 2022 01:33:09 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302e3d24862203426b8ad799b0ccf323a227be762d42c8592d9de3cf67c47377`  
		Last Modified: Thu, 23 Jun 2022 01:33:09 GMT  
		Size: 2.2 KB (2185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66b8990f4d7ba62fff96860921dae1c48d5826104ead7d5d1d6574470b914a1`  
		Last Modified: Thu, 23 Jun 2022 01:33:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; ppc64le

```console
$ docker pull couchdb@sha256:f95e2cea87b96ad9d1f58b2f7a1cc297fafa4a0ba2ac8264ac49d1638308fc9f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93222784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64b27bcbda415fb7a19f938be7247b5b8374059229cdc9cd529fb5307a210896`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Sat, 28 May 2022 01:22:54 GMT
ADD file:64e264b12eed99d87380e38f36bfecd62b9bb1e5460f0242cfbc5dc76c212ead in / 
# Sat, 28 May 2022 01:22:59 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:40:22 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 28 May 2022 03:40:30 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 28 May 2022 03:41:22 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:41:35 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Sat, 28 May 2022 03:41:39 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Sat, 28 May 2022 03:42:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:42:07 GMT
ENV COUCHDB_VERSION=3.2.2
# Sat, 28 May 2022 03:42:12 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Sat, 28 May 2022 03:42:55 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 28 May 2022 03:42:58 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 28 May 2022 03:42:59 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 28 May 2022 03:43:00 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Sat, 28 May 2022 03:43:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 28 May 2022 03:43:09 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 28 May 2022 03:43:12 GMT
VOLUME [/opt/couchdb/data]
# Sat, 28 May 2022 03:43:14 GMT
EXPOSE 4369 5984 9100
# Sat, 28 May 2022 03:43:17 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:893e245a8f6219935016f2dd4422ec4b7fdab43d98ba29c024ec0d9ce57794ba`  
		Last Modified: Sat, 28 May 2022 01:32:28 GMT  
		Size: 35.3 MB (35286698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:875b56da848a25def16ef02568eeffc6bbc68f8a2468a40da18f7804d2dd4dc9`  
		Last Modified: Sat, 28 May 2022 03:43:47 GMT  
		Size: 3.4 KB (3410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c308e008e7e9f9a18c5718a2d3de1662a1db954494a646fdf8ba6d823e164163`  
		Last Modified: Sat, 28 May 2022 03:43:46 GMT  
		Size: 6.0 MB (6043917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5459503824efb70b765dc12230fae1a2e7f1d57ba12e7e9167fb178b49e2d7eb`  
		Last Modified: Sat, 28 May 2022 03:43:45 GMT  
		Size: 1.5 MB (1509317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc78eafedf794548c6bb2337ef3e6c836e38b32b8614595cba142a46bf2e9dd7`  
		Last Modified: Sat, 28 May 2022 03:43:44 GMT  
		Size: 295.7 KB (295711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a0c9e549e3260acc9bf35d347a6d917255de993dd25ed0b87d3e42a07e7db8`  
		Last Modified: Sat, 28 May 2022 03:43:44 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a195ecb14f19305eece3c42f9ca34a34d6b56c3068466d8bb2bbd3e718b6946e`  
		Last Modified: Sat, 28 May 2022 03:43:52 GMT  
		Size: 50.1 MB (50080003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12dfd3f63efba486fe137f4f549db8e61c85af415f596ed332b7c0c8b59ee455`  
		Last Modified: Sat, 28 May 2022 03:43:42 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b986d6fa4c295a869df86de585d8914fe5b1a862f8bd8b6e7eb7b271f8095833`  
		Last Modified: Sat, 28 May 2022 03:43:42 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa73f76a3e72dfaf15f902a8ab24390ed60ac0c9ee076c28ea9e6b81e55ce9a`  
		Last Modified: Sat, 28 May 2022 03:43:42 GMT  
		Size: 2.2 KB (2183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e53af1ea2a6650916769ea2f4ba0611b52a7bc36e0e0c1d740aeb583a7add7`  
		Last Modified: Sat, 28 May 2022 03:43:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
