## `couchdb:latest`

```console
$ docker pull couchdb@sha256:632f5f811d8ec0205872ba8e8cae6e43ad989d58f89da9c9360a8c910db023f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:aa4ca065a91c36bbee201730dbd34bed1685a11a75e15bb4973268407a15bf79
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.8 MB (83771234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cf953a0e1c4aa635d7979afd3b6e4c7c723955e4527dd39b91f1efb018c7bbc`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:29:49 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 22 Jul 2021 01:29:50 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 22 Jul 2021 01:29:58 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:30:02 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 22 Jul 2021 01:30:03 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 22 Jul 2021 01:30:11 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:30:11 GMT
ENV COUCHDB_VERSION=3.1.1
# Thu, 22 Jul 2021 01:30:12 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 22 Jul 2021 01:30:31 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 22 Jul 2021 01:30:31 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 22 Jul 2021 01:30:32 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 22 Jul 2021 01:30:32 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Thu, 22 Jul 2021 01:30:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 22 Jul 2021 01:30:34 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:30:34 GMT
VOLUME [/opt/couchdb/data]
# Thu, 22 Jul 2021 01:30:35 GMT
EXPOSE 4369 5984 9100
# Thu, 22 Jul 2021 01:30:35 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835b688d207b5ab9e89d8cca5f4bf328bfe1f1ede763194a4538ea6fa23da011`  
		Last Modified: Thu, 22 Jul 2021 01:31:45 GMT  
		Size: 3.4 KB (3415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04943acd4d5ea8d1bedf669be78f6a293687056354f3d796a81843b9ec6d2f6e`  
		Last Modified: Thu, 22 Jul 2021 01:31:45 GMT  
		Size: 6.7 MB (6690574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9997c1f5399e25cd41b8489eb0e0394b2f5fba04b0d872a546cb32cf7c272535`  
		Last Modified: Thu, 22 Jul 2021 01:31:43 GMT  
		Size: 1.3 MB (1258344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:429ec9af1234b1a0ca0cb627723e4f03410bc1972d6fe4f15b4a730bd3bfd651`  
		Last Modified: Thu, 22 Jul 2021 01:31:42 GMT  
		Size: 293.0 KB (293013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc6e010df6e6b577a74e9eea1410a6eed1ad69db8d5cfce8c7b0fefc22609b9`  
		Last Modified: Thu, 22 Jul 2021 01:31:42 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c88c15d7fabfe39975f3b6b5d177076bdfae08e05b8462f20bea42544c8aa8`  
		Last Modified: Thu, 22 Jul 2021 01:31:48 GMT  
		Size: 48.4 MB (48376497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97242ba0044f0aec5fbf85a67230ca43fa4981f44ed600a3452fc15492d43374`  
		Last Modified: Thu, 22 Jul 2021 01:31:40 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6403aee522aab15bca7e6422b1ce27325056865370e375bd73f4f660ee9ce5`  
		Last Modified: Thu, 22 Jul 2021 01:31:39 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a327d1fe4ab8fce33608f39b7631107d9c8573e22e829fe9f914463bff6a02e2`  
		Last Modified: Thu, 22 Jul 2021 01:31:39 GMT  
		Size: 2.1 KB (2055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c492e57bffa3b58bf0eb05858221452abb78712c4c06bd72d08193648342b699`  
		Last Modified: Thu, 22 Jul 2021 01:31:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:dd84e57fbd0faf425780658104d397b60e416045e79a1d9ad6875f94136db802
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.8 MB (78786772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e503901387235ad71719d6b858db23dfa2790c3feb5fe61cd18caf43eff221b0`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 08:09:33 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 17 Aug 2021 08:09:33 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 17 Aug 2021 08:09:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 08:09:45 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 17 Aug 2021 08:09:45 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 17 Aug 2021 08:09:51 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 08:09:51 GMT
ENV COUCHDB_VERSION=3.1.1
# Tue, 17 Aug 2021 08:09:52 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 17 Aug 2021 08:10:05 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 17 Aug 2021 08:10:05 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 17 Aug 2021 08:10:05 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 17 Aug 2021 08:10:05 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 17 Aug 2021 08:10:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 17 Aug 2021 08:10:06 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 08:10:06 GMT
VOLUME [/opt/couchdb/data]
# Tue, 17 Aug 2021 08:10:07 GMT
EXPOSE 4369 5984 9100
# Tue, 17 Aug 2021 08:10:07 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab787026ef6a8144c5eabbda8d5bdf43afc3c79eef1ada02802921541490d37`  
		Last Modified: Tue, 17 Aug 2021 08:11:00 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08ebe0a9c5656679672b817a6a586b31d8a518f90b2f77b5e5a0d70841c93a47`  
		Last Modified: Tue, 17 Aug 2021 08:10:59 GMT  
		Size: 6.6 MB (6550146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67fe32ef3fc734dde11d93c43255cdc4631d4f400588f69dbd6fca417c452e7`  
		Last Modified: Tue, 17 Aug 2021 08:10:57 GMT  
		Size: 1.2 MB (1163423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a7736bc7346c11850cfda36cd6466ed5503f0bbaf145f42af99fbc8e23ee4c`  
		Last Modified: Tue, 17 Aug 2021 08:10:57 GMT  
		Size: 292.8 KB (292835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674f4f8ee188a1fc3881a8df04010762aea5571dbd6f6f94bde11b6d99fcd226`  
		Last Modified: Tue, 17 Aug 2021 08:10:57 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7357dc2ac83e096d9a5a8339d536e1f107fe6ec9aa137f55f22ca3dc5b50ce2d`  
		Last Modified: Tue, 17 Aug 2021 08:11:01 GMT  
		Size: 44.9 MB (44858259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd867e8dd88bd32c96ea29ef89ca9d1a96eb3f2cecce22f7ed0bf15e53a5d973`  
		Last Modified: Tue, 17 Aug 2021 08:10:55 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdee44909007a1881df438bf583366a0a50b63445592b3768da9eb3e9a02c66b`  
		Last Modified: Tue, 17 Aug 2021 08:10:55 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5af2b755a984a8b02e191a3d99bc10694845107932d5b1388e565f5ae05b54`  
		Last Modified: Tue, 17 Aug 2021 08:10:55 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40fbecafdba0dbcfe6591ece6bd85ddce50a962bbbdc03a262a86ff64dc5caea`  
		Last Modified: Tue, 17 Aug 2021 08:10:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
