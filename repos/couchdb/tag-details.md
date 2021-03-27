<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `couchdb`

-	[`couchdb:2`](#couchdb2)
-	[`couchdb:2.3`](#couchdb23)
-	[`couchdb:2.3.1`](#couchdb231)
-	[`couchdb:3`](#couchdb3)
-	[`couchdb:3.0`](#couchdb30)
-	[`couchdb:3.0.1`](#couchdb301)
-	[`couchdb:3.1`](#couchdb31)
-	[`couchdb:3.1.1`](#couchdb311)
-	[`couchdb:latest`](#couchdblatest)

## `couchdb:2`

```console
$ docker pull couchdb@sha256:73338a474e40231b43dccc05eed9bf9eed17301f93dfa9639bb6cd1bbce89c6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2` - linux; amd64

```console
$ docker pull couchdb@sha256:5dcfd18d8d2a0e84d5e5a626e77e15ab691ba201eeabdac61d682e725f0933ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.4 MB (82424956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:630fa38714bd96c4c6f4f41f7f2488ef20ccc60b78978370ce210a3ef699d393`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 26 Mar 2021 15:23:32 GMT
ADD file:72268d05e43fe7fe347fba8d003dbe9926a595c116e761cf3997af09cfa0ee19 in / 
# Fri, 26 Mar 2021 15:23:32 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:42:33 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 27 Mar 2021 05:42:35 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 27 Mar 2021 05:42:44 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:42:45 GMT
ENV GOSU_VERSION=1.11
# Sat, 27 Mar 2021 05:42:45 GMT
ENV TINI_VERSION=0.18.0
# Sat, 27 Mar 2021 05:45:04 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Sat, 27 Mar 2021 05:45:04 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Sat, 27 Mar 2021 05:46:37 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Sat, 27 Mar 2021 05:46:37 GMT
ENV COUCHDB_VERSION=2.3.1
# Sat, 27 Mar 2021 05:46:38 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb stretch main" > /etc/apt/sources.list.d/couchdb.list
# Sat, 27 Mar 2021 05:46:56 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~stretch     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 27 Mar 2021 05:46:56 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Sat, 27 Mar 2021 05:46:56 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 27 Mar 2021 05:46:57 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Sat, 27 Mar 2021 05:46:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 27 Mar 2021 05:46:58 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 27 Mar 2021 05:46:58 GMT
VOLUME [/opt/couchdb/data]
# Sat, 27 Mar 2021 05:46:58 GMT
EXPOSE 4369 5984 9100
# Sat, 27 Mar 2021 05:46:58 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b5887238bf65fc2f40fdd004509b96300faa112cc64eb2865a09895474269ee7`  
		Last Modified: Fri, 26 Mar 2021 15:32:49 GMT  
		Size: 22.5 MB (22528402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:869de91543a1874c31616d911b6e47462a7292ce7c38cacb6e9245ca157fb758`  
		Last Modified: Sat, 27 Mar 2021 05:48:12 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d929433accc43e0a7687af5222a7cda11ea81e74ff9712718e8e6d5cd7e8efbb`  
		Last Modified: Sat, 27 Mar 2021 05:48:11 GMT  
		Size: 8.5 MB (8489858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefd4ed5f2d2888f2644fdd4816dcd4fc8fa775d1ea2033f36bb1c0c4e853561`  
		Last Modified: Sat, 27 Mar 2021 05:48:10 GMT  
		Size: 1.2 MB (1190557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cd664c872554994e53db9a670b3ae88a28e4d919665e75fe49f588a6ece1e7`  
		Last Modified: Sat, 27 Mar 2021 05:48:09 GMT  
		Size: 3.1 KB (3059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ce62f781e076563d81d65fe82139ecbcc593d290daa1b4138f9ce619c96e40`  
		Last Modified: Sat, 27 Mar 2021 05:48:09 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c23f3f44c922ac8e83a5e7c1cff426063589aa7bed4059479399e2683a54d0`  
		Last Modified: Sat, 27 Mar 2021 05:48:14 GMT  
		Size: 50.2 MB (50206098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dcc57954428d6192191c30aae9430c0f47d09c180cdb7bb20dd1f0bdea2a534`  
		Last Modified: Sat, 27 Mar 2021 05:48:07 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e5b3b53eac88171512491acc36d835b219256912ecbb9a17a20a9a4f33a26a`  
		Last Modified: Sat, 27 Mar 2021 05:48:07 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34dc5bccd2cc05eb6289cedb697561a10b1858e2b36223584f60f3f74a92104a`  
		Last Modified: Sat, 27 Mar 2021 05:48:07 GMT  
		Size: 2.1 KB (2072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbca5db77d3d2b484bd2a3fad58d249f22bfe57217e1b0d257f82f1f853161cf`  
		Last Modified: Sat, 27 Mar 2021 05:48:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:1edcb1db0b75b1b554c362d083f0953c713bca1b493b404c6cca870937efe215
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76959146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00ff23d012c8e30cad67c8ca7273138b294771d882c7cc05908b102fea001a85`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 26 Mar 2021 15:44:41 GMT
ADD file:d54d0988e0451a81b9cd10a0eb2d8dd60d3b53434cf64e32131fb89d6569b469 in / 
# Fri, 26 Mar 2021 15:44:43 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 04:00:39 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 27 Mar 2021 04:00:42 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 27 Mar 2021 04:01:01 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 04:01:02 GMT
ENV GOSU_VERSION=1.11
# Sat, 27 Mar 2021 04:01:03 GMT
ENV TINI_VERSION=0.18.0
# Sat, 27 Mar 2021 04:02:53 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Sat, 27 Mar 2021 04:02:54 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Sat, 27 Mar 2021 04:03:58 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Sat, 27 Mar 2021 04:03:59 GMT
ENV COUCHDB_VERSION=2.3.1
# Sat, 27 Mar 2021 04:04:01 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb stretch main" > /etc/apt/sources.list.d/couchdb.list
# Sat, 27 Mar 2021 04:04:36 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~stretch     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 27 Mar 2021 04:04:38 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Sat, 27 Mar 2021 04:04:39 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 27 Mar 2021 04:04:40 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Sat, 27 Mar 2021 04:04:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 27 Mar 2021 04:04:43 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 27 Mar 2021 04:04:44 GMT
VOLUME [/opt/couchdb/data]
# Sat, 27 Mar 2021 04:04:45 GMT
EXPOSE 4369 5984 9100
# Sat, 27 Mar 2021 04:04:45 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:a1d6052e2be30a420519e61a06519837b570da894327e9db568747653c30343f`  
		Last Modified: Fri, 26 Mar 2021 15:51:19 GMT  
		Size: 20.4 MB (20389256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fbd185d3b4ead20ae011b672d4f87c0709f2c36e2aae6a3dc6fc4329b9fa2f`  
		Last Modified: Sat, 27 Mar 2021 04:05:53 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc16ba82598746a938697a291ae93bb394799db333abd13f4887db68a2268a9`  
		Last Modified: Sat, 27 Mar 2021 04:05:53 GMT  
		Size: 7.6 MB (7628964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d33eaa55c917da475658744d2c69f2aecd9ea8fc55ac3ca67eeace50015c065`  
		Last Modified: Sat, 27 Mar 2021 04:05:51 GMT  
		Size: 1.1 MB (1125084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf64d904c0553e6b5fa2a8a66fd10866c3a8770caeb28c143db9e83d830009fb`  
		Last Modified: Sat, 27 Mar 2021 04:05:51 GMT  
		Size: 3.1 KB (3059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2b6d899f6130f02eeeb78e6dedc1480d48e616f6944cd362205f2480b6ddae`  
		Last Modified: Sat, 27 Mar 2021 04:05:51 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:332297dc0a9c9a03e1e830c953b43c2c1643fc5e1d1f1aa3cc6cb4cf75198058`  
		Last Modified: Sat, 27 Mar 2021 04:05:59 GMT  
		Size: 47.8 MB (47805771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a237cf53916a9b90257bc22a4d71f823447099c53884fef5300c1fe83f1ae717`  
		Last Modified: Sat, 27 Mar 2021 04:05:49 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ae6584736dac7c5e8cb375902cbebddc7793e8cb73bed69696ebcd2a8edefb`  
		Last Modified: Sat, 27 Mar 2021 04:05:49 GMT  
		Size: 768.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf67f1fb7f6e438ae77dffbcc5bf7cadfa675a2a18d0049d234e8637b0db3cb7`  
		Last Modified: Sat, 27 Mar 2021 04:05:49 GMT  
		Size: 2.1 KB (2072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661b2a4950e2a4d35dff01c2c06ddd480bcf67b1a63f2af9676665ad6190ca3c`  
		Last Modified: Sat, 27 Mar 2021 04:05:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3`

```console
$ docker pull couchdb@sha256:73338a474e40231b43dccc05eed9bf9eed17301f93dfa9639bb6cd1bbce89c6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:5dcfd18d8d2a0e84d5e5a626e77e15ab691ba201eeabdac61d682e725f0933ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.4 MB (82424956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:630fa38714bd96c4c6f4f41f7f2488ef20ccc60b78978370ce210a3ef699d393`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 26 Mar 2021 15:23:32 GMT
ADD file:72268d05e43fe7fe347fba8d003dbe9926a595c116e761cf3997af09cfa0ee19 in / 
# Fri, 26 Mar 2021 15:23:32 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:42:33 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 27 Mar 2021 05:42:35 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 27 Mar 2021 05:42:44 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:42:45 GMT
ENV GOSU_VERSION=1.11
# Sat, 27 Mar 2021 05:42:45 GMT
ENV TINI_VERSION=0.18.0
# Sat, 27 Mar 2021 05:45:04 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Sat, 27 Mar 2021 05:45:04 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Sat, 27 Mar 2021 05:46:37 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Sat, 27 Mar 2021 05:46:37 GMT
ENV COUCHDB_VERSION=2.3.1
# Sat, 27 Mar 2021 05:46:38 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb stretch main" > /etc/apt/sources.list.d/couchdb.list
# Sat, 27 Mar 2021 05:46:56 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~stretch     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 27 Mar 2021 05:46:56 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Sat, 27 Mar 2021 05:46:56 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 27 Mar 2021 05:46:57 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Sat, 27 Mar 2021 05:46:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 27 Mar 2021 05:46:58 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 27 Mar 2021 05:46:58 GMT
VOLUME [/opt/couchdb/data]
# Sat, 27 Mar 2021 05:46:58 GMT
EXPOSE 4369 5984 9100
# Sat, 27 Mar 2021 05:46:58 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b5887238bf65fc2f40fdd004509b96300faa112cc64eb2865a09895474269ee7`  
		Last Modified: Fri, 26 Mar 2021 15:32:49 GMT  
		Size: 22.5 MB (22528402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:869de91543a1874c31616d911b6e47462a7292ce7c38cacb6e9245ca157fb758`  
		Last Modified: Sat, 27 Mar 2021 05:48:12 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d929433accc43e0a7687af5222a7cda11ea81e74ff9712718e8e6d5cd7e8efbb`  
		Last Modified: Sat, 27 Mar 2021 05:48:11 GMT  
		Size: 8.5 MB (8489858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefd4ed5f2d2888f2644fdd4816dcd4fc8fa775d1ea2033f36bb1c0c4e853561`  
		Last Modified: Sat, 27 Mar 2021 05:48:10 GMT  
		Size: 1.2 MB (1190557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cd664c872554994e53db9a670b3ae88a28e4d919665e75fe49f588a6ece1e7`  
		Last Modified: Sat, 27 Mar 2021 05:48:09 GMT  
		Size: 3.1 KB (3059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ce62f781e076563d81d65fe82139ecbcc593d290daa1b4138f9ce619c96e40`  
		Last Modified: Sat, 27 Mar 2021 05:48:09 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c23f3f44c922ac8e83a5e7c1cff426063589aa7bed4059479399e2683a54d0`  
		Last Modified: Sat, 27 Mar 2021 05:48:14 GMT  
		Size: 50.2 MB (50206098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dcc57954428d6192191c30aae9430c0f47d09c180cdb7bb20dd1f0bdea2a534`  
		Last Modified: Sat, 27 Mar 2021 05:48:07 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e5b3b53eac88171512491acc36d835b219256912ecbb9a17a20a9a4f33a26a`  
		Last Modified: Sat, 27 Mar 2021 05:48:07 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34dc5bccd2cc05eb6289cedb697561a10b1858e2b36223584f60f3f74a92104a`  
		Last Modified: Sat, 27 Mar 2021 05:48:07 GMT  
		Size: 2.1 KB (2072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbca5db77d3d2b484bd2a3fad58d249f22bfe57217e1b0d257f82f1f853161cf`  
		Last Modified: Sat, 27 Mar 2021 05:48:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:1edcb1db0b75b1b554c362d083f0953c713bca1b493b404c6cca870937efe215
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76959146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00ff23d012c8e30cad67c8ca7273138b294771d882c7cc05908b102fea001a85`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 26 Mar 2021 15:44:41 GMT
ADD file:d54d0988e0451a81b9cd10a0eb2d8dd60d3b53434cf64e32131fb89d6569b469 in / 
# Fri, 26 Mar 2021 15:44:43 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 04:00:39 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 27 Mar 2021 04:00:42 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 27 Mar 2021 04:01:01 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 04:01:02 GMT
ENV GOSU_VERSION=1.11
# Sat, 27 Mar 2021 04:01:03 GMT
ENV TINI_VERSION=0.18.0
# Sat, 27 Mar 2021 04:02:53 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Sat, 27 Mar 2021 04:02:54 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Sat, 27 Mar 2021 04:03:58 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Sat, 27 Mar 2021 04:03:59 GMT
ENV COUCHDB_VERSION=2.3.1
# Sat, 27 Mar 2021 04:04:01 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb stretch main" > /etc/apt/sources.list.d/couchdb.list
# Sat, 27 Mar 2021 04:04:36 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~stretch     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 27 Mar 2021 04:04:38 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Sat, 27 Mar 2021 04:04:39 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 27 Mar 2021 04:04:40 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Sat, 27 Mar 2021 04:04:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 27 Mar 2021 04:04:43 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 27 Mar 2021 04:04:44 GMT
VOLUME [/opt/couchdb/data]
# Sat, 27 Mar 2021 04:04:45 GMT
EXPOSE 4369 5984 9100
# Sat, 27 Mar 2021 04:04:45 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:a1d6052e2be30a420519e61a06519837b570da894327e9db568747653c30343f`  
		Last Modified: Fri, 26 Mar 2021 15:51:19 GMT  
		Size: 20.4 MB (20389256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fbd185d3b4ead20ae011b672d4f87c0709f2c36e2aae6a3dc6fc4329b9fa2f`  
		Last Modified: Sat, 27 Mar 2021 04:05:53 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc16ba82598746a938697a291ae93bb394799db333abd13f4887db68a2268a9`  
		Last Modified: Sat, 27 Mar 2021 04:05:53 GMT  
		Size: 7.6 MB (7628964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d33eaa55c917da475658744d2c69f2aecd9ea8fc55ac3ca67eeace50015c065`  
		Last Modified: Sat, 27 Mar 2021 04:05:51 GMT  
		Size: 1.1 MB (1125084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf64d904c0553e6b5fa2a8a66fd10866c3a8770caeb28c143db9e83d830009fb`  
		Last Modified: Sat, 27 Mar 2021 04:05:51 GMT  
		Size: 3.1 KB (3059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2b6d899f6130f02eeeb78e6dedc1480d48e616f6944cd362205f2480b6ddae`  
		Last Modified: Sat, 27 Mar 2021 04:05:51 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:332297dc0a9c9a03e1e830c953b43c2c1643fc5e1d1f1aa3cc6cb4cf75198058`  
		Last Modified: Sat, 27 Mar 2021 04:05:59 GMT  
		Size: 47.8 MB (47805771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a237cf53916a9b90257bc22a4d71f823447099c53884fef5300c1fe83f1ae717`  
		Last Modified: Sat, 27 Mar 2021 04:05:49 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ae6584736dac7c5e8cb375902cbebddc7793e8cb73bed69696ebcd2a8edefb`  
		Last Modified: Sat, 27 Mar 2021 04:05:49 GMT  
		Size: 768.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf67f1fb7f6e438ae77dffbcc5bf7cadfa675a2a18d0049d234e8637b0db3cb7`  
		Last Modified: Sat, 27 Mar 2021 04:05:49 GMT  
		Size: 2.1 KB (2072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661b2a4950e2a4d35dff01c2c06ddd480bcf67b1a63f2af9676665ad6190ca3c`  
		Last Modified: Sat, 27 Mar 2021 04:05:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3.1`

```console
$ docker pull couchdb@sha256:73338a474e40231b43dccc05eed9bf9eed17301f93dfa9639bb6cd1bbce89c6c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:5dcfd18d8d2a0e84d5e5a626e77e15ab691ba201eeabdac61d682e725f0933ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.4 MB (82424956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:630fa38714bd96c4c6f4f41f7f2488ef20ccc60b78978370ce210a3ef699d393`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 26 Mar 2021 15:23:32 GMT
ADD file:72268d05e43fe7fe347fba8d003dbe9926a595c116e761cf3997af09cfa0ee19 in / 
# Fri, 26 Mar 2021 15:23:32 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:42:33 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 27 Mar 2021 05:42:35 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 27 Mar 2021 05:42:44 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:42:45 GMT
ENV GOSU_VERSION=1.11
# Sat, 27 Mar 2021 05:42:45 GMT
ENV TINI_VERSION=0.18.0
# Sat, 27 Mar 2021 05:45:04 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Sat, 27 Mar 2021 05:45:04 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Sat, 27 Mar 2021 05:46:37 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Sat, 27 Mar 2021 05:46:37 GMT
ENV COUCHDB_VERSION=2.3.1
# Sat, 27 Mar 2021 05:46:38 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb stretch main" > /etc/apt/sources.list.d/couchdb.list
# Sat, 27 Mar 2021 05:46:56 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~stretch     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 27 Mar 2021 05:46:56 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Sat, 27 Mar 2021 05:46:56 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 27 Mar 2021 05:46:57 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Sat, 27 Mar 2021 05:46:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 27 Mar 2021 05:46:58 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 27 Mar 2021 05:46:58 GMT
VOLUME [/opt/couchdb/data]
# Sat, 27 Mar 2021 05:46:58 GMT
EXPOSE 4369 5984 9100
# Sat, 27 Mar 2021 05:46:58 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b5887238bf65fc2f40fdd004509b96300faa112cc64eb2865a09895474269ee7`  
		Last Modified: Fri, 26 Mar 2021 15:32:49 GMT  
		Size: 22.5 MB (22528402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:869de91543a1874c31616d911b6e47462a7292ce7c38cacb6e9245ca157fb758`  
		Last Modified: Sat, 27 Mar 2021 05:48:12 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d929433accc43e0a7687af5222a7cda11ea81e74ff9712718e8e6d5cd7e8efbb`  
		Last Modified: Sat, 27 Mar 2021 05:48:11 GMT  
		Size: 8.5 MB (8489858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefd4ed5f2d2888f2644fdd4816dcd4fc8fa775d1ea2033f36bb1c0c4e853561`  
		Last Modified: Sat, 27 Mar 2021 05:48:10 GMT  
		Size: 1.2 MB (1190557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cd664c872554994e53db9a670b3ae88a28e4d919665e75fe49f588a6ece1e7`  
		Last Modified: Sat, 27 Mar 2021 05:48:09 GMT  
		Size: 3.1 KB (3059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ce62f781e076563d81d65fe82139ecbcc593d290daa1b4138f9ce619c96e40`  
		Last Modified: Sat, 27 Mar 2021 05:48:09 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c23f3f44c922ac8e83a5e7c1cff426063589aa7bed4059479399e2683a54d0`  
		Last Modified: Sat, 27 Mar 2021 05:48:14 GMT  
		Size: 50.2 MB (50206098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dcc57954428d6192191c30aae9430c0f47d09c180cdb7bb20dd1f0bdea2a534`  
		Last Modified: Sat, 27 Mar 2021 05:48:07 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e5b3b53eac88171512491acc36d835b219256912ecbb9a17a20a9a4f33a26a`  
		Last Modified: Sat, 27 Mar 2021 05:48:07 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34dc5bccd2cc05eb6289cedb697561a10b1858e2b36223584f60f3f74a92104a`  
		Last Modified: Sat, 27 Mar 2021 05:48:07 GMT  
		Size: 2.1 KB (2072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbca5db77d3d2b484bd2a3fad58d249f22bfe57217e1b0d257f82f1f853161cf`  
		Last Modified: Sat, 27 Mar 2021 05:48:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:1edcb1db0b75b1b554c362d083f0953c713bca1b493b404c6cca870937efe215
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76959146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00ff23d012c8e30cad67c8ca7273138b294771d882c7cc05908b102fea001a85`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 26 Mar 2021 15:44:41 GMT
ADD file:d54d0988e0451a81b9cd10a0eb2d8dd60d3b53434cf64e32131fb89d6569b469 in / 
# Fri, 26 Mar 2021 15:44:43 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 04:00:39 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 27 Mar 2021 04:00:42 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 27 Mar 2021 04:01:01 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 04:01:02 GMT
ENV GOSU_VERSION=1.11
# Sat, 27 Mar 2021 04:01:03 GMT
ENV TINI_VERSION=0.18.0
# Sat, 27 Mar 2021 04:02:53 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Sat, 27 Mar 2021 04:02:54 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Sat, 27 Mar 2021 04:03:58 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Sat, 27 Mar 2021 04:03:59 GMT
ENV COUCHDB_VERSION=2.3.1
# Sat, 27 Mar 2021 04:04:01 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb stretch main" > /etc/apt/sources.list.d/couchdb.list
# Sat, 27 Mar 2021 04:04:36 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~stretch     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 27 Mar 2021 04:04:38 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Sat, 27 Mar 2021 04:04:39 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 27 Mar 2021 04:04:40 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Sat, 27 Mar 2021 04:04:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 27 Mar 2021 04:04:43 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 27 Mar 2021 04:04:44 GMT
VOLUME [/opt/couchdb/data]
# Sat, 27 Mar 2021 04:04:45 GMT
EXPOSE 4369 5984 9100
# Sat, 27 Mar 2021 04:04:45 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:a1d6052e2be30a420519e61a06519837b570da894327e9db568747653c30343f`  
		Last Modified: Fri, 26 Mar 2021 15:51:19 GMT  
		Size: 20.4 MB (20389256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fbd185d3b4ead20ae011b672d4f87c0709f2c36e2aae6a3dc6fc4329b9fa2f`  
		Last Modified: Sat, 27 Mar 2021 04:05:53 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc16ba82598746a938697a291ae93bb394799db333abd13f4887db68a2268a9`  
		Last Modified: Sat, 27 Mar 2021 04:05:53 GMT  
		Size: 7.6 MB (7628964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d33eaa55c917da475658744d2c69f2aecd9ea8fc55ac3ca67eeace50015c065`  
		Last Modified: Sat, 27 Mar 2021 04:05:51 GMT  
		Size: 1.1 MB (1125084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf64d904c0553e6b5fa2a8a66fd10866c3a8770caeb28c143db9e83d830009fb`  
		Last Modified: Sat, 27 Mar 2021 04:05:51 GMT  
		Size: 3.1 KB (3059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea2b6d899f6130f02eeeb78e6dedc1480d48e616f6944cd362205f2480b6ddae`  
		Last Modified: Sat, 27 Mar 2021 04:05:51 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:332297dc0a9c9a03e1e830c953b43c2c1643fc5e1d1f1aa3cc6cb4cf75198058`  
		Last Modified: Sat, 27 Mar 2021 04:05:59 GMT  
		Size: 47.8 MB (47805771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a237cf53916a9b90257bc22a4d71f823447099c53884fef5300c1fe83f1ae717`  
		Last Modified: Sat, 27 Mar 2021 04:05:49 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ae6584736dac7c5e8cb375902cbebddc7793e8cb73bed69696ebcd2a8edefb`  
		Last Modified: Sat, 27 Mar 2021 04:05:49 GMT  
		Size: 768.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf67f1fb7f6e438ae77dffbcc5bf7cadfa675a2a18d0049d234e8637b0db3cb7`  
		Last Modified: Sat, 27 Mar 2021 04:05:49 GMT  
		Size: 2.1 KB (2072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661b2a4950e2a4d35dff01c2c06ddd480bcf67b1a63f2af9676665ad6190ca3c`  
		Last Modified: Sat, 27 Mar 2021 04:05:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3`

```console
$ docker pull couchdb@sha256:bbfa9db04a940916fca50a4eb0057b210ac7f8184400c7cae7247085bd444efd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3` - linux; amd64

```console
$ docker pull couchdb@sha256:34f99d0a7afd22dd2211f78d22cb0313285d21f0a1714ec5b4845a88465afe1a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.4 MB (83366837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:639e80b8aac0ffff7bba56ae979dc4bfece49dd7485550808ab1260a8bdfebb2`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 26 Mar 2021 15:20:59 GMT
ADD file:b2085f4b0a7cb0e5754874c712254e5cd941062b27b8d7ed2080520196b91597 in / 
# Fri, 26 Mar 2021 15:20:59 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:39:57 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 27 Mar 2021 05:39:58 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 27 Mar 2021 05:40:07 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:40:07 GMT
ENV GOSU_VERSION=1.11
# Sat, 27 Mar 2021 05:40:07 GMT
ENV TINI_VERSION=0.18.0
# Sat, 27 Mar 2021 05:40:20 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Sat, 27 Mar 2021 05:40:20 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Sat, 27 Mar 2021 05:41:43 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Sat, 27 Mar 2021 05:41:44 GMT
ENV COUCHDB_VERSION=3.1.1
# Sat, 27 Mar 2021 05:41:45 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb buster main" > /etc/apt/sources.list.d/couchdb.list
# Sat, 27 Mar 2021 05:41:59 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 27 Mar 2021 05:41:59 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 27 Mar 2021 05:41:59 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 27 Mar 2021 05:42:00 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Sat, 27 Mar 2021 05:42:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 27 Mar 2021 05:42:01 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 27 Mar 2021 05:42:01 GMT
VOLUME [/opt/couchdb/data]
# Sat, 27 Mar 2021 05:42:01 GMT
EXPOSE 4369 5984 9100
# Sat, 27 Mar 2021 05:42:02 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ac2522cc72690febc428fb46fb39a4efc5e0a721c3ad15d9992b01515f2fad1a`  
		Last Modified: Fri, 26 Mar 2021 15:27:47 GMT  
		Size: 27.1 MB (27100996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd85d6fda1932ecaf8b874bfe43a05c51749b96b06a6444b9fd7b5e2a13a39a`  
		Last Modified: Sat, 27 Mar 2021 05:47:32 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688cb4b1dcebeaded848ad0def250dfab09a6a744e72bf1d648d389ab3f61dbc`  
		Last Modified: Sat, 27 Mar 2021 05:47:30 GMT  
		Size: 6.7 MB (6690481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b47df997a5ff452e78398fdec86929de1eba2999b37337df310700de6e1e20`  
		Last Modified: Sat, 27 Mar 2021 05:47:29 GMT  
		Size: 1.2 MB (1192799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df16dcc32fe4243098a9d68357e33780d55fb244daadab1f1d8952d73cd7c78`  
		Last Modified: Sat, 27 Mar 2021 05:47:29 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5319a774b98363bda874f2ee59e7889c7823c7d348df7e06beebbcb76cadd0c`  
		Last Modified: Sat, 27 Mar 2021 05:47:29 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52dbd6d0c0a88fc1a974aaa936755b95facbbb5d4ff7fdc4d46c43514304ea79`  
		Last Modified: Sat, 27 Mar 2021 05:47:32 GMT  
		Size: 48.4 MB (48373108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566cbdd2257fd82b3e7ed8ab84f5bb30474c7f85094eb4aa5a89706887763431`  
		Last Modified: Sat, 27 Mar 2021 05:47:26 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d0983079f7919550f3f82ba1307da276bbf8ceb7463f3004ce982f609390ce`  
		Last Modified: Sat, 27 Mar 2021 05:47:26 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44e12b8c2d1ed8bf84e30d70cb635917e7b0e3dcbe3caaad90775b11597514e`  
		Last Modified: Sat, 27 Mar 2021 05:47:27 GMT  
		Size: 2.1 KB (2062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e6e2faee2471a6db48bc41ca8965739a40b952e3496e7370e5b526a33e5016`  
		Last Modified: Sat, 27 Mar 2021 05:47:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:7e5a4b7f65e823b0bfdd5513e0e9c1f153569f1cf28b5b0ce06e64142de8027e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.4 MB (78399848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bab4ab6118c87902dfea4f501aaf7b7ea7ac8571a451e7e3d0637b6782ba9dff`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 26 Mar 2021 15:41:54 GMT
ADD file:c8c0d923527574a26725e0a1995051870ed169ff6b6ebfe77c50810f5583690b in / 
# Fri, 26 Mar 2021 15:41:56 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 03:56:47 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 27 Mar 2021 03:56:51 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 27 Mar 2021 03:57:11 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 03:57:13 GMT
ENV GOSU_VERSION=1.11
# Sat, 27 Mar 2021 03:57:16 GMT
ENV TINI_VERSION=0.18.0
# Sat, 27 Mar 2021 03:58:55 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Sat, 27 Mar 2021 03:58:56 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Sat, 27 Mar 2021 03:58:59 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Sat, 27 Mar 2021 03:59:00 GMT
ENV COUCHDB_VERSION=3.1.1
# Sat, 27 Mar 2021 03:59:02 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb buster main" > /etc/apt/sources.list.d/couchdb.list
# Sat, 27 Mar 2021 03:59:25 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 27 Mar 2021 03:59:27 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 27 Mar 2021 03:59:28 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 27 Mar 2021 03:59:29 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Sat, 27 Mar 2021 03:59:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 27 Mar 2021 03:59:35 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 27 Mar 2021 03:59:36 GMT
VOLUME [/opt/couchdb/data]
# Sat, 27 Mar 2021 03:59:37 GMT
EXPOSE 4369 5984 9100
# Sat, 27 Mar 2021 03:59:39 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:989f98f7e44fde3e2eb49bc6d2bfed15401201d21cd90f42cd9fc4c26eef8bb0`  
		Last Modified: Fri, 26 Mar 2021 15:48:47 GMT  
		Size: 25.9 MB (25856384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c07bb39a6cb2e40e6fc495018e6a5e67e72664e64fde7be07a00af7efcfdb25`  
		Last Modified: Sat, 27 Mar 2021 04:05:15 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23021ef367eef3af8f8baca64bef5704978b3fa30ed3fbf3ad185cc433635f1c`  
		Last Modified: Sat, 27 Mar 2021 04:05:15 GMT  
		Size: 6.6 MB (6550237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16580e7719e6f506b8fc0760128bfe3831b3616113ed738be5f1bbf3946e5ab7`  
		Last Modified: Sat, 27 Mar 2021 04:05:13 GMT  
		Size: 1.1 MB (1127209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c22f172537b79c577ed6ce4bf2ca28014d7b916ee66d8eca7cafc5ae9e2fdf7`  
		Last Modified: Sat, 27 Mar 2021 04:05:13 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03023b4142a3b5ee76506db88343d2f3134ac7e144161e6761330cf1329a178`  
		Last Modified: Sat, 27 Mar 2021 04:05:13 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426c9a8c52fd17f4838ec640d534c927944ec23d8291da83ac67bba359cce2c1`  
		Last Modified: Sat, 27 Mar 2021 04:05:20 GMT  
		Size: 44.9 MB (44856541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911410d0a5f93377e0a28c1c5c000418220ee85adf99e24241395dfef52cbdf4`  
		Last Modified: Sat, 27 Mar 2021 04:05:11 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0c193871be5b8d9e61be9d947be65a92e5747e9ce01656015d5065d3ac9dd5`  
		Last Modified: Sat, 27 Mar 2021 04:05:11 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69a19510ccf86e9cddee6a5674df81f2dfa153e8704424907f3ee48299f6b85`  
		Last Modified: Sat, 27 Mar 2021 04:05:11 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538f0a77085e6cf6646f8f5bd704b6d957dfc04f89b71ecba0a2ac6462ba462f`  
		Last Modified: Sat, 27 Mar 2021 04:05:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.0`

```console
$ docker pull couchdb@sha256:10087c3a8f8522993d37e6f19bfb7e3dc09b21e0ef5005d56cd50f98edc1c30c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.0` - linux; amd64

```console
$ docker pull couchdb@sha256:e1e1f5ad7e118eaeb5dc1030f57f561b9c86f5f975cf84323eec8ad10906c3a5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.2 MB (83224227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8931b630568501a99837af1bf1e8984e345cd8f25815cef0b2c377deb1df3fb`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 26 Mar 2021 15:20:59 GMT
ADD file:b2085f4b0a7cb0e5754874c712254e5cd941062b27b8d7ed2080520196b91597 in / 
# Fri, 26 Mar 2021 15:20:59 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:39:57 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 27 Mar 2021 05:39:58 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 27 Mar 2021 05:40:07 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:40:07 GMT
ENV GOSU_VERSION=1.11
# Sat, 27 Mar 2021 05:40:07 GMT
ENV TINI_VERSION=0.18.0
# Sat, 27 Mar 2021 05:40:20 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Sat, 27 Mar 2021 05:40:20 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Sat, 27 Mar 2021 05:41:43 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Sat, 27 Mar 2021 05:42:08 GMT
ENV COUCHDB_VERSION=3.0.1
# Sat, 27 Mar 2021 05:42:09 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb buster main" > /etc/apt/sources.list.d/couchdb.list
# Sat, 27 Mar 2021 05:42:23 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 27 Mar 2021 05:42:24 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 27 Mar 2021 05:42:24 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 27 Mar 2021 05:42:25 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Sat, 27 Mar 2021 05:42:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 27 Mar 2021 05:42:26 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 27 Mar 2021 05:42:26 GMT
VOLUME [/opt/couchdb/data]
# Sat, 27 Mar 2021 05:42:26 GMT
EXPOSE 4369 5984 9100
# Sat, 27 Mar 2021 05:42:27 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ac2522cc72690febc428fb46fb39a4efc5e0a721c3ad15d9992b01515f2fad1a`  
		Last Modified: Fri, 26 Mar 2021 15:27:47 GMT  
		Size: 27.1 MB (27100996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd85d6fda1932ecaf8b874bfe43a05c51749b96b06a6444b9fd7b5e2a13a39a`  
		Last Modified: Sat, 27 Mar 2021 05:47:32 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688cb4b1dcebeaded848ad0def250dfab09a6a744e72bf1d648d389ab3f61dbc`  
		Last Modified: Sat, 27 Mar 2021 05:47:30 GMT  
		Size: 6.7 MB (6690481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b47df997a5ff452e78398fdec86929de1eba2999b37337df310700de6e1e20`  
		Last Modified: Sat, 27 Mar 2021 05:47:29 GMT  
		Size: 1.2 MB (1192799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df16dcc32fe4243098a9d68357e33780d55fb244daadab1f1d8952d73cd7c78`  
		Last Modified: Sat, 27 Mar 2021 05:47:29 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716cc13e299ff4ceeda43be8f9b98a4ee66521e5ded55f5042eb24559c554da4`  
		Last Modified: Sat, 27 Mar 2021 05:47:52 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911fb3d69712fbcb2bf62ee3b827493436a7f7cd61aa7e6cfc1bacc56043bcf7`  
		Last Modified: Sat, 27 Mar 2021 05:47:56 GMT  
		Size: 48.2 MB (48230498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0c6184dda282e0d97c8ecc22a30595031ff566c6e453704f77a9b61ff05133`  
		Last Modified: Sat, 27 Mar 2021 05:47:50 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c539750a568bef5973e967f7bffc8972f1596dcc5d1f47e1e1a087672d38d4d`  
		Last Modified: Sat, 27 Mar 2021 05:47:49 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b10f198bc44aa0f207506829935326532f36001004385ed38b776a2484191ed`  
		Last Modified: Sat, 27 Mar 2021 05:47:49 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7277b9a5c8962672f9ab71431aef1544a5d1705e04399f17875d2ad7e18398c`  
		Last Modified: Sat, 27 Mar 2021 05:47:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.0` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:a3e769ca3b9950cf8b48ff4fbb9824da7c4c2fb8d2696d99f4afcadcdb7f13b3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78251756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b370da5c1801d07e61a2768d0f19f6d248e431a0037957460ad24f25a597495`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 26 Mar 2021 15:41:54 GMT
ADD file:c8c0d923527574a26725e0a1995051870ed169ff6b6ebfe77c50810f5583690b in / 
# Fri, 26 Mar 2021 15:41:56 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 03:56:47 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 27 Mar 2021 03:56:51 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 27 Mar 2021 03:57:11 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 03:57:13 GMT
ENV GOSU_VERSION=1.11
# Sat, 27 Mar 2021 03:57:16 GMT
ENV TINI_VERSION=0.18.0
# Sat, 27 Mar 2021 03:58:55 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Sat, 27 Mar 2021 03:58:56 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Sat, 27 Mar 2021 03:58:59 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Sat, 27 Mar 2021 03:59:49 GMT
ENV COUCHDB_VERSION=3.0.1
# Sat, 27 Mar 2021 03:59:52 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb buster main" > /etc/apt/sources.list.d/couchdb.list
# Sat, 27 Mar 2021 04:00:15 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 27 Mar 2021 04:00:16 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 27 Mar 2021 04:00:18 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 27 Mar 2021 04:00:18 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Sat, 27 Mar 2021 04:00:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 27 Mar 2021 04:00:23 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 27 Mar 2021 04:00:24 GMT
VOLUME [/opt/couchdb/data]
# Sat, 27 Mar 2021 04:00:25 GMT
EXPOSE 4369 5984 9100
# Sat, 27 Mar 2021 04:00:26 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:989f98f7e44fde3e2eb49bc6d2bfed15401201d21cd90f42cd9fc4c26eef8bb0`  
		Last Modified: Fri, 26 Mar 2021 15:48:47 GMT  
		Size: 25.9 MB (25856384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c07bb39a6cb2e40e6fc495018e6a5e67e72664e64fde7be07a00af7efcfdb25`  
		Last Modified: Sat, 27 Mar 2021 04:05:15 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23021ef367eef3af8f8baca64bef5704978b3fa30ed3fbf3ad185cc433635f1c`  
		Last Modified: Sat, 27 Mar 2021 04:05:15 GMT  
		Size: 6.6 MB (6550237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16580e7719e6f506b8fc0760128bfe3831b3616113ed738be5f1bbf3946e5ab7`  
		Last Modified: Sat, 27 Mar 2021 04:05:13 GMT  
		Size: 1.1 MB (1127209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c22f172537b79c577ed6ce4bf2ca28014d7b916ee66d8eca7cafc5ae9e2fdf7`  
		Last Modified: Sat, 27 Mar 2021 04:05:13 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed333509257c33586565b08ad8152b97789a038695aef7bca3185893567ad72`  
		Last Modified: Sat, 27 Mar 2021 04:05:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af9a43d12665902e62b566a86d1b01ca4b8b4653b94fd442c9bbfabb8bc7c25`  
		Last Modified: Sat, 27 Mar 2021 04:05:42 GMT  
		Size: 44.7 MB (44708448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac7033145d975dcb41d9f0429f11de5e598afd68de85c3b90782c257ba9e5a2a`  
		Last Modified: Sat, 27 Mar 2021 04:05:33 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73706bbb6f62cc38352e8788852e3b7b4cac047b9008363c94e217f6bd9b6a8`  
		Last Modified: Sat, 27 Mar 2021 04:05:33 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0756706b206dd320cc270d01cb5d3fd09af607b3a12333c6a46f87ec4ac6ec5`  
		Last Modified: Sat, 27 Mar 2021 04:05:33 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420ca416128a980b79f17457e0c76330acff2d1b418119a282d9893d0101e3cd`  
		Last Modified: Sat, 27 Mar 2021 04:05:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.0.1`

```console
$ docker pull couchdb@sha256:10087c3a8f8522993d37e6f19bfb7e3dc09b21e0ef5005d56cd50f98edc1c30c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.0.1` - linux; amd64

```console
$ docker pull couchdb@sha256:e1e1f5ad7e118eaeb5dc1030f57f561b9c86f5f975cf84323eec8ad10906c3a5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.2 MB (83224227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8931b630568501a99837af1bf1e8984e345cd8f25815cef0b2c377deb1df3fb`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 26 Mar 2021 15:20:59 GMT
ADD file:b2085f4b0a7cb0e5754874c712254e5cd941062b27b8d7ed2080520196b91597 in / 
# Fri, 26 Mar 2021 15:20:59 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:39:57 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 27 Mar 2021 05:39:58 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 27 Mar 2021 05:40:07 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:40:07 GMT
ENV GOSU_VERSION=1.11
# Sat, 27 Mar 2021 05:40:07 GMT
ENV TINI_VERSION=0.18.0
# Sat, 27 Mar 2021 05:40:20 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Sat, 27 Mar 2021 05:40:20 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Sat, 27 Mar 2021 05:41:43 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Sat, 27 Mar 2021 05:42:08 GMT
ENV COUCHDB_VERSION=3.0.1
# Sat, 27 Mar 2021 05:42:09 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb buster main" > /etc/apt/sources.list.d/couchdb.list
# Sat, 27 Mar 2021 05:42:23 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 27 Mar 2021 05:42:24 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 27 Mar 2021 05:42:24 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 27 Mar 2021 05:42:25 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Sat, 27 Mar 2021 05:42:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 27 Mar 2021 05:42:26 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 27 Mar 2021 05:42:26 GMT
VOLUME [/opt/couchdb/data]
# Sat, 27 Mar 2021 05:42:26 GMT
EXPOSE 4369 5984 9100
# Sat, 27 Mar 2021 05:42:27 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ac2522cc72690febc428fb46fb39a4efc5e0a721c3ad15d9992b01515f2fad1a`  
		Last Modified: Fri, 26 Mar 2021 15:27:47 GMT  
		Size: 27.1 MB (27100996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd85d6fda1932ecaf8b874bfe43a05c51749b96b06a6444b9fd7b5e2a13a39a`  
		Last Modified: Sat, 27 Mar 2021 05:47:32 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688cb4b1dcebeaded848ad0def250dfab09a6a744e72bf1d648d389ab3f61dbc`  
		Last Modified: Sat, 27 Mar 2021 05:47:30 GMT  
		Size: 6.7 MB (6690481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b47df997a5ff452e78398fdec86929de1eba2999b37337df310700de6e1e20`  
		Last Modified: Sat, 27 Mar 2021 05:47:29 GMT  
		Size: 1.2 MB (1192799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df16dcc32fe4243098a9d68357e33780d55fb244daadab1f1d8952d73cd7c78`  
		Last Modified: Sat, 27 Mar 2021 05:47:29 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716cc13e299ff4ceeda43be8f9b98a4ee66521e5ded55f5042eb24559c554da4`  
		Last Modified: Sat, 27 Mar 2021 05:47:52 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911fb3d69712fbcb2bf62ee3b827493436a7f7cd61aa7e6cfc1bacc56043bcf7`  
		Last Modified: Sat, 27 Mar 2021 05:47:56 GMT  
		Size: 48.2 MB (48230498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0c6184dda282e0d97c8ecc22a30595031ff566c6e453704f77a9b61ff05133`  
		Last Modified: Sat, 27 Mar 2021 05:47:50 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c539750a568bef5973e967f7bffc8972f1596dcc5d1f47e1e1a087672d38d4d`  
		Last Modified: Sat, 27 Mar 2021 05:47:49 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b10f198bc44aa0f207506829935326532f36001004385ed38b776a2484191ed`  
		Last Modified: Sat, 27 Mar 2021 05:47:49 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7277b9a5c8962672f9ab71431aef1544a5d1705e04399f17875d2ad7e18398c`  
		Last Modified: Sat, 27 Mar 2021 05:47:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.0.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:a3e769ca3b9950cf8b48ff4fbb9824da7c4c2fb8d2696d99f4afcadcdb7f13b3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.3 MB (78251756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b370da5c1801d07e61a2768d0f19f6d248e431a0037957460ad24f25a597495`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 26 Mar 2021 15:41:54 GMT
ADD file:c8c0d923527574a26725e0a1995051870ed169ff6b6ebfe77c50810f5583690b in / 
# Fri, 26 Mar 2021 15:41:56 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 03:56:47 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 27 Mar 2021 03:56:51 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 27 Mar 2021 03:57:11 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 03:57:13 GMT
ENV GOSU_VERSION=1.11
# Sat, 27 Mar 2021 03:57:16 GMT
ENV TINI_VERSION=0.18.0
# Sat, 27 Mar 2021 03:58:55 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Sat, 27 Mar 2021 03:58:56 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Sat, 27 Mar 2021 03:58:59 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Sat, 27 Mar 2021 03:59:49 GMT
ENV COUCHDB_VERSION=3.0.1
# Sat, 27 Mar 2021 03:59:52 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb buster main" > /etc/apt/sources.list.d/couchdb.list
# Sat, 27 Mar 2021 04:00:15 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 27 Mar 2021 04:00:16 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 27 Mar 2021 04:00:18 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 27 Mar 2021 04:00:18 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Sat, 27 Mar 2021 04:00:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 27 Mar 2021 04:00:23 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 27 Mar 2021 04:00:24 GMT
VOLUME [/opt/couchdb/data]
# Sat, 27 Mar 2021 04:00:25 GMT
EXPOSE 4369 5984 9100
# Sat, 27 Mar 2021 04:00:26 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:989f98f7e44fde3e2eb49bc6d2bfed15401201d21cd90f42cd9fc4c26eef8bb0`  
		Last Modified: Fri, 26 Mar 2021 15:48:47 GMT  
		Size: 25.9 MB (25856384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c07bb39a6cb2e40e6fc495018e6a5e67e72664e64fde7be07a00af7efcfdb25`  
		Last Modified: Sat, 27 Mar 2021 04:05:15 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23021ef367eef3af8f8baca64bef5704978b3fa30ed3fbf3ad185cc433635f1c`  
		Last Modified: Sat, 27 Mar 2021 04:05:15 GMT  
		Size: 6.6 MB (6550237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16580e7719e6f506b8fc0760128bfe3831b3616113ed738be5f1bbf3946e5ab7`  
		Last Modified: Sat, 27 Mar 2021 04:05:13 GMT  
		Size: 1.1 MB (1127209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c22f172537b79c577ed6ce4bf2ca28014d7b916ee66d8eca7cafc5ae9e2fdf7`  
		Last Modified: Sat, 27 Mar 2021 04:05:13 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed333509257c33586565b08ad8152b97789a038695aef7bca3185893567ad72`  
		Last Modified: Sat, 27 Mar 2021 04:05:34 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af9a43d12665902e62b566a86d1b01ca4b8b4653b94fd442c9bbfabb8bc7c25`  
		Last Modified: Sat, 27 Mar 2021 04:05:42 GMT  
		Size: 44.7 MB (44708448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac7033145d975dcb41d9f0429f11de5e598afd68de85c3b90782c257ba9e5a2a`  
		Last Modified: Sat, 27 Mar 2021 04:05:33 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73706bbb6f62cc38352e8788852e3b7b4cac047b9008363c94e217f6bd9b6a8`  
		Last Modified: Sat, 27 Mar 2021 04:05:33 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0756706b206dd320cc270d01cb5d3fd09af607b3a12333c6a46f87ec4ac6ec5`  
		Last Modified: Sat, 27 Mar 2021 04:05:33 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420ca416128a980b79f17457e0c76330acff2d1b418119a282d9893d0101e3cd`  
		Last Modified: Sat, 27 Mar 2021 04:05:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1`

```console
$ docker pull couchdb@sha256:bbfa9db04a940916fca50a4eb0057b210ac7f8184400c7cae7247085bd444efd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:34f99d0a7afd22dd2211f78d22cb0313285d21f0a1714ec5b4845a88465afe1a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.4 MB (83366837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:639e80b8aac0ffff7bba56ae979dc4bfece49dd7485550808ab1260a8bdfebb2`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 26 Mar 2021 15:20:59 GMT
ADD file:b2085f4b0a7cb0e5754874c712254e5cd941062b27b8d7ed2080520196b91597 in / 
# Fri, 26 Mar 2021 15:20:59 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:39:57 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 27 Mar 2021 05:39:58 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 27 Mar 2021 05:40:07 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:40:07 GMT
ENV GOSU_VERSION=1.11
# Sat, 27 Mar 2021 05:40:07 GMT
ENV TINI_VERSION=0.18.0
# Sat, 27 Mar 2021 05:40:20 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Sat, 27 Mar 2021 05:40:20 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Sat, 27 Mar 2021 05:41:43 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Sat, 27 Mar 2021 05:41:44 GMT
ENV COUCHDB_VERSION=3.1.1
# Sat, 27 Mar 2021 05:41:45 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb buster main" > /etc/apt/sources.list.d/couchdb.list
# Sat, 27 Mar 2021 05:41:59 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 27 Mar 2021 05:41:59 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 27 Mar 2021 05:41:59 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 27 Mar 2021 05:42:00 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Sat, 27 Mar 2021 05:42:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 27 Mar 2021 05:42:01 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 27 Mar 2021 05:42:01 GMT
VOLUME [/opt/couchdb/data]
# Sat, 27 Mar 2021 05:42:01 GMT
EXPOSE 4369 5984 9100
# Sat, 27 Mar 2021 05:42:02 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ac2522cc72690febc428fb46fb39a4efc5e0a721c3ad15d9992b01515f2fad1a`  
		Last Modified: Fri, 26 Mar 2021 15:27:47 GMT  
		Size: 27.1 MB (27100996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd85d6fda1932ecaf8b874bfe43a05c51749b96b06a6444b9fd7b5e2a13a39a`  
		Last Modified: Sat, 27 Mar 2021 05:47:32 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688cb4b1dcebeaded848ad0def250dfab09a6a744e72bf1d648d389ab3f61dbc`  
		Last Modified: Sat, 27 Mar 2021 05:47:30 GMT  
		Size: 6.7 MB (6690481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b47df997a5ff452e78398fdec86929de1eba2999b37337df310700de6e1e20`  
		Last Modified: Sat, 27 Mar 2021 05:47:29 GMT  
		Size: 1.2 MB (1192799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df16dcc32fe4243098a9d68357e33780d55fb244daadab1f1d8952d73cd7c78`  
		Last Modified: Sat, 27 Mar 2021 05:47:29 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5319a774b98363bda874f2ee59e7889c7823c7d348df7e06beebbcb76cadd0c`  
		Last Modified: Sat, 27 Mar 2021 05:47:29 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52dbd6d0c0a88fc1a974aaa936755b95facbbb5d4ff7fdc4d46c43514304ea79`  
		Last Modified: Sat, 27 Mar 2021 05:47:32 GMT  
		Size: 48.4 MB (48373108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566cbdd2257fd82b3e7ed8ab84f5bb30474c7f85094eb4aa5a89706887763431`  
		Last Modified: Sat, 27 Mar 2021 05:47:26 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d0983079f7919550f3f82ba1307da276bbf8ceb7463f3004ce982f609390ce`  
		Last Modified: Sat, 27 Mar 2021 05:47:26 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44e12b8c2d1ed8bf84e30d70cb635917e7b0e3dcbe3caaad90775b11597514e`  
		Last Modified: Sat, 27 Mar 2021 05:47:27 GMT  
		Size: 2.1 KB (2062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e6e2faee2471a6db48bc41ca8965739a40b952e3496e7370e5b526a33e5016`  
		Last Modified: Sat, 27 Mar 2021 05:47:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:7e5a4b7f65e823b0bfdd5513e0e9c1f153569f1cf28b5b0ce06e64142de8027e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.4 MB (78399848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bab4ab6118c87902dfea4f501aaf7b7ea7ac8571a451e7e3d0637b6782ba9dff`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 26 Mar 2021 15:41:54 GMT
ADD file:c8c0d923527574a26725e0a1995051870ed169ff6b6ebfe77c50810f5583690b in / 
# Fri, 26 Mar 2021 15:41:56 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 03:56:47 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 27 Mar 2021 03:56:51 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 27 Mar 2021 03:57:11 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 03:57:13 GMT
ENV GOSU_VERSION=1.11
# Sat, 27 Mar 2021 03:57:16 GMT
ENV TINI_VERSION=0.18.0
# Sat, 27 Mar 2021 03:58:55 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Sat, 27 Mar 2021 03:58:56 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Sat, 27 Mar 2021 03:58:59 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Sat, 27 Mar 2021 03:59:00 GMT
ENV COUCHDB_VERSION=3.1.1
# Sat, 27 Mar 2021 03:59:02 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb buster main" > /etc/apt/sources.list.d/couchdb.list
# Sat, 27 Mar 2021 03:59:25 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 27 Mar 2021 03:59:27 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 27 Mar 2021 03:59:28 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 27 Mar 2021 03:59:29 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Sat, 27 Mar 2021 03:59:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 27 Mar 2021 03:59:35 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 27 Mar 2021 03:59:36 GMT
VOLUME [/opt/couchdb/data]
# Sat, 27 Mar 2021 03:59:37 GMT
EXPOSE 4369 5984 9100
# Sat, 27 Mar 2021 03:59:39 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:989f98f7e44fde3e2eb49bc6d2bfed15401201d21cd90f42cd9fc4c26eef8bb0`  
		Last Modified: Fri, 26 Mar 2021 15:48:47 GMT  
		Size: 25.9 MB (25856384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c07bb39a6cb2e40e6fc495018e6a5e67e72664e64fde7be07a00af7efcfdb25`  
		Last Modified: Sat, 27 Mar 2021 04:05:15 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23021ef367eef3af8f8baca64bef5704978b3fa30ed3fbf3ad185cc433635f1c`  
		Last Modified: Sat, 27 Mar 2021 04:05:15 GMT  
		Size: 6.6 MB (6550237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16580e7719e6f506b8fc0760128bfe3831b3616113ed738be5f1bbf3946e5ab7`  
		Last Modified: Sat, 27 Mar 2021 04:05:13 GMT  
		Size: 1.1 MB (1127209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c22f172537b79c577ed6ce4bf2ca28014d7b916ee66d8eca7cafc5ae9e2fdf7`  
		Last Modified: Sat, 27 Mar 2021 04:05:13 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03023b4142a3b5ee76506db88343d2f3134ac7e144161e6761330cf1329a178`  
		Last Modified: Sat, 27 Mar 2021 04:05:13 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426c9a8c52fd17f4838ec640d534c927944ec23d8291da83ac67bba359cce2c1`  
		Last Modified: Sat, 27 Mar 2021 04:05:20 GMT  
		Size: 44.9 MB (44856541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911410d0a5f93377e0a28c1c5c000418220ee85adf99e24241395dfef52cbdf4`  
		Last Modified: Sat, 27 Mar 2021 04:05:11 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0c193871be5b8d9e61be9d947be65a92e5747e9ce01656015d5065d3ac9dd5`  
		Last Modified: Sat, 27 Mar 2021 04:05:11 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69a19510ccf86e9cddee6a5674df81f2dfa153e8704424907f3ee48299f6b85`  
		Last Modified: Sat, 27 Mar 2021 04:05:11 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538f0a77085e6cf6646f8f5bd704b6d957dfc04f89b71ecba0a2ac6462ba462f`  
		Last Modified: Sat, 27 Mar 2021 04:05:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1.1`

```console
$ docker pull couchdb@sha256:bbfa9db04a940916fca50a4eb0057b210ac7f8184400c7cae7247085bd444efd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1.1` - linux; amd64

```console
$ docker pull couchdb@sha256:34f99d0a7afd22dd2211f78d22cb0313285d21f0a1714ec5b4845a88465afe1a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.4 MB (83366837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:639e80b8aac0ffff7bba56ae979dc4bfece49dd7485550808ab1260a8bdfebb2`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 26 Mar 2021 15:20:59 GMT
ADD file:b2085f4b0a7cb0e5754874c712254e5cd941062b27b8d7ed2080520196b91597 in / 
# Fri, 26 Mar 2021 15:20:59 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:39:57 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 27 Mar 2021 05:39:58 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 27 Mar 2021 05:40:07 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:40:07 GMT
ENV GOSU_VERSION=1.11
# Sat, 27 Mar 2021 05:40:07 GMT
ENV TINI_VERSION=0.18.0
# Sat, 27 Mar 2021 05:40:20 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Sat, 27 Mar 2021 05:40:20 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Sat, 27 Mar 2021 05:41:43 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Sat, 27 Mar 2021 05:41:44 GMT
ENV COUCHDB_VERSION=3.1.1
# Sat, 27 Mar 2021 05:41:45 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb buster main" > /etc/apt/sources.list.d/couchdb.list
# Sat, 27 Mar 2021 05:41:59 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 27 Mar 2021 05:41:59 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 27 Mar 2021 05:41:59 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 27 Mar 2021 05:42:00 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Sat, 27 Mar 2021 05:42:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 27 Mar 2021 05:42:01 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 27 Mar 2021 05:42:01 GMT
VOLUME [/opt/couchdb/data]
# Sat, 27 Mar 2021 05:42:01 GMT
EXPOSE 4369 5984 9100
# Sat, 27 Mar 2021 05:42:02 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ac2522cc72690febc428fb46fb39a4efc5e0a721c3ad15d9992b01515f2fad1a`  
		Last Modified: Fri, 26 Mar 2021 15:27:47 GMT  
		Size: 27.1 MB (27100996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd85d6fda1932ecaf8b874bfe43a05c51749b96b06a6444b9fd7b5e2a13a39a`  
		Last Modified: Sat, 27 Mar 2021 05:47:32 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688cb4b1dcebeaded848ad0def250dfab09a6a744e72bf1d648d389ab3f61dbc`  
		Last Modified: Sat, 27 Mar 2021 05:47:30 GMT  
		Size: 6.7 MB (6690481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b47df997a5ff452e78398fdec86929de1eba2999b37337df310700de6e1e20`  
		Last Modified: Sat, 27 Mar 2021 05:47:29 GMT  
		Size: 1.2 MB (1192799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df16dcc32fe4243098a9d68357e33780d55fb244daadab1f1d8952d73cd7c78`  
		Last Modified: Sat, 27 Mar 2021 05:47:29 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5319a774b98363bda874f2ee59e7889c7823c7d348df7e06beebbcb76cadd0c`  
		Last Modified: Sat, 27 Mar 2021 05:47:29 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52dbd6d0c0a88fc1a974aaa936755b95facbbb5d4ff7fdc4d46c43514304ea79`  
		Last Modified: Sat, 27 Mar 2021 05:47:32 GMT  
		Size: 48.4 MB (48373108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566cbdd2257fd82b3e7ed8ab84f5bb30474c7f85094eb4aa5a89706887763431`  
		Last Modified: Sat, 27 Mar 2021 05:47:26 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d0983079f7919550f3f82ba1307da276bbf8ceb7463f3004ce982f609390ce`  
		Last Modified: Sat, 27 Mar 2021 05:47:26 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44e12b8c2d1ed8bf84e30d70cb635917e7b0e3dcbe3caaad90775b11597514e`  
		Last Modified: Sat, 27 Mar 2021 05:47:27 GMT  
		Size: 2.1 KB (2062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e6e2faee2471a6db48bc41ca8965739a40b952e3496e7370e5b526a33e5016`  
		Last Modified: Sat, 27 Mar 2021 05:47:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:7e5a4b7f65e823b0bfdd5513e0e9c1f153569f1cf28b5b0ce06e64142de8027e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.4 MB (78399848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bab4ab6118c87902dfea4f501aaf7b7ea7ac8571a451e7e3d0637b6782ba9dff`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 26 Mar 2021 15:41:54 GMT
ADD file:c8c0d923527574a26725e0a1995051870ed169ff6b6ebfe77c50810f5583690b in / 
# Fri, 26 Mar 2021 15:41:56 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 03:56:47 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 27 Mar 2021 03:56:51 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 27 Mar 2021 03:57:11 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 03:57:13 GMT
ENV GOSU_VERSION=1.11
# Sat, 27 Mar 2021 03:57:16 GMT
ENV TINI_VERSION=0.18.0
# Sat, 27 Mar 2021 03:58:55 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Sat, 27 Mar 2021 03:58:56 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Sat, 27 Mar 2021 03:58:59 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Sat, 27 Mar 2021 03:59:00 GMT
ENV COUCHDB_VERSION=3.1.1
# Sat, 27 Mar 2021 03:59:02 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb buster main" > /etc/apt/sources.list.d/couchdb.list
# Sat, 27 Mar 2021 03:59:25 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 27 Mar 2021 03:59:27 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 27 Mar 2021 03:59:28 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 27 Mar 2021 03:59:29 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Sat, 27 Mar 2021 03:59:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 27 Mar 2021 03:59:35 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 27 Mar 2021 03:59:36 GMT
VOLUME [/opt/couchdb/data]
# Sat, 27 Mar 2021 03:59:37 GMT
EXPOSE 4369 5984 9100
# Sat, 27 Mar 2021 03:59:39 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:989f98f7e44fde3e2eb49bc6d2bfed15401201d21cd90f42cd9fc4c26eef8bb0`  
		Last Modified: Fri, 26 Mar 2021 15:48:47 GMT  
		Size: 25.9 MB (25856384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c07bb39a6cb2e40e6fc495018e6a5e67e72664e64fde7be07a00af7efcfdb25`  
		Last Modified: Sat, 27 Mar 2021 04:05:15 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23021ef367eef3af8f8baca64bef5704978b3fa30ed3fbf3ad185cc433635f1c`  
		Last Modified: Sat, 27 Mar 2021 04:05:15 GMT  
		Size: 6.6 MB (6550237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16580e7719e6f506b8fc0760128bfe3831b3616113ed738be5f1bbf3946e5ab7`  
		Last Modified: Sat, 27 Mar 2021 04:05:13 GMT  
		Size: 1.1 MB (1127209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c22f172537b79c577ed6ce4bf2ca28014d7b916ee66d8eca7cafc5ae9e2fdf7`  
		Last Modified: Sat, 27 Mar 2021 04:05:13 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03023b4142a3b5ee76506db88343d2f3134ac7e144161e6761330cf1329a178`  
		Last Modified: Sat, 27 Mar 2021 04:05:13 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426c9a8c52fd17f4838ec640d534c927944ec23d8291da83ac67bba359cce2c1`  
		Last Modified: Sat, 27 Mar 2021 04:05:20 GMT  
		Size: 44.9 MB (44856541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911410d0a5f93377e0a28c1c5c000418220ee85adf99e24241395dfef52cbdf4`  
		Last Modified: Sat, 27 Mar 2021 04:05:11 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0c193871be5b8d9e61be9d947be65a92e5747e9ce01656015d5065d3ac9dd5`  
		Last Modified: Sat, 27 Mar 2021 04:05:11 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69a19510ccf86e9cddee6a5674df81f2dfa153e8704424907f3ee48299f6b85`  
		Last Modified: Sat, 27 Mar 2021 04:05:11 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538f0a77085e6cf6646f8f5bd704b6d957dfc04f89b71ecba0a2ac6462ba462f`  
		Last Modified: Sat, 27 Mar 2021 04:05:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:latest`

```console
$ docker pull couchdb@sha256:bbfa9db04a940916fca50a4eb0057b210ac7f8184400c7cae7247085bd444efd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:34f99d0a7afd22dd2211f78d22cb0313285d21f0a1714ec5b4845a88465afe1a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.4 MB (83366837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:639e80b8aac0ffff7bba56ae979dc4bfece49dd7485550808ab1260a8bdfebb2`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 26 Mar 2021 15:20:59 GMT
ADD file:b2085f4b0a7cb0e5754874c712254e5cd941062b27b8d7ed2080520196b91597 in / 
# Fri, 26 Mar 2021 15:20:59 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:39:57 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 27 Mar 2021 05:39:58 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 27 Mar 2021 05:40:07 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:40:07 GMT
ENV GOSU_VERSION=1.11
# Sat, 27 Mar 2021 05:40:07 GMT
ENV TINI_VERSION=0.18.0
# Sat, 27 Mar 2021 05:40:20 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Sat, 27 Mar 2021 05:40:20 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Sat, 27 Mar 2021 05:41:43 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Sat, 27 Mar 2021 05:41:44 GMT
ENV COUCHDB_VERSION=3.1.1
# Sat, 27 Mar 2021 05:41:45 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb buster main" > /etc/apt/sources.list.d/couchdb.list
# Sat, 27 Mar 2021 05:41:59 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 27 Mar 2021 05:41:59 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 27 Mar 2021 05:41:59 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 27 Mar 2021 05:42:00 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Sat, 27 Mar 2021 05:42:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 27 Mar 2021 05:42:01 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 27 Mar 2021 05:42:01 GMT
VOLUME [/opt/couchdb/data]
# Sat, 27 Mar 2021 05:42:01 GMT
EXPOSE 4369 5984 9100
# Sat, 27 Mar 2021 05:42:02 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ac2522cc72690febc428fb46fb39a4efc5e0a721c3ad15d9992b01515f2fad1a`  
		Last Modified: Fri, 26 Mar 2021 15:27:47 GMT  
		Size: 27.1 MB (27100996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd85d6fda1932ecaf8b874bfe43a05c51749b96b06a6444b9fd7b5e2a13a39a`  
		Last Modified: Sat, 27 Mar 2021 05:47:32 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688cb4b1dcebeaded848ad0def250dfab09a6a744e72bf1d648d389ab3f61dbc`  
		Last Modified: Sat, 27 Mar 2021 05:47:30 GMT  
		Size: 6.7 MB (6690481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b47df997a5ff452e78398fdec86929de1eba2999b37337df310700de6e1e20`  
		Last Modified: Sat, 27 Mar 2021 05:47:29 GMT  
		Size: 1.2 MB (1192799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df16dcc32fe4243098a9d68357e33780d55fb244daadab1f1d8952d73cd7c78`  
		Last Modified: Sat, 27 Mar 2021 05:47:29 GMT  
		Size: 2.5 KB (2491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5319a774b98363bda874f2ee59e7889c7823c7d348df7e06beebbcb76cadd0c`  
		Last Modified: Sat, 27 Mar 2021 05:47:29 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52dbd6d0c0a88fc1a974aaa936755b95facbbb5d4ff7fdc4d46c43514304ea79`  
		Last Modified: Sat, 27 Mar 2021 05:47:32 GMT  
		Size: 48.4 MB (48373108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566cbdd2257fd82b3e7ed8ab84f5bb30474c7f85094eb4aa5a89706887763431`  
		Last Modified: Sat, 27 Mar 2021 05:47:26 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d0983079f7919550f3f82ba1307da276bbf8ceb7463f3004ce982f609390ce`  
		Last Modified: Sat, 27 Mar 2021 05:47:26 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44e12b8c2d1ed8bf84e30d70cb635917e7b0e3dcbe3caaad90775b11597514e`  
		Last Modified: Sat, 27 Mar 2021 05:47:27 GMT  
		Size: 2.1 KB (2062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e6e2faee2471a6db48bc41ca8965739a40b952e3496e7370e5b526a33e5016`  
		Last Modified: Sat, 27 Mar 2021 05:47:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:7e5a4b7f65e823b0bfdd5513e0e9c1f153569f1cf28b5b0ce06e64142de8027e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.4 MB (78399848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bab4ab6118c87902dfea4f501aaf7b7ea7ac8571a451e7e3d0637b6782ba9dff`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Fri, 26 Mar 2021 15:41:54 GMT
ADD file:c8c0d923527574a26725e0a1995051870ed169ff6b6ebfe77c50810f5583690b in / 
# Fri, 26 Mar 2021 15:41:56 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 03:56:47 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Sat, 27 Mar 2021 03:56:51 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Sat, 27 Mar 2021 03:57:11 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 03:57:13 GMT
ENV GOSU_VERSION=1.11
# Sat, 27 Mar 2021 03:57:16 GMT
ENV TINI_VERSION=0.18.0
# Sat, 27 Mar 2021 03:58:55 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends wget;     rm -rf /var/lib/apt/lists/*;         dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')";         wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/${GOSU_VERSION}/gosu-$dpkgArch";     wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4 && break || : ;     done;     gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu;     rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc;     chmod +x /usr/local/bin/gosu;     gosu nobody true;         wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch";     wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v${TINI_VERSION}/tini-$dpkgArch.asc";     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do     gpg --batch --keyserver $server --recv-keys 595E85A6B1B4779EA4DAAEC70B588DFF0527A9B7 && break || : ;     done;     gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini;     rm -rf "$GNUPGHOME" /usr/local/bin/tini.asc;     chmod +x /usr/local/bin/tini;     apt-get purge -y --auto-remove wget;     tini --version
# Sat, 27 Mar 2021 03:58:56 GMT
ENV GPG_COUCH_KEY=8756C4F765C9AC3CB6B85D62379CE192D401AB61
# Sat, 27 Mar 2021 03:58:59 GMT
RUN set -xe;     export GNUPGHOME="$(mktemp -d)";     echo "disable-ipv6" >> ${GNUPGHOME}/dirmngr.conf;     for server in $(shuf -e pgpkeys.mit.edu         ha.pool.sks-keyservers.net         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu) ; do         gpg --batch --keyserver $server --recv-keys $GPG_COUCH_KEY && break || : ;     done;     gpg --batch --export $GPG_COUCH_KEY > /etc/apt/trusted.gpg.d/couchdb.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list
# Sat, 27 Mar 2021 03:59:00 GMT
ENV COUCHDB_VERSION=3.1.1
# Sat, 27 Mar 2021 03:59:02 GMT
RUN echo "deb https://apache.bintray.com/couchdb-deb buster main" > /etc/apt/sources.list.d/couchdb.list
# Sat, 27 Mar 2021 03:59:25 GMT
RUN set -xe;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 27 Mar 2021 03:59:27 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 27 Mar 2021 03:59:28 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 27 Mar 2021 03:59:29 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Sat, 27 Mar 2021 03:59:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 27 Mar 2021 03:59:35 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 27 Mar 2021 03:59:36 GMT
VOLUME [/opt/couchdb/data]
# Sat, 27 Mar 2021 03:59:37 GMT
EXPOSE 4369 5984 9100
# Sat, 27 Mar 2021 03:59:39 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:989f98f7e44fde3e2eb49bc6d2bfed15401201d21cd90f42cd9fc4c26eef8bb0`  
		Last Modified: Fri, 26 Mar 2021 15:48:47 GMT  
		Size: 25.9 MB (25856384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c07bb39a6cb2e40e6fc495018e6a5e67e72664e64fde7be07a00af7efcfdb25`  
		Last Modified: Sat, 27 Mar 2021 04:05:15 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23021ef367eef3af8f8baca64bef5704978b3fa30ed3fbf3ad185cc433635f1c`  
		Last Modified: Sat, 27 Mar 2021 04:05:15 GMT  
		Size: 6.6 MB (6550237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16580e7719e6f506b8fc0760128bfe3831b3616113ed738be5f1bbf3946e5ab7`  
		Last Modified: Sat, 27 Mar 2021 04:05:13 GMT  
		Size: 1.1 MB (1127209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c22f172537b79c577ed6ce4bf2ca28014d7b916ee66d8eca7cafc5ae9e2fdf7`  
		Last Modified: Sat, 27 Mar 2021 04:05:13 GMT  
		Size: 2.5 KB (2489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03023b4142a3b5ee76506db88343d2f3134ac7e144161e6761330cf1329a178`  
		Last Modified: Sat, 27 Mar 2021 04:05:13 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426c9a8c52fd17f4838ec640d534c927944ec23d8291da83ac67bba359cce2c1`  
		Last Modified: Sat, 27 Mar 2021 04:05:20 GMT  
		Size: 44.9 MB (44856541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911410d0a5f93377e0a28c1c5c000418220ee85adf99e24241395dfef52cbdf4`  
		Last Modified: Sat, 27 Mar 2021 04:05:11 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0c193871be5b8d9e61be9d947be65a92e5747e9ce01656015d5065d3ac9dd5`  
		Last Modified: Sat, 27 Mar 2021 04:05:11 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69a19510ccf86e9cddee6a5674df81f2dfa153e8704424907f3ee48299f6b85`  
		Last Modified: Sat, 27 Mar 2021 04:05:11 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538f0a77085e6cf6646f8f5bd704b6d957dfc04f89b71ecba0a2ac6462ba462f`  
		Last Modified: Sat, 27 Mar 2021 04:05:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
