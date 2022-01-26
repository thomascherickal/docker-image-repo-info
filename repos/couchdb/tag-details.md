<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `couchdb`

-	[`couchdb:2`](#couchdb2)
-	[`couchdb:2.3`](#couchdb23)
-	[`couchdb:2.3.1`](#couchdb231)
-	[`couchdb:3`](#couchdb3)
-	[`couchdb:3.1`](#couchdb31)
-	[`couchdb:3.1.2`](#couchdb312)
-	[`couchdb:3.2`](#couchdb32)
-	[`couchdb:3.2.1`](#couchdb321)
-	[`couchdb:latest`](#couchdblatest)

## `couchdb:2`

```console
$ docker pull couchdb@sha256:7dd10ed219d292cba7e65e1dd123085389b3f6b93d291823a39297b5c0323356
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2` - linux; amd64

```console
$ docker pull couchdb@sha256:4ab72c0332f55ab6dd8059c150803e90a12ec9cb9378dd427c306204e8c1e41f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84517393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b82088c4dbbbd17c9ffb41f7d820af88b3c6073268e43c338f8807492c9281c8`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:32:37 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 26 Jan 2022 02:32:38 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 26 Jan 2022 02:32:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:32:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 26 Jan 2022 02:32:54 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 26 Jan 2022 02:33:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:33:49 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 26 Jan 2022 02:33:50 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 26 Jan 2022 02:34:09 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Jan 2022 02:34:10 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 26 Jan 2022 02:34:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 26 Jan 2022 02:34:10 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 26 Jan 2022 02:34:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 02:34:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 26 Jan 2022 02:34:12 GMT
VOLUME [/opt/couchdb/data]
# Wed, 26 Jan 2022 02:34:12 GMT
EXPOSE 4369 5984 9100
# Wed, 26 Jan 2022 02:34:12 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2303b379bad4b145fe698823516aef43ea73893435a56d56461915d3b67e5ab1`  
		Last Modified: Wed, 26 Jan 2022 02:34:36 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e159d27bba2524eba26ded6aaf13a78457ce9243d40892098fba794fa0d3367`  
		Last Modified: Wed, 26 Jan 2022 02:34:35 GMT  
		Size: 6.7 MB (6691340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3664a86635c3e52a3c405c92976b193da350069cd0d39885217558722501adc3`  
		Last Modified: Wed, 26 Jan 2022 02:34:34 GMT  
		Size: 1.3 MB (1258362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0206c27a3c9eb755f3fc3ea0dd401a0b9ca39beb997f6aba6f29291c70a66d0c`  
		Last Modified: Wed, 26 Jan 2022 02:34:34 GMT  
		Size: 293.0 KB (293041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34765ab501aabe41ffeef7aab12d2ebc2dfe83d56ad878597696b89747a63dac`  
		Last Modified: Wed, 26 Jan 2022 02:35:15 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d591bef59be521b2fc6356caac9ef1ff8a7577ff3f02ea30ca11242e6cc0cdf7`  
		Last Modified: Wed, 26 Jan 2022 02:35:19 GMT  
		Size: 49.1 MB (49113904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dfe9e7899557ea2d3ad94893f2fabed57dfa577a89cddc25a6e15c6800aa402`  
		Last Modified: Wed, 26 Jan 2022 02:35:12 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f956d2382a7998d1b628f5cacc29786d98e01e08bbc428928aca4c32df1ff617`  
		Last Modified: Wed, 26 Jan 2022 02:35:12 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deba864ada3af15db9694092245c13b7805ea46d9b682ce6275e5e214f692ab6`  
		Last Modified: Wed, 26 Jan 2022 02:35:12 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b79c471aa6dd817b6dcfbbcd37c623b6c2e35fcbe9b75c5496e44008cde4e26`  
		Last Modified: Wed, 26 Jan 2022 02:35:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:a8910eda154fb2670cebf4cc072a18307c893a00d5d3fb39d83e4bd3e3682222
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72523043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8ba16fe8039bb0b2a7105771aa4eeb593488cfbf04163e0953ca12d599013a7`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:33:55 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 26 Jan 2022 02:33:56 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 26 Jan 2022 02:34:04 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:34:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 26 Jan 2022 02:34:09 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 26 Jan 2022 02:34:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:35:33 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 26 Jan 2022 02:35:34 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 26 Jan 2022 02:35:52 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Jan 2022 02:35:53 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 26 Jan 2022 02:35:54 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 26 Jan 2022 02:35:55 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 26 Jan 2022 02:35:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 02:35:56 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 26 Jan 2022 02:35:57 GMT
VOLUME [/opt/couchdb/data]
# Wed, 26 Jan 2022 02:35:58 GMT
EXPOSE 4369 5984 9100
# Wed, 26 Jan 2022 02:35:59 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22044b828c1c3fec0f66406d0b4914affa5a4c233a8d1a024e840db18c3717ef`  
		Last Modified: Wed, 26 Jan 2022 02:36:29 GMT  
		Size: 3.3 KB (3322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0132d29a5665e429cb69b2ed2fc2161bcc92bbd0a38d0641b9f514400bd6a0d1`  
		Last Modified: Wed, 26 Jan 2022 02:36:28 GMT  
		Size: 6.5 MB (6549949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6721695d9885aa7b6fb16b43b993093ab01fe96b75f137ad3e7760abf4b73a`  
		Last Modified: Wed, 26 Jan 2022 02:36:27 GMT  
		Size: 951.2 KB (951153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a62fc4090c90113d86eaece64a0ad9474d88e015afa7c449020962191af77f`  
		Last Modified: Wed, 26 Jan 2022 02:36:26 GMT  
		Size: 79.9 KB (79897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a54380ddace77254d3a7eef5aea81131a1c70a1ab560ab9f7c2288b37fe9288`  
		Last Modified: Wed, 26 Jan 2022 02:37:06 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6fba6e4534a2d397cbc79ca495f925dca6384c78ff2a35736ce104f11a50d32`  
		Last Modified: Wed, 26 Jan 2022 02:37:09 GMT  
		Size: 39.0 MB (39011903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fada3abcceccd793c9fb393c41d7993c4af1d1741878cdd3ecbdbb148f4e90`  
		Last Modified: Wed, 26 Jan 2022 02:37:04 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f971f5f71777b59bf08438f14025fb9610ec4f00314708fa849d239ebbe6fede`  
		Last Modified: Wed, 26 Jan 2022 02:37:04 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c341e2778945c5566e24ea5c9c95094d1fa0512c377996f005aa6ff413e237a`  
		Last Modified: Wed, 26 Jan 2022 02:37:04 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1bc007a15a59f1b8238cbe6cd01e252c5d593ba5ea9b6273e249d41730ae68`  
		Last Modified: Wed, 26 Jan 2022 02:37:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3`

```console
$ docker pull couchdb@sha256:7dd10ed219d292cba7e65e1dd123085389b3f6b93d291823a39297b5c0323356
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:4ab72c0332f55ab6dd8059c150803e90a12ec9cb9378dd427c306204e8c1e41f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84517393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b82088c4dbbbd17c9ffb41f7d820af88b3c6073268e43c338f8807492c9281c8`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:32:37 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 26 Jan 2022 02:32:38 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 26 Jan 2022 02:32:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:32:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 26 Jan 2022 02:32:54 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 26 Jan 2022 02:33:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:33:49 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 26 Jan 2022 02:33:50 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 26 Jan 2022 02:34:09 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Jan 2022 02:34:10 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 26 Jan 2022 02:34:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 26 Jan 2022 02:34:10 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 26 Jan 2022 02:34:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 02:34:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 26 Jan 2022 02:34:12 GMT
VOLUME [/opt/couchdb/data]
# Wed, 26 Jan 2022 02:34:12 GMT
EXPOSE 4369 5984 9100
# Wed, 26 Jan 2022 02:34:12 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2303b379bad4b145fe698823516aef43ea73893435a56d56461915d3b67e5ab1`  
		Last Modified: Wed, 26 Jan 2022 02:34:36 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e159d27bba2524eba26ded6aaf13a78457ce9243d40892098fba794fa0d3367`  
		Last Modified: Wed, 26 Jan 2022 02:34:35 GMT  
		Size: 6.7 MB (6691340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3664a86635c3e52a3c405c92976b193da350069cd0d39885217558722501adc3`  
		Last Modified: Wed, 26 Jan 2022 02:34:34 GMT  
		Size: 1.3 MB (1258362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0206c27a3c9eb755f3fc3ea0dd401a0b9ca39beb997f6aba6f29291c70a66d0c`  
		Last Modified: Wed, 26 Jan 2022 02:34:34 GMT  
		Size: 293.0 KB (293041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34765ab501aabe41ffeef7aab12d2ebc2dfe83d56ad878597696b89747a63dac`  
		Last Modified: Wed, 26 Jan 2022 02:35:15 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d591bef59be521b2fc6356caac9ef1ff8a7577ff3f02ea30ca11242e6cc0cdf7`  
		Last Modified: Wed, 26 Jan 2022 02:35:19 GMT  
		Size: 49.1 MB (49113904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dfe9e7899557ea2d3ad94893f2fabed57dfa577a89cddc25a6e15c6800aa402`  
		Last Modified: Wed, 26 Jan 2022 02:35:12 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f956d2382a7998d1b628f5cacc29786d98e01e08bbc428928aca4c32df1ff617`  
		Last Modified: Wed, 26 Jan 2022 02:35:12 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deba864ada3af15db9694092245c13b7805ea46d9b682ce6275e5e214f692ab6`  
		Last Modified: Wed, 26 Jan 2022 02:35:12 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b79c471aa6dd817b6dcfbbcd37c623b6c2e35fcbe9b75c5496e44008cde4e26`  
		Last Modified: Wed, 26 Jan 2022 02:35:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:a8910eda154fb2670cebf4cc072a18307c893a00d5d3fb39d83e4bd3e3682222
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72523043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8ba16fe8039bb0b2a7105771aa4eeb593488cfbf04163e0953ca12d599013a7`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:33:55 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 26 Jan 2022 02:33:56 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 26 Jan 2022 02:34:04 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:34:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 26 Jan 2022 02:34:09 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 26 Jan 2022 02:34:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:35:33 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 26 Jan 2022 02:35:34 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 26 Jan 2022 02:35:52 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Jan 2022 02:35:53 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 26 Jan 2022 02:35:54 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 26 Jan 2022 02:35:55 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 26 Jan 2022 02:35:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 02:35:56 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 26 Jan 2022 02:35:57 GMT
VOLUME [/opt/couchdb/data]
# Wed, 26 Jan 2022 02:35:58 GMT
EXPOSE 4369 5984 9100
# Wed, 26 Jan 2022 02:35:59 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22044b828c1c3fec0f66406d0b4914affa5a4c233a8d1a024e840db18c3717ef`  
		Last Modified: Wed, 26 Jan 2022 02:36:29 GMT  
		Size: 3.3 KB (3322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0132d29a5665e429cb69b2ed2fc2161bcc92bbd0a38d0641b9f514400bd6a0d1`  
		Last Modified: Wed, 26 Jan 2022 02:36:28 GMT  
		Size: 6.5 MB (6549949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6721695d9885aa7b6fb16b43b993093ab01fe96b75f137ad3e7760abf4b73a`  
		Last Modified: Wed, 26 Jan 2022 02:36:27 GMT  
		Size: 951.2 KB (951153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a62fc4090c90113d86eaece64a0ad9474d88e015afa7c449020962191af77f`  
		Last Modified: Wed, 26 Jan 2022 02:36:26 GMT  
		Size: 79.9 KB (79897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a54380ddace77254d3a7eef5aea81131a1c70a1ab560ab9f7c2288b37fe9288`  
		Last Modified: Wed, 26 Jan 2022 02:37:06 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6fba6e4534a2d397cbc79ca495f925dca6384c78ff2a35736ce104f11a50d32`  
		Last Modified: Wed, 26 Jan 2022 02:37:09 GMT  
		Size: 39.0 MB (39011903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fada3abcceccd793c9fb393c41d7993c4af1d1741878cdd3ecbdbb148f4e90`  
		Last Modified: Wed, 26 Jan 2022 02:37:04 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f971f5f71777b59bf08438f14025fb9610ec4f00314708fa849d239ebbe6fede`  
		Last Modified: Wed, 26 Jan 2022 02:37:04 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c341e2778945c5566e24ea5c9c95094d1fa0512c377996f005aa6ff413e237a`  
		Last Modified: Wed, 26 Jan 2022 02:37:04 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1bc007a15a59f1b8238cbe6cd01e252c5d593ba5ea9b6273e249d41730ae68`  
		Last Modified: Wed, 26 Jan 2022 02:37:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3.1`

```console
$ docker pull couchdb@sha256:7dd10ed219d292cba7e65e1dd123085389b3f6b93d291823a39297b5c0323356
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:4ab72c0332f55ab6dd8059c150803e90a12ec9cb9378dd427c306204e8c1e41f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84517393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b82088c4dbbbd17c9ffb41f7d820af88b3c6073268e43c338f8807492c9281c8`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:32:37 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 26 Jan 2022 02:32:38 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 26 Jan 2022 02:32:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:32:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 26 Jan 2022 02:32:54 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 26 Jan 2022 02:33:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:33:49 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 26 Jan 2022 02:33:50 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 26 Jan 2022 02:34:09 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Jan 2022 02:34:10 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 26 Jan 2022 02:34:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 26 Jan 2022 02:34:10 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 26 Jan 2022 02:34:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 02:34:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 26 Jan 2022 02:34:12 GMT
VOLUME [/opt/couchdb/data]
# Wed, 26 Jan 2022 02:34:12 GMT
EXPOSE 4369 5984 9100
# Wed, 26 Jan 2022 02:34:12 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2303b379bad4b145fe698823516aef43ea73893435a56d56461915d3b67e5ab1`  
		Last Modified: Wed, 26 Jan 2022 02:34:36 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e159d27bba2524eba26ded6aaf13a78457ce9243d40892098fba794fa0d3367`  
		Last Modified: Wed, 26 Jan 2022 02:34:35 GMT  
		Size: 6.7 MB (6691340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3664a86635c3e52a3c405c92976b193da350069cd0d39885217558722501adc3`  
		Last Modified: Wed, 26 Jan 2022 02:34:34 GMT  
		Size: 1.3 MB (1258362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0206c27a3c9eb755f3fc3ea0dd401a0b9ca39beb997f6aba6f29291c70a66d0c`  
		Last Modified: Wed, 26 Jan 2022 02:34:34 GMT  
		Size: 293.0 KB (293041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34765ab501aabe41ffeef7aab12d2ebc2dfe83d56ad878597696b89747a63dac`  
		Last Modified: Wed, 26 Jan 2022 02:35:15 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d591bef59be521b2fc6356caac9ef1ff8a7577ff3f02ea30ca11242e6cc0cdf7`  
		Last Modified: Wed, 26 Jan 2022 02:35:19 GMT  
		Size: 49.1 MB (49113904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dfe9e7899557ea2d3ad94893f2fabed57dfa577a89cddc25a6e15c6800aa402`  
		Last Modified: Wed, 26 Jan 2022 02:35:12 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f956d2382a7998d1b628f5cacc29786d98e01e08bbc428928aca4c32df1ff617`  
		Last Modified: Wed, 26 Jan 2022 02:35:12 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deba864ada3af15db9694092245c13b7805ea46d9b682ce6275e5e214f692ab6`  
		Last Modified: Wed, 26 Jan 2022 02:35:12 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b79c471aa6dd817b6dcfbbcd37c623b6c2e35fcbe9b75c5496e44008cde4e26`  
		Last Modified: Wed, 26 Jan 2022 02:35:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:a8910eda154fb2670cebf4cc072a18307c893a00d5d3fb39d83e4bd3e3682222
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72523043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8ba16fe8039bb0b2a7105771aa4eeb593488cfbf04163e0953ca12d599013a7`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:33:55 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 26 Jan 2022 02:33:56 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 26 Jan 2022 02:34:04 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:34:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 26 Jan 2022 02:34:09 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 26 Jan 2022 02:34:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:35:33 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 26 Jan 2022 02:35:34 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 26 Jan 2022 02:35:52 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Jan 2022 02:35:53 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 26 Jan 2022 02:35:54 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 26 Jan 2022 02:35:55 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 26 Jan 2022 02:35:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 02:35:56 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 26 Jan 2022 02:35:57 GMT
VOLUME [/opt/couchdb/data]
# Wed, 26 Jan 2022 02:35:58 GMT
EXPOSE 4369 5984 9100
# Wed, 26 Jan 2022 02:35:59 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22044b828c1c3fec0f66406d0b4914affa5a4c233a8d1a024e840db18c3717ef`  
		Last Modified: Wed, 26 Jan 2022 02:36:29 GMT  
		Size: 3.3 KB (3322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0132d29a5665e429cb69b2ed2fc2161bcc92bbd0a38d0641b9f514400bd6a0d1`  
		Last Modified: Wed, 26 Jan 2022 02:36:28 GMT  
		Size: 6.5 MB (6549949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6721695d9885aa7b6fb16b43b993093ab01fe96b75f137ad3e7760abf4b73a`  
		Last Modified: Wed, 26 Jan 2022 02:36:27 GMT  
		Size: 951.2 KB (951153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a62fc4090c90113d86eaece64a0ad9474d88e015afa7c449020962191af77f`  
		Last Modified: Wed, 26 Jan 2022 02:36:26 GMT  
		Size: 79.9 KB (79897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a54380ddace77254d3a7eef5aea81131a1c70a1ab560ab9f7c2288b37fe9288`  
		Last Modified: Wed, 26 Jan 2022 02:37:06 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6fba6e4534a2d397cbc79ca495f925dca6384c78ff2a35736ce104f11a50d32`  
		Last Modified: Wed, 26 Jan 2022 02:37:09 GMT  
		Size: 39.0 MB (39011903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fada3abcceccd793c9fb393c41d7993c4af1d1741878cdd3ecbdbb148f4e90`  
		Last Modified: Wed, 26 Jan 2022 02:37:04 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f971f5f71777b59bf08438f14025fb9610ec4f00314708fa849d239ebbe6fede`  
		Last Modified: Wed, 26 Jan 2022 02:37:04 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c341e2778945c5566e24ea5c9c95094d1fa0512c377996f005aa6ff413e237a`  
		Last Modified: Wed, 26 Jan 2022 02:37:04 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1bc007a15a59f1b8238cbe6cd01e252c5d593ba5ea9b6273e249d41730ae68`  
		Last Modified: Wed, 26 Jan 2022 02:37:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3`

```console
$ docker pull couchdb@sha256:4ff3a8e198b926536b8bd494949326f9dd5eda90966f7b6ae3cd8b0053afaeaf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3` - linux; amd64

```console
$ docker pull couchdb@sha256:27cf9fd3c312f7fbd1d139dc20a4f29a98dd208159fddb2035f39ae386598856
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.5 MB (80511881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83340d0da20685e8eaf98edd23b5243b14d460d8b1ef7e3b18b533242448f360`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:32:37 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 26 Jan 2022 02:32:38 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 26 Jan 2022 02:32:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:32:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 26 Jan 2022 02:32:54 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 26 Jan 2022 02:33:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:33:03 GMT
ENV COUCHDB_VERSION=3.2.1
# Wed, 26 Jan 2022 02:33:04 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 26 Jan 2022 02:33:19 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Jan 2022 02:33:19 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 26 Jan 2022 02:33:20 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 26 Jan 2022 02:33:20 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 26 Jan 2022 02:33:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 02:33:21 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 26 Jan 2022 02:33:21 GMT
VOLUME [/opt/couchdb/data]
# Wed, 26 Jan 2022 02:33:21 GMT
EXPOSE 4369 5984 9100
# Wed, 26 Jan 2022 02:33:22 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2303b379bad4b145fe698823516aef43ea73893435a56d56461915d3b67e5ab1`  
		Last Modified: Wed, 26 Jan 2022 02:34:36 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e159d27bba2524eba26ded6aaf13a78457ce9243d40892098fba794fa0d3367`  
		Last Modified: Wed, 26 Jan 2022 02:34:35 GMT  
		Size: 6.7 MB (6691340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3664a86635c3e52a3c405c92976b193da350069cd0d39885217558722501adc3`  
		Last Modified: Wed, 26 Jan 2022 02:34:34 GMT  
		Size: 1.3 MB (1258362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0206c27a3c9eb755f3fc3ea0dd401a0b9ca39beb997f6aba6f29291c70a66d0c`  
		Last Modified: Wed, 26 Jan 2022 02:34:34 GMT  
		Size: 293.0 KB (293041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ffe4963654404902d1a74392463b561007d38b0659031754da497e44626407`  
		Last Modified: Wed, 26 Jan 2022 02:34:33 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe6be15fc53f7b26698a3821efcc1d75c483590b716a855cd8124b8289f1b62c`  
		Last Modified: Wed, 26 Jan 2022 02:34:37 GMT  
		Size: 45.1 MB (45108392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b749a628c011c8a6c43a7fc8b8bef4424779673eab2c8b6b54a6fe6d2fff51`  
		Last Modified: Wed, 26 Jan 2022 02:34:31 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f2e94bcfe9882b0d8ef693f72d44cd5fdea432a24ca644274c3a1869822be4`  
		Last Modified: Wed, 26 Jan 2022 02:34:31 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5147ccc68ff28ed1b1a7c6577ca6199353c874f4bb317fd70069c8891381b1b4`  
		Last Modified: Wed, 26 Jan 2022 02:34:31 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84db6c90182d957a03aba893d17fadbc59978dfe3f498300dcb7a4fc4d135998`  
		Last Modified: Wed, 26 Jan 2022 02:34:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:36030f3d064dd9f9d1c4d9269860694a3116c9f110081bf5e14ddc013b97bb48
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75204151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8636a3c2f3df5b3dca45b55119a179bbddb66469d6eb2686340eaaaeae0ace7c`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:33:55 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 26 Jan 2022 02:33:56 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 26 Jan 2022 02:34:04 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:34:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 26 Jan 2022 02:34:09 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 26 Jan 2022 02:34:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:34:17 GMT
ENV COUCHDB_VERSION=3.2.1
# Wed, 26 Jan 2022 02:34:18 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 26 Jan 2022 02:34:41 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Jan 2022 02:34:42 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 26 Jan 2022 02:34:43 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 26 Jan 2022 02:34:44 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 26 Jan 2022 02:34:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 02:34:45 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 26 Jan 2022 02:34:46 GMT
VOLUME [/opt/couchdb/data]
# Wed, 26 Jan 2022 02:34:47 GMT
EXPOSE 4369 5984 9100
# Wed, 26 Jan 2022 02:34:48 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22044b828c1c3fec0f66406d0b4914affa5a4c233a8d1a024e840db18c3717ef`  
		Last Modified: Wed, 26 Jan 2022 02:36:29 GMT  
		Size: 3.3 KB (3322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0132d29a5665e429cb69b2ed2fc2161bcc92bbd0a38d0641b9f514400bd6a0d1`  
		Last Modified: Wed, 26 Jan 2022 02:36:28 GMT  
		Size: 6.5 MB (6549949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6721695d9885aa7b6fb16b43b993093ab01fe96b75f137ad3e7760abf4b73a`  
		Last Modified: Wed, 26 Jan 2022 02:36:27 GMT  
		Size: 951.2 KB (951153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a62fc4090c90113d86eaece64a0ad9474d88e015afa7c449020962191af77f`  
		Last Modified: Wed, 26 Jan 2022 02:36:26 GMT  
		Size: 79.9 KB (79897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badba65efbbe297653466d430c9b2cdb3f9e8c759a7bdb3285ac9be4a9c8fbd1`  
		Last Modified: Wed, 26 Jan 2022 02:36:26 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7db08bdf6ab0e635fde441d8dabc8cafdbfbb432bdfae708ccde8af80181d84`  
		Last Modified: Wed, 26 Jan 2022 02:36:29 GMT  
		Size: 41.7 MB (41693012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cb69b5c6628a231b29e4709490eb6b2b57f87f2ec5d9edf37016b79bb9da67`  
		Last Modified: Wed, 26 Jan 2022 02:36:24 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4add30705b5038b05f39f809f6635f44f7216f3b97af1debfad73b4a95b47a29`  
		Last Modified: Wed, 26 Jan 2022 02:36:24 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a69ba249989080975d5aaeaebc272d240ad14ab4269a6c17122781261c47bd`  
		Last Modified: Wed, 26 Jan 2022 02:36:25 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d06125201f6057ca7660ccd901a38c224532eb64994f85430e49470353228c`  
		Last Modified: Wed, 26 Jan 2022 02:36:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1`

```console
$ docker pull couchdb@sha256:04c671ca53880b8837d7f6abc82b529440e0a18480df0ea51110fc52600d3fb5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:0d1c2da3fed97e16bc52fae9adee0ebfa003691770e9f651ab7d3d488f4343ff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80003181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83a725351cd6011e75819ee926c4a1eccb853bae57ea69859ddbaa985f12f32a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:32:37 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 26 Jan 2022 02:32:38 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 26 Jan 2022 02:32:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:32:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 26 Jan 2022 02:32:54 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 26 Jan 2022 02:33:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:33:25 GMT
ENV COUCHDB_VERSION=3.1.2
# Wed, 26 Jan 2022 02:33:26 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 26 Jan 2022 02:33:41 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Jan 2022 02:33:41 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 26 Jan 2022 02:33:42 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 26 Jan 2022 02:33:42 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 26 Jan 2022 02:33:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 02:33:43 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 26 Jan 2022 02:33:44 GMT
VOLUME [/opt/couchdb/data]
# Wed, 26 Jan 2022 02:33:44 GMT
EXPOSE 4369 5984 9100
# Wed, 26 Jan 2022 02:33:44 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2303b379bad4b145fe698823516aef43ea73893435a56d56461915d3b67e5ab1`  
		Last Modified: Wed, 26 Jan 2022 02:34:36 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e159d27bba2524eba26ded6aaf13a78457ce9243d40892098fba794fa0d3367`  
		Last Modified: Wed, 26 Jan 2022 02:34:35 GMT  
		Size: 6.7 MB (6691340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3664a86635c3e52a3c405c92976b193da350069cd0d39885217558722501adc3`  
		Last Modified: Wed, 26 Jan 2022 02:34:34 GMT  
		Size: 1.3 MB (1258362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0206c27a3c9eb755f3fc3ea0dd401a0b9ca39beb997f6aba6f29291c70a66d0c`  
		Last Modified: Wed, 26 Jan 2022 02:34:34 GMT  
		Size: 293.0 KB (293041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9623d0946d58d217923210fa0575dc954e830ce42a1d54d55f6b275119da35f`  
		Last Modified: Wed, 26 Jan 2022 02:34:57 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162d84a37e4ce723e62ec3371fde043c070245368768752902cae62bfd225f37`  
		Last Modified: Wed, 26 Jan 2022 02:35:01 GMT  
		Size: 44.6 MB (44599686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21107e5359d6e70cda88e9628544411dd4e0b16a48959b9e2fe81e82e936d519`  
		Last Modified: Wed, 26 Jan 2022 02:34:55 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46eef3ce7fd60c724872864f10ece9578864b5ab2af92c93433949806b38e3c9`  
		Last Modified: Wed, 26 Jan 2022 02:34:55 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6c9c35c34a7f1a580b368afd94bd75c0366dc8a3c08d4556fe9b525136c204`  
		Last Modified: Wed, 26 Jan 2022 02:34:55 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9d3e8b3b68bfd938d01fd244e7ce8fe2397fa6a988433964ed9112ba83080b`  
		Last Modified: Wed, 26 Jan 2022 02:34:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:708648024b9924a68102ed3187be35a99995452b829a2f6e87a723554056c2c7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74611841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:821856bdb89c0bce9f85a9c54245f21b887bf078c082fe51d2c7852aa3226ad6`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:33:55 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 26 Jan 2022 02:33:56 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 26 Jan 2022 02:34:04 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:34:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 26 Jan 2022 02:34:09 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 26 Jan 2022 02:34:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:34:56 GMT
ENV COUCHDB_VERSION=3.1.2
# Wed, 26 Jan 2022 02:34:57 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 26 Jan 2022 02:35:17 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Jan 2022 02:35:18 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 26 Jan 2022 02:35:19 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 26 Jan 2022 02:35:20 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 26 Jan 2022 02:35:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 02:35:21 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 26 Jan 2022 02:35:22 GMT
VOLUME [/opt/couchdb/data]
# Wed, 26 Jan 2022 02:35:23 GMT
EXPOSE 4369 5984 9100
# Wed, 26 Jan 2022 02:35:24 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22044b828c1c3fec0f66406d0b4914affa5a4c233a8d1a024e840db18c3717ef`  
		Last Modified: Wed, 26 Jan 2022 02:36:29 GMT  
		Size: 3.3 KB (3322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0132d29a5665e429cb69b2ed2fc2161bcc92bbd0a38d0641b9f514400bd6a0d1`  
		Last Modified: Wed, 26 Jan 2022 02:36:28 GMT  
		Size: 6.5 MB (6549949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6721695d9885aa7b6fb16b43b993093ab01fe96b75f137ad3e7760abf4b73a`  
		Last Modified: Wed, 26 Jan 2022 02:36:27 GMT  
		Size: 951.2 KB (951153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a62fc4090c90113d86eaece64a0ad9474d88e015afa7c449020962191af77f`  
		Last Modified: Wed, 26 Jan 2022 02:36:26 GMT  
		Size: 79.9 KB (79897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7404580d7e167cdbd29f2ce61354a7f004a70675be67a9001ad17488742bff5`  
		Last Modified: Wed, 26 Jan 2022 02:36:49 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5e29ee260a1e4625f1137ede4535f1ef5fc43d48d42a315f12cff7ca49df47`  
		Last Modified: Wed, 26 Jan 2022 02:36:53 GMT  
		Size: 41.1 MB (41100706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c77f5b3a74ef0d03e9a4a279aa595162ad32c6279a100e5067a9c4ebac29a68`  
		Last Modified: Wed, 26 Jan 2022 02:36:47 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1146c2b9a27b9224a2020c308f8d0ba764fa8bd7d5014851489c675cfe23633d`  
		Last Modified: Wed, 26 Jan 2022 02:36:47 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06c08ff015700215b1925adb4bb349adde5a16b0a83ff117b8aef0ebe887060e`  
		Last Modified: Wed, 26 Jan 2022 02:36:47 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a076695fd1fc16a303c5f2cf86b8c0db9bfd6df3894238bf8961b4cb99547c`  
		Last Modified: Wed, 26 Jan 2022 02:36:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1.2`

```console
$ docker pull couchdb@sha256:04c671ca53880b8837d7f6abc82b529440e0a18480df0ea51110fc52600d3fb5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1.2` - linux; amd64

```console
$ docker pull couchdb@sha256:0d1c2da3fed97e16bc52fae9adee0ebfa003691770e9f651ab7d3d488f4343ff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80003181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83a725351cd6011e75819ee926c4a1eccb853bae57ea69859ddbaa985f12f32a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:32:37 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 26 Jan 2022 02:32:38 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 26 Jan 2022 02:32:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:32:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 26 Jan 2022 02:32:54 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 26 Jan 2022 02:33:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:33:25 GMT
ENV COUCHDB_VERSION=3.1.2
# Wed, 26 Jan 2022 02:33:26 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 26 Jan 2022 02:33:41 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Jan 2022 02:33:41 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 26 Jan 2022 02:33:42 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 26 Jan 2022 02:33:42 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 26 Jan 2022 02:33:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 02:33:43 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 26 Jan 2022 02:33:44 GMT
VOLUME [/opt/couchdb/data]
# Wed, 26 Jan 2022 02:33:44 GMT
EXPOSE 4369 5984 9100
# Wed, 26 Jan 2022 02:33:44 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2303b379bad4b145fe698823516aef43ea73893435a56d56461915d3b67e5ab1`  
		Last Modified: Wed, 26 Jan 2022 02:34:36 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e159d27bba2524eba26ded6aaf13a78457ce9243d40892098fba794fa0d3367`  
		Last Modified: Wed, 26 Jan 2022 02:34:35 GMT  
		Size: 6.7 MB (6691340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3664a86635c3e52a3c405c92976b193da350069cd0d39885217558722501adc3`  
		Last Modified: Wed, 26 Jan 2022 02:34:34 GMT  
		Size: 1.3 MB (1258362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0206c27a3c9eb755f3fc3ea0dd401a0b9ca39beb997f6aba6f29291c70a66d0c`  
		Last Modified: Wed, 26 Jan 2022 02:34:34 GMT  
		Size: 293.0 KB (293041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9623d0946d58d217923210fa0575dc954e830ce42a1d54d55f6b275119da35f`  
		Last Modified: Wed, 26 Jan 2022 02:34:57 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162d84a37e4ce723e62ec3371fde043c070245368768752902cae62bfd225f37`  
		Last Modified: Wed, 26 Jan 2022 02:35:01 GMT  
		Size: 44.6 MB (44599686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21107e5359d6e70cda88e9628544411dd4e0b16a48959b9e2fe81e82e936d519`  
		Last Modified: Wed, 26 Jan 2022 02:34:55 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46eef3ce7fd60c724872864f10ece9578864b5ab2af92c93433949806b38e3c9`  
		Last Modified: Wed, 26 Jan 2022 02:34:55 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6c9c35c34a7f1a580b368afd94bd75c0366dc8a3c08d4556fe9b525136c204`  
		Last Modified: Wed, 26 Jan 2022 02:34:55 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9d3e8b3b68bfd938d01fd244e7ce8fe2397fa6a988433964ed9112ba83080b`  
		Last Modified: Wed, 26 Jan 2022 02:34:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:708648024b9924a68102ed3187be35a99995452b829a2f6e87a723554056c2c7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74611841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:821856bdb89c0bce9f85a9c54245f21b887bf078c082fe51d2c7852aa3226ad6`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:33:55 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 26 Jan 2022 02:33:56 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 26 Jan 2022 02:34:04 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:34:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 26 Jan 2022 02:34:09 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 26 Jan 2022 02:34:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:34:56 GMT
ENV COUCHDB_VERSION=3.1.2
# Wed, 26 Jan 2022 02:34:57 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 26 Jan 2022 02:35:17 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Jan 2022 02:35:18 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 26 Jan 2022 02:35:19 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 26 Jan 2022 02:35:20 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 26 Jan 2022 02:35:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 02:35:21 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 26 Jan 2022 02:35:22 GMT
VOLUME [/opt/couchdb/data]
# Wed, 26 Jan 2022 02:35:23 GMT
EXPOSE 4369 5984 9100
# Wed, 26 Jan 2022 02:35:24 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22044b828c1c3fec0f66406d0b4914affa5a4c233a8d1a024e840db18c3717ef`  
		Last Modified: Wed, 26 Jan 2022 02:36:29 GMT  
		Size: 3.3 KB (3322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0132d29a5665e429cb69b2ed2fc2161bcc92bbd0a38d0641b9f514400bd6a0d1`  
		Last Modified: Wed, 26 Jan 2022 02:36:28 GMT  
		Size: 6.5 MB (6549949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6721695d9885aa7b6fb16b43b993093ab01fe96b75f137ad3e7760abf4b73a`  
		Last Modified: Wed, 26 Jan 2022 02:36:27 GMT  
		Size: 951.2 KB (951153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a62fc4090c90113d86eaece64a0ad9474d88e015afa7c449020962191af77f`  
		Last Modified: Wed, 26 Jan 2022 02:36:26 GMT  
		Size: 79.9 KB (79897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7404580d7e167cdbd29f2ce61354a7f004a70675be67a9001ad17488742bff5`  
		Last Modified: Wed, 26 Jan 2022 02:36:49 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5e29ee260a1e4625f1137ede4535f1ef5fc43d48d42a315f12cff7ca49df47`  
		Last Modified: Wed, 26 Jan 2022 02:36:53 GMT  
		Size: 41.1 MB (41100706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c77f5b3a74ef0d03e9a4a279aa595162ad32c6279a100e5067a9c4ebac29a68`  
		Last Modified: Wed, 26 Jan 2022 02:36:47 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1146c2b9a27b9224a2020c308f8d0ba764fa8bd7d5014851489c675cfe23633d`  
		Last Modified: Wed, 26 Jan 2022 02:36:47 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06c08ff015700215b1925adb4bb349adde5a16b0a83ff117b8aef0ebe887060e`  
		Last Modified: Wed, 26 Jan 2022 02:36:47 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a076695fd1fc16a303c5f2cf86b8c0db9bfd6df3894238bf8961b4cb99547c`  
		Last Modified: Wed, 26 Jan 2022 02:36:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2`

```console
$ docker pull couchdb@sha256:4ff3a8e198b926536b8bd494949326f9dd5eda90966f7b6ae3cd8b0053afaeaf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.2` - linux; amd64

```console
$ docker pull couchdb@sha256:27cf9fd3c312f7fbd1d139dc20a4f29a98dd208159fddb2035f39ae386598856
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.5 MB (80511881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83340d0da20685e8eaf98edd23b5243b14d460d8b1ef7e3b18b533242448f360`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:32:37 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 26 Jan 2022 02:32:38 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 26 Jan 2022 02:32:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:32:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 26 Jan 2022 02:32:54 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 26 Jan 2022 02:33:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:33:03 GMT
ENV COUCHDB_VERSION=3.2.1
# Wed, 26 Jan 2022 02:33:04 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 26 Jan 2022 02:33:19 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Jan 2022 02:33:19 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 26 Jan 2022 02:33:20 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 26 Jan 2022 02:33:20 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 26 Jan 2022 02:33:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 02:33:21 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 26 Jan 2022 02:33:21 GMT
VOLUME [/opt/couchdb/data]
# Wed, 26 Jan 2022 02:33:21 GMT
EXPOSE 4369 5984 9100
# Wed, 26 Jan 2022 02:33:22 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2303b379bad4b145fe698823516aef43ea73893435a56d56461915d3b67e5ab1`  
		Last Modified: Wed, 26 Jan 2022 02:34:36 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e159d27bba2524eba26ded6aaf13a78457ce9243d40892098fba794fa0d3367`  
		Last Modified: Wed, 26 Jan 2022 02:34:35 GMT  
		Size: 6.7 MB (6691340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3664a86635c3e52a3c405c92976b193da350069cd0d39885217558722501adc3`  
		Last Modified: Wed, 26 Jan 2022 02:34:34 GMT  
		Size: 1.3 MB (1258362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0206c27a3c9eb755f3fc3ea0dd401a0b9ca39beb997f6aba6f29291c70a66d0c`  
		Last Modified: Wed, 26 Jan 2022 02:34:34 GMT  
		Size: 293.0 KB (293041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ffe4963654404902d1a74392463b561007d38b0659031754da497e44626407`  
		Last Modified: Wed, 26 Jan 2022 02:34:33 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe6be15fc53f7b26698a3821efcc1d75c483590b716a855cd8124b8289f1b62c`  
		Last Modified: Wed, 26 Jan 2022 02:34:37 GMT  
		Size: 45.1 MB (45108392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b749a628c011c8a6c43a7fc8b8bef4424779673eab2c8b6b54a6fe6d2fff51`  
		Last Modified: Wed, 26 Jan 2022 02:34:31 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f2e94bcfe9882b0d8ef693f72d44cd5fdea432a24ca644274c3a1869822be4`  
		Last Modified: Wed, 26 Jan 2022 02:34:31 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5147ccc68ff28ed1b1a7c6577ca6199353c874f4bb317fd70069c8891381b1b4`  
		Last Modified: Wed, 26 Jan 2022 02:34:31 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84db6c90182d957a03aba893d17fadbc59978dfe3f498300dcb7a4fc4d135998`  
		Last Modified: Wed, 26 Jan 2022 02:34:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:36030f3d064dd9f9d1c4d9269860694a3116c9f110081bf5e14ddc013b97bb48
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75204151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8636a3c2f3df5b3dca45b55119a179bbddb66469d6eb2686340eaaaeae0ace7c`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:33:55 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 26 Jan 2022 02:33:56 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 26 Jan 2022 02:34:04 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:34:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 26 Jan 2022 02:34:09 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 26 Jan 2022 02:34:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:34:17 GMT
ENV COUCHDB_VERSION=3.2.1
# Wed, 26 Jan 2022 02:34:18 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 26 Jan 2022 02:34:41 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Jan 2022 02:34:42 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 26 Jan 2022 02:34:43 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 26 Jan 2022 02:34:44 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 26 Jan 2022 02:34:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 02:34:45 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 26 Jan 2022 02:34:46 GMT
VOLUME [/opt/couchdb/data]
# Wed, 26 Jan 2022 02:34:47 GMT
EXPOSE 4369 5984 9100
# Wed, 26 Jan 2022 02:34:48 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22044b828c1c3fec0f66406d0b4914affa5a4c233a8d1a024e840db18c3717ef`  
		Last Modified: Wed, 26 Jan 2022 02:36:29 GMT  
		Size: 3.3 KB (3322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0132d29a5665e429cb69b2ed2fc2161bcc92bbd0a38d0641b9f514400bd6a0d1`  
		Last Modified: Wed, 26 Jan 2022 02:36:28 GMT  
		Size: 6.5 MB (6549949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6721695d9885aa7b6fb16b43b993093ab01fe96b75f137ad3e7760abf4b73a`  
		Last Modified: Wed, 26 Jan 2022 02:36:27 GMT  
		Size: 951.2 KB (951153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a62fc4090c90113d86eaece64a0ad9474d88e015afa7c449020962191af77f`  
		Last Modified: Wed, 26 Jan 2022 02:36:26 GMT  
		Size: 79.9 KB (79897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badba65efbbe297653466d430c9b2cdb3f9e8c759a7bdb3285ac9be4a9c8fbd1`  
		Last Modified: Wed, 26 Jan 2022 02:36:26 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7db08bdf6ab0e635fde441d8dabc8cafdbfbb432bdfae708ccde8af80181d84`  
		Last Modified: Wed, 26 Jan 2022 02:36:29 GMT  
		Size: 41.7 MB (41693012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cb69b5c6628a231b29e4709490eb6b2b57f87f2ec5d9edf37016b79bb9da67`  
		Last Modified: Wed, 26 Jan 2022 02:36:24 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4add30705b5038b05f39f809f6635f44f7216f3b97af1debfad73b4a95b47a29`  
		Last Modified: Wed, 26 Jan 2022 02:36:24 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a69ba249989080975d5aaeaebc272d240ad14ab4269a6c17122781261c47bd`  
		Last Modified: Wed, 26 Jan 2022 02:36:25 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d06125201f6057ca7660ccd901a38c224532eb64994f85430e49470353228c`  
		Last Modified: Wed, 26 Jan 2022 02:36:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2.1`

```console
$ docker pull couchdb@sha256:4ff3a8e198b926536b8bd494949326f9dd5eda90966f7b6ae3cd8b0053afaeaf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.2.1` - linux; amd64

```console
$ docker pull couchdb@sha256:27cf9fd3c312f7fbd1d139dc20a4f29a98dd208159fddb2035f39ae386598856
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.5 MB (80511881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83340d0da20685e8eaf98edd23b5243b14d460d8b1ef7e3b18b533242448f360`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:32:37 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 26 Jan 2022 02:32:38 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 26 Jan 2022 02:32:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:32:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 26 Jan 2022 02:32:54 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 26 Jan 2022 02:33:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:33:03 GMT
ENV COUCHDB_VERSION=3.2.1
# Wed, 26 Jan 2022 02:33:04 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 26 Jan 2022 02:33:19 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Jan 2022 02:33:19 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 26 Jan 2022 02:33:20 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 26 Jan 2022 02:33:20 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 26 Jan 2022 02:33:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 02:33:21 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 26 Jan 2022 02:33:21 GMT
VOLUME [/opt/couchdb/data]
# Wed, 26 Jan 2022 02:33:21 GMT
EXPOSE 4369 5984 9100
# Wed, 26 Jan 2022 02:33:22 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2303b379bad4b145fe698823516aef43ea73893435a56d56461915d3b67e5ab1`  
		Last Modified: Wed, 26 Jan 2022 02:34:36 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e159d27bba2524eba26ded6aaf13a78457ce9243d40892098fba794fa0d3367`  
		Last Modified: Wed, 26 Jan 2022 02:34:35 GMT  
		Size: 6.7 MB (6691340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3664a86635c3e52a3c405c92976b193da350069cd0d39885217558722501adc3`  
		Last Modified: Wed, 26 Jan 2022 02:34:34 GMT  
		Size: 1.3 MB (1258362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0206c27a3c9eb755f3fc3ea0dd401a0b9ca39beb997f6aba6f29291c70a66d0c`  
		Last Modified: Wed, 26 Jan 2022 02:34:34 GMT  
		Size: 293.0 KB (293041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ffe4963654404902d1a74392463b561007d38b0659031754da497e44626407`  
		Last Modified: Wed, 26 Jan 2022 02:34:33 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe6be15fc53f7b26698a3821efcc1d75c483590b716a855cd8124b8289f1b62c`  
		Last Modified: Wed, 26 Jan 2022 02:34:37 GMT  
		Size: 45.1 MB (45108392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b749a628c011c8a6c43a7fc8b8bef4424779673eab2c8b6b54a6fe6d2fff51`  
		Last Modified: Wed, 26 Jan 2022 02:34:31 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f2e94bcfe9882b0d8ef693f72d44cd5fdea432a24ca644274c3a1869822be4`  
		Last Modified: Wed, 26 Jan 2022 02:34:31 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5147ccc68ff28ed1b1a7c6577ca6199353c874f4bb317fd70069c8891381b1b4`  
		Last Modified: Wed, 26 Jan 2022 02:34:31 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84db6c90182d957a03aba893d17fadbc59978dfe3f498300dcb7a4fc4d135998`  
		Last Modified: Wed, 26 Jan 2022 02:34:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:36030f3d064dd9f9d1c4d9269860694a3116c9f110081bf5e14ddc013b97bb48
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75204151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8636a3c2f3df5b3dca45b55119a179bbddb66469d6eb2686340eaaaeae0ace7c`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:33:55 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 26 Jan 2022 02:33:56 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 26 Jan 2022 02:34:04 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:34:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 26 Jan 2022 02:34:09 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 26 Jan 2022 02:34:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:34:17 GMT
ENV COUCHDB_VERSION=3.2.1
# Wed, 26 Jan 2022 02:34:18 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 26 Jan 2022 02:34:41 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Jan 2022 02:34:42 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 26 Jan 2022 02:34:43 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 26 Jan 2022 02:34:44 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 26 Jan 2022 02:34:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 02:34:45 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 26 Jan 2022 02:34:46 GMT
VOLUME [/opt/couchdb/data]
# Wed, 26 Jan 2022 02:34:47 GMT
EXPOSE 4369 5984 9100
# Wed, 26 Jan 2022 02:34:48 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22044b828c1c3fec0f66406d0b4914affa5a4c233a8d1a024e840db18c3717ef`  
		Last Modified: Wed, 26 Jan 2022 02:36:29 GMT  
		Size: 3.3 KB (3322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0132d29a5665e429cb69b2ed2fc2161bcc92bbd0a38d0641b9f514400bd6a0d1`  
		Last Modified: Wed, 26 Jan 2022 02:36:28 GMT  
		Size: 6.5 MB (6549949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6721695d9885aa7b6fb16b43b993093ab01fe96b75f137ad3e7760abf4b73a`  
		Last Modified: Wed, 26 Jan 2022 02:36:27 GMT  
		Size: 951.2 KB (951153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a62fc4090c90113d86eaece64a0ad9474d88e015afa7c449020962191af77f`  
		Last Modified: Wed, 26 Jan 2022 02:36:26 GMT  
		Size: 79.9 KB (79897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badba65efbbe297653466d430c9b2cdb3f9e8c759a7bdb3285ac9be4a9c8fbd1`  
		Last Modified: Wed, 26 Jan 2022 02:36:26 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7db08bdf6ab0e635fde441d8dabc8cafdbfbb432bdfae708ccde8af80181d84`  
		Last Modified: Wed, 26 Jan 2022 02:36:29 GMT  
		Size: 41.7 MB (41693012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cb69b5c6628a231b29e4709490eb6b2b57f87f2ec5d9edf37016b79bb9da67`  
		Last Modified: Wed, 26 Jan 2022 02:36:24 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4add30705b5038b05f39f809f6635f44f7216f3b97af1debfad73b4a95b47a29`  
		Last Modified: Wed, 26 Jan 2022 02:36:24 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a69ba249989080975d5aaeaebc272d240ad14ab4269a6c17122781261c47bd`  
		Last Modified: Wed, 26 Jan 2022 02:36:25 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d06125201f6057ca7660ccd901a38c224532eb64994f85430e49470353228c`  
		Last Modified: Wed, 26 Jan 2022 02:36:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:latest`

```console
$ docker pull couchdb@sha256:4ff3a8e198b926536b8bd494949326f9dd5eda90966f7b6ae3cd8b0053afaeaf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:27cf9fd3c312f7fbd1d139dc20a4f29a98dd208159fddb2035f39ae386598856
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.5 MB (80511881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83340d0da20685e8eaf98edd23b5243b14d460d8b1ef7e3b18b533242448f360`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:32:37 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 26 Jan 2022 02:32:38 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 26 Jan 2022 02:32:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:32:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 26 Jan 2022 02:32:54 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 26 Jan 2022 02:33:03 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:33:03 GMT
ENV COUCHDB_VERSION=3.2.1
# Wed, 26 Jan 2022 02:33:04 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 26 Jan 2022 02:33:19 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Jan 2022 02:33:19 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 26 Jan 2022 02:33:20 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 26 Jan 2022 02:33:20 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 26 Jan 2022 02:33:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 02:33:21 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 26 Jan 2022 02:33:21 GMT
VOLUME [/opt/couchdb/data]
# Wed, 26 Jan 2022 02:33:21 GMT
EXPOSE 4369 5984 9100
# Wed, 26 Jan 2022 02:33:22 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2303b379bad4b145fe698823516aef43ea73893435a56d56461915d3b67e5ab1`  
		Last Modified: Wed, 26 Jan 2022 02:34:36 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e159d27bba2524eba26ded6aaf13a78457ce9243d40892098fba794fa0d3367`  
		Last Modified: Wed, 26 Jan 2022 02:34:35 GMT  
		Size: 6.7 MB (6691340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3664a86635c3e52a3c405c92976b193da350069cd0d39885217558722501adc3`  
		Last Modified: Wed, 26 Jan 2022 02:34:34 GMT  
		Size: 1.3 MB (1258362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0206c27a3c9eb755f3fc3ea0dd401a0b9ca39beb997f6aba6f29291c70a66d0c`  
		Last Modified: Wed, 26 Jan 2022 02:34:34 GMT  
		Size: 293.0 KB (293041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ffe4963654404902d1a74392463b561007d38b0659031754da497e44626407`  
		Last Modified: Wed, 26 Jan 2022 02:34:33 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe6be15fc53f7b26698a3821efcc1d75c483590b716a855cd8124b8289f1b62c`  
		Last Modified: Wed, 26 Jan 2022 02:34:37 GMT  
		Size: 45.1 MB (45108392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b749a628c011c8a6c43a7fc8b8bef4424779673eab2c8b6b54a6fe6d2fff51`  
		Last Modified: Wed, 26 Jan 2022 02:34:31 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f2e94bcfe9882b0d8ef693f72d44cd5fdea432a24ca644274c3a1869822be4`  
		Last Modified: Wed, 26 Jan 2022 02:34:31 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5147ccc68ff28ed1b1a7c6577ca6199353c874f4bb317fd70069c8891381b1b4`  
		Last Modified: Wed, 26 Jan 2022 02:34:31 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84db6c90182d957a03aba893d17fadbc59978dfe3f498300dcb7a4fc4d135998`  
		Last Modified: Wed, 26 Jan 2022 02:34:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:36030f3d064dd9f9d1c4d9269860694a3116c9f110081bf5e14ddc013b97bb48
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75204151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8636a3c2f3df5b3dca45b55119a179bbddb66469d6eb2686340eaaaeae0ace7c`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:33:55 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 26 Jan 2022 02:33:56 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 26 Jan 2022 02:34:04 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:34:08 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 26 Jan 2022 02:34:09 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 26 Jan 2022 02:34:16 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:34:17 GMT
ENV COUCHDB_VERSION=3.2.1
# Wed, 26 Jan 2022 02:34:18 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 26 Jan 2022 02:34:41 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 26 Jan 2022 02:34:42 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 26 Jan 2022 02:34:43 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 26 Jan 2022 02:34:44 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 26 Jan 2022 02:34:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 26 Jan 2022 02:34:45 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 26 Jan 2022 02:34:46 GMT
VOLUME [/opt/couchdb/data]
# Wed, 26 Jan 2022 02:34:47 GMT
EXPOSE 4369 5984 9100
# Wed, 26 Jan 2022 02:34:48 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22044b828c1c3fec0f66406d0b4914affa5a4c233a8d1a024e840db18c3717ef`  
		Last Modified: Wed, 26 Jan 2022 02:36:29 GMT  
		Size: 3.3 KB (3322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0132d29a5665e429cb69b2ed2fc2161bcc92bbd0a38d0641b9f514400bd6a0d1`  
		Last Modified: Wed, 26 Jan 2022 02:36:28 GMT  
		Size: 6.5 MB (6549949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6721695d9885aa7b6fb16b43b993093ab01fe96b75f137ad3e7760abf4b73a`  
		Last Modified: Wed, 26 Jan 2022 02:36:27 GMT  
		Size: 951.2 KB (951153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a62fc4090c90113d86eaece64a0ad9474d88e015afa7c449020962191af77f`  
		Last Modified: Wed, 26 Jan 2022 02:36:26 GMT  
		Size: 79.9 KB (79897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badba65efbbe297653466d430c9b2cdb3f9e8c759a7bdb3285ac9be4a9c8fbd1`  
		Last Modified: Wed, 26 Jan 2022 02:36:26 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7db08bdf6ab0e635fde441d8dabc8cafdbfbb432bdfae708ccde8af80181d84`  
		Last Modified: Wed, 26 Jan 2022 02:36:29 GMT  
		Size: 41.7 MB (41693012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cb69b5c6628a231b29e4709490eb6b2b57f87f2ec5d9edf37016b79bb9da67`  
		Last Modified: Wed, 26 Jan 2022 02:36:24 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4add30705b5038b05f39f809f6635f44f7216f3b97af1debfad73b4a95b47a29`  
		Last Modified: Wed, 26 Jan 2022 02:36:24 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a69ba249989080975d5aaeaebc272d240ad14ab4269a6c17122781261c47bd`  
		Last Modified: Wed, 26 Jan 2022 02:36:25 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d06125201f6057ca7660ccd901a38c224532eb64994f85430e49470353228c`  
		Last Modified: Wed, 26 Jan 2022 02:36:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
