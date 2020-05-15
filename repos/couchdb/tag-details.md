<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `couchdb`

-	[`couchdb:2`](#couchdb2)
-	[`couchdb:2.3`](#couchdb23)
-	[`couchdb:2.3.1`](#couchdb231)
-	[`couchdb:3`](#couchdb3)
-	[`couchdb:3.0`](#couchdb30)
-	[`couchdb:3.0.1`](#couchdb301)
-	[`couchdb:3.1`](#couchdb31)
-	[`couchdb:3.1.0`](#couchdb310)
-	[`couchdb:latest`](#couchdblatest)

## `couchdb:2`

```console
$ docker pull couchdb@sha256:530734af5ab6f120421218e97793488343d3bc94a482f33f6e9f522ba9e788fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:2` - linux; amd64

```console
$ docker pull couchdb@sha256:13bcfa1f89f9a98c32c644f74c07da9b5df75af1d1b5f84fa7b9f3d5cb524f7f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.4 MB (82435186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81e56652900022f120dc43209e678679e47a21c9937f3d54f3c26fba81600811`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 18:13:18 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 15 May 2020 18:13:19 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 15 May 2020 18:13:29 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 18:13:29 GMT
ENV GOSU_VERSION=1.11
# Fri, 15 May 2020 18:13:30 GMT
ENV TINI_VERSION=0.18.0
# Fri, 15 May 2020 18:14:26 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Fri, 15 May 2020 18:14:27 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Fri, 15 May 2020 18:14:30 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Fri, 15 May 2020 18:14:30 GMT
ENV COUCHDB_VERSION=2.3.1
# Fri, 15 May 2020 18:14:31 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb stretch main" > /etc/apt/sources.list.d/couchdb.list
# Fri, 15 May 2020 18:14:53 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~stretch     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 15 May 2020 18:14:54 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Fri, 15 May 2020 18:14:54 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 15 May 2020 18:14:54 GMT
COPY file:5b465eec9f6f6fe5ff9abac1313cd161fcf9b5299d43cfb10ee0dd1935c99af4 in /usr/local/bin 
# Fri, 15 May 2020 18:14:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 15 May 2020 18:14:55 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 15 May 2020 18:14:55 GMT
VOLUME [/opt/couchdb/data]
# Fri, 15 May 2020 18:14:56 GMT
EXPOSE 4369 5984 9100
# Fri, 15 May 2020 18:14:56 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae17bf830d5c7f4017f7d358c431ffc488af80c717a9af597502caa0850a688`  
		Last Modified: Fri, 15 May 2020 18:15:42 GMT  
		Size: 3.4 KB (3416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c89a198000731720c257c505ba673e16122743472eb20bb413b706c355f47f5`  
		Last Modified: Fri, 15 May 2020 18:15:43 GMT  
		Size: 8.5 MB (8515134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09815a5893a7a236d254d84e6deabaac8f231c0d48b986815ee4c446781c22f8`  
		Last Modified: Fri, 15 May 2020 18:15:41 GMT  
		Size: 1.2 MB (1190710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3856fa5cc7cf8b1b9264a6ba6d8a253f7c24943241df26e00401df74956074ef`  
		Last Modified: Fri, 15 May 2020 18:15:41 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6544587f4aad837b2317dbe5c3773cdb9c78bb5bc6c200ee96a2f58c78abae32`  
		Last Modified: Fri, 15 May 2020 18:15:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d29e28a5747bf336273bb695ddc2bc7be4a6c5211e33c073eba8997b62bbfd09`  
		Last Modified: Fri, 15 May 2020 18:15:47 GMT  
		Size: 50.2 MB (50199994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9913ca42e32cea716d02cf7bb36ba2e517e35b9b0fccda3577821087620541c5`  
		Last Modified: Fri, 15 May 2020 18:15:39 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030f84bc109957f6addad53c8e48d75eadc9cc3398a36329d5c70ece6d1c742d`  
		Last Modified: Fri, 15 May 2020 18:15:39 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49e2942e15f39163009f042c0241e478a09051860f1c69dcf7b375bcb0592e1`  
		Last Modified: Fri, 15 May 2020 18:15:39 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c90779812142bac82d6985de583ce473ee4bc150f6b831a54a833f84a319687`  
		Last Modified: Fri, 15 May 2020 18:15:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:a3632ea9cc176b41f68f2e7c309045adda3c12236cdcd3b4751b8b34f6594a62
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76967446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02f7c6bfe5f6704bdff3a8ca636c7f47ae06650af995024492a57f20d03e3e8e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 15 May 2020 12:48:45 GMT
ADD file:a808acc4967ce5ecee8ba7a3e8769d6b91e38fecad2a792c8bd5aeef0007c6c0 in / 
# Fri, 15 May 2020 12:48:49 GMT
CMD ["bash"]
# Fri, 15 May 2020 20:46:22 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 15 May 2020 20:46:24 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 15 May 2020 20:46:43 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 20:46:44 GMT
ENV GOSU_VERSION=1.11
# Fri, 15 May 2020 20:46:45 GMT
ENV TINI_VERSION=0.18.0
# Fri, 15 May 2020 20:47:00 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Fri, 15 May 2020 20:47:01 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Fri, 15 May 2020 20:47:05 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Fri, 15 May 2020 20:47:06 GMT
ENV COUCHDB_VERSION=2.3.1
# Fri, 15 May 2020 20:47:08 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb stretch main" > /etc/apt/sources.list.d/couchdb.list
# Fri, 15 May 2020 20:47:41 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~stretch     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 15 May 2020 20:47:43 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Fri, 15 May 2020 20:47:44 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 15 May 2020 20:47:44 GMT
COPY file:5b465eec9f6f6fe5ff9abac1313cd161fcf9b5299d43cfb10ee0dd1935c99af4 in /usr/local/bin 
# Fri, 15 May 2020 20:47:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 15 May 2020 20:47:46 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 15 May 2020 20:47:47 GMT
VOLUME [/opt/couchdb/data]
# Fri, 15 May 2020 20:47:48 GMT
EXPOSE 4369 5984 9100
# Fri, 15 May 2020 20:47:48 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:7f439267e48f39a2f7463f7ec54d4ccd7f849de1dd6fd575bc2ee51c096b1da5`  
		Last Modified: Fri, 15 May 2020 12:56:01 GMT  
		Size: 20.4 MB (20375567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188a9c3447af22efe0b6b60010a280ca8a446f135900217964c954cbb6286053`  
		Last Modified: Fri, 15 May 2020 20:48:34 GMT  
		Size: 3.4 KB (3439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c16e5b60fb95f2ab9823bdd772fad8d4418983f5966ef16168c8caa809db35d`  
		Last Modified: Fri, 15 May 2020 20:48:35 GMT  
		Size: 7.7 MB (7655239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfac69bd809d9b5c95e237a6c606a9744946fe3f472c159a911fb4c9efd7258f`  
		Last Modified: Fri, 15 May 2020 20:48:33 GMT  
		Size: 1.1 MB (1125176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9ef11f43552f81aa0e45919af542da76d32eec8d757a0aa2e008ffc2840725`  
		Last Modified: Fri, 15 May 2020 20:48:33 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff027aa903830075c5cc2d1589a2f371019e90d1b486c9d03f1a73cf8bf351d1`  
		Last Modified: Fri, 15 May 2020 20:48:33 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa40728da06374e64b2eeb63bbc29018a7437f56f803ce01ac33d84d4ad3aad`  
		Last Modified: Fri, 15 May 2020 20:48:43 GMT  
		Size: 47.8 MB (47801971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d26d47fe0ab93460761aef656d13f3c91a47512b66327c539e21ab5d6d48ad`  
		Last Modified: Fri, 15 May 2020 20:48:32 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f6ca5675e02632898abb000b02da7fa92eacfd07518b6dc110c8903aa911d9`  
		Last Modified: Fri, 15 May 2020 20:48:31 GMT  
		Size: 768.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f0b79066d10a103782957bbdbf7cf5a30b39c51c860732042e0d6ae8839cd8`  
		Last Modified: Fri, 15 May 2020 20:48:31 GMT  
		Size: 2.1 KB (2061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b986b515be88cf3f1e19ca9c06c7c2d3891904f0a6b49095b240f2899ec83280`  
		Last Modified: Fri, 15 May 2020 20:48:32 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2` - linux; ppc64le

```console
$ docker pull couchdb@sha256:2638231caec3716d402975c66d4851a9c9305aba878f9c04ce40b7483d36b6e1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.2 MB (81217121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfe6b387ada120d7bca498ab7322657ee76479c8a9b25f66f69ffc1d54ac1bf1`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 13 May 2020 22:42:09 GMT
ADD file:341dbc564992a44e81b3a4f399f7de14d7340a45b73c577edb78e16da2c14584 in / 
# Wed, 13 May 2020 22:42:12 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:50:24 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 14 May 2020 00:50:37 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 14 May 2020 00:52:32 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:52:36 GMT
ENV GOSU_VERSION=1.11
# Thu, 14 May 2020 00:52:41 GMT
ENV TINI_VERSION=0.18.0
# Thu, 14 May 2020 00:53:13 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Thu, 14 May 2020 00:53:15 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Thu, 14 May 2020 00:53:22 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Thu, 14 May 2020 00:53:27 GMT
ENV COUCHDB_VERSION=2.3.1
# Thu, 14 May 2020 00:53:34 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb stretch main" > /etc/apt/sources.list.d/couchdb.list
# Thu, 14 May 2020 00:54:51 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~stretch     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 14 May 2020 00:54:55 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Thu, 14 May 2020 00:54:56 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 14 May 2020 00:54:57 GMT
COPY file:5b465eec9f6f6fe5ff9abac1313cd161fcf9b5299d43cfb10ee0dd1935c99af4 in /usr/local/bin 
# Thu, 14 May 2020 00:55:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 14 May 2020 00:55:09 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 14 May 2020 00:55:14 GMT
VOLUME [/opt/couchdb/data]
# Thu, 14 May 2020 00:55:19 GMT
EXPOSE 4369 5984 9100
# Thu, 14 May 2020 00:55:23 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:3b6ae894780534c0f99588e9cce4beb8fb7884b4578e6206b72f2db75116bb1c`  
		Last Modified: Wed, 13 May 2020 23:02:51 GMT  
		Size: 22.8 MB (22785361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c18509798b282bfa588f81e9600cf2f22f360f58297bac34227fa3655763fd6`  
		Last Modified: Thu, 14 May 2020 00:56:51 GMT  
		Size: 3.4 KB (3418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9838b2df91d2eee01d043f25a1d09479d9bce0c2c76f08a1a86dfd27e34e8073`  
		Last Modified: Thu, 14 May 2020 00:56:47 GMT  
		Size: 8.0 MB (7998426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf3599c9ca361654fc74215f1d77c8a1042958af57170e098e058400caf2548`  
		Last Modified: Thu, 14 May 2020 00:56:47 GMT  
		Size: 1.1 MB (1114275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7caa3e2e28d292a124d3a0e93a0f5875fee5e12d73371e53f3d8265eb980f9e9`  
		Last Modified: Thu, 14 May 2020 00:56:44 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0229f5e350ef91c592b92444637e8d12a018f3c61b4fc8e5b6fe0b12ff9965`  
		Last Modified: Thu, 14 May 2020 00:56:44 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddaa56938924b7e6720f5434c49861506db4d66944164af8a1fba2cf3746ce6`  
		Last Modified: Thu, 14 May 2020 00:56:45 GMT  
		Size: 49.3 MB (49309584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93a61c44aec91bff63040618cb963e41791caa8359e8d1f857110605ffd774ae`  
		Last Modified: Thu, 14 May 2020 00:56:36 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f6ce944881061ccafa8419715f1675ee881509149e1afd41114ef5b5e19965`  
		Last Modified: Thu, 14 May 2020 00:56:36 GMT  
		Size: 768.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d270ec9c719ad3e448019be0663a6a551a08633340ff00be404aa77e7eb323e7`  
		Last Modified: Thu, 14 May 2020 00:56:36 GMT  
		Size: 2.1 KB (2062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca73f12be5238f15f5375c9e1a348e2c576217af0d1a08a113b96d068de178fd`  
		Last Modified: Thu, 14 May 2020 00:56:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3`

```console
$ docker pull couchdb@sha256:530734af5ab6f120421218e97793488343d3bc94a482f33f6e9f522ba9e788fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:13bcfa1f89f9a98c32c644f74c07da9b5df75af1d1b5f84fa7b9f3d5cb524f7f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.4 MB (82435186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81e56652900022f120dc43209e678679e47a21c9937f3d54f3c26fba81600811`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 18:13:18 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 15 May 2020 18:13:19 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 15 May 2020 18:13:29 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 18:13:29 GMT
ENV GOSU_VERSION=1.11
# Fri, 15 May 2020 18:13:30 GMT
ENV TINI_VERSION=0.18.0
# Fri, 15 May 2020 18:14:26 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Fri, 15 May 2020 18:14:27 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Fri, 15 May 2020 18:14:30 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Fri, 15 May 2020 18:14:30 GMT
ENV COUCHDB_VERSION=2.3.1
# Fri, 15 May 2020 18:14:31 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb stretch main" > /etc/apt/sources.list.d/couchdb.list
# Fri, 15 May 2020 18:14:53 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~stretch     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 15 May 2020 18:14:54 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Fri, 15 May 2020 18:14:54 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 15 May 2020 18:14:54 GMT
COPY file:5b465eec9f6f6fe5ff9abac1313cd161fcf9b5299d43cfb10ee0dd1935c99af4 in /usr/local/bin 
# Fri, 15 May 2020 18:14:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 15 May 2020 18:14:55 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 15 May 2020 18:14:55 GMT
VOLUME [/opt/couchdb/data]
# Fri, 15 May 2020 18:14:56 GMT
EXPOSE 4369 5984 9100
# Fri, 15 May 2020 18:14:56 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae17bf830d5c7f4017f7d358c431ffc488af80c717a9af597502caa0850a688`  
		Last Modified: Fri, 15 May 2020 18:15:42 GMT  
		Size: 3.4 KB (3416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c89a198000731720c257c505ba673e16122743472eb20bb413b706c355f47f5`  
		Last Modified: Fri, 15 May 2020 18:15:43 GMT  
		Size: 8.5 MB (8515134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09815a5893a7a236d254d84e6deabaac8f231c0d48b986815ee4c446781c22f8`  
		Last Modified: Fri, 15 May 2020 18:15:41 GMT  
		Size: 1.2 MB (1190710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3856fa5cc7cf8b1b9264a6ba6d8a253f7c24943241df26e00401df74956074ef`  
		Last Modified: Fri, 15 May 2020 18:15:41 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6544587f4aad837b2317dbe5c3773cdb9c78bb5bc6c200ee96a2f58c78abae32`  
		Last Modified: Fri, 15 May 2020 18:15:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d29e28a5747bf336273bb695ddc2bc7be4a6c5211e33c073eba8997b62bbfd09`  
		Last Modified: Fri, 15 May 2020 18:15:47 GMT  
		Size: 50.2 MB (50199994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9913ca42e32cea716d02cf7bb36ba2e517e35b9b0fccda3577821087620541c5`  
		Last Modified: Fri, 15 May 2020 18:15:39 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030f84bc109957f6addad53c8e48d75eadc9cc3398a36329d5c70ece6d1c742d`  
		Last Modified: Fri, 15 May 2020 18:15:39 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49e2942e15f39163009f042c0241e478a09051860f1c69dcf7b375bcb0592e1`  
		Last Modified: Fri, 15 May 2020 18:15:39 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c90779812142bac82d6985de583ce473ee4bc150f6b831a54a833f84a319687`  
		Last Modified: Fri, 15 May 2020 18:15:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:a3632ea9cc176b41f68f2e7c309045adda3c12236cdcd3b4751b8b34f6594a62
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76967446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02f7c6bfe5f6704bdff3a8ca636c7f47ae06650af995024492a57f20d03e3e8e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 15 May 2020 12:48:45 GMT
ADD file:a808acc4967ce5ecee8ba7a3e8769d6b91e38fecad2a792c8bd5aeef0007c6c0 in / 
# Fri, 15 May 2020 12:48:49 GMT
CMD ["bash"]
# Fri, 15 May 2020 20:46:22 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 15 May 2020 20:46:24 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 15 May 2020 20:46:43 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 20:46:44 GMT
ENV GOSU_VERSION=1.11
# Fri, 15 May 2020 20:46:45 GMT
ENV TINI_VERSION=0.18.0
# Fri, 15 May 2020 20:47:00 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Fri, 15 May 2020 20:47:01 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Fri, 15 May 2020 20:47:05 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Fri, 15 May 2020 20:47:06 GMT
ENV COUCHDB_VERSION=2.3.1
# Fri, 15 May 2020 20:47:08 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb stretch main" > /etc/apt/sources.list.d/couchdb.list
# Fri, 15 May 2020 20:47:41 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~stretch     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 15 May 2020 20:47:43 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Fri, 15 May 2020 20:47:44 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 15 May 2020 20:47:44 GMT
COPY file:5b465eec9f6f6fe5ff9abac1313cd161fcf9b5299d43cfb10ee0dd1935c99af4 in /usr/local/bin 
# Fri, 15 May 2020 20:47:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 15 May 2020 20:47:46 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 15 May 2020 20:47:47 GMT
VOLUME [/opt/couchdb/data]
# Fri, 15 May 2020 20:47:48 GMT
EXPOSE 4369 5984 9100
# Fri, 15 May 2020 20:47:48 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:7f439267e48f39a2f7463f7ec54d4ccd7f849de1dd6fd575bc2ee51c096b1da5`  
		Last Modified: Fri, 15 May 2020 12:56:01 GMT  
		Size: 20.4 MB (20375567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188a9c3447af22efe0b6b60010a280ca8a446f135900217964c954cbb6286053`  
		Last Modified: Fri, 15 May 2020 20:48:34 GMT  
		Size: 3.4 KB (3439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c16e5b60fb95f2ab9823bdd772fad8d4418983f5966ef16168c8caa809db35d`  
		Last Modified: Fri, 15 May 2020 20:48:35 GMT  
		Size: 7.7 MB (7655239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfac69bd809d9b5c95e237a6c606a9744946fe3f472c159a911fb4c9efd7258f`  
		Last Modified: Fri, 15 May 2020 20:48:33 GMT  
		Size: 1.1 MB (1125176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9ef11f43552f81aa0e45919af542da76d32eec8d757a0aa2e008ffc2840725`  
		Last Modified: Fri, 15 May 2020 20:48:33 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff027aa903830075c5cc2d1589a2f371019e90d1b486c9d03f1a73cf8bf351d1`  
		Last Modified: Fri, 15 May 2020 20:48:33 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa40728da06374e64b2eeb63bbc29018a7437f56f803ce01ac33d84d4ad3aad`  
		Last Modified: Fri, 15 May 2020 20:48:43 GMT  
		Size: 47.8 MB (47801971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d26d47fe0ab93460761aef656d13f3c91a47512b66327c539e21ab5d6d48ad`  
		Last Modified: Fri, 15 May 2020 20:48:32 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f6ca5675e02632898abb000b02da7fa92eacfd07518b6dc110c8903aa911d9`  
		Last Modified: Fri, 15 May 2020 20:48:31 GMT  
		Size: 768.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f0b79066d10a103782957bbdbf7cf5a30b39c51c860732042e0d6ae8839cd8`  
		Last Modified: Fri, 15 May 2020 20:48:31 GMT  
		Size: 2.1 KB (2061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b986b515be88cf3f1e19ca9c06c7c2d3891904f0a6b49095b240f2899ec83280`  
		Last Modified: Fri, 15 May 2020 20:48:32 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3` - linux; ppc64le

```console
$ docker pull couchdb@sha256:2638231caec3716d402975c66d4851a9c9305aba878f9c04ce40b7483d36b6e1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.2 MB (81217121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfe6b387ada120d7bca498ab7322657ee76479c8a9b25f66f69ffc1d54ac1bf1`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 13 May 2020 22:42:09 GMT
ADD file:341dbc564992a44e81b3a4f399f7de14d7340a45b73c577edb78e16da2c14584 in / 
# Wed, 13 May 2020 22:42:12 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:50:24 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 14 May 2020 00:50:37 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 14 May 2020 00:52:32 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:52:36 GMT
ENV GOSU_VERSION=1.11
# Thu, 14 May 2020 00:52:41 GMT
ENV TINI_VERSION=0.18.0
# Thu, 14 May 2020 00:53:13 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Thu, 14 May 2020 00:53:15 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Thu, 14 May 2020 00:53:22 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Thu, 14 May 2020 00:53:27 GMT
ENV COUCHDB_VERSION=2.3.1
# Thu, 14 May 2020 00:53:34 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb stretch main" > /etc/apt/sources.list.d/couchdb.list
# Thu, 14 May 2020 00:54:51 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~stretch     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 14 May 2020 00:54:55 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Thu, 14 May 2020 00:54:56 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 14 May 2020 00:54:57 GMT
COPY file:5b465eec9f6f6fe5ff9abac1313cd161fcf9b5299d43cfb10ee0dd1935c99af4 in /usr/local/bin 
# Thu, 14 May 2020 00:55:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 14 May 2020 00:55:09 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 14 May 2020 00:55:14 GMT
VOLUME [/opt/couchdb/data]
# Thu, 14 May 2020 00:55:19 GMT
EXPOSE 4369 5984 9100
# Thu, 14 May 2020 00:55:23 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:3b6ae894780534c0f99588e9cce4beb8fb7884b4578e6206b72f2db75116bb1c`  
		Last Modified: Wed, 13 May 2020 23:02:51 GMT  
		Size: 22.8 MB (22785361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c18509798b282bfa588f81e9600cf2f22f360f58297bac34227fa3655763fd6`  
		Last Modified: Thu, 14 May 2020 00:56:51 GMT  
		Size: 3.4 KB (3418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9838b2df91d2eee01d043f25a1d09479d9bce0c2c76f08a1a86dfd27e34e8073`  
		Last Modified: Thu, 14 May 2020 00:56:47 GMT  
		Size: 8.0 MB (7998426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf3599c9ca361654fc74215f1d77c8a1042958af57170e098e058400caf2548`  
		Last Modified: Thu, 14 May 2020 00:56:47 GMT  
		Size: 1.1 MB (1114275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7caa3e2e28d292a124d3a0e93a0f5875fee5e12d73371e53f3d8265eb980f9e9`  
		Last Modified: Thu, 14 May 2020 00:56:44 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0229f5e350ef91c592b92444637e8d12a018f3c61b4fc8e5b6fe0b12ff9965`  
		Last Modified: Thu, 14 May 2020 00:56:44 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddaa56938924b7e6720f5434c49861506db4d66944164af8a1fba2cf3746ce6`  
		Last Modified: Thu, 14 May 2020 00:56:45 GMT  
		Size: 49.3 MB (49309584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93a61c44aec91bff63040618cb963e41791caa8359e8d1f857110605ffd774ae`  
		Last Modified: Thu, 14 May 2020 00:56:36 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f6ce944881061ccafa8419715f1675ee881509149e1afd41114ef5b5e19965`  
		Last Modified: Thu, 14 May 2020 00:56:36 GMT  
		Size: 768.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d270ec9c719ad3e448019be0663a6a551a08633340ff00be404aa77e7eb323e7`  
		Last Modified: Thu, 14 May 2020 00:56:36 GMT  
		Size: 2.1 KB (2062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca73f12be5238f15f5375c9e1a348e2c576217af0d1a08a113b96d068de178fd`  
		Last Modified: Thu, 14 May 2020 00:56:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3.1`

```console
$ docker pull couchdb@sha256:530734af5ab6f120421218e97793488343d3bc94a482f33f6e9f522ba9e788fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:2.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:13bcfa1f89f9a98c32c644f74c07da9b5df75af1d1b5f84fa7b9f3d5cb524f7f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.4 MB (82435186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81e56652900022f120dc43209e678679e47a21c9937f3d54f3c26fba81600811`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 18:13:18 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 15 May 2020 18:13:19 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 15 May 2020 18:13:29 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 18:13:29 GMT
ENV GOSU_VERSION=1.11
# Fri, 15 May 2020 18:13:30 GMT
ENV TINI_VERSION=0.18.0
# Fri, 15 May 2020 18:14:26 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Fri, 15 May 2020 18:14:27 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Fri, 15 May 2020 18:14:30 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Fri, 15 May 2020 18:14:30 GMT
ENV COUCHDB_VERSION=2.3.1
# Fri, 15 May 2020 18:14:31 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb stretch main" > /etc/apt/sources.list.d/couchdb.list
# Fri, 15 May 2020 18:14:53 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~stretch     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 15 May 2020 18:14:54 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Fri, 15 May 2020 18:14:54 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 15 May 2020 18:14:54 GMT
COPY file:5b465eec9f6f6fe5ff9abac1313cd161fcf9b5299d43cfb10ee0dd1935c99af4 in /usr/local/bin 
# Fri, 15 May 2020 18:14:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 15 May 2020 18:14:55 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 15 May 2020 18:14:55 GMT
VOLUME [/opt/couchdb/data]
# Fri, 15 May 2020 18:14:56 GMT
EXPOSE 4369 5984 9100
# Fri, 15 May 2020 18:14:56 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae17bf830d5c7f4017f7d358c431ffc488af80c717a9af597502caa0850a688`  
		Last Modified: Fri, 15 May 2020 18:15:42 GMT  
		Size: 3.4 KB (3416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c89a198000731720c257c505ba673e16122743472eb20bb413b706c355f47f5`  
		Last Modified: Fri, 15 May 2020 18:15:43 GMT  
		Size: 8.5 MB (8515134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09815a5893a7a236d254d84e6deabaac8f231c0d48b986815ee4c446781c22f8`  
		Last Modified: Fri, 15 May 2020 18:15:41 GMT  
		Size: 1.2 MB (1190710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3856fa5cc7cf8b1b9264a6ba6d8a253f7c24943241df26e00401df74956074ef`  
		Last Modified: Fri, 15 May 2020 18:15:41 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6544587f4aad837b2317dbe5c3773cdb9c78bb5bc6c200ee96a2f58c78abae32`  
		Last Modified: Fri, 15 May 2020 18:15:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d29e28a5747bf336273bb695ddc2bc7be4a6c5211e33c073eba8997b62bbfd09`  
		Last Modified: Fri, 15 May 2020 18:15:47 GMT  
		Size: 50.2 MB (50199994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9913ca42e32cea716d02cf7bb36ba2e517e35b9b0fccda3577821087620541c5`  
		Last Modified: Fri, 15 May 2020 18:15:39 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030f84bc109957f6addad53c8e48d75eadc9cc3398a36329d5c70ece6d1c742d`  
		Last Modified: Fri, 15 May 2020 18:15:39 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49e2942e15f39163009f042c0241e478a09051860f1c69dcf7b375bcb0592e1`  
		Last Modified: Fri, 15 May 2020 18:15:39 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c90779812142bac82d6985de583ce473ee4bc150f6b831a54a833f84a319687`  
		Last Modified: Fri, 15 May 2020 18:15:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:a3632ea9cc176b41f68f2e7c309045adda3c12236cdcd3b4751b8b34f6594a62
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76967446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02f7c6bfe5f6704bdff3a8ca636c7f47ae06650af995024492a57f20d03e3e8e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 15 May 2020 12:48:45 GMT
ADD file:a808acc4967ce5ecee8ba7a3e8769d6b91e38fecad2a792c8bd5aeef0007c6c0 in / 
# Fri, 15 May 2020 12:48:49 GMT
CMD ["bash"]
# Fri, 15 May 2020 20:46:22 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 15 May 2020 20:46:24 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 15 May 2020 20:46:43 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 20:46:44 GMT
ENV GOSU_VERSION=1.11
# Fri, 15 May 2020 20:46:45 GMT
ENV TINI_VERSION=0.18.0
# Fri, 15 May 2020 20:47:00 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Fri, 15 May 2020 20:47:01 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Fri, 15 May 2020 20:47:05 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Fri, 15 May 2020 20:47:06 GMT
ENV COUCHDB_VERSION=2.3.1
# Fri, 15 May 2020 20:47:08 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb stretch main" > /etc/apt/sources.list.d/couchdb.list
# Fri, 15 May 2020 20:47:41 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~stretch     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 15 May 2020 20:47:43 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Fri, 15 May 2020 20:47:44 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 15 May 2020 20:47:44 GMT
COPY file:5b465eec9f6f6fe5ff9abac1313cd161fcf9b5299d43cfb10ee0dd1935c99af4 in /usr/local/bin 
# Fri, 15 May 2020 20:47:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 15 May 2020 20:47:46 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 15 May 2020 20:47:47 GMT
VOLUME [/opt/couchdb/data]
# Fri, 15 May 2020 20:47:48 GMT
EXPOSE 4369 5984 9100
# Fri, 15 May 2020 20:47:48 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:7f439267e48f39a2f7463f7ec54d4ccd7f849de1dd6fd575bc2ee51c096b1da5`  
		Last Modified: Fri, 15 May 2020 12:56:01 GMT  
		Size: 20.4 MB (20375567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188a9c3447af22efe0b6b60010a280ca8a446f135900217964c954cbb6286053`  
		Last Modified: Fri, 15 May 2020 20:48:34 GMT  
		Size: 3.4 KB (3439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c16e5b60fb95f2ab9823bdd772fad8d4418983f5966ef16168c8caa809db35d`  
		Last Modified: Fri, 15 May 2020 20:48:35 GMT  
		Size: 7.7 MB (7655239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfac69bd809d9b5c95e237a6c606a9744946fe3f472c159a911fb4c9efd7258f`  
		Last Modified: Fri, 15 May 2020 20:48:33 GMT  
		Size: 1.1 MB (1125176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9ef11f43552f81aa0e45919af542da76d32eec8d757a0aa2e008ffc2840725`  
		Last Modified: Fri, 15 May 2020 20:48:33 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff027aa903830075c5cc2d1589a2f371019e90d1b486c9d03f1a73cf8bf351d1`  
		Last Modified: Fri, 15 May 2020 20:48:33 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa40728da06374e64b2eeb63bbc29018a7437f56f803ce01ac33d84d4ad3aad`  
		Last Modified: Fri, 15 May 2020 20:48:43 GMT  
		Size: 47.8 MB (47801971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d26d47fe0ab93460761aef656d13f3c91a47512b66327c539e21ab5d6d48ad`  
		Last Modified: Fri, 15 May 2020 20:48:32 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f6ca5675e02632898abb000b02da7fa92eacfd07518b6dc110c8903aa911d9`  
		Last Modified: Fri, 15 May 2020 20:48:31 GMT  
		Size: 768.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f0b79066d10a103782957bbdbf7cf5a30b39c51c860732042e0d6ae8839cd8`  
		Last Modified: Fri, 15 May 2020 20:48:31 GMT  
		Size: 2.1 KB (2061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b986b515be88cf3f1e19ca9c06c7c2d3891904f0a6b49095b240f2899ec83280`  
		Last Modified: Fri, 15 May 2020 20:48:32 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3.1` - linux; ppc64le

```console
$ docker pull couchdb@sha256:2638231caec3716d402975c66d4851a9c9305aba878f9c04ce40b7483d36b6e1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.2 MB (81217121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfe6b387ada120d7bca498ab7322657ee76479c8a9b25f66f69ffc1d54ac1bf1`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 13 May 2020 22:42:09 GMT
ADD file:341dbc564992a44e81b3a4f399f7de14d7340a45b73c577edb78e16da2c14584 in / 
# Wed, 13 May 2020 22:42:12 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:50:24 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 14 May 2020 00:50:37 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 14 May 2020 00:52:32 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:52:36 GMT
ENV GOSU_VERSION=1.11
# Thu, 14 May 2020 00:52:41 GMT
ENV TINI_VERSION=0.18.0
# Thu, 14 May 2020 00:53:13 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Thu, 14 May 2020 00:53:15 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Thu, 14 May 2020 00:53:22 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Thu, 14 May 2020 00:53:27 GMT
ENV COUCHDB_VERSION=2.3.1
# Thu, 14 May 2020 00:53:34 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb stretch main" > /etc/apt/sources.list.d/couchdb.list
# Thu, 14 May 2020 00:54:51 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~stretch     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 14 May 2020 00:54:55 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Thu, 14 May 2020 00:54:56 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 14 May 2020 00:54:57 GMT
COPY file:5b465eec9f6f6fe5ff9abac1313cd161fcf9b5299d43cfb10ee0dd1935c99af4 in /usr/local/bin 
# Thu, 14 May 2020 00:55:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 14 May 2020 00:55:09 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 14 May 2020 00:55:14 GMT
VOLUME [/opt/couchdb/data]
# Thu, 14 May 2020 00:55:19 GMT
EXPOSE 4369 5984 9100
# Thu, 14 May 2020 00:55:23 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:3b6ae894780534c0f99588e9cce4beb8fb7884b4578e6206b72f2db75116bb1c`  
		Last Modified: Wed, 13 May 2020 23:02:51 GMT  
		Size: 22.8 MB (22785361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c18509798b282bfa588f81e9600cf2f22f360f58297bac34227fa3655763fd6`  
		Last Modified: Thu, 14 May 2020 00:56:51 GMT  
		Size: 3.4 KB (3418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9838b2df91d2eee01d043f25a1d09479d9bce0c2c76f08a1a86dfd27e34e8073`  
		Last Modified: Thu, 14 May 2020 00:56:47 GMT  
		Size: 8.0 MB (7998426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf3599c9ca361654fc74215f1d77c8a1042958af57170e098e058400caf2548`  
		Last Modified: Thu, 14 May 2020 00:56:47 GMT  
		Size: 1.1 MB (1114275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7caa3e2e28d292a124d3a0e93a0f5875fee5e12d73371e53f3d8265eb980f9e9`  
		Last Modified: Thu, 14 May 2020 00:56:44 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0229f5e350ef91c592b92444637e8d12a018f3c61b4fc8e5b6fe0b12ff9965`  
		Last Modified: Thu, 14 May 2020 00:56:44 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddaa56938924b7e6720f5434c49861506db4d66944164af8a1fba2cf3746ce6`  
		Last Modified: Thu, 14 May 2020 00:56:45 GMT  
		Size: 49.3 MB (49309584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93a61c44aec91bff63040618cb963e41791caa8359e8d1f857110605ffd774ae`  
		Last Modified: Thu, 14 May 2020 00:56:36 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f6ce944881061ccafa8419715f1675ee881509149e1afd41114ef5b5e19965`  
		Last Modified: Thu, 14 May 2020 00:56:36 GMT  
		Size: 768.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d270ec9c719ad3e448019be0663a6a551a08633340ff00be404aa77e7eb323e7`  
		Last Modified: Thu, 14 May 2020 00:56:36 GMT  
		Size: 2.1 KB (2062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca73f12be5238f15f5375c9e1a348e2c576217af0d1a08a113b96d068de178fd`  
		Last Modified: Thu, 14 May 2020 00:56:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3`

```console
$ docker pull couchdb@sha256:4a693ab0787663eb9a8507455f8f99c81cad1aef3224c015adddf760086ffe30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3` - linux; amd64

```console
$ docker pull couchdb@sha256:5ee5bc0e5ff1ea8d8e49519c2e12c2f7a5bd51cfd5aa13158ac70a654e0d685d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.2 MB (83244990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19586d4569840f999b3d828f267be2df149df731d5e3d6c3452ce79d3f5dc92b`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 18:10:38 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 15 May 2020 18:10:39 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 15 May 2020 18:10:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 18:10:49 GMT
ENV GOSU_VERSION=1.11
# Fri, 15 May 2020 18:10:50 GMT
ENV TINI_VERSION=0.18.0
# Fri, 15 May 2020 18:10:57 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Fri, 15 May 2020 18:10:57 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Fri, 15 May 2020 18:12:16 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Fri, 15 May 2020 18:12:17 GMT
ENV COUCHDB_VERSION=3.1.0
# Fri, 15 May 2020 18:12:18 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb buster main" > /etc/apt/sources.list.d/couchdb.list
# Fri, 15 May 2020 18:12:43 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 15 May 2020 18:12:43 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 15 May 2020 18:12:43 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 15 May 2020 18:12:43 GMT
COPY file:6952d2d38c707f223d813efd2d2969873cdd4b66d733559ef9be855aff5d8579 in /usr/local/bin 
# Fri, 15 May 2020 18:12:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 15 May 2020 18:12:44 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 15 May 2020 18:12:44 GMT
VOLUME [/opt/couchdb/data]
# Fri, 15 May 2020 18:12:45 GMT
EXPOSE 4369 5984 9100
# Fri, 15 May 2020 18:12:45 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea6be28d7902b2201739acc3aae5aa3f18ba5afdacc7453b7c1f625e7f242ac`  
		Last Modified: Fri, 15 May 2020 18:15:17 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2373eeb040b3133b40730e37185883a9bdfdad233a3841c8c0631555cd8a00c`  
		Last Modified: Fri, 15 May 2020 18:15:18 GMT  
		Size: 6.7 MB (6669989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6daa02d0e34d93f24791a9e9faa13c4fcad714b07a6b967218dd878309149d15`  
		Last Modified: Fri, 15 May 2020 18:15:17 GMT  
		Size: 1.2 MB (1192675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4f6e83db190adc7bba9232dab7492acd463b20a490f510cfcfb127c502ae46`  
		Last Modified: Fri, 15 May 2020 18:15:16 GMT  
		Size: 2.5 KB (2498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b4d696612496fbde66fcd130b817fd5437eff50e3a11f1b0fee0b2a42d49dc`  
		Last Modified: Fri, 15 May 2020 18:15:16 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43dfb476083a3cf9272f624a25e5c918ef3354356e658c731d16a43905d312d5`  
		Last Modified: Fri, 15 May 2020 18:15:21 GMT  
		Size: 48.3 MB (48274109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2322eca64972ff3114224aa8326a43f82cbe6c5b6e21d8b1fe9d8d4ec74bbcbc`  
		Last Modified: Fri, 15 May 2020 18:15:15 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2469b30b1ef30cc98a919e2319ac31a51ff88e8b0ab4c4f4cd23fdc4352804`  
		Last Modified: Fri, 15 May 2020 18:15:15 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6a34055fb7a96f96ad4ca65db87de927a7a113ff81f32c9a3bde59cc6a7a24`  
		Last Modified: Fri, 15 May 2020 18:15:15 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb5d9e7f3bd1cd11fcb0c53c740dde4bcb0d201167c2456a0a46073808334a5`  
		Last Modified: Fri, 15 May 2020 18:15:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:867d5ad3af217c527fcb9b8bcdfde874b01345607725d0c9fb6c2faa711f3e9f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78300791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48ff54be60f6acfe8ff0f96aa73954fa0cd64f7a948e2472bfc62f742b793a9e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 15 May 2020 12:44:06 GMT
ADD file:b305c1792102142f183d3084026f0fc6be3ddf8d1959b32f0a5d22d35eebcd15 in / 
# Fri, 15 May 2020 12:44:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 20:44:21 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 15 May 2020 20:44:22 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 15 May 2020 20:44:37 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 20:44:38 GMT
ENV GOSU_VERSION=1.11
# Fri, 15 May 2020 20:44:38 GMT
ENV TINI_VERSION=0.18.0
# Fri, 15 May 2020 20:44:53 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Fri, 15 May 2020 20:44:53 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Fri, 15 May 2020 20:44:56 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Fri, 15 May 2020 20:44:56 GMT
ENV COUCHDB_VERSION=3.1.0
# Fri, 15 May 2020 20:44:58 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb buster main" > /etc/apt/sources.list.d/couchdb.list
# Fri, 15 May 2020 20:45:23 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 15 May 2020 20:45:25 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 15 May 2020 20:45:26 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 15 May 2020 20:45:26 GMT
COPY file:6952d2d38c707f223d813efd2d2969873cdd4b66d733559ef9be855aff5d8579 in /usr/local/bin 
# Fri, 15 May 2020 20:45:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 15 May 2020 20:45:28 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 15 May 2020 20:45:29 GMT
VOLUME [/opt/couchdb/data]
# Fri, 15 May 2020 20:45:30 GMT
EXPOSE 4369 5984 9100
# Fri, 15 May 2020 20:45:30 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:8a7e1e68c24e5cac20ef26d29505c58456b561c431f0c683b66d1a0943f40dd4`  
		Last Modified: Fri, 15 May 2020 12:53:36 GMT  
		Size: 25.9 MB (25857195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33f13673e13d4045cd69130d2b65b00925d74929cc353756fd95cc78283aeb6`  
		Last Modified: Fri, 15 May 2020 20:48:03 GMT  
		Size: 3.4 KB (3436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca7cf6c706b4b74e6deb10fa874bce2cda5deda579b9afe75fba27737caf94b`  
		Last Modified: Fri, 15 May 2020 20:48:04 GMT  
		Size: 6.5 MB (6532335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abf2a3054613ab16eca0c5a9fd2705202ad6f626fc50ededfb92a884be8960a`  
		Last Modified: Fri, 15 May 2020 20:48:02 GMT  
		Size: 1.1 MB (1127105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adc39eed34a1a3dfe8cb06a085711f26033d016749241dec4e28e24c747a487`  
		Last Modified: Fri, 15 May 2020 20:48:02 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5902890c65495acd3018ad8fb2a6479c04e689e924258de4bec7ae320fa02429`  
		Last Modified: Fri, 15 May 2020 20:48:01 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12550950b7340e50916bb36021141da0a7d82805657d8dfa4af83f7fd048c3f9`  
		Last Modified: Fri, 15 May 2020 20:48:10 GMT  
		Size: 44.8 MB (44774682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd76bb158a698aa9a7d07fdf11194e793ce5e042ee0002982b6c6ee5589174e9`  
		Last Modified: Fri, 15 May 2020 20:48:00 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372cf04fe00b45260eb383e1b2df7c40cba81696fd984b41ead7a5a39a18e61a`  
		Last Modified: Fri, 15 May 2020 20:48:00 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c2d1f8c041a469e737e0f870b8292034314a3207920dce08612212def01367`  
		Last Modified: Fri, 15 May 2020 20:48:01 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c220bf124059d8f3acbf820793a260cab8fc5f7f64c4deede16d087a38bd725c`  
		Last Modified: Fri, 15 May 2020 20:48:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; ppc64le

```console
$ docker pull couchdb@sha256:3087c57e737ce170ac3cd533474da348a88d5a1fb24baf77009e7c168377477b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.4 MB (88390353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c15d44a2aff7b17fe29e337cdd29787e3689b0b1f3a3e63d3e969b74619455e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 13 May 2020 22:22:26 GMT
ADD file:53bd5d792aec2fc8af7c0c836e64979e003b2cecaaf5153bd456cb4e97ba5a0e in / 
# Wed, 13 May 2020 22:22:29 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:42:44 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 14 May 2020 00:42:58 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 14 May 2020 00:44:04 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:44:07 GMT
ENV GOSU_VERSION=1.11
# Thu, 14 May 2020 00:44:11 GMT
ENV TINI_VERSION=0.18.0
# Thu, 14 May 2020 00:44:45 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Thu, 14 May 2020 00:44:50 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Thu, 14 May 2020 00:46:05 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Thu, 14 May 2020 00:46:10 GMT
ENV COUCHDB_VERSION=3.1.0
# Thu, 14 May 2020 00:46:20 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb buster main" > /etc/apt/sources.list.d/couchdb.list
# Thu, 14 May 2020 00:47:28 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 14 May 2020 00:47:32 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 14 May 2020 00:47:33 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 14 May 2020 00:47:36 GMT
COPY file:6952d2d38c707f223d813efd2d2969873cdd4b66d733559ef9be855aff5d8579 in /usr/local/bin 
# Thu, 14 May 2020 00:47:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 14 May 2020 00:47:52 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 14 May 2020 00:47:59 GMT
VOLUME [/opt/couchdb/data]
# Thu, 14 May 2020 00:48:03 GMT
EXPOSE 4369 5984 9100
# Thu, 14 May 2020 00:48:14 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:d23cb84f4d6399958c00ec4c457e9c302763ee7dd86a0fb5540f75ed550c17d6`  
		Last Modified: Wed, 13 May 2020 22:57:57 GMT  
		Size: 30.5 MB (30518701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26548553458f4ed416116e39b84467c40a671ac87e3f5cd4bb78a3a0080b7beb`  
		Last Modified: Thu, 14 May 2020 00:55:56 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8eae6eed5d50faa81b267e24cda74e7dfc6159b14852c9795c8b4d659d3fd96`  
		Last Modified: Thu, 14 May 2020 00:55:54 GMT  
		Size: 7.6 MB (7578671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9f26ac2928f15ea53d3af08f5a2eb6d650cc33ac2bcd457c31fc789b92af35`  
		Last Modified: Thu, 14 May 2020 00:55:52 GMT  
		Size: 1.1 MB (1116070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e10211cda3e526eb08d0c51941c90282f66f6b67dfcdcb2bd6939907da884be`  
		Last Modified: Thu, 14 May 2020 00:55:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69ff280ba732d5f17d93a1e794aa96874e6f75c087fec5e7e537db74282f9cc`  
		Last Modified: Thu, 14 May 2020 00:55:50 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e9cb55a291cc31be0d1685bf33e4b2d7900d3ccd1502a51cb83dc0fb0f3b4c`  
		Last Modified: Thu, 14 May 2020 00:55:57 GMT  
		Size: 49.2 MB (49167458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ff7551b04433bf28ca7a9a5f8b670343a63d69dcff048aad0324722c1ccf1b`  
		Last Modified: Thu, 14 May 2020 00:55:48 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82315bbdd629134a846f8bf5754591a7d11d7328cb23ffd6ba1cbda1bdbdd40`  
		Last Modified: Thu, 14 May 2020 00:55:48 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf39863aed28c1f60c53fdc0ac072258c1d3ea5f9e39afb775a810c84b8cbe`  
		Last Modified: Thu, 14 May 2020 00:55:48 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7061e2c71165d321eae6b2fae61213c8b24b4cc955082b047b8c37924cd8c177`  
		Last Modified: Thu, 14 May 2020 00:55:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.0`

```console
$ docker pull couchdb@sha256:cdbe518822fe1a8c3d40a9abea737f4552dd7d7ce58c00afa777eae30b538e95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.0` - linux; amd64

```console
$ docker pull couchdb@sha256:986998a363c4e2d017279d4261e3006a526b99f78405b82974a20f938e1dddbb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.2 MB (83200438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ead3c12d4f794371a769b2dacbc006f270009f93325779da96fa2d33f695c38`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 18:10:38 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 15 May 2020 18:10:39 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 15 May 2020 18:10:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 18:10:49 GMT
ENV GOSU_VERSION=1.11
# Fri, 15 May 2020 18:10:50 GMT
ENV TINI_VERSION=0.18.0
# Fri, 15 May 2020 18:10:57 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Fri, 15 May 2020 18:10:57 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Fri, 15 May 2020 18:12:16 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Fri, 15 May 2020 18:12:53 GMT
ENV COUCHDB_VERSION=3.0.1
# Fri, 15 May 2020 18:12:54 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb buster main" > /etc/apt/sources.list.d/couchdb.list
# Fri, 15 May 2020 18:13:12 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 15 May 2020 18:13:12 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 15 May 2020 18:13:12 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 15 May 2020 18:13:13 GMT
COPY file:6952d2d38c707f223d813efd2d2969873cdd4b66d733559ef9be855aff5d8579 in /usr/local/bin 
# Fri, 15 May 2020 18:13:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 15 May 2020 18:13:14 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 15 May 2020 18:13:14 GMT
VOLUME [/opt/couchdb/data]
# Fri, 15 May 2020 18:13:14 GMT
EXPOSE 4369 5984 9100
# Fri, 15 May 2020 18:13:14 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea6be28d7902b2201739acc3aae5aa3f18ba5afdacc7453b7c1f625e7f242ac`  
		Last Modified: Fri, 15 May 2020 18:15:17 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2373eeb040b3133b40730e37185883a9bdfdad233a3841c8c0631555cd8a00c`  
		Last Modified: Fri, 15 May 2020 18:15:18 GMT  
		Size: 6.7 MB (6669989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6daa02d0e34d93f24791a9e9faa13c4fcad714b07a6b967218dd878309149d15`  
		Last Modified: Fri, 15 May 2020 18:15:17 GMT  
		Size: 1.2 MB (1192675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4f6e83db190adc7bba9232dab7492acd463b20a490f510cfcfb127c502ae46`  
		Last Modified: Fri, 15 May 2020 18:15:16 GMT  
		Size: 2.5 KB (2498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd398947a66b5d6cc2fbe9b6362201455a00b8633a33116df2ec61d2055b0d4`  
		Last Modified: Fri, 15 May 2020 18:15:29 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12587bfb6442de91953d384ee8b8a0672bd844cc7182dcb22e8236eefa9ef9a3`  
		Last Modified: Fri, 15 May 2020 18:15:35 GMT  
		Size: 48.2 MB (48229566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e0fb830180e150fb6ecf460d23ba43bf8ff0c13c7b05083fff9d002589558f`  
		Last Modified: Fri, 15 May 2020 18:15:28 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285ec6bc0bef9b0f7b4a64f9a34fcaad7df5b6d6533336515d3e6d60ef768a5c`  
		Last Modified: Fri, 15 May 2020 18:15:28 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e9a921f00b7dd783baf19788d0ce765059caf1e0015b9573e7542beeb85221`  
		Last Modified: Fri, 15 May 2020 18:15:28 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157026b1c49a32cd3cd895951470ba427aeedab93f9b2bdd5c97ddc11923253e`  
		Last Modified: Fri, 15 May 2020 18:15:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.0` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:c82decc85b297d08b1006db7be36f35439a02483dbd8915c59a17170109b3c3e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.2 MB (78234814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef8450230d96332ef270fffcff4dc198bb8e4bf212d06f642af11ed015821751`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 15 May 2020 12:44:06 GMT
ADD file:b305c1792102142f183d3084026f0fc6be3ddf8d1959b32f0a5d22d35eebcd15 in / 
# Fri, 15 May 2020 12:44:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 20:44:21 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 15 May 2020 20:44:22 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 15 May 2020 20:44:37 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 20:44:38 GMT
ENV GOSU_VERSION=1.11
# Fri, 15 May 2020 20:44:38 GMT
ENV TINI_VERSION=0.18.0
# Fri, 15 May 2020 20:44:53 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Fri, 15 May 2020 20:44:53 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Fri, 15 May 2020 20:44:56 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Fri, 15 May 2020 20:45:39 GMT
ENV COUCHDB_VERSION=3.0.1
# Fri, 15 May 2020 20:45:41 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb buster main" > /etc/apt/sources.list.d/couchdb.list
# Fri, 15 May 2020 20:46:06 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 15 May 2020 20:46:08 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 15 May 2020 20:46:08 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 15 May 2020 20:46:09 GMT
COPY file:6952d2d38c707f223d813efd2d2969873cdd4b66d733559ef9be855aff5d8579 in /usr/local/bin 
# Fri, 15 May 2020 20:46:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 15 May 2020 20:46:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 15 May 2020 20:46:12 GMT
VOLUME [/opt/couchdb/data]
# Fri, 15 May 2020 20:46:12 GMT
EXPOSE 4369 5984 9100
# Fri, 15 May 2020 20:46:13 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:8a7e1e68c24e5cac20ef26d29505c58456b561c431f0c683b66d1a0943f40dd4`  
		Last Modified: Fri, 15 May 2020 12:53:36 GMT  
		Size: 25.9 MB (25857195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33f13673e13d4045cd69130d2b65b00925d74929cc353756fd95cc78283aeb6`  
		Last Modified: Fri, 15 May 2020 20:48:03 GMT  
		Size: 3.4 KB (3436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca7cf6c706b4b74e6deb10fa874bce2cda5deda579b9afe75fba27737caf94b`  
		Last Modified: Fri, 15 May 2020 20:48:04 GMT  
		Size: 6.5 MB (6532335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abf2a3054613ab16eca0c5a9fd2705202ad6f626fc50ededfb92a884be8960a`  
		Last Modified: Fri, 15 May 2020 20:48:02 GMT  
		Size: 1.1 MB (1127105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adc39eed34a1a3dfe8cb06a085711f26033d016749241dec4e28e24c747a487`  
		Last Modified: Fri, 15 May 2020 20:48:02 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b951b99d4edeb3c6dd48af76152691c29bf18ee7a87ff176741b8d863a997de`  
		Last Modified: Fri, 15 May 2020 20:48:19 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501b8d24a5a424094237d50dcb88deedb8cd434f7dd2ad6f326fe3dadca6086c`  
		Last Modified: Fri, 15 May 2020 20:48:26 GMT  
		Size: 44.7 MB (44708709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82b3c1dbd1450e29724bc3c2adcf6c0f4e09419b3117e154aac86050f78e6dd`  
		Last Modified: Fri, 15 May 2020 20:48:17 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49f90ad7dba7433915e44fe913e34fa6f6c72a707f2e2a38f3942159bd84bdc`  
		Last Modified: Fri, 15 May 2020 20:48:18 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbbb2ecb70c397a259a86a9e42045e022997d9f89aff763ae28a5186579a386`  
		Last Modified: Fri, 15 May 2020 20:48:17 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f04c517a6da0bb12bb9a05967b0100a635dd530c6c490502e2fe21567b3713`  
		Last Modified: Fri, 15 May 2020 20:48:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.0` - linux; ppc64le

```console
$ docker pull couchdb@sha256:9c0e4e1d2efb7a745bbaeeb1f44c17d84e7437aab7d4df11585712de4902dcc2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.3 MB (88346854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ed7c0d37ddb7b5d8f0735e62e549ff95a35f40e72044d1a3bea669550c1f5c4`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 13 May 2020 22:22:26 GMT
ADD file:53bd5d792aec2fc8af7c0c836e64979e003b2cecaaf5153bd456cb4e97ba5a0e in / 
# Wed, 13 May 2020 22:22:29 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:42:44 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 14 May 2020 00:42:58 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 14 May 2020 00:44:04 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:44:07 GMT
ENV GOSU_VERSION=1.11
# Thu, 14 May 2020 00:44:11 GMT
ENV TINI_VERSION=0.18.0
# Thu, 14 May 2020 00:44:45 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Thu, 14 May 2020 00:44:50 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Thu, 14 May 2020 00:46:05 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Thu, 14 May 2020 00:48:30 GMT
ENV COUCHDB_VERSION=3.0.1
# Thu, 14 May 2020 00:48:41 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb buster main" > /etc/apt/sources.list.d/couchdb.list
# Thu, 14 May 2020 00:49:39 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 14 May 2020 00:49:41 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 14 May 2020 00:49:42 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 14 May 2020 00:49:43 GMT
COPY file:6952d2d38c707f223d813efd2d2969873cdd4b66d733559ef9be855aff5d8579 in /usr/local/bin 
# Thu, 14 May 2020 00:49:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 14 May 2020 00:50:01 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 14 May 2020 00:50:05 GMT
VOLUME [/opt/couchdb/data]
# Thu, 14 May 2020 00:50:07 GMT
EXPOSE 4369 5984 9100
# Thu, 14 May 2020 00:50:09 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:d23cb84f4d6399958c00ec4c457e9c302763ee7dd86a0fb5540f75ed550c17d6`  
		Last Modified: Wed, 13 May 2020 22:57:57 GMT  
		Size: 30.5 MB (30518701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26548553458f4ed416116e39b84467c40a671ac87e3f5cd4bb78a3a0080b7beb`  
		Last Modified: Thu, 14 May 2020 00:55:56 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8eae6eed5d50faa81b267e24cda74e7dfc6159b14852c9795c8b4d659d3fd96`  
		Last Modified: Thu, 14 May 2020 00:55:54 GMT  
		Size: 7.6 MB (7578671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9f26ac2928f15ea53d3af08f5a2eb6d650cc33ac2bcd457c31fc789b92af35`  
		Last Modified: Thu, 14 May 2020 00:55:52 GMT  
		Size: 1.1 MB (1116070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e10211cda3e526eb08d0c51941c90282f66f6b67dfcdcb2bd6939907da884be`  
		Last Modified: Thu, 14 May 2020 00:55:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c7ebbb3dce01ad81c079e805b9a5c4cdf20a0f5837ba00882ff57badaa5a13`  
		Last Modified: Thu, 14 May 2020 00:56:17 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f715c48ae0a2852cb7866bbeeea1c421e56c725da014380918d067132b2875`  
		Last Modified: Thu, 14 May 2020 00:56:22 GMT  
		Size: 49.1 MB (49123961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4140a9478395a72b1792d375d89da4743e93d563364665cdd5e2bd0566f5c8`  
		Last Modified: Thu, 14 May 2020 00:56:14 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6423d2161b3acb88ff67b02a68658d4c7f4d7d53ef5cbae7facc29ee3a534ae2`  
		Last Modified: Thu, 14 May 2020 00:56:14 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b510de5c1815400d5b34d04d0b32d8a855558646e54b8d381cf3a002cefc2c44`  
		Last Modified: Thu, 14 May 2020 00:56:14 GMT  
		Size: 2.0 KB (2050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c74ea1ac228511b630ffe0d1250b7ab1be8d3c85034ff18da1d52e4f46dbe8`  
		Last Modified: Thu, 14 May 2020 00:56:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.0.1`

```console
$ docker pull couchdb@sha256:cdbe518822fe1a8c3d40a9abea737f4552dd7d7ce58c00afa777eae30b538e95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.0.1` - linux; amd64

```console
$ docker pull couchdb@sha256:986998a363c4e2d017279d4261e3006a526b99f78405b82974a20f938e1dddbb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.2 MB (83200438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ead3c12d4f794371a769b2dacbc006f270009f93325779da96fa2d33f695c38`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 18:10:38 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 15 May 2020 18:10:39 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 15 May 2020 18:10:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 18:10:49 GMT
ENV GOSU_VERSION=1.11
# Fri, 15 May 2020 18:10:50 GMT
ENV TINI_VERSION=0.18.0
# Fri, 15 May 2020 18:10:57 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Fri, 15 May 2020 18:10:57 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Fri, 15 May 2020 18:12:16 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Fri, 15 May 2020 18:12:53 GMT
ENV COUCHDB_VERSION=3.0.1
# Fri, 15 May 2020 18:12:54 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb buster main" > /etc/apt/sources.list.d/couchdb.list
# Fri, 15 May 2020 18:13:12 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 15 May 2020 18:13:12 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 15 May 2020 18:13:12 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 15 May 2020 18:13:13 GMT
COPY file:6952d2d38c707f223d813efd2d2969873cdd4b66d733559ef9be855aff5d8579 in /usr/local/bin 
# Fri, 15 May 2020 18:13:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 15 May 2020 18:13:14 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 15 May 2020 18:13:14 GMT
VOLUME [/opt/couchdb/data]
# Fri, 15 May 2020 18:13:14 GMT
EXPOSE 4369 5984 9100
# Fri, 15 May 2020 18:13:14 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea6be28d7902b2201739acc3aae5aa3f18ba5afdacc7453b7c1f625e7f242ac`  
		Last Modified: Fri, 15 May 2020 18:15:17 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2373eeb040b3133b40730e37185883a9bdfdad233a3841c8c0631555cd8a00c`  
		Last Modified: Fri, 15 May 2020 18:15:18 GMT  
		Size: 6.7 MB (6669989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6daa02d0e34d93f24791a9e9faa13c4fcad714b07a6b967218dd878309149d15`  
		Last Modified: Fri, 15 May 2020 18:15:17 GMT  
		Size: 1.2 MB (1192675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4f6e83db190adc7bba9232dab7492acd463b20a490f510cfcfb127c502ae46`  
		Last Modified: Fri, 15 May 2020 18:15:16 GMT  
		Size: 2.5 KB (2498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd398947a66b5d6cc2fbe9b6362201455a00b8633a33116df2ec61d2055b0d4`  
		Last Modified: Fri, 15 May 2020 18:15:29 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12587bfb6442de91953d384ee8b8a0672bd844cc7182dcb22e8236eefa9ef9a3`  
		Last Modified: Fri, 15 May 2020 18:15:35 GMT  
		Size: 48.2 MB (48229566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e0fb830180e150fb6ecf460d23ba43bf8ff0c13c7b05083fff9d002589558f`  
		Last Modified: Fri, 15 May 2020 18:15:28 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285ec6bc0bef9b0f7b4a64f9a34fcaad7df5b6d6533336515d3e6d60ef768a5c`  
		Last Modified: Fri, 15 May 2020 18:15:28 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e9a921f00b7dd783baf19788d0ce765059caf1e0015b9573e7542beeb85221`  
		Last Modified: Fri, 15 May 2020 18:15:28 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157026b1c49a32cd3cd895951470ba427aeedab93f9b2bdd5c97ddc11923253e`  
		Last Modified: Fri, 15 May 2020 18:15:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.0.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:c82decc85b297d08b1006db7be36f35439a02483dbd8915c59a17170109b3c3e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.2 MB (78234814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef8450230d96332ef270fffcff4dc198bb8e4bf212d06f642af11ed015821751`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 15 May 2020 12:44:06 GMT
ADD file:b305c1792102142f183d3084026f0fc6be3ddf8d1959b32f0a5d22d35eebcd15 in / 
# Fri, 15 May 2020 12:44:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 20:44:21 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 15 May 2020 20:44:22 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 15 May 2020 20:44:37 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 20:44:38 GMT
ENV GOSU_VERSION=1.11
# Fri, 15 May 2020 20:44:38 GMT
ENV TINI_VERSION=0.18.0
# Fri, 15 May 2020 20:44:53 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Fri, 15 May 2020 20:44:53 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Fri, 15 May 2020 20:44:56 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Fri, 15 May 2020 20:45:39 GMT
ENV COUCHDB_VERSION=3.0.1
# Fri, 15 May 2020 20:45:41 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb buster main" > /etc/apt/sources.list.d/couchdb.list
# Fri, 15 May 2020 20:46:06 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 15 May 2020 20:46:08 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 15 May 2020 20:46:08 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 15 May 2020 20:46:09 GMT
COPY file:6952d2d38c707f223d813efd2d2969873cdd4b66d733559ef9be855aff5d8579 in /usr/local/bin 
# Fri, 15 May 2020 20:46:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 15 May 2020 20:46:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 15 May 2020 20:46:12 GMT
VOLUME [/opt/couchdb/data]
# Fri, 15 May 2020 20:46:12 GMT
EXPOSE 4369 5984 9100
# Fri, 15 May 2020 20:46:13 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:8a7e1e68c24e5cac20ef26d29505c58456b561c431f0c683b66d1a0943f40dd4`  
		Last Modified: Fri, 15 May 2020 12:53:36 GMT  
		Size: 25.9 MB (25857195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33f13673e13d4045cd69130d2b65b00925d74929cc353756fd95cc78283aeb6`  
		Last Modified: Fri, 15 May 2020 20:48:03 GMT  
		Size: 3.4 KB (3436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca7cf6c706b4b74e6deb10fa874bce2cda5deda579b9afe75fba27737caf94b`  
		Last Modified: Fri, 15 May 2020 20:48:04 GMT  
		Size: 6.5 MB (6532335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abf2a3054613ab16eca0c5a9fd2705202ad6f626fc50ededfb92a884be8960a`  
		Last Modified: Fri, 15 May 2020 20:48:02 GMT  
		Size: 1.1 MB (1127105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adc39eed34a1a3dfe8cb06a085711f26033d016749241dec4e28e24c747a487`  
		Last Modified: Fri, 15 May 2020 20:48:02 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b951b99d4edeb3c6dd48af76152691c29bf18ee7a87ff176741b8d863a997de`  
		Last Modified: Fri, 15 May 2020 20:48:19 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501b8d24a5a424094237d50dcb88deedb8cd434f7dd2ad6f326fe3dadca6086c`  
		Last Modified: Fri, 15 May 2020 20:48:26 GMT  
		Size: 44.7 MB (44708709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b82b3c1dbd1450e29724bc3c2adcf6c0f4e09419b3117e154aac86050f78e6dd`  
		Last Modified: Fri, 15 May 2020 20:48:17 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49f90ad7dba7433915e44fe913e34fa6f6c72a707f2e2a38f3942159bd84bdc`  
		Last Modified: Fri, 15 May 2020 20:48:18 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbbb2ecb70c397a259a86a9e42045e022997d9f89aff763ae28a5186579a386`  
		Last Modified: Fri, 15 May 2020 20:48:17 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f04c517a6da0bb12bb9a05967b0100a635dd530c6c490502e2fe21567b3713`  
		Last Modified: Fri, 15 May 2020 20:48:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.0.1` - linux; ppc64le

```console
$ docker pull couchdb@sha256:9c0e4e1d2efb7a745bbaeeb1f44c17d84e7437aab7d4df11585712de4902dcc2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.3 MB (88346854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ed7c0d37ddb7b5d8f0735e62e549ff95a35f40e72044d1a3bea669550c1f5c4`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 13 May 2020 22:22:26 GMT
ADD file:53bd5d792aec2fc8af7c0c836e64979e003b2cecaaf5153bd456cb4e97ba5a0e in / 
# Wed, 13 May 2020 22:22:29 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:42:44 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 14 May 2020 00:42:58 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 14 May 2020 00:44:04 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:44:07 GMT
ENV GOSU_VERSION=1.11
# Thu, 14 May 2020 00:44:11 GMT
ENV TINI_VERSION=0.18.0
# Thu, 14 May 2020 00:44:45 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Thu, 14 May 2020 00:44:50 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Thu, 14 May 2020 00:46:05 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Thu, 14 May 2020 00:48:30 GMT
ENV COUCHDB_VERSION=3.0.1
# Thu, 14 May 2020 00:48:41 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb buster main" > /etc/apt/sources.list.d/couchdb.list
# Thu, 14 May 2020 00:49:39 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 14 May 2020 00:49:41 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 14 May 2020 00:49:42 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 14 May 2020 00:49:43 GMT
COPY file:6952d2d38c707f223d813efd2d2969873cdd4b66d733559ef9be855aff5d8579 in /usr/local/bin 
# Thu, 14 May 2020 00:49:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 14 May 2020 00:50:01 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 14 May 2020 00:50:05 GMT
VOLUME [/opt/couchdb/data]
# Thu, 14 May 2020 00:50:07 GMT
EXPOSE 4369 5984 9100
# Thu, 14 May 2020 00:50:09 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:d23cb84f4d6399958c00ec4c457e9c302763ee7dd86a0fb5540f75ed550c17d6`  
		Last Modified: Wed, 13 May 2020 22:57:57 GMT  
		Size: 30.5 MB (30518701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26548553458f4ed416116e39b84467c40a671ac87e3f5cd4bb78a3a0080b7beb`  
		Last Modified: Thu, 14 May 2020 00:55:56 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8eae6eed5d50faa81b267e24cda74e7dfc6159b14852c9795c8b4d659d3fd96`  
		Last Modified: Thu, 14 May 2020 00:55:54 GMT  
		Size: 7.6 MB (7578671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9f26ac2928f15ea53d3af08f5a2eb6d650cc33ac2bcd457c31fc789b92af35`  
		Last Modified: Thu, 14 May 2020 00:55:52 GMT  
		Size: 1.1 MB (1116070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e10211cda3e526eb08d0c51941c90282f66f6b67dfcdcb2bd6939907da884be`  
		Last Modified: Thu, 14 May 2020 00:55:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c7ebbb3dce01ad81c079e805b9a5c4cdf20a0f5837ba00882ff57badaa5a13`  
		Last Modified: Thu, 14 May 2020 00:56:17 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f715c48ae0a2852cb7866bbeeea1c421e56c725da014380918d067132b2875`  
		Last Modified: Thu, 14 May 2020 00:56:22 GMT  
		Size: 49.1 MB (49123961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4140a9478395a72b1792d375d89da4743e93d563364665cdd5e2bd0566f5c8`  
		Last Modified: Thu, 14 May 2020 00:56:14 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6423d2161b3acb88ff67b02a68658d4c7f4d7d53ef5cbae7facc29ee3a534ae2`  
		Last Modified: Thu, 14 May 2020 00:56:14 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b510de5c1815400d5b34d04d0b32d8a855558646e54b8d381cf3a002cefc2c44`  
		Last Modified: Thu, 14 May 2020 00:56:14 GMT  
		Size: 2.0 KB (2050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c74ea1ac228511b630ffe0d1250b7ab1be8d3c85034ff18da1d52e4f46dbe8`  
		Last Modified: Thu, 14 May 2020 00:56:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1`

```console
$ docker pull couchdb@sha256:4a693ab0787663eb9a8507455f8f99c81cad1aef3224c015adddf760086ffe30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:5ee5bc0e5ff1ea8d8e49519c2e12c2f7a5bd51cfd5aa13158ac70a654e0d685d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.2 MB (83244990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19586d4569840f999b3d828f267be2df149df731d5e3d6c3452ce79d3f5dc92b`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 18:10:38 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 15 May 2020 18:10:39 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 15 May 2020 18:10:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 18:10:49 GMT
ENV GOSU_VERSION=1.11
# Fri, 15 May 2020 18:10:50 GMT
ENV TINI_VERSION=0.18.0
# Fri, 15 May 2020 18:10:57 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Fri, 15 May 2020 18:10:57 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Fri, 15 May 2020 18:12:16 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Fri, 15 May 2020 18:12:17 GMT
ENV COUCHDB_VERSION=3.1.0
# Fri, 15 May 2020 18:12:18 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb buster main" > /etc/apt/sources.list.d/couchdb.list
# Fri, 15 May 2020 18:12:43 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 15 May 2020 18:12:43 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 15 May 2020 18:12:43 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 15 May 2020 18:12:43 GMT
COPY file:6952d2d38c707f223d813efd2d2969873cdd4b66d733559ef9be855aff5d8579 in /usr/local/bin 
# Fri, 15 May 2020 18:12:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 15 May 2020 18:12:44 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 15 May 2020 18:12:44 GMT
VOLUME [/opt/couchdb/data]
# Fri, 15 May 2020 18:12:45 GMT
EXPOSE 4369 5984 9100
# Fri, 15 May 2020 18:12:45 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea6be28d7902b2201739acc3aae5aa3f18ba5afdacc7453b7c1f625e7f242ac`  
		Last Modified: Fri, 15 May 2020 18:15:17 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2373eeb040b3133b40730e37185883a9bdfdad233a3841c8c0631555cd8a00c`  
		Last Modified: Fri, 15 May 2020 18:15:18 GMT  
		Size: 6.7 MB (6669989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6daa02d0e34d93f24791a9e9faa13c4fcad714b07a6b967218dd878309149d15`  
		Last Modified: Fri, 15 May 2020 18:15:17 GMT  
		Size: 1.2 MB (1192675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4f6e83db190adc7bba9232dab7492acd463b20a490f510cfcfb127c502ae46`  
		Last Modified: Fri, 15 May 2020 18:15:16 GMT  
		Size: 2.5 KB (2498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b4d696612496fbde66fcd130b817fd5437eff50e3a11f1b0fee0b2a42d49dc`  
		Last Modified: Fri, 15 May 2020 18:15:16 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43dfb476083a3cf9272f624a25e5c918ef3354356e658c731d16a43905d312d5`  
		Last Modified: Fri, 15 May 2020 18:15:21 GMT  
		Size: 48.3 MB (48274109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2322eca64972ff3114224aa8326a43f82cbe6c5b6e21d8b1fe9d8d4ec74bbcbc`  
		Last Modified: Fri, 15 May 2020 18:15:15 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2469b30b1ef30cc98a919e2319ac31a51ff88e8b0ab4c4f4cd23fdc4352804`  
		Last Modified: Fri, 15 May 2020 18:15:15 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6a34055fb7a96f96ad4ca65db87de927a7a113ff81f32c9a3bde59cc6a7a24`  
		Last Modified: Fri, 15 May 2020 18:15:15 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb5d9e7f3bd1cd11fcb0c53c740dde4bcb0d201167c2456a0a46073808334a5`  
		Last Modified: Fri, 15 May 2020 18:15:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:867d5ad3af217c527fcb9b8bcdfde874b01345607725d0c9fb6c2faa711f3e9f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78300791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48ff54be60f6acfe8ff0f96aa73954fa0cd64f7a948e2472bfc62f742b793a9e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 15 May 2020 12:44:06 GMT
ADD file:b305c1792102142f183d3084026f0fc6be3ddf8d1959b32f0a5d22d35eebcd15 in / 
# Fri, 15 May 2020 12:44:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 20:44:21 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 15 May 2020 20:44:22 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 15 May 2020 20:44:37 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 20:44:38 GMT
ENV GOSU_VERSION=1.11
# Fri, 15 May 2020 20:44:38 GMT
ENV TINI_VERSION=0.18.0
# Fri, 15 May 2020 20:44:53 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Fri, 15 May 2020 20:44:53 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Fri, 15 May 2020 20:44:56 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Fri, 15 May 2020 20:44:56 GMT
ENV COUCHDB_VERSION=3.1.0
# Fri, 15 May 2020 20:44:58 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb buster main" > /etc/apt/sources.list.d/couchdb.list
# Fri, 15 May 2020 20:45:23 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 15 May 2020 20:45:25 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 15 May 2020 20:45:26 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 15 May 2020 20:45:26 GMT
COPY file:6952d2d38c707f223d813efd2d2969873cdd4b66d733559ef9be855aff5d8579 in /usr/local/bin 
# Fri, 15 May 2020 20:45:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 15 May 2020 20:45:28 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 15 May 2020 20:45:29 GMT
VOLUME [/opt/couchdb/data]
# Fri, 15 May 2020 20:45:30 GMT
EXPOSE 4369 5984 9100
# Fri, 15 May 2020 20:45:30 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:8a7e1e68c24e5cac20ef26d29505c58456b561c431f0c683b66d1a0943f40dd4`  
		Last Modified: Fri, 15 May 2020 12:53:36 GMT  
		Size: 25.9 MB (25857195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33f13673e13d4045cd69130d2b65b00925d74929cc353756fd95cc78283aeb6`  
		Last Modified: Fri, 15 May 2020 20:48:03 GMT  
		Size: 3.4 KB (3436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca7cf6c706b4b74e6deb10fa874bce2cda5deda579b9afe75fba27737caf94b`  
		Last Modified: Fri, 15 May 2020 20:48:04 GMT  
		Size: 6.5 MB (6532335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abf2a3054613ab16eca0c5a9fd2705202ad6f626fc50ededfb92a884be8960a`  
		Last Modified: Fri, 15 May 2020 20:48:02 GMT  
		Size: 1.1 MB (1127105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adc39eed34a1a3dfe8cb06a085711f26033d016749241dec4e28e24c747a487`  
		Last Modified: Fri, 15 May 2020 20:48:02 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5902890c65495acd3018ad8fb2a6479c04e689e924258de4bec7ae320fa02429`  
		Last Modified: Fri, 15 May 2020 20:48:01 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12550950b7340e50916bb36021141da0a7d82805657d8dfa4af83f7fd048c3f9`  
		Last Modified: Fri, 15 May 2020 20:48:10 GMT  
		Size: 44.8 MB (44774682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd76bb158a698aa9a7d07fdf11194e793ce5e042ee0002982b6c6ee5589174e9`  
		Last Modified: Fri, 15 May 2020 20:48:00 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372cf04fe00b45260eb383e1b2df7c40cba81696fd984b41ead7a5a39a18e61a`  
		Last Modified: Fri, 15 May 2020 20:48:00 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c2d1f8c041a469e737e0f870b8292034314a3207920dce08612212def01367`  
		Last Modified: Fri, 15 May 2020 20:48:01 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c220bf124059d8f3acbf820793a260cab8fc5f7f64c4deede16d087a38bd725c`  
		Last Modified: Fri, 15 May 2020 20:48:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1` - linux; ppc64le

```console
$ docker pull couchdb@sha256:3087c57e737ce170ac3cd533474da348a88d5a1fb24baf77009e7c168377477b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.4 MB (88390353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c15d44a2aff7b17fe29e337cdd29787e3689b0b1f3a3e63d3e969b74619455e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 13 May 2020 22:22:26 GMT
ADD file:53bd5d792aec2fc8af7c0c836e64979e003b2cecaaf5153bd456cb4e97ba5a0e in / 
# Wed, 13 May 2020 22:22:29 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:42:44 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 14 May 2020 00:42:58 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 14 May 2020 00:44:04 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:44:07 GMT
ENV GOSU_VERSION=1.11
# Thu, 14 May 2020 00:44:11 GMT
ENV TINI_VERSION=0.18.0
# Thu, 14 May 2020 00:44:45 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Thu, 14 May 2020 00:44:50 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Thu, 14 May 2020 00:46:05 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Thu, 14 May 2020 00:46:10 GMT
ENV COUCHDB_VERSION=3.1.0
# Thu, 14 May 2020 00:46:20 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb buster main" > /etc/apt/sources.list.d/couchdb.list
# Thu, 14 May 2020 00:47:28 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 14 May 2020 00:47:32 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 14 May 2020 00:47:33 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 14 May 2020 00:47:36 GMT
COPY file:6952d2d38c707f223d813efd2d2969873cdd4b66d733559ef9be855aff5d8579 in /usr/local/bin 
# Thu, 14 May 2020 00:47:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 14 May 2020 00:47:52 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 14 May 2020 00:47:59 GMT
VOLUME [/opt/couchdb/data]
# Thu, 14 May 2020 00:48:03 GMT
EXPOSE 4369 5984 9100
# Thu, 14 May 2020 00:48:14 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:d23cb84f4d6399958c00ec4c457e9c302763ee7dd86a0fb5540f75ed550c17d6`  
		Last Modified: Wed, 13 May 2020 22:57:57 GMT  
		Size: 30.5 MB (30518701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26548553458f4ed416116e39b84467c40a671ac87e3f5cd4bb78a3a0080b7beb`  
		Last Modified: Thu, 14 May 2020 00:55:56 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8eae6eed5d50faa81b267e24cda74e7dfc6159b14852c9795c8b4d659d3fd96`  
		Last Modified: Thu, 14 May 2020 00:55:54 GMT  
		Size: 7.6 MB (7578671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9f26ac2928f15ea53d3af08f5a2eb6d650cc33ac2bcd457c31fc789b92af35`  
		Last Modified: Thu, 14 May 2020 00:55:52 GMT  
		Size: 1.1 MB (1116070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e10211cda3e526eb08d0c51941c90282f66f6b67dfcdcb2bd6939907da884be`  
		Last Modified: Thu, 14 May 2020 00:55:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69ff280ba732d5f17d93a1e794aa96874e6f75c087fec5e7e537db74282f9cc`  
		Last Modified: Thu, 14 May 2020 00:55:50 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e9cb55a291cc31be0d1685bf33e4b2d7900d3ccd1502a51cb83dc0fb0f3b4c`  
		Last Modified: Thu, 14 May 2020 00:55:57 GMT  
		Size: 49.2 MB (49167458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ff7551b04433bf28ca7a9a5f8b670343a63d69dcff048aad0324722c1ccf1b`  
		Last Modified: Thu, 14 May 2020 00:55:48 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82315bbdd629134a846f8bf5754591a7d11d7328cb23ffd6ba1cbda1bdbdd40`  
		Last Modified: Thu, 14 May 2020 00:55:48 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf39863aed28c1f60c53fdc0ac072258c1d3ea5f9e39afb775a810c84b8cbe`  
		Last Modified: Thu, 14 May 2020 00:55:48 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7061e2c71165d321eae6b2fae61213c8b24b4cc955082b047b8c37924cd8c177`  
		Last Modified: Thu, 14 May 2020 00:55:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1.0`

```console
$ docker pull couchdb@sha256:4a693ab0787663eb9a8507455f8f99c81cad1aef3224c015adddf760086ffe30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.1.0` - linux; amd64

```console
$ docker pull couchdb@sha256:5ee5bc0e5ff1ea8d8e49519c2e12c2f7a5bd51cfd5aa13158ac70a654e0d685d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.2 MB (83244990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19586d4569840f999b3d828f267be2df149df731d5e3d6c3452ce79d3f5dc92b`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 18:10:38 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 15 May 2020 18:10:39 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 15 May 2020 18:10:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 18:10:49 GMT
ENV GOSU_VERSION=1.11
# Fri, 15 May 2020 18:10:50 GMT
ENV TINI_VERSION=0.18.0
# Fri, 15 May 2020 18:10:57 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Fri, 15 May 2020 18:10:57 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Fri, 15 May 2020 18:12:16 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Fri, 15 May 2020 18:12:17 GMT
ENV COUCHDB_VERSION=3.1.0
# Fri, 15 May 2020 18:12:18 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb buster main" > /etc/apt/sources.list.d/couchdb.list
# Fri, 15 May 2020 18:12:43 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 15 May 2020 18:12:43 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 15 May 2020 18:12:43 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 15 May 2020 18:12:43 GMT
COPY file:6952d2d38c707f223d813efd2d2969873cdd4b66d733559ef9be855aff5d8579 in /usr/local/bin 
# Fri, 15 May 2020 18:12:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 15 May 2020 18:12:44 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 15 May 2020 18:12:44 GMT
VOLUME [/opt/couchdb/data]
# Fri, 15 May 2020 18:12:45 GMT
EXPOSE 4369 5984 9100
# Fri, 15 May 2020 18:12:45 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea6be28d7902b2201739acc3aae5aa3f18ba5afdacc7453b7c1f625e7f242ac`  
		Last Modified: Fri, 15 May 2020 18:15:17 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2373eeb040b3133b40730e37185883a9bdfdad233a3841c8c0631555cd8a00c`  
		Last Modified: Fri, 15 May 2020 18:15:18 GMT  
		Size: 6.7 MB (6669989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6daa02d0e34d93f24791a9e9faa13c4fcad714b07a6b967218dd878309149d15`  
		Last Modified: Fri, 15 May 2020 18:15:17 GMT  
		Size: 1.2 MB (1192675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4f6e83db190adc7bba9232dab7492acd463b20a490f510cfcfb127c502ae46`  
		Last Modified: Fri, 15 May 2020 18:15:16 GMT  
		Size: 2.5 KB (2498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b4d696612496fbde66fcd130b817fd5437eff50e3a11f1b0fee0b2a42d49dc`  
		Last Modified: Fri, 15 May 2020 18:15:16 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43dfb476083a3cf9272f624a25e5c918ef3354356e658c731d16a43905d312d5`  
		Last Modified: Fri, 15 May 2020 18:15:21 GMT  
		Size: 48.3 MB (48274109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2322eca64972ff3114224aa8326a43f82cbe6c5b6e21d8b1fe9d8d4ec74bbcbc`  
		Last Modified: Fri, 15 May 2020 18:15:15 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2469b30b1ef30cc98a919e2319ac31a51ff88e8b0ab4c4f4cd23fdc4352804`  
		Last Modified: Fri, 15 May 2020 18:15:15 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6a34055fb7a96f96ad4ca65db87de927a7a113ff81f32c9a3bde59cc6a7a24`  
		Last Modified: Fri, 15 May 2020 18:15:15 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb5d9e7f3bd1cd11fcb0c53c740dde4bcb0d201167c2456a0a46073808334a5`  
		Last Modified: Fri, 15 May 2020 18:15:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1.0` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:867d5ad3af217c527fcb9b8bcdfde874b01345607725d0c9fb6c2faa711f3e9f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78300791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48ff54be60f6acfe8ff0f96aa73954fa0cd64f7a948e2472bfc62f742b793a9e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 15 May 2020 12:44:06 GMT
ADD file:b305c1792102142f183d3084026f0fc6be3ddf8d1959b32f0a5d22d35eebcd15 in / 
# Fri, 15 May 2020 12:44:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 20:44:21 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 15 May 2020 20:44:22 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 15 May 2020 20:44:37 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 20:44:38 GMT
ENV GOSU_VERSION=1.11
# Fri, 15 May 2020 20:44:38 GMT
ENV TINI_VERSION=0.18.0
# Fri, 15 May 2020 20:44:53 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Fri, 15 May 2020 20:44:53 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Fri, 15 May 2020 20:44:56 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Fri, 15 May 2020 20:44:56 GMT
ENV COUCHDB_VERSION=3.1.0
# Fri, 15 May 2020 20:44:58 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb buster main" > /etc/apt/sources.list.d/couchdb.list
# Fri, 15 May 2020 20:45:23 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 15 May 2020 20:45:25 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 15 May 2020 20:45:26 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 15 May 2020 20:45:26 GMT
COPY file:6952d2d38c707f223d813efd2d2969873cdd4b66d733559ef9be855aff5d8579 in /usr/local/bin 
# Fri, 15 May 2020 20:45:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 15 May 2020 20:45:28 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 15 May 2020 20:45:29 GMT
VOLUME [/opt/couchdb/data]
# Fri, 15 May 2020 20:45:30 GMT
EXPOSE 4369 5984 9100
# Fri, 15 May 2020 20:45:30 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:8a7e1e68c24e5cac20ef26d29505c58456b561c431f0c683b66d1a0943f40dd4`  
		Last Modified: Fri, 15 May 2020 12:53:36 GMT  
		Size: 25.9 MB (25857195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33f13673e13d4045cd69130d2b65b00925d74929cc353756fd95cc78283aeb6`  
		Last Modified: Fri, 15 May 2020 20:48:03 GMT  
		Size: 3.4 KB (3436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca7cf6c706b4b74e6deb10fa874bce2cda5deda579b9afe75fba27737caf94b`  
		Last Modified: Fri, 15 May 2020 20:48:04 GMT  
		Size: 6.5 MB (6532335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abf2a3054613ab16eca0c5a9fd2705202ad6f626fc50ededfb92a884be8960a`  
		Last Modified: Fri, 15 May 2020 20:48:02 GMT  
		Size: 1.1 MB (1127105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adc39eed34a1a3dfe8cb06a085711f26033d016749241dec4e28e24c747a487`  
		Last Modified: Fri, 15 May 2020 20:48:02 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5902890c65495acd3018ad8fb2a6479c04e689e924258de4bec7ae320fa02429`  
		Last Modified: Fri, 15 May 2020 20:48:01 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12550950b7340e50916bb36021141da0a7d82805657d8dfa4af83f7fd048c3f9`  
		Last Modified: Fri, 15 May 2020 20:48:10 GMT  
		Size: 44.8 MB (44774682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd76bb158a698aa9a7d07fdf11194e793ce5e042ee0002982b6c6ee5589174e9`  
		Last Modified: Fri, 15 May 2020 20:48:00 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372cf04fe00b45260eb383e1b2df7c40cba81696fd984b41ead7a5a39a18e61a`  
		Last Modified: Fri, 15 May 2020 20:48:00 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c2d1f8c041a469e737e0f870b8292034314a3207920dce08612212def01367`  
		Last Modified: Fri, 15 May 2020 20:48:01 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c220bf124059d8f3acbf820793a260cab8fc5f7f64c4deede16d087a38bd725c`  
		Last Modified: Fri, 15 May 2020 20:48:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1.0` - linux; ppc64le

```console
$ docker pull couchdb@sha256:3087c57e737ce170ac3cd533474da348a88d5a1fb24baf77009e7c168377477b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.4 MB (88390353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c15d44a2aff7b17fe29e337cdd29787e3689b0b1f3a3e63d3e969b74619455e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 13 May 2020 22:22:26 GMT
ADD file:53bd5d792aec2fc8af7c0c836e64979e003b2cecaaf5153bd456cb4e97ba5a0e in / 
# Wed, 13 May 2020 22:22:29 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:42:44 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 14 May 2020 00:42:58 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 14 May 2020 00:44:04 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:44:07 GMT
ENV GOSU_VERSION=1.11
# Thu, 14 May 2020 00:44:11 GMT
ENV TINI_VERSION=0.18.0
# Thu, 14 May 2020 00:44:45 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Thu, 14 May 2020 00:44:50 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Thu, 14 May 2020 00:46:05 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Thu, 14 May 2020 00:46:10 GMT
ENV COUCHDB_VERSION=3.1.0
# Thu, 14 May 2020 00:46:20 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb buster main" > /etc/apt/sources.list.d/couchdb.list
# Thu, 14 May 2020 00:47:28 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 14 May 2020 00:47:32 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 14 May 2020 00:47:33 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 14 May 2020 00:47:36 GMT
COPY file:6952d2d38c707f223d813efd2d2969873cdd4b66d733559ef9be855aff5d8579 in /usr/local/bin 
# Thu, 14 May 2020 00:47:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 14 May 2020 00:47:52 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 14 May 2020 00:47:59 GMT
VOLUME [/opt/couchdb/data]
# Thu, 14 May 2020 00:48:03 GMT
EXPOSE 4369 5984 9100
# Thu, 14 May 2020 00:48:14 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:d23cb84f4d6399958c00ec4c457e9c302763ee7dd86a0fb5540f75ed550c17d6`  
		Last Modified: Wed, 13 May 2020 22:57:57 GMT  
		Size: 30.5 MB (30518701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26548553458f4ed416116e39b84467c40a671ac87e3f5cd4bb78a3a0080b7beb`  
		Last Modified: Thu, 14 May 2020 00:55:56 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8eae6eed5d50faa81b267e24cda74e7dfc6159b14852c9795c8b4d659d3fd96`  
		Last Modified: Thu, 14 May 2020 00:55:54 GMT  
		Size: 7.6 MB (7578671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9f26ac2928f15ea53d3af08f5a2eb6d650cc33ac2bcd457c31fc789b92af35`  
		Last Modified: Thu, 14 May 2020 00:55:52 GMT  
		Size: 1.1 MB (1116070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e10211cda3e526eb08d0c51941c90282f66f6b67dfcdcb2bd6939907da884be`  
		Last Modified: Thu, 14 May 2020 00:55:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69ff280ba732d5f17d93a1e794aa96874e6f75c087fec5e7e537db74282f9cc`  
		Last Modified: Thu, 14 May 2020 00:55:50 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e9cb55a291cc31be0d1685bf33e4b2d7900d3ccd1502a51cb83dc0fb0f3b4c`  
		Last Modified: Thu, 14 May 2020 00:55:57 GMT  
		Size: 49.2 MB (49167458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ff7551b04433bf28ca7a9a5f8b670343a63d69dcff048aad0324722c1ccf1b`  
		Last Modified: Thu, 14 May 2020 00:55:48 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82315bbdd629134a846f8bf5754591a7d11d7328cb23ffd6ba1cbda1bdbdd40`  
		Last Modified: Thu, 14 May 2020 00:55:48 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf39863aed28c1f60c53fdc0ac072258c1d3ea5f9e39afb775a810c84b8cbe`  
		Last Modified: Thu, 14 May 2020 00:55:48 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7061e2c71165d321eae6b2fae61213c8b24b4cc955082b047b8c37924cd8c177`  
		Last Modified: Thu, 14 May 2020 00:55:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:latest`

```console
$ docker pull couchdb@sha256:4a693ab0787663eb9a8507455f8f99c81cad1aef3224c015adddf760086ffe30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:5ee5bc0e5ff1ea8d8e49519c2e12c2f7a5bd51cfd5aa13158ac70a654e0d685d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.2 MB (83244990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19586d4569840f999b3d828f267be2df149df731d5e3d6c3452ce79d3f5dc92b`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 18:10:38 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 15 May 2020 18:10:39 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 15 May 2020 18:10:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 18:10:49 GMT
ENV GOSU_VERSION=1.11
# Fri, 15 May 2020 18:10:50 GMT
ENV TINI_VERSION=0.18.0
# Fri, 15 May 2020 18:10:57 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Fri, 15 May 2020 18:10:57 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Fri, 15 May 2020 18:12:16 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Fri, 15 May 2020 18:12:17 GMT
ENV COUCHDB_VERSION=3.1.0
# Fri, 15 May 2020 18:12:18 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb buster main" > /etc/apt/sources.list.d/couchdb.list
# Fri, 15 May 2020 18:12:43 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 15 May 2020 18:12:43 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 15 May 2020 18:12:43 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 15 May 2020 18:12:43 GMT
COPY file:6952d2d38c707f223d813efd2d2969873cdd4b66d733559ef9be855aff5d8579 in /usr/local/bin 
# Fri, 15 May 2020 18:12:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 15 May 2020 18:12:44 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 15 May 2020 18:12:44 GMT
VOLUME [/opt/couchdb/data]
# Fri, 15 May 2020 18:12:45 GMT
EXPOSE 4369 5984 9100
# Fri, 15 May 2020 18:12:45 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea6be28d7902b2201739acc3aae5aa3f18ba5afdacc7453b7c1f625e7f242ac`  
		Last Modified: Fri, 15 May 2020 18:15:17 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2373eeb040b3133b40730e37185883a9bdfdad233a3841c8c0631555cd8a00c`  
		Last Modified: Fri, 15 May 2020 18:15:18 GMT  
		Size: 6.7 MB (6669989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6daa02d0e34d93f24791a9e9faa13c4fcad714b07a6b967218dd878309149d15`  
		Last Modified: Fri, 15 May 2020 18:15:17 GMT  
		Size: 1.2 MB (1192675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4f6e83db190adc7bba9232dab7492acd463b20a490f510cfcfb127c502ae46`  
		Last Modified: Fri, 15 May 2020 18:15:16 GMT  
		Size: 2.5 KB (2498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b4d696612496fbde66fcd130b817fd5437eff50e3a11f1b0fee0b2a42d49dc`  
		Last Modified: Fri, 15 May 2020 18:15:16 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43dfb476083a3cf9272f624a25e5c918ef3354356e658c731d16a43905d312d5`  
		Last Modified: Fri, 15 May 2020 18:15:21 GMT  
		Size: 48.3 MB (48274109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2322eca64972ff3114224aa8326a43f82cbe6c5b6e21d8b1fe9d8d4ec74bbcbc`  
		Last Modified: Fri, 15 May 2020 18:15:15 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2469b30b1ef30cc98a919e2319ac31a51ff88e8b0ab4c4f4cd23fdc4352804`  
		Last Modified: Fri, 15 May 2020 18:15:15 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6a34055fb7a96f96ad4ca65db87de927a7a113ff81f32c9a3bde59cc6a7a24`  
		Last Modified: Fri, 15 May 2020 18:15:15 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb5d9e7f3bd1cd11fcb0c53c740dde4bcb0d201167c2456a0a46073808334a5`  
		Last Modified: Fri, 15 May 2020 18:15:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:867d5ad3af217c527fcb9b8bcdfde874b01345607725d0c9fb6c2faa711f3e9f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78300791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48ff54be60f6acfe8ff0f96aa73954fa0cd64f7a948e2472bfc62f742b793a9e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 15 May 2020 12:44:06 GMT
ADD file:b305c1792102142f183d3084026f0fc6be3ddf8d1959b32f0a5d22d35eebcd15 in / 
# Fri, 15 May 2020 12:44:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 20:44:21 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Fri, 15 May 2020 20:44:22 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Fri, 15 May 2020 20:44:37 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 20:44:38 GMT
ENV GOSU_VERSION=1.11
# Fri, 15 May 2020 20:44:38 GMT
ENV TINI_VERSION=0.18.0
# Fri, 15 May 2020 20:44:53 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Fri, 15 May 2020 20:44:53 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Fri, 15 May 2020 20:44:56 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Fri, 15 May 2020 20:44:56 GMT
ENV COUCHDB_VERSION=3.1.0
# Fri, 15 May 2020 20:44:58 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb buster main" > /etc/apt/sources.list.d/couchdb.list
# Fri, 15 May 2020 20:45:23 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 15 May 2020 20:45:25 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 15 May 2020 20:45:26 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 15 May 2020 20:45:26 GMT
COPY file:6952d2d38c707f223d813efd2d2969873cdd4b66d733559ef9be855aff5d8579 in /usr/local/bin 
# Fri, 15 May 2020 20:45:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 15 May 2020 20:45:28 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 15 May 2020 20:45:29 GMT
VOLUME [/opt/couchdb/data]
# Fri, 15 May 2020 20:45:30 GMT
EXPOSE 4369 5984 9100
# Fri, 15 May 2020 20:45:30 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:8a7e1e68c24e5cac20ef26d29505c58456b561c431f0c683b66d1a0943f40dd4`  
		Last Modified: Fri, 15 May 2020 12:53:36 GMT  
		Size: 25.9 MB (25857195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33f13673e13d4045cd69130d2b65b00925d74929cc353756fd95cc78283aeb6`  
		Last Modified: Fri, 15 May 2020 20:48:03 GMT  
		Size: 3.4 KB (3436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca7cf6c706b4b74e6deb10fa874bce2cda5deda579b9afe75fba27737caf94b`  
		Last Modified: Fri, 15 May 2020 20:48:04 GMT  
		Size: 6.5 MB (6532335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abf2a3054613ab16eca0c5a9fd2705202ad6f626fc50ededfb92a884be8960a`  
		Last Modified: Fri, 15 May 2020 20:48:02 GMT  
		Size: 1.1 MB (1127105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adc39eed34a1a3dfe8cb06a085711f26033d016749241dec4e28e24c747a487`  
		Last Modified: Fri, 15 May 2020 20:48:02 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5902890c65495acd3018ad8fb2a6479c04e689e924258de4bec7ae320fa02429`  
		Last Modified: Fri, 15 May 2020 20:48:01 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12550950b7340e50916bb36021141da0a7d82805657d8dfa4af83f7fd048c3f9`  
		Last Modified: Fri, 15 May 2020 20:48:10 GMT  
		Size: 44.8 MB (44774682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd76bb158a698aa9a7d07fdf11194e793ce5e042ee0002982b6c6ee5589174e9`  
		Last Modified: Fri, 15 May 2020 20:48:00 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372cf04fe00b45260eb383e1b2df7c40cba81696fd984b41ead7a5a39a18e61a`  
		Last Modified: Fri, 15 May 2020 20:48:00 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c2d1f8c041a469e737e0f870b8292034314a3207920dce08612212def01367`  
		Last Modified: Fri, 15 May 2020 20:48:01 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c220bf124059d8f3acbf820793a260cab8fc5f7f64c4deede16d087a38bd725c`  
		Last Modified: Fri, 15 May 2020 20:48:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; ppc64le

```console
$ docker pull couchdb@sha256:3087c57e737ce170ac3cd533474da348a88d5a1fb24baf77009e7c168377477b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.4 MB (88390353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c15d44a2aff7b17fe29e337cdd29787e3689b0b1f3a3e63d3e969b74619455e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 13 May 2020 22:22:26 GMT
ADD file:53bd5d792aec2fc8af7c0c836e64979e003b2cecaaf5153bd456cb4e97ba5a0e in / 
# Wed, 13 May 2020 22:22:29 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:42:44 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 14 May 2020 00:42:58 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 14 May 2020 00:44:04 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:44:07 GMT
ENV GOSU_VERSION=1.11
# Thu, 14 May 2020 00:44:11 GMT
ENV TINI_VERSION=0.18.0
# Thu, 14 May 2020 00:44:45 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Thu, 14 May 2020 00:44:50 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Thu, 14 May 2020 00:46:05 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Thu, 14 May 2020 00:46:10 GMT
ENV COUCHDB_VERSION=3.1.0
# Thu, 14 May 2020 00:46:20 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb buster main" > /etc/apt/sources.list.d/couchdb.list
# Thu, 14 May 2020 00:47:28 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 14 May 2020 00:47:32 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 14 May 2020 00:47:33 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 14 May 2020 00:47:36 GMT
COPY file:6952d2d38c707f223d813efd2d2969873cdd4b66d733559ef9be855aff5d8579 in /usr/local/bin 
# Thu, 14 May 2020 00:47:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 14 May 2020 00:47:52 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 14 May 2020 00:47:59 GMT
VOLUME [/opt/couchdb/data]
# Thu, 14 May 2020 00:48:03 GMT
EXPOSE 4369 5984 9100
# Thu, 14 May 2020 00:48:14 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:d23cb84f4d6399958c00ec4c457e9c302763ee7dd86a0fb5540f75ed550c17d6`  
		Last Modified: Wed, 13 May 2020 22:57:57 GMT  
		Size: 30.5 MB (30518701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26548553458f4ed416116e39b84467c40a671ac87e3f5cd4bb78a3a0080b7beb`  
		Last Modified: Thu, 14 May 2020 00:55:56 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8eae6eed5d50faa81b267e24cda74e7dfc6159b14852c9795c8b4d659d3fd96`  
		Last Modified: Thu, 14 May 2020 00:55:54 GMT  
		Size: 7.6 MB (7578671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9f26ac2928f15ea53d3af08f5a2eb6d650cc33ac2bcd457c31fc789b92af35`  
		Last Modified: Thu, 14 May 2020 00:55:52 GMT  
		Size: 1.1 MB (1116070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e10211cda3e526eb08d0c51941c90282f66f6b67dfcdcb2bd6939907da884be`  
		Last Modified: Thu, 14 May 2020 00:55:51 GMT  
		Size: 2.5 KB (2493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69ff280ba732d5f17d93a1e794aa96874e6f75c087fec5e7e537db74282f9cc`  
		Last Modified: Thu, 14 May 2020 00:55:50 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e9cb55a291cc31be0d1685bf33e4b2d7900d3ccd1502a51cb83dc0fb0f3b4c`  
		Last Modified: Thu, 14 May 2020 00:55:57 GMT  
		Size: 49.2 MB (49167458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ff7551b04433bf28ca7a9a5f8b670343a63d69dcff048aad0324722c1ccf1b`  
		Last Modified: Thu, 14 May 2020 00:55:48 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82315bbdd629134a846f8bf5754591a7d11d7328cb23ffd6ba1cbda1bdbdd40`  
		Last Modified: Thu, 14 May 2020 00:55:48 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf39863aed28c1f60c53fdc0ac072258c1d3ea5f9e39afb775a810c84b8cbe`  
		Last Modified: Thu, 14 May 2020 00:55:48 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7061e2c71165d321eae6b2fae61213c8b24b4cc955082b047b8c37924cd8c177`  
		Last Modified: Thu, 14 May 2020 00:55:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
