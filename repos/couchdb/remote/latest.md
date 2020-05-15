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
