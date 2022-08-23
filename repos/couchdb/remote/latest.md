## `couchdb:latest`

```console
$ docker pull couchdb@sha256:fd7a739e37deab2c10119a81886ff8c626f9e1de6e786ed60b31ca9c30450035
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:28124b34f4148ed792f9bf2c71207cc3ea9bb7e76546d67daffb19234952df81
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87503932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0396728d49f5ac43a68e07bf8b23d34cdbcec06f4aa08229ce8b509f9f465c64`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:59:42 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 23 Aug 2022 00:59:42 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 23 Aug 2022 00:59:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:59:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 23 Aug 2022 00:59:53 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 23 Aug 2022 00:59:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:59:59 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 23 Aug 2022 00:59:59 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 23 Aug 2022 01:00:13 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 23 Aug 2022 01:00:13 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 23 Aug 2022 01:00:13 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 23 Aug 2022 01:00:14 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 23 Aug 2022 01:00:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 23 Aug 2022 01:00:14 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 23 Aug 2022 01:00:14 GMT
VOLUME [/opt/couchdb/data]
# Tue, 23 Aug 2022 01:00:14 GMT
EXPOSE 4369 5984 9100
# Tue, 23 Aug 2022 01:00:15 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1836a36860638007d7b2592171befa5754532a9d47de8f0e775fad866c82393e`  
		Last Modified: Tue, 23 Aug 2022 01:01:43 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e2e2b5b7b5034043633af72843d3b8666f8ccc0c2aeae43af0afe8e9fdb2c8`  
		Last Modified: Tue, 23 Aug 2022 01:01:43 GMT  
		Size: 5.2 MB (5224227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c99ac86ee0acd5521ed2df4dce63d77342c2a96acff9b2af72b76e5893f62f`  
		Last Modified: Tue, 23 Aug 2022 01:01:42 GMT  
		Size: 1.6 MB (1553304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8979b473c30718ae0cbb8a38a2e402f873ad242554184f7beabb593d4451bfc0`  
		Last Modified: Tue, 23 Aug 2022 01:01:41 GMT  
		Size: 295.6 KB (295581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510ed5a8f7236ce7e23d8bb548f076632c0b48a3e1e8430e0e262ef6647f7ebc`  
		Last Modified: Tue, 23 Aug 2022 01:01:41 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e968620046651f8bd94db8256d249f0684ba2a454fb63d1c109ca1b45920ae`  
		Last Modified: Tue, 23 Aug 2022 01:01:45 GMT  
		Size: 49.0 MB (49042191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8920bb938feadb5c2b98dd12c72f655b1e47b736dd024cf1098c3f1acb2e645`  
		Last Modified: Tue, 23 Aug 2022 01:01:39 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a6954a2f0617948efb306d9b1a5b784d64a0beff38481b6828d069ca696e18`  
		Last Modified: Tue, 23 Aug 2022 01:01:39 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41292b445e0d087758fc8486322576d3605d68a540ca3fb3243dbc84ab1d4dda`  
		Last Modified: Tue, 23 Aug 2022 01:01:39 GMT  
		Size: 2.2 KB (2185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eaa46afbe00ace5c0c20bfc3c7912cde4600f9e8f942d5149e988d0473464fc`  
		Last Modified: Tue, 23 Aug 2022 01:01:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:2cc537fd46496d460ec408ea389dd4cc27c180608e89c59761c4682d6dac0cbd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.6 MB (85622605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faece9a6aa805f3e9d71e0136a8c7add2db196a28de98b26dc652d2eb88bf4ee`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:38 GMT
ADD file:6039adfbca55ed34a719c37672c664e3524130a0e2a3b8663629b8120b81b790 in / 
# Tue, 02 Aug 2022 00:40:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:53:11 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 02 Aug 2022 01:53:11 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 02 Aug 2022 01:53:19 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:53:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 02 Aug 2022 01:53:23 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 02 Aug 2022 01:53:29 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:53:29 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 02 Aug 2022 01:53:30 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 02 Aug 2022 01:53:44 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 02 Aug 2022 01:53:45 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 02 Aug 2022 01:53:46 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 02 Aug 2022 01:53:47 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 02 Aug 2022 01:53:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 02 Aug 2022 01:53:48 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 02 Aug 2022 01:53:49 GMT
VOLUME [/opt/couchdb/data]
# Tue, 02 Aug 2022 01:53:50 GMT
EXPOSE 4369 5984 9100
# Tue, 02 Aug 2022 01:53:51 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:a9fe95647e78b5516c7e2327355b6996e2ea295cd76ae242cbfe87f016b4e760`  
		Last Modified: Tue, 02 Aug 2022 00:46:05 GMT  
		Size: 30.1 MB (30054304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f36ebccf7ea0ca6c4e42a56d3e761f51620dde7809ff4cd6c9c47f4d92dda45`  
		Last Modified: Tue, 02 Aug 2022 01:56:00 GMT  
		Size: 3.3 KB (3320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57988538f1066bad59a075d99704fbc2ed80b7f279168e98ae1ac061cddb0e54`  
		Last Modified: Tue, 02 Aug 2022 01:55:59 GMT  
		Size: 5.2 MB (5207882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d6f84207bfc6da3f978a06e64089cd163b0b7cfce56aa03f050fffcf6aa1fa`  
		Last Modified: Tue, 02 Aug 2022 01:55:59 GMT  
		Size: 1.2 MB (1221114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f79004f600a1443f5dd0ab501f8d2726ae96d9790d635ef946c8ab58fc7639`  
		Last Modified: Tue, 02 Aug 2022 01:55:58 GMT  
		Size: 79.2 KB (79204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea246a4776bb764303aebd0c230598840bac0a3067bf67395be8aa1d4a9796c0`  
		Last Modified: Tue, 02 Aug 2022 01:55:58 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afec05def1afee67aa528ce2ecc14afe3dd947292160af59436483a6eb8307d8`  
		Last Modified: Tue, 02 Aug 2022 01:56:02 GMT  
		Size: 49.1 MB (49053054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f205452c1f21b508f3eff3ca454e831b24598073851b7c10ad77092021c63b80`  
		Last Modified: Tue, 02 Aug 2022 01:55:56 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb0d06feb8b8d747a8a616d3dbdb4dbff7f3d1c07726fc7fabbd0d857588a65`  
		Last Modified: Tue, 02 Aug 2022 01:55:56 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833640fe1553f0d57940524d810c11944b07d0171e7979f091beca62d8c235a2`  
		Last Modified: Tue, 02 Aug 2022 01:55:56 GMT  
		Size: 2.2 KB (2184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c60df208533e1fc53978ad88b63060ba603756eef0b46beaa35572ff7fc1aa2`  
		Last Modified: Tue, 02 Aug 2022 01:55:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; ppc64le

```console
$ docker pull couchdb@sha256:1e403730c20e44b3297dc2ca59567dc4f7f8608ea517c016cf6b814fa428f6f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93209223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9532ba1899566dfcf8498c068f3eca6b79c8afa3fae5d939c52255a7ae9d96b4`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 02 Aug 2022 01:17:30 GMT
ADD file:3a95a896d463569ce82199957052b3467123a4bd3385a0a4e397cf08402a99c3 in / 
# Tue, 02 Aug 2022 01:17:32 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:45:51 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 02 Aug 2022 01:45:52 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 02 Aug 2022 01:46:07 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:46:13 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 02 Aug 2022 01:46:14 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 02 Aug 2022 01:46:24 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:46:24 GMT
ENV COUCHDB_VERSION=3.2.2
# Tue, 02 Aug 2022 01:46:25 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 02 Aug 2022 01:46:47 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 02 Aug 2022 01:46:48 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 02 Aug 2022 01:46:49 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 02 Aug 2022 01:46:49 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 02 Aug 2022 01:46:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 02 Aug 2022 01:46:50 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 02 Aug 2022 01:46:51 GMT
VOLUME [/opt/couchdb/data]
# Tue, 02 Aug 2022 01:46:51 GMT
EXPOSE 4369 5984 9100
# Tue, 02 Aug 2022 01:46:51 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:5241cd116d6e6e2d62f3d8c2245b74daca9f6cc154eaccd738feb41984c74714`  
		Last Modified: Tue, 02 Aug 2022 01:24:39 GMT  
		Size: 35.3 MB (35272771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd616d47d2a8f573397f07010fd143095697a31e5f728cac1c1b7269738c47a`  
		Last Modified: Tue, 02 Aug 2022 01:47:19 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1a77f89868067efb94d63fe88604742503d85f515b25f7ab84711a016d3e4f`  
		Last Modified: Tue, 02 Aug 2022 01:47:19 GMT  
		Size: 6.0 MB (6043687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f741e9865e3fdcb0bd227a5993c271ef87a11ea1804cdbbdd3814773c085fd4`  
		Last Modified: Tue, 02 Aug 2022 01:47:17 GMT  
		Size: 1.5 MB (1509129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a56ea83b77070cf87034a857804e0e5dc6e22a75e16d352364a0c6f2cf81cd`  
		Last Modified: Tue, 02 Aug 2022 01:47:17 GMT  
		Size: 295.5 KB (295465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe12fc56262eb1a9961df421373e9e93f9755a2e423207066c543f023b488f7`  
		Last Modified: Tue, 02 Aug 2022 01:47:17 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51cf6274a3105c304db4a54d429807a6d97294428538c809f791158d3a610942`  
		Last Modified: Tue, 02 Aug 2022 01:47:24 GMT  
		Size: 50.1 MB (50081019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48855ad409841498cce766b60da4e1cd5f59a6da57e69031b5cb1e70944c7e06`  
		Last Modified: Tue, 02 Aug 2022 01:47:14 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d93f33d896f43831a247689b5fe6b3c85972c92c57c27a55ae2ca50fd89216c`  
		Last Modified: Tue, 02 Aug 2022 01:47:15 GMT  
		Size: 768.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2efe54a8f4ae1598aa0cad697c24d96e9bd6701de850e533e452cb0ddc5df62`  
		Last Modified: Tue, 02 Aug 2022 01:47:15 GMT  
		Size: 2.2 KB (2188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58fa6fb130ed09e3914ae920a1e5cd0affdd896fa22de827e2b222afb58a04e4`  
		Last Modified: Tue, 02 Aug 2022 01:47:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
