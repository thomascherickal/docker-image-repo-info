<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `couchdb`

-	[`couchdb:2`](#couchdb2)
-	[`couchdb:2.3`](#couchdb23)
-	[`couchdb:2.3.1`](#couchdb231)
-	[`couchdb:3`](#couchdb3)
-	[`couchdb:3.1`](#couchdb31)
-	[`couchdb:3.1.2`](#couchdb312)
-	[`couchdb:3.2`](#couchdb32)
-	[`couchdb:3.2.2`](#couchdb322)
-	[`couchdb:3.3`](#couchdb33)
-	[`couchdb:3.3.1`](#couchdb331)
-	[`couchdb:latest`](#couchdblatest)

## `couchdb:2`

```console
$ docker pull couchdb@sha256:51463aea58b86f23e62c9022ba23001d952583fae86d824d648aac612b5b581c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2` - linux; amd64

```console
$ docker pull couchdb@sha256:d897124cc1fb7c2b6e587c51fef80759ac6b60e2b314a9ea20b7621bb0335ab8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84539097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1625a43dc510f1cd112d2299cefa16d76d4a47efac07dcc357b4c2a51edc140`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:50 GMT
ADD file:52316aa7d631242cd16337be337e57187ef07d3965e6284321fbdcd5b4f92b64 in / 
# Thu, 23 Mar 2023 01:30:51 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:14:14 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 23 Mar 2023 06:14:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 23 Mar 2023 06:14:22 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:14:26 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 23 Mar 2023 06:14:26 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 23 Mar 2023 06:14:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:14:54 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Thu, 23 Mar 2023 06:14:55 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 23 Mar 2023 06:15:12 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 23 Mar 2023 06:15:12 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Thu, 23 Mar 2023 06:15:12 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 23 Mar 2023 06:15:12 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Thu, 23 Mar 2023 06:15:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 06:15:13 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 06:15:13 GMT
VOLUME [/opt/couchdb/data]
# Thu, 23 Mar 2023 06:15:13 GMT
EXPOSE 4369 5984 9100
# Thu, 23 Mar 2023 06:15:13 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:3689b8de819b48387712c6d4d62d26a52a04c9e88afc68fb9d1dbe48bfa9e21d`  
		Last Modified: Thu, 23 Mar 2023 01:35:01 GMT  
		Size: 27.1 MB (27139869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07228e786e9fcae89eb2cc59a0752d290f19a708f0296ba7c17d1a55a4a80243`  
		Last Modified: Thu, 23 Mar 2023 06:16:03 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4700a153729c2edb362e307d55407cfeca29dc1d2e309a9c41e60a5edf2ee909`  
		Last Modified: Thu, 23 Mar 2023 06:16:02 GMT  
		Size: 6.7 MB (6705910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48402339fa56c0ac77cffd1a404f50aa8baee7a84f48d4ac30ad21dbe244bb60`  
		Last Modified: Thu, 23 Mar 2023 06:16:01 GMT  
		Size: 1.3 MB (1259595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de61bdb3ed274c78ebcd762fd00ffafeb1800d4f89ac1935ed0c5c0112738a9`  
		Last Modified: Thu, 23 Mar 2023 06:16:01 GMT  
		Size: 294.3 KB (294308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09828b0ad787ccc70ab5384663a5eebfb0de21879e3744086a981944399af163`  
		Last Modified: Thu, 23 Mar 2023 06:16:15 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9456a91d45977c57d79bfeae0b01294cc8a90da7508a632d733875832ae9796`  
		Last Modified: Thu, 23 Mar 2023 06:16:19 GMT  
		Size: 49.1 MB (49132402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14cbb10181487d791c698ef0220b9e934c3526d9b28d496ae841b0ab75589b2`  
		Last Modified: Thu, 23 Mar 2023 06:16:13 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a4afcb05d9a4b703dfb73eebdfd5e7b719323bdccbaf0006630697f59b4546`  
		Last Modified: Thu, 23 Mar 2023 06:16:13 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c74fc0a87059073c5f4204dea243c2c84fd2d3de6f1b7051dfa8b9ac5493585`  
		Last Modified: Thu, 23 Mar 2023 06:16:13 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b293d5f0522e749edbf4cf9cd8b9d118b16f2fc1224f0f0f69b07d01b1d337c`  
		Last Modified: Thu, 23 Mar 2023 06:16:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:f26338905cfef82b1c3b98668815faee16df60e1f1cfbcbcb01bf23c38df8f13
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72997052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:378ddae722d95218e9ea965ba00c139fd30a0cf3b1287d69075be9f43dfadf8c`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:23 GMT
ADD file:44e400cc6a1bc5df5a57bda478c9accf9b58950fa2fd069cc7620128fe786770 in / 
# Thu, 23 Mar 2023 00:45:23 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:20:41 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 23 Mar 2023 07:20:42 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 23 Mar 2023 07:20:48 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:20:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 23 Mar 2023 07:20:52 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 23 Mar 2023 07:20:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:21:14 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Thu, 23 Mar 2023 07:21:15 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 23 Mar 2023 07:21:26 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 23 Mar 2023 07:21:26 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Thu, 23 Mar 2023 07:21:26 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 23 Mar 2023 07:21:26 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Thu, 23 Mar 2023 07:21:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 07:21:27 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 07:21:27 GMT
VOLUME [/opt/couchdb/data]
# Thu, 23 Mar 2023 07:21:27 GMT
EXPOSE 4369 5984 9100
# Thu, 23 Mar 2023 07:21:27 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:cfe0f778e53ce031ef449bc02975a07f2568716dea807ed2f390d352c0001972`  
		Last Modified: Thu, 23 Mar 2023 00:48:45 GMT  
		Size: 25.9 MB (25922660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037538668954fe82bbe2e635a631e36780ef15998a07b238b91da1991b30abed`  
		Last Modified: Thu, 23 Mar 2023 07:22:12 GMT  
		Size: 3.4 KB (3434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b0009f03b4cc05f74eb4b4bd8ab0ebafc260f3f74d25ba8fc8f089a108b9c55`  
		Last Modified: Thu, 23 Mar 2023 07:22:11 GMT  
		Size: 6.6 MB (6579451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f1f9f14a5ccaec42852a7b41044e85fb849ec6d2b8b4d52b627f88a8664c86`  
		Last Modified: Thu, 23 Mar 2023 07:22:10 GMT  
		Size: 1.2 MB (1164523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68f0b4ec14b9eaedd46f27ebe44d30eb877b71e65c14c22d90f46cf6a92f9eb`  
		Last Modified: Thu, 23 Mar 2023 07:22:10 GMT  
		Size: 294.1 KB (294127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581e7873e9d1cff45cfe0b6a81f0ae2eeaeeacc57e5daaf3b84a361852e89b9e`  
		Last Modified: Thu, 23 Mar 2023 07:22:22 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1fc3f02dfb5b2a49da78bed468a8760607fbf73b57bf5009e1782947fe8855c`  
		Last Modified: Thu, 23 Mar 2023 07:22:24 GMT  
		Size: 39.0 MB (39029258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7442e502d15f1a588b3ff55118e637a9a8b42e98c424492b800454aecd8b113`  
		Last Modified: Thu, 23 Mar 2023 07:22:20 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c6a3c93062d6f0dc73fac47a397eae854a2bcdf5b1143fc684dbf93f8951c5`  
		Last Modified: Thu, 23 Mar 2023 07:22:20 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a03c1aa1eaf7dce756cddd74fe9f1a465d16d5a609abd477cf79a61cea71c5e`  
		Last Modified: Thu, 23 Mar 2023 07:22:20 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070ca35370089cfad095bbe4fe09b48f119a1203ae0d3ded1cb0aaa96b7b440e`  
		Last Modified: Thu, 23 Mar 2023 07:22:20 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3`

```console
$ docker pull couchdb@sha256:51463aea58b86f23e62c9022ba23001d952583fae86d824d648aac612b5b581c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:d897124cc1fb7c2b6e587c51fef80759ac6b60e2b314a9ea20b7621bb0335ab8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84539097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1625a43dc510f1cd112d2299cefa16d76d4a47efac07dcc357b4c2a51edc140`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:50 GMT
ADD file:52316aa7d631242cd16337be337e57187ef07d3965e6284321fbdcd5b4f92b64 in / 
# Thu, 23 Mar 2023 01:30:51 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:14:14 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 23 Mar 2023 06:14:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 23 Mar 2023 06:14:22 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:14:26 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 23 Mar 2023 06:14:26 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 23 Mar 2023 06:14:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:14:54 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Thu, 23 Mar 2023 06:14:55 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 23 Mar 2023 06:15:12 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 23 Mar 2023 06:15:12 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Thu, 23 Mar 2023 06:15:12 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 23 Mar 2023 06:15:12 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Thu, 23 Mar 2023 06:15:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 06:15:13 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 06:15:13 GMT
VOLUME [/opt/couchdb/data]
# Thu, 23 Mar 2023 06:15:13 GMT
EXPOSE 4369 5984 9100
# Thu, 23 Mar 2023 06:15:13 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:3689b8de819b48387712c6d4d62d26a52a04c9e88afc68fb9d1dbe48bfa9e21d`  
		Last Modified: Thu, 23 Mar 2023 01:35:01 GMT  
		Size: 27.1 MB (27139869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07228e786e9fcae89eb2cc59a0752d290f19a708f0296ba7c17d1a55a4a80243`  
		Last Modified: Thu, 23 Mar 2023 06:16:03 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4700a153729c2edb362e307d55407cfeca29dc1d2e309a9c41e60a5edf2ee909`  
		Last Modified: Thu, 23 Mar 2023 06:16:02 GMT  
		Size: 6.7 MB (6705910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48402339fa56c0ac77cffd1a404f50aa8baee7a84f48d4ac30ad21dbe244bb60`  
		Last Modified: Thu, 23 Mar 2023 06:16:01 GMT  
		Size: 1.3 MB (1259595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de61bdb3ed274c78ebcd762fd00ffafeb1800d4f89ac1935ed0c5c0112738a9`  
		Last Modified: Thu, 23 Mar 2023 06:16:01 GMT  
		Size: 294.3 KB (294308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09828b0ad787ccc70ab5384663a5eebfb0de21879e3744086a981944399af163`  
		Last Modified: Thu, 23 Mar 2023 06:16:15 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9456a91d45977c57d79bfeae0b01294cc8a90da7508a632d733875832ae9796`  
		Last Modified: Thu, 23 Mar 2023 06:16:19 GMT  
		Size: 49.1 MB (49132402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14cbb10181487d791c698ef0220b9e934c3526d9b28d496ae841b0ab75589b2`  
		Last Modified: Thu, 23 Mar 2023 06:16:13 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a4afcb05d9a4b703dfb73eebdfd5e7b719323bdccbaf0006630697f59b4546`  
		Last Modified: Thu, 23 Mar 2023 06:16:13 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c74fc0a87059073c5f4204dea243c2c84fd2d3de6f1b7051dfa8b9ac5493585`  
		Last Modified: Thu, 23 Mar 2023 06:16:13 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b293d5f0522e749edbf4cf9cd8b9d118b16f2fc1224f0f0f69b07d01b1d337c`  
		Last Modified: Thu, 23 Mar 2023 06:16:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:f26338905cfef82b1c3b98668815faee16df60e1f1cfbcbcb01bf23c38df8f13
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72997052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:378ddae722d95218e9ea965ba00c139fd30a0cf3b1287d69075be9f43dfadf8c`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:23 GMT
ADD file:44e400cc6a1bc5df5a57bda478c9accf9b58950fa2fd069cc7620128fe786770 in / 
# Thu, 23 Mar 2023 00:45:23 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:20:41 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 23 Mar 2023 07:20:42 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 23 Mar 2023 07:20:48 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:20:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 23 Mar 2023 07:20:52 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 23 Mar 2023 07:20:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:21:14 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Thu, 23 Mar 2023 07:21:15 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 23 Mar 2023 07:21:26 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 23 Mar 2023 07:21:26 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Thu, 23 Mar 2023 07:21:26 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 23 Mar 2023 07:21:26 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Thu, 23 Mar 2023 07:21:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 07:21:27 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 07:21:27 GMT
VOLUME [/opt/couchdb/data]
# Thu, 23 Mar 2023 07:21:27 GMT
EXPOSE 4369 5984 9100
# Thu, 23 Mar 2023 07:21:27 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:cfe0f778e53ce031ef449bc02975a07f2568716dea807ed2f390d352c0001972`  
		Last Modified: Thu, 23 Mar 2023 00:48:45 GMT  
		Size: 25.9 MB (25922660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037538668954fe82bbe2e635a631e36780ef15998a07b238b91da1991b30abed`  
		Last Modified: Thu, 23 Mar 2023 07:22:12 GMT  
		Size: 3.4 KB (3434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b0009f03b4cc05f74eb4b4bd8ab0ebafc260f3f74d25ba8fc8f089a108b9c55`  
		Last Modified: Thu, 23 Mar 2023 07:22:11 GMT  
		Size: 6.6 MB (6579451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f1f9f14a5ccaec42852a7b41044e85fb849ec6d2b8b4d52b627f88a8664c86`  
		Last Modified: Thu, 23 Mar 2023 07:22:10 GMT  
		Size: 1.2 MB (1164523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68f0b4ec14b9eaedd46f27ebe44d30eb877b71e65c14c22d90f46cf6a92f9eb`  
		Last Modified: Thu, 23 Mar 2023 07:22:10 GMT  
		Size: 294.1 KB (294127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581e7873e9d1cff45cfe0b6a81f0ae2eeaeeacc57e5daaf3b84a361852e89b9e`  
		Last Modified: Thu, 23 Mar 2023 07:22:22 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1fc3f02dfb5b2a49da78bed468a8760607fbf73b57bf5009e1782947fe8855c`  
		Last Modified: Thu, 23 Mar 2023 07:22:24 GMT  
		Size: 39.0 MB (39029258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7442e502d15f1a588b3ff55118e637a9a8b42e98c424492b800454aecd8b113`  
		Last Modified: Thu, 23 Mar 2023 07:22:20 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c6a3c93062d6f0dc73fac47a397eae854a2bcdf5b1143fc684dbf93f8951c5`  
		Last Modified: Thu, 23 Mar 2023 07:22:20 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a03c1aa1eaf7dce756cddd74fe9f1a465d16d5a609abd477cf79a61cea71c5e`  
		Last Modified: Thu, 23 Mar 2023 07:22:20 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070ca35370089cfad095bbe4fe09b48f119a1203ae0d3ded1cb0aaa96b7b440e`  
		Last Modified: Thu, 23 Mar 2023 07:22:20 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3.1`

```console
$ docker pull couchdb@sha256:51463aea58b86f23e62c9022ba23001d952583fae86d824d648aac612b5b581c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:d897124cc1fb7c2b6e587c51fef80759ac6b60e2b314a9ea20b7621bb0335ab8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84539097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1625a43dc510f1cd112d2299cefa16d76d4a47efac07dcc357b4c2a51edc140`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:50 GMT
ADD file:52316aa7d631242cd16337be337e57187ef07d3965e6284321fbdcd5b4f92b64 in / 
# Thu, 23 Mar 2023 01:30:51 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:14:14 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 23 Mar 2023 06:14:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 23 Mar 2023 06:14:22 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:14:26 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 23 Mar 2023 06:14:26 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 23 Mar 2023 06:14:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:14:54 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Thu, 23 Mar 2023 06:14:55 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 23 Mar 2023 06:15:12 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 23 Mar 2023 06:15:12 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Thu, 23 Mar 2023 06:15:12 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 23 Mar 2023 06:15:12 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Thu, 23 Mar 2023 06:15:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 06:15:13 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 06:15:13 GMT
VOLUME [/opt/couchdb/data]
# Thu, 23 Mar 2023 06:15:13 GMT
EXPOSE 4369 5984 9100
# Thu, 23 Mar 2023 06:15:13 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:3689b8de819b48387712c6d4d62d26a52a04c9e88afc68fb9d1dbe48bfa9e21d`  
		Last Modified: Thu, 23 Mar 2023 01:35:01 GMT  
		Size: 27.1 MB (27139869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07228e786e9fcae89eb2cc59a0752d290f19a708f0296ba7c17d1a55a4a80243`  
		Last Modified: Thu, 23 Mar 2023 06:16:03 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4700a153729c2edb362e307d55407cfeca29dc1d2e309a9c41e60a5edf2ee909`  
		Last Modified: Thu, 23 Mar 2023 06:16:02 GMT  
		Size: 6.7 MB (6705910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48402339fa56c0ac77cffd1a404f50aa8baee7a84f48d4ac30ad21dbe244bb60`  
		Last Modified: Thu, 23 Mar 2023 06:16:01 GMT  
		Size: 1.3 MB (1259595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de61bdb3ed274c78ebcd762fd00ffafeb1800d4f89ac1935ed0c5c0112738a9`  
		Last Modified: Thu, 23 Mar 2023 06:16:01 GMT  
		Size: 294.3 KB (294308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09828b0ad787ccc70ab5384663a5eebfb0de21879e3744086a981944399af163`  
		Last Modified: Thu, 23 Mar 2023 06:16:15 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9456a91d45977c57d79bfeae0b01294cc8a90da7508a632d733875832ae9796`  
		Last Modified: Thu, 23 Mar 2023 06:16:19 GMT  
		Size: 49.1 MB (49132402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14cbb10181487d791c698ef0220b9e934c3526d9b28d496ae841b0ab75589b2`  
		Last Modified: Thu, 23 Mar 2023 06:16:13 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a4afcb05d9a4b703dfb73eebdfd5e7b719323bdccbaf0006630697f59b4546`  
		Last Modified: Thu, 23 Mar 2023 06:16:13 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c74fc0a87059073c5f4204dea243c2c84fd2d3de6f1b7051dfa8b9ac5493585`  
		Last Modified: Thu, 23 Mar 2023 06:16:13 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b293d5f0522e749edbf4cf9cd8b9d118b16f2fc1224f0f0f69b07d01b1d337c`  
		Last Modified: Thu, 23 Mar 2023 06:16:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:f26338905cfef82b1c3b98668815faee16df60e1f1cfbcbcb01bf23c38df8f13
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72997052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:378ddae722d95218e9ea965ba00c139fd30a0cf3b1287d69075be9f43dfadf8c`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:23 GMT
ADD file:44e400cc6a1bc5df5a57bda478c9accf9b58950fa2fd069cc7620128fe786770 in / 
# Thu, 23 Mar 2023 00:45:23 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:20:41 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 23 Mar 2023 07:20:42 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 23 Mar 2023 07:20:48 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:20:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 23 Mar 2023 07:20:52 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 23 Mar 2023 07:20:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:21:14 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Thu, 23 Mar 2023 07:21:15 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 23 Mar 2023 07:21:26 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 23 Mar 2023 07:21:26 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Thu, 23 Mar 2023 07:21:26 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 23 Mar 2023 07:21:26 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Thu, 23 Mar 2023 07:21:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 07:21:27 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 07:21:27 GMT
VOLUME [/opt/couchdb/data]
# Thu, 23 Mar 2023 07:21:27 GMT
EXPOSE 4369 5984 9100
# Thu, 23 Mar 2023 07:21:27 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:cfe0f778e53ce031ef449bc02975a07f2568716dea807ed2f390d352c0001972`  
		Last Modified: Thu, 23 Mar 2023 00:48:45 GMT  
		Size: 25.9 MB (25922660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037538668954fe82bbe2e635a631e36780ef15998a07b238b91da1991b30abed`  
		Last Modified: Thu, 23 Mar 2023 07:22:12 GMT  
		Size: 3.4 KB (3434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b0009f03b4cc05f74eb4b4bd8ab0ebafc260f3f74d25ba8fc8f089a108b9c55`  
		Last Modified: Thu, 23 Mar 2023 07:22:11 GMT  
		Size: 6.6 MB (6579451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f1f9f14a5ccaec42852a7b41044e85fb849ec6d2b8b4d52b627f88a8664c86`  
		Last Modified: Thu, 23 Mar 2023 07:22:10 GMT  
		Size: 1.2 MB (1164523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68f0b4ec14b9eaedd46f27ebe44d30eb877b71e65c14c22d90f46cf6a92f9eb`  
		Last Modified: Thu, 23 Mar 2023 07:22:10 GMT  
		Size: 294.1 KB (294127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581e7873e9d1cff45cfe0b6a81f0ae2eeaeeacc57e5daaf3b84a361852e89b9e`  
		Last Modified: Thu, 23 Mar 2023 07:22:22 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1fc3f02dfb5b2a49da78bed468a8760607fbf73b57bf5009e1782947fe8855c`  
		Last Modified: Thu, 23 Mar 2023 07:22:24 GMT  
		Size: 39.0 MB (39029258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7442e502d15f1a588b3ff55118e637a9a8b42e98c424492b800454aecd8b113`  
		Last Modified: Thu, 23 Mar 2023 07:22:20 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c6a3c93062d6f0dc73fac47a397eae854a2bcdf5b1143fc684dbf93f8951c5`  
		Last Modified: Thu, 23 Mar 2023 07:22:20 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a03c1aa1eaf7dce756cddd74fe9f1a465d16d5a609abd477cf79a61cea71c5e`  
		Last Modified: Thu, 23 Mar 2023 07:22:20 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070ca35370089cfad095bbe4fe09b48f119a1203ae0d3ded1cb0aaa96b7b440e`  
		Last Modified: Thu, 23 Mar 2023 07:22:20 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3`

```console
$ docker pull couchdb@sha256:8ce476fe6b8b35ce832975e5d939b549bac95758180c67a8e8e8c6865f742086
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3` - linux; amd64

```console
$ docker pull couchdb@sha256:942b2819b96e3cad608505e0d8b61c214458eaceb385af57c257ca6f69f1c300
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90222373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c0e30e9019e2508b12ee524ce325482a6fd58d3c6a0fdc9ea99b2d337e8e52a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:13:24 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 23 Mar 2023 06:13:24 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 23 Mar 2023 06:13:31 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:13:34 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Thu, 23 Mar 2023 06:13:34 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 23 Mar 2023 06:13:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:13:39 GMT
ENV COUCHDB_VERSION=3.3.1
# Thu, 23 Mar 2023 06:13:40 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 23 Mar 2023 06:13:52 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 23 Mar 2023 06:13:52 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 23 Mar 2023 06:13:52 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 28 Mar 2023 21:19:31 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 28 Mar 2023 21:19:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 28 Mar 2023 21:19:31 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 28 Mar 2023 21:19:31 GMT
VOLUME [/opt/couchdb/data]
# Tue, 28 Mar 2023 21:19:32 GMT
EXPOSE 4369 5984 9100
# Tue, 28 Mar 2023 21:19:32 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba7ecd554a3d4cf20e4ee469e50a84ca5ead219a9332ac2c6513b786ab45a20`  
		Last Modified: Thu, 23 Mar 2023 06:15:32 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf01ea1c10cd75a87cff41983af228c45207a118df39f5dd2acb35eb6e18493`  
		Last Modified: Thu, 23 Mar 2023 06:15:31 GMT  
		Size: 5.2 MB (5224316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1fbbca32dec7f4366b57f47aacb4a53e29dd34d19a1d2669ad8af5d98124f7f`  
		Last Modified: Thu, 23 Mar 2023 06:15:30 GMT  
		Size: 610.2 KB (610176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e4e83c342a4a54e132a73b8675b297b02519b678488148700ffa6a3170b6c3`  
		Last Modified: Thu, 23 Mar 2023 06:15:30 GMT  
		Size: 294.3 KB (294302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ccd3165750d901110930a16292f5edaba6dd5399dec993874714e8f23c1f50`  
		Last Modified: Thu, 23 Mar 2023 06:15:30 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed541acd6911a891764e6cdc4031f6f68a387f76a1f5a5878e152debaafe714`  
		Last Modified: Thu, 23 Mar 2023 06:15:33 GMT  
		Size: 52.7 MB (52674763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf4cde9fd11e08968ce2cc685f120862e2d15da31b8168fb33c0c1ff434d48c`  
		Last Modified: Thu, 23 Mar 2023 06:15:28 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de559f5eb2fdb1986baf60340fd174b8acb2c179d27512a14469a241159f7d3`  
		Last Modified: Thu, 23 Mar 2023 06:15:28 GMT  
		Size: 999.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359fb838be8a71de551cb09fc37132882b763aa0ea031c05b6d7338781393237`  
		Last Modified: Tue, 28 Mar 2023 21:19:47 GMT  
		Size: 2.2 KB (2225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb77a1648ee0a099a1c369d785d5cd5352a58de70a8f0294bfcececafd759718`  
		Last Modified: Tue, 28 Mar 2023 21:19:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:4b60ada569d87db6ccc751c48c1af2b7fa32c104f63eb2d01a164ec3d0c76c46
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88670375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6be0e185d26400b7885515277bb9ccf533d0857fe9229ec9ba5610a141630bcf`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:19:52 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 23 Mar 2023 07:19:53 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 23 Mar 2023 07:19:58 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:20:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Thu, 23 Mar 2023 07:20:01 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 23 Mar 2023 07:20:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:20:05 GMT
ENV COUCHDB_VERSION=3.3.1
# Thu, 23 Mar 2023 07:20:06 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 23 Mar 2023 07:20:18 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 23 Mar 2023 07:20:18 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 23 Mar 2023 07:20:18 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 28 Mar 2023 21:39:21 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 28 Mar 2023 21:39:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 28 Mar 2023 21:39:21 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 28 Mar 2023 21:39:21 GMT
VOLUME [/opt/couchdb/data]
# Tue, 28 Mar 2023 21:39:21 GMT
EXPOSE 4369 5984 9100
# Tue, 28 Mar 2023 21:39:21 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1618330853d06ff84cee3f0710edfa89620b7487477fe25b6b9b4c9b5aa6ecbb`  
		Last Modified: Thu, 23 Mar 2023 07:21:43 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25bf7f910cfd6147a589be1daa4d2747b9e79d4b1d620411cfa8b04f76fd78e6`  
		Last Modified: Thu, 23 Mar 2023 07:21:41 GMT  
		Size: 5.2 MB (5209441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8294faa460f96deaf9b020aa5d39f46693755c3e5d8e8e4021da77fd768966c`  
		Last Modified: Thu, 23 Mar 2023 07:21:41 GMT  
		Size: 566.2 KB (566228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99ddcc79770483aa72f62fe1c7042aa2e477e62db34074fbf35070ba0ce4d93`  
		Last Modified: Thu, 23 Mar 2023 07:21:41 GMT  
		Size: 294.3 KB (294251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b9d4aebd4a140d75fee1de8edabce6c8429a4598bdff86308bafb92d7d2722`  
		Last Modified: Thu, 23 Mar 2023 07:21:40 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bd5745764bcdb5b3c74099f609a4f68ed855974ce55b5f5c3e0999ddf36c12`  
		Last Modified: Thu, 23 Mar 2023 07:21:43 GMT  
		Size: 52.5 MB (52530318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea0a2deba7b340cab49bd537bf108fe1d34fd11b565d39b074edece47dddd8c`  
		Last Modified: Thu, 23 Mar 2023 07:21:39 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1132ca9468038cb38834f462df91e0b09daaf709a9b937bc51839654e94c7cdf`  
		Last Modified: Thu, 23 Mar 2023 07:21:39 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e6dda382f5b7956361954059b4221ebc90e5f87e2ebc7d06595856f820fdad`  
		Last Modified: Tue, 28 Mar 2023 21:39:34 GMT  
		Size: 2.2 KB (2223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc09b0172825078f89e56cb53b8b4244542b21acf87f46a1f8a84c6198671feb`  
		Last Modified: Tue, 28 Mar 2023 21:39:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; ppc64le

```console
$ docker pull couchdb@sha256:5e55ccae68b16be2f006024bd6fe20d7e360ecd3a593bdc58cbfa4d7890cd9d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.8 MB (95828939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0d438d66e59e61a0215d65cac76fc59d710d226a36ee012fd5515f21d0eaadd`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 23 Mar 2023 01:19:48 GMT
ADD file:fbd36b7667327dd30171fc49b8e028b8371fdbc7d30ee673808d508557f78bf1 in / 
# Thu, 23 Mar 2023 01:19:49 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:28:20 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 23 Mar 2023 13:28:21 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 23 Mar 2023 13:28:39 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:28:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Thu, 23 Mar 2023 13:28:46 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 23 Mar 2023 13:28:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:28:57 GMT
ENV COUCHDB_VERSION=3.3.1
# Thu, 23 Mar 2023 13:28:58 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 23 Mar 2023 13:29:21 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 23 Mar 2023 13:29:23 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 23 Mar 2023 13:29:23 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 28 Mar 2023 22:16:24 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 28 Mar 2023 22:16:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 28 Mar 2023 22:16:25 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 28 Mar 2023 22:16:25 GMT
VOLUME [/opt/couchdb/data]
# Tue, 28 Mar 2023 22:16:26 GMT
EXPOSE 4369 5984 9100
# Tue, 28 Mar 2023 22:16:26 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:8f472ad0a3fa58b4e304d1a974f25615d5bd3b7a99dff9c8202bd30facef0155`  
		Last Modified: Thu, 23 Mar 2023 01:24:22 GMT  
		Size: 35.3 MB (35288050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5c7bf4c8ed82b56f645f6dd5aef795b2ebaf5ad9b12975fd4dc50d3b628832`  
		Last Modified: Thu, 23 Mar 2023 13:30:19 GMT  
		Size: 3.4 KB (3407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5bb5aa4fc53a24f4d3c36f1ec2657044eb895eafc16d3f2d40984403310d682`  
		Last Modified: Thu, 23 Mar 2023 13:30:19 GMT  
		Size: 6.0 MB (6043906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593ab4aa61259780aec8601aa2e5cb0d1890c9fb72572f36731ca410c39ed987`  
		Last Modified: Thu, 23 Mar 2023 13:30:17 GMT  
		Size: 662.0 KB (661975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98e8db79171155dcffbbda14008a110076ea43e1558c06b12047967e48ce9b7`  
		Last Modified: Thu, 23 Mar 2023 13:30:17 GMT  
		Size: 294.2 KB (294213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7edda1bfbb4044153d412476d8d1c3e0ec7e5b7c37abc6bae358c21d80f4c8ca`  
		Last Modified: Thu, 23 Mar 2023 13:30:17 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84d062db9934f420046117f415d6341c3456e5c410555dbfcbf6b2e0f7921cc`  
		Last Modified: Thu, 23 Mar 2023 13:30:24 GMT  
		Size: 53.5 MB (53533380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f78e4dc952cdcc9c77fe3044eea84c6dba34374cda602d50ec9ece0d6a55913`  
		Last Modified: Thu, 23 Mar 2023 13:30:15 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6fa201c8642622fbd3a9430eab8b6e769c4fd523830e5ef0f34f786f6c1b01`  
		Last Modified: Thu, 23 Mar 2023 13:30:15 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bccd1544b83d012a35e53196df3b474db7c88911964af7648fdb7c520803aa9`  
		Last Modified: Tue, 28 Mar 2023 22:16:41 GMT  
		Size: 2.2 KB (2228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b1dd1214b7c873d5119e167b6674ff08970c879fb33604314e473a5b80833f`  
		Last Modified: Tue, 28 Mar 2023 22:16:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1`

```console
$ docker pull couchdb@sha256:66bac7903a4e17db3649a18f332cd65df484307ae02487639421f704fa27c9ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:9c5bed9e161a88706babbb6b04305dc1be2a4551c9c7059315679d4f0da4b237
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80025811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a09f029450e820442e63986cb2d110c20018ff0d68db3a45cfbe713b53398e90`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:50 GMT
ADD file:52316aa7d631242cd16337be337e57187ef07d3965e6284321fbdcd5b4f92b64 in / 
# Thu, 23 Mar 2023 01:30:51 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:14:14 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 23 Mar 2023 06:14:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 23 Mar 2023 06:14:22 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:14:26 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 23 Mar 2023 06:14:26 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 23 Mar 2023 06:14:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:14:32 GMT
ENV COUCHDB_VERSION=3.1.2
# Thu, 23 Mar 2023 06:14:32 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 23 Mar 2023 06:14:46 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 23 Mar 2023 06:14:46 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 23 Mar 2023 06:14:46 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 23 Mar 2023 06:14:46 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Thu, 23 Mar 2023 06:14:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 06:14:47 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 06:14:47 GMT
VOLUME [/opt/couchdb/data]
# Thu, 23 Mar 2023 06:14:47 GMT
EXPOSE 4369 5984 9100
# Thu, 23 Mar 2023 06:14:47 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:3689b8de819b48387712c6d4d62d26a52a04c9e88afc68fb9d1dbe48bfa9e21d`  
		Last Modified: Thu, 23 Mar 2023 01:35:01 GMT  
		Size: 27.1 MB (27139869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07228e786e9fcae89eb2cc59a0752d290f19a708f0296ba7c17d1a55a4a80243`  
		Last Modified: Thu, 23 Mar 2023 06:16:03 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4700a153729c2edb362e307d55407cfeca29dc1d2e309a9c41e60a5edf2ee909`  
		Last Modified: Thu, 23 Mar 2023 06:16:02 GMT  
		Size: 6.7 MB (6705910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48402339fa56c0ac77cffd1a404f50aa8baee7a84f48d4ac30ad21dbe244bb60`  
		Last Modified: Thu, 23 Mar 2023 06:16:01 GMT  
		Size: 1.3 MB (1259595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de61bdb3ed274c78ebcd762fd00ffafeb1800d4f89ac1935ed0c5c0112738a9`  
		Last Modified: Thu, 23 Mar 2023 06:16:01 GMT  
		Size: 294.3 KB (294308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc989df998f70f4b181efedbff884c927a37b61f2e44a67b1403f6f643aa2650`  
		Last Modified: Thu, 23 Mar 2023 06:16:01 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad9087ae5138e25ea489e43561567a6903006d0d2bbedb7cab959681a3e25b1`  
		Last Modified: Thu, 23 Mar 2023 06:16:04 GMT  
		Size: 44.6 MB (44619123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f067b5db26ceb60ab48b562e0834a9cbf0aa2c746ca41a6d3534c3d2ace501`  
		Last Modified: Thu, 23 Mar 2023 06:15:59 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce279f4cea7576f92970a6e870f623baeef904de274580e19ee5706ff0aa59f`  
		Last Modified: Thu, 23 Mar 2023 06:15:59 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba3d851e93a6d9c0ee745e88f6a5ccfd028406bf228c7c39b96103c63bca773`  
		Last Modified: Thu, 23 Mar 2023 06:15:59 GMT  
		Size: 2.1 KB (2056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf524db70ed0600990e1e8d18aa195e77ff6bb8750df7ae06abb44ef40663715`  
		Last Modified: Thu, 23 Mar 2023 06:15:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:d2218d2668f3102cff159f42b6c3950e48e7f6a6703abdb850352c0d0459afdc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75093199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:328d05b24191f0e2ae8050f3f2e7f3f334f4c023d05446445799d0971edffa57`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:23 GMT
ADD file:44e400cc6a1bc5df5a57bda478c9accf9b58950fa2fd069cc7620128fe786770 in / 
# Thu, 23 Mar 2023 00:45:23 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:20:41 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 23 Mar 2023 07:20:42 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 23 Mar 2023 07:20:48 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:20:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 23 Mar 2023 07:20:52 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 23 Mar 2023 07:20:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:20:58 GMT
ENV COUCHDB_VERSION=3.1.2
# Thu, 23 Mar 2023 07:20:58 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 23 Mar 2023 07:21:10 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 23 Mar 2023 07:21:10 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 23 Mar 2023 07:21:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 23 Mar 2023 07:21:10 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Thu, 23 Mar 2023 07:21:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 07:21:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 07:21:11 GMT
VOLUME [/opt/couchdb/data]
# Thu, 23 Mar 2023 07:21:11 GMT
EXPOSE 4369 5984 9100
# Thu, 23 Mar 2023 07:21:11 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:cfe0f778e53ce031ef449bc02975a07f2568716dea807ed2f390d352c0001972`  
		Last Modified: Thu, 23 Mar 2023 00:48:45 GMT  
		Size: 25.9 MB (25922660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037538668954fe82bbe2e635a631e36780ef15998a07b238b91da1991b30abed`  
		Last Modified: Thu, 23 Mar 2023 07:22:12 GMT  
		Size: 3.4 KB (3434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b0009f03b4cc05f74eb4b4bd8ab0ebafc260f3f74d25ba8fc8f089a108b9c55`  
		Last Modified: Thu, 23 Mar 2023 07:22:11 GMT  
		Size: 6.6 MB (6579451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f1f9f14a5ccaec42852a7b41044e85fb849ec6d2b8b4d52b627f88a8664c86`  
		Last Modified: Thu, 23 Mar 2023 07:22:10 GMT  
		Size: 1.2 MB (1164523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68f0b4ec14b9eaedd46f27ebe44d30eb877b71e65c14c22d90f46cf6a92f9eb`  
		Last Modified: Thu, 23 Mar 2023 07:22:10 GMT  
		Size: 294.1 KB (294127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c3bc8ab1cb6dd3df30ad663b38dd0bf15bb45653f69d587bd30620cb2bf1781`  
		Last Modified: Thu, 23 Mar 2023 07:22:10 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f213dc01a57c4684c8443611e45420e204519aa5336c966132ac21ae499a1cf`  
		Last Modified: Thu, 23 Mar 2023 07:22:12 GMT  
		Size: 41.1 MB (41125407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5783f48edf7f1498f333b97edab202bfebe078b3e44b08121ce74da0708187ca`  
		Last Modified: Thu, 23 Mar 2023 07:22:08 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6f21d8a360504d33f65cbb6ab98b48921cdcd25c611c0b4a8dc00b183204e4`  
		Last Modified: Thu, 23 Mar 2023 07:22:08 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792aa638de99e4c85b519761e3bcb6a6136a7a89b03e87d0cc3e93104e45f6e0`  
		Last Modified: Thu, 23 Mar 2023 07:22:08 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a7a1c08ea0f3572b745d6f0c0e1b29e2d3469979e33b2f5145209b5e80300c`  
		Last Modified: Thu, 23 Mar 2023 07:22:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1.2`

```console
$ docker pull couchdb@sha256:66bac7903a4e17db3649a18f332cd65df484307ae02487639421f704fa27c9ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1.2` - linux; amd64

```console
$ docker pull couchdb@sha256:9c5bed9e161a88706babbb6b04305dc1be2a4551c9c7059315679d4f0da4b237
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80025811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a09f029450e820442e63986cb2d110c20018ff0d68db3a45cfbe713b53398e90`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:50 GMT
ADD file:52316aa7d631242cd16337be337e57187ef07d3965e6284321fbdcd5b4f92b64 in / 
# Thu, 23 Mar 2023 01:30:51 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:14:14 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 23 Mar 2023 06:14:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 23 Mar 2023 06:14:22 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:14:26 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 23 Mar 2023 06:14:26 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 23 Mar 2023 06:14:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:14:32 GMT
ENV COUCHDB_VERSION=3.1.2
# Thu, 23 Mar 2023 06:14:32 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 23 Mar 2023 06:14:46 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 23 Mar 2023 06:14:46 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 23 Mar 2023 06:14:46 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 23 Mar 2023 06:14:46 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Thu, 23 Mar 2023 06:14:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 06:14:47 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 06:14:47 GMT
VOLUME [/opt/couchdb/data]
# Thu, 23 Mar 2023 06:14:47 GMT
EXPOSE 4369 5984 9100
# Thu, 23 Mar 2023 06:14:47 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:3689b8de819b48387712c6d4d62d26a52a04c9e88afc68fb9d1dbe48bfa9e21d`  
		Last Modified: Thu, 23 Mar 2023 01:35:01 GMT  
		Size: 27.1 MB (27139869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07228e786e9fcae89eb2cc59a0752d290f19a708f0296ba7c17d1a55a4a80243`  
		Last Modified: Thu, 23 Mar 2023 06:16:03 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4700a153729c2edb362e307d55407cfeca29dc1d2e309a9c41e60a5edf2ee909`  
		Last Modified: Thu, 23 Mar 2023 06:16:02 GMT  
		Size: 6.7 MB (6705910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48402339fa56c0ac77cffd1a404f50aa8baee7a84f48d4ac30ad21dbe244bb60`  
		Last Modified: Thu, 23 Mar 2023 06:16:01 GMT  
		Size: 1.3 MB (1259595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de61bdb3ed274c78ebcd762fd00ffafeb1800d4f89ac1935ed0c5c0112738a9`  
		Last Modified: Thu, 23 Mar 2023 06:16:01 GMT  
		Size: 294.3 KB (294308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc989df998f70f4b181efedbff884c927a37b61f2e44a67b1403f6f643aa2650`  
		Last Modified: Thu, 23 Mar 2023 06:16:01 GMT  
		Size: 273.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad9087ae5138e25ea489e43561567a6903006d0d2bbedb7cab959681a3e25b1`  
		Last Modified: Thu, 23 Mar 2023 06:16:04 GMT  
		Size: 44.6 MB (44619123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f067b5db26ceb60ab48b562e0834a9cbf0aa2c746ca41a6d3534c3d2ace501`  
		Last Modified: Thu, 23 Mar 2023 06:15:59 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce279f4cea7576f92970a6e870f623baeef904de274580e19ee5706ff0aa59f`  
		Last Modified: Thu, 23 Mar 2023 06:15:59 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba3d851e93a6d9c0ee745e88f6a5ccfd028406bf228c7c39b96103c63bca773`  
		Last Modified: Thu, 23 Mar 2023 06:15:59 GMT  
		Size: 2.1 KB (2056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf524db70ed0600990e1e8d18aa195e77ff6bb8750df7ae06abb44ef40663715`  
		Last Modified: Thu, 23 Mar 2023 06:15:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:d2218d2668f3102cff159f42b6c3950e48e7f6a6703abdb850352c0d0459afdc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75093199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:328d05b24191f0e2ae8050f3f2e7f3f334f4c023d05446445799d0971edffa57`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:23 GMT
ADD file:44e400cc6a1bc5df5a57bda478c9accf9b58950fa2fd069cc7620128fe786770 in / 
# Thu, 23 Mar 2023 00:45:23 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:20:41 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 23 Mar 2023 07:20:42 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 23 Mar 2023 07:20:48 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:20:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 23 Mar 2023 07:20:52 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 23 Mar 2023 07:20:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:20:58 GMT
ENV COUCHDB_VERSION=3.1.2
# Thu, 23 Mar 2023 07:20:58 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 23 Mar 2023 07:21:10 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 23 Mar 2023 07:21:10 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 23 Mar 2023 07:21:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 23 Mar 2023 07:21:10 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Thu, 23 Mar 2023 07:21:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 07:21:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 07:21:11 GMT
VOLUME [/opt/couchdb/data]
# Thu, 23 Mar 2023 07:21:11 GMT
EXPOSE 4369 5984 9100
# Thu, 23 Mar 2023 07:21:11 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:cfe0f778e53ce031ef449bc02975a07f2568716dea807ed2f390d352c0001972`  
		Last Modified: Thu, 23 Mar 2023 00:48:45 GMT  
		Size: 25.9 MB (25922660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:037538668954fe82bbe2e635a631e36780ef15998a07b238b91da1991b30abed`  
		Last Modified: Thu, 23 Mar 2023 07:22:12 GMT  
		Size: 3.4 KB (3434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b0009f03b4cc05f74eb4b4bd8ab0ebafc260f3f74d25ba8fc8f089a108b9c55`  
		Last Modified: Thu, 23 Mar 2023 07:22:11 GMT  
		Size: 6.6 MB (6579451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f1f9f14a5ccaec42852a7b41044e85fb849ec6d2b8b4d52b627f88a8664c86`  
		Last Modified: Thu, 23 Mar 2023 07:22:10 GMT  
		Size: 1.2 MB (1164523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68f0b4ec14b9eaedd46f27ebe44d30eb877b71e65c14c22d90f46cf6a92f9eb`  
		Last Modified: Thu, 23 Mar 2023 07:22:10 GMT  
		Size: 294.1 KB (294127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c3bc8ab1cb6dd3df30ad663b38dd0bf15bb45653f69d587bd30620cb2bf1781`  
		Last Modified: Thu, 23 Mar 2023 07:22:10 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f213dc01a57c4684c8443611e45420e204519aa5336c966132ac21ae499a1cf`  
		Last Modified: Thu, 23 Mar 2023 07:22:12 GMT  
		Size: 41.1 MB (41125407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5783f48edf7f1498f333b97edab202bfebe078b3e44b08121ce74da0708187ca`  
		Last Modified: Thu, 23 Mar 2023 07:22:08 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6f21d8a360504d33f65cbb6ab98b48921cdcd25c611c0b4a8dc00b183204e4`  
		Last Modified: Thu, 23 Mar 2023 07:22:08 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792aa638de99e4c85b519761e3bcb6a6136a7a89b03e87d0cc3e93104e45f6e0`  
		Last Modified: Thu, 23 Mar 2023 07:22:08 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a7a1c08ea0f3572b745d6f0c0e1b29e2d3469979e33b2f5145209b5e80300c`  
		Last Modified: Thu, 23 Mar 2023 07:22:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2`

```console
$ docker pull couchdb@sha256:bd22ac9ed0ef5da920d8acfa5287bdce9a93698dfa3368fb70227e940d845325
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2` - linux; amd64

```console
$ docker pull couchdb@sha256:f0bfde87b296fe0c4a08b769e4a5cfcfb79d72d010fb34609d632e9193c78644
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.6 MB (86593039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56293d86c0da0bc7ce91e25e6d5def18bcb66338fc94c6bea5f659a4dffe5675`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:13:24 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 23 Mar 2023 06:13:24 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 23 Mar 2023 06:13:31 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:13:34 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Thu, 23 Mar 2023 06:13:34 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 23 Mar 2023 06:13:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:13:57 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Thu, 23 Mar 2023 06:13:58 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 23 Mar 2023 06:14:10 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 23 Mar 2023 06:14:11 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 23 Mar 2023 06:14:11 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 28 Mar 2023 21:19:34 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 28 Mar 2023 21:19:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 28 Mar 2023 21:19:34 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 28 Mar 2023 21:19:34 GMT
VOLUME [/opt/couchdb/data]
# Tue, 28 Mar 2023 21:19:35 GMT
EXPOSE 4369 5984 9100
# Tue, 28 Mar 2023 21:19:35 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba7ecd554a3d4cf20e4ee469e50a84ca5ead219a9332ac2c6513b786ab45a20`  
		Last Modified: Thu, 23 Mar 2023 06:15:32 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf01ea1c10cd75a87cff41983af228c45207a118df39f5dd2acb35eb6e18493`  
		Last Modified: Thu, 23 Mar 2023 06:15:31 GMT  
		Size: 5.2 MB (5224316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1fbbca32dec7f4366b57f47aacb4a53e29dd34d19a1d2669ad8af5d98124f7f`  
		Last Modified: Thu, 23 Mar 2023 06:15:30 GMT  
		Size: 610.2 KB (610176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e4e83c342a4a54e132a73b8675b297b02519b678488148700ffa6a3170b6c3`  
		Last Modified: Thu, 23 Mar 2023 06:15:30 GMT  
		Size: 294.3 KB (294302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c190d42526db1adeac71872c6efdbd5d33ac9907a879368f2f6fc0def35cf6cd`  
		Last Modified: Thu, 23 Mar 2023 06:15:47 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba016658688dbcc8ce8b661ec904f4196537c4a93cfa327bb3f2d183af231f4`  
		Last Modified: Thu, 23 Mar 2023 06:15:51 GMT  
		Size: 49.0 MB (49045663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c805b0b636b68aa4d1c54b968b28cd1f33d2cb669aedf9fb10b5b7f4acf567`  
		Last Modified: Thu, 23 Mar 2023 06:15:46 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500ad38b9405ea121550439060b2dfff766da4be801a6b4a79873a5d66b3de83`  
		Last Modified: Thu, 23 Mar 2023 06:15:46 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20c4bc235a576b723cd9b17a707410685a24d101dd7c86d2e2ea1f574bd3fe9`  
		Last Modified: Tue, 28 Mar 2023 21:20:00 GMT  
		Size: 2.2 KB (2224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81170392a105a90d578d538a202454ce5286b8e25ea0683ac2f464f8bff1aa0b`  
		Last Modified: Tue, 28 Mar 2023 21:20:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:e86c65a957306bdb13f3636f1bc70655c9f9d0dc56ac8bd5727a793131a04e0b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.2 MB (85203833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e8bb1ca56a113727707d0ba7bba040eb2fc26e95e7597b3dec1d80c623a1d62`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:19:52 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 23 Mar 2023 07:19:53 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 23 Mar 2023 07:19:58 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:20:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Thu, 23 Mar 2023 07:20:01 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 23 Mar 2023 07:20:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:20:25 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Thu, 23 Mar 2023 07:20:26 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 23 Mar 2023 07:20:37 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 23 Mar 2023 07:20:37 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 23 Mar 2023 07:20:37 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 28 Mar 2023 21:39:23 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 28 Mar 2023 21:39:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 28 Mar 2023 21:39:24 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 28 Mar 2023 21:39:24 GMT
VOLUME [/opt/couchdb/data]
# Tue, 28 Mar 2023 21:39:24 GMT
EXPOSE 4369 5984 9100
# Tue, 28 Mar 2023 21:39:24 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1618330853d06ff84cee3f0710edfa89620b7487477fe25b6b9b4c9b5aa6ecbb`  
		Last Modified: Thu, 23 Mar 2023 07:21:43 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25bf7f910cfd6147a589be1daa4d2747b9e79d4b1d620411cfa8b04f76fd78e6`  
		Last Modified: Thu, 23 Mar 2023 07:21:41 GMT  
		Size: 5.2 MB (5209441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8294faa460f96deaf9b020aa5d39f46693755c3e5d8e8e4021da77fd768966c`  
		Last Modified: Thu, 23 Mar 2023 07:21:41 GMT  
		Size: 566.2 KB (566228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99ddcc79770483aa72f62fe1c7042aa2e477e62db34074fbf35070ba0ce4d93`  
		Last Modified: Thu, 23 Mar 2023 07:21:41 GMT  
		Size: 294.3 KB (294251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519ee759a9efc18188816d60f574ea263fabc1529440688a1e0bb26f3a181d9c`  
		Last Modified: Thu, 23 Mar 2023 07:21:57 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1281cea07657fd3a32491b45ebed78f3e6008492d3131d3df13575ebe98ab771`  
		Last Modified: Thu, 23 Mar 2023 07:22:00 GMT  
		Size: 49.1 MB (49064012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4006b8c513aa04e257e8e39e1bd3c2c8fc0613d3d61ef75c5c0c1974f994ff6b`  
		Last Modified: Thu, 23 Mar 2023 07:21:55 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25aac636e6f113c12ec6590d89f5eb9dab32b9035e543ad77515d156a853a3a4`  
		Last Modified: Thu, 23 Mar 2023 07:21:56 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759a56af3f0fb0b101eea0b72ab6724d3252eea1522e91685a3cb85ccdab59a6`  
		Last Modified: Tue, 28 Mar 2023 21:39:46 GMT  
		Size: 2.2 KB (2224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe12680c687dc266c8573bdbd53931c5249e0ca40a3b3c7f36bf256dacddbfc`  
		Last Modified: Tue, 28 Mar 2023 21:39:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; ppc64le

```console
$ docker pull couchdb@sha256:df3a80841cffeba37a76e6b58e83b9be2c60dc8366ca4dd0095721dcdee1c1da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.4 MB (92380030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33ced65e491079a85581d0214cf7a25d61bf731fe67e242a43dc05ba8bd4738e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 23 Mar 2023 01:19:48 GMT
ADD file:fbd36b7667327dd30171fc49b8e028b8371fdbc7d30ee673808d508557f78bf1 in / 
# Thu, 23 Mar 2023 01:19:49 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:28:20 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 23 Mar 2023 13:28:21 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 23 Mar 2023 13:28:39 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:28:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Thu, 23 Mar 2023 13:28:46 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 23 Mar 2023 13:28:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:29:30 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Thu, 23 Mar 2023 13:29:31 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 23 Mar 2023 13:29:55 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 23 Mar 2023 13:29:57 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 23 Mar 2023 13:29:57 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 28 Mar 2023 22:16:29 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 28 Mar 2023 22:16:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 28 Mar 2023 22:16:30 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 28 Mar 2023 22:16:30 GMT
VOLUME [/opt/couchdb/data]
# Tue, 28 Mar 2023 22:16:31 GMT
EXPOSE 4369 5984 9100
# Tue, 28 Mar 2023 22:16:31 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:8f472ad0a3fa58b4e304d1a974f25615d5bd3b7a99dff9c8202bd30facef0155`  
		Last Modified: Thu, 23 Mar 2023 01:24:22 GMT  
		Size: 35.3 MB (35288050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5c7bf4c8ed82b56f645f6dd5aef795b2ebaf5ad9b12975fd4dc50d3b628832`  
		Last Modified: Thu, 23 Mar 2023 13:30:19 GMT  
		Size: 3.4 KB (3407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5bb5aa4fc53a24f4d3c36f1ec2657044eb895eafc16d3f2d40984403310d682`  
		Last Modified: Thu, 23 Mar 2023 13:30:19 GMT  
		Size: 6.0 MB (6043906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593ab4aa61259780aec8601aa2e5cb0d1890c9fb72572f36731ca410c39ed987`  
		Last Modified: Thu, 23 Mar 2023 13:30:17 GMT  
		Size: 662.0 KB (661975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98e8db79171155dcffbbda14008a110076ea43e1558c06b12047967e48ce9b7`  
		Last Modified: Thu, 23 Mar 2023 13:30:17 GMT  
		Size: 294.2 KB (294213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2380208f0bae22032b4af8ab358cb65c6fc3ca2c10cc881ffcf6ded31942bbe5`  
		Last Modified: Thu, 23 Mar 2023 13:30:40 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4493108391c1be8708baea3eb2098fea267aaf0b6af9241114522662d0ce50`  
		Last Modified: Thu, 23 Mar 2023 13:30:48 GMT  
		Size: 50.1 MB (50084709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c374cb46e5f6a6d7fe4e7ee28a22e99305cc209f54639278be2d94a231bb95`  
		Last Modified: Thu, 23 Mar 2023 13:30:38 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e6fabfacb5354b1a4e4e48f9bacb83d61c9cb50a5dba3cfb98f5f2735927aa`  
		Last Modified: Thu, 23 Mar 2023 13:30:38 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d192a8bbc09526b5389d24f2f8cdee3d4e608a51526cbb59822819ef27e2edd5`  
		Last Modified: Tue, 28 Mar 2023 22:16:55 GMT  
		Size: 2.2 KB (2227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49065007d8be6182686632cc059276bac1e7721fbfb18c5b8eac1b9feb8e7c16`  
		Last Modified: Tue, 28 Mar 2023 22:16:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2.2`

```console
$ docker pull couchdb@sha256:bd22ac9ed0ef5da920d8acfa5287bdce9a93698dfa3368fb70227e940d845325
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2.2` - linux; amd64

```console
$ docker pull couchdb@sha256:f0bfde87b296fe0c4a08b769e4a5cfcfb79d72d010fb34609d632e9193c78644
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.6 MB (86593039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56293d86c0da0bc7ce91e25e6d5def18bcb66338fc94c6bea5f659a4dffe5675`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:13:24 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 23 Mar 2023 06:13:24 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 23 Mar 2023 06:13:31 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:13:34 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Thu, 23 Mar 2023 06:13:34 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 23 Mar 2023 06:13:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:13:57 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Thu, 23 Mar 2023 06:13:58 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 23 Mar 2023 06:14:10 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 23 Mar 2023 06:14:11 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 23 Mar 2023 06:14:11 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 28 Mar 2023 21:19:34 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 28 Mar 2023 21:19:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 28 Mar 2023 21:19:34 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 28 Mar 2023 21:19:34 GMT
VOLUME [/opt/couchdb/data]
# Tue, 28 Mar 2023 21:19:35 GMT
EXPOSE 4369 5984 9100
# Tue, 28 Mar 2023 21:19:35 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba7ecd554a3d4cf20e4ee469e50a84ca5ead219a9332ac2c6513b786ab45a20`  
		Last Modified: Thu, 23 Mar 2023 06:15:32 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf01ea1c10cd75a87cff41983af228c45207a118df39f5dd2acb35eb6e18493`  
		Last Modified: Thu, 23 Mar 2023 06:15:31 GMT  
		Size: 5.2 MB (5224316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1fbbca32dec7f4366b57f47aacb4a53e29dd34d19a1d2669ad8af5d98124f7f`  
		Last Modified: Thu, 23 Mar 2023 06:15:30 GMT  
		Size: 610.2 KB (610176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e4e83c342a4a54e132a73b8675b297b02519b678488148700ffa6a3170b6c3`  
		Last Modified: Thu, 23 Mar 2023 06:15:30 GMT  
		Size: 294.3 KB (294302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c190d42526db1adeac71872c6efdbd5d33ac9907a879368f2f6fc0def35cf6cd`  
		Last Modified: Thu, 23 Mar 2023 06:15:47 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba016658688dbcc8ce8b661ec904f4196537c4a93cfa327bb3f2d183af231f4`  
		Last Modified: Thu, 23 Mar 2023 06:15:51 GMT  
		Size: 49.0 MB (49045663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c805b0b636b68aa4d1c54b968b28cd1f33d2cb669aedf9fb10b5b7f4acf567`  
		Last Modified: Thu, 23 Mar 2023 06:15:46 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500ad38b9405ea121550439060b2dfff766da4be801a6b4a79873a5d66b3de83`  
		Last Modified: Thu, 23 Mar 2023 06:15:46 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20c4bc235a576b723cd9b17a707410685a24d101dd7c86d2e2ea1f574bd3fe9`  
		Last Modified: Tue, 28 Mar 2023 21:20:00 GMT  
		Size: 2.2 KB (2224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81170392a105a90d578d538a202454ce5286b8e25ea0683ac2f464f8bff1aa0b`  
		Last Modified: Tue, 28 Mar 2023 21:20:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:e86c65a957306bdb13f3636f1bc70655c9f9d0dc56ac8bd5727a793131a04e0b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.2 MB (85203833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e8bb1ca56a113727707d0ba7bba040eb2fc26e95e7597b3dec1d80c623a1d62`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:19:52 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 23 Mar 2023 07:19:53 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 23 Mar 2023 07:19:58 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:20:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Thu, 23 Mar 2023 07:20:01 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 23 Mar 2023 07:20:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:20:25 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Thu, 23 Mar 2023 07:20:26 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 23 Mar 2023 07:20:37 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 23 Mar 2023 07:20:37 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 23 Mar 2023 07:20:37 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 28 Mar 2023 21:39:23 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 28 Mar 2023 21:39:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 28 Mar 2023 21:39:24 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 28 Mar 2023 21:39:24 GMT
VOLUME [/opt/couchdb/data]
# Tue, 28 Mar 2023 21:39:24 GMT
EXPOSE 4369 5984 9100
# Tue, 28 Mar 2023 21:39:24 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1618330853d06ff84cee3f0710edfa89620b7487477fe25b6b9b4c9b5aa6ecbb`  
		Last Modified: Thu, 23 Mar 2023 07:21:43 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25bf7f910cfd6147a589be1daa4d2747b9e79d4b1d620411cfa8b04f76fd78e6`  
		Last Modified: Thu, 23 Mar 2023 07:21:41 GMT  
		Size: 5.2 MB (5209441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8294faa460f96deaf9b020aa5d39f46693755c3e5d8e8e4021da77fd768966c`  
		Last Modified: Thu, 23 Mar 2023 07:21:41 GMT  
		Size: 566.2 KB (566228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99ddcc79770483aa72f62fe1c7042aa2e477e62db34074fbf35070ba0ce4d93`  
		Last Modified: Thu, 23 Mar 2023 07:21:41 GMT  
		Size: 294.3 KB (294251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519ee759a9efc18188816d60f574ea263fabc1529440688a1e0bb26f3a181d9c`  
		Last Modified: Thu, 23 Mar 2023 07:21:57 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1281cea07657fd3a32491b45ebed78f3e6008492d3131d3df13575ebe98ab771`  
		Last Modified: Thu, 23 Mar 2023 07:22:00 GMT  
		Size: 49.1 MB (49064012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4006b8c513aa04e257e8e39e1bd3c2c8fc0613d3d61ef75c5c0c1974f994ff6b`  
		Last Modified: Thu, 23 Mar 2023 07:21:55 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25aac636e6f113c12ec6590d89f5eb9dab32b9035e543ad77515d156a853a3a4`  
		Last Modified: Thu, 23 Mar 2023 07:21:56 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759a56af3f0fb0b101eea0b72ab6724d3252eea1522e91685a3cb85ccdab59a6`  
		Last Modified: Tue, 28 Mar 2023 21:39:46 GMT  
		Size: 2.2 KB (2224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe12680c687dc266c8573bdbd53931c5249e0ca40a3b3c7f36bf256dacddbfc`  
		Last Modified: Tue, 28 Mar 2023 21:39:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2.2` - linux; ppc64le

```console
$ docker pull couchdb@sha256:df3a80841cffeba37a76e6b58e83b9be2c60dc8366ca4dd0095721dcdee1c1da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.4 MB (92380030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33ced65e491079a85581d0214cf7a25d61bf731fe67e242a43dc05ba8bd4738e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 23 Mar 2023 01:19:48 GMT
ADD file:fbd36b7667327dd30171fc49b8e028b8371fdbc7d30ee673808d508557f78bf1 in / 
# Thu, 23 Mar 2023 01:19:49 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:28:20 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 23 Mar 2023 13:28:21 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 23 Mar 2023 13:28:39 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:28:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Thu, 23 Mar 2023 13:28:46 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 23 Mar 2023 13:28:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:29:30 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Thu, 23 Mar 2023 13:29:31 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 23 Mar 2023 13:29:55 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 23 Mar 2023 13:29:57 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 23 Mar 2023 13:29:57 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 28 Mar 2023 22:16:29 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 28 Mar 2023 22:16:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 28 Mar 2023 22:16:30 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 28 Mar 2023 22:16:30 GMT
VOLUME [/opt/couchdb/data]
# Tue, 28 Mar 2023 22:16:31 GMT
EXPOSE 4369 5984 9100
# Tue, 28 Mar 2023 22:16:31 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:8f472ad0a3fa58b4e304d1a974f25615d5bd3b7a99dff9c8202bd30facef0155`  
		Last Modified: Thu, 23 Mar 2023 01:24:22 GMT  
		Size: 35.3 MB (35288050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5c7bf4c8ed82b56f645f6dd5aef795b2ebaf5ad9b12975fd4dc50d3b628832`  
		Last Modified: Thu, 23 Mar 2023 13:30:19 GMT  
		Size: 3.4 KB (3407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5bb5aa4fc53a24f4d3c36f1ec2657044eb895eafc16d3f2d40984403310d682`  
		Last Modified: Thu, 23 Mar 2023 13:30:19 GMT  
		Size: 6.0 MB (6043906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593ab4aa61259780aec8601aa2e5cb0d1890c9fb72572f36731ca410c39ed987`  
		Last Modified: Thu, 23 Mar 2023 13:30:17 GMT  
		Size: 662.0 KB (661975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98e8db79171155dcffbbda14008a110076ea43e1558c06b12047967e48ce9b7`  
		Last Modified: Thu, 23 Mar 2023 13:30:17 GMT  
		Size: 294.2 KB (294213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2380208f0bae22032b4af8ab358cb65c6fc3ca2c10cc881ffcf6ded31942bbe5`  
		Last Modified: Thu, 23 Mar 2023 13:30:40 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4493108391c1be8708baea3eb2098fea267aaf0b6af9241114522662d0ce50`  
		Last Modified: Thu, 23 Mar 2023 13:30:48 GMT  
		Size: 50.1 MB (50084709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c374cb46e5f6a6d7fe4e7ee28a22e99305cc209f54639278be2d94a231bb95`  
		Last Modified: Thu, 23 Mar 2023 13:30:38 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e6fabfacb5354b1a4e4e48f9bacb83d61c9cb50a5dba3cfb98f5f2735927aa`  
		Last Modified: Thu, 23 Mar 2023 13:30:38 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d192a8bbc09526b5389d24f2f8cdee3d4e608a51526cbb59822819ef27e2edd5`  
		Last Modified: Tue, 28 Mar 2023 22:16:55 GMT  
		Size: 2.2 KB (2227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49065007d8be6182686632cc059276bac1e7721fbfb18c5b8eac1b9feb8e7c16`  
		Last Modified: Tue, 28 Mar 2023 22:16:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.3`

```console
$ docker pull couchdb@sha256:8ce476fe6b8b35ce832975e5d939b549bac95758180c67a8e8e8c6865f742086
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.3` - linux; amd64

```console
$ docker pull couchdb@sha256:942b2819b96e3cad608505e0d8b61c214458eaceb385af57c257ca6f69f1c300
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90222373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c0e30e9019e2508b12ee524ce325482a6fd58d3c6a0fdc9ea99b2d337e8e52a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:13:24 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 23 Mar 2023 06:13:24 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 23 Mar 2023 06:13:31 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:13:34 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Thu, 23 Mar 2023 06:13:34 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 23 Mar 2023 06:13:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:13:39 GMT
ENV COUCHDB_VERSION=3.3.1
# Thu, 23 Mar 2023 06:13:40 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 23 Mar 2023 06:13:52 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 23 Mar 2023 06:13:52 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 23 Mar 2023 06:13:52 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 28 Mar 2023 21:19:31 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 28 Mar 2023 21:19:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 28 Mar 2023 21:19:31 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 28 Mar 2023 21:19:31 GMT
VOLUME [/opt/couchdb/data]
# Tue, 28 Mar 2023 21:19:32 GMT
EXPOSE 4369 5984 9100
# Tue, 28 Mar 2023 21:19:32 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba7ecd554a3d4cf20e4ee469e50a84ca5ead219a9332ac2c6513b786ab45a20`  
		Last Modified: Thu, 23 Mar 2023 06:15:32 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf01ea1c10cd75a87cff41983af228c45207a118df39f5dd2acb35eb6e18493`  
		Last Modified: Thu, 23 Mar 2023 06:15:31 GMT  
		Size: 5.2 MB (5224316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1fbbca32dec7f4366b57f47aacb4a53e29dd34d19a1d2669ad8af5d98124f7f`  
		Last Modified: Thu, 23 Mar 2023 06:15:30 GMT  
		Size: 610.2 KB (610176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e4e83c342a4a54e132a73b8675b297b02519b678488148700ffa6a3170b6c3`  
		Last Modified: Thu, 23 Mar 2023 06:15:30 GMT  
		Size: 294.3 KB (294302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ccd3165750d901110930a16292f5edaba6dd5399dec993874714e8f23c1f50`  
		Last Modified: Thu, 23 Mar 2023 06:15:30 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed541acd6911a891764e6cdc4031f6f68a387f76a1f5a5878e152debaafe714`  
		Last Modified: Thu, 23 Mar 2023 06:15:33 GMT  
		Size: 52.7 MB (52674763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf4cde9fd11e08968ce2cc685f120862e2d15da31b8168fb33c0c1ff434d48c`  
		Last Modified: Thu, 23 Mar 2023 06:15:28 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de559f5eb2fdb1986baf60340fd174b8acb2c179d27512a14469a241159f7d3`  
		Last Modified: Thu, 23 Mar 2023 06:15:28 GMT  
		Size: 999.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359fb838be8a71de551cb09fc37132882b763aa0ea031c05b6d7338781393237`  
		Last Modified: Tue, 28 Mar 2023 21:19:47 GMT  
		Size: 2.2 KB (2225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb77a1648ee0a099a1c369d785d5cd5352a58de70a8f0294bfcececafd759718`  
		Last Modified: Tue, 28 Mar 2023 21:19:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:4b60ada569d87db6ccc751c48c1af2b7fa32c104f63eb2d01a164ec3d0c76c46
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88670375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6be0e185d26400b7885515277bb9ccf533d0857fe9229ec9ba5610a141630bcf`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:19:52 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 23 Mar 2023 07:19:53 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 23 Mar 2023 07:19:58 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:20:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Thu, 23 Mar 2023 07:20:01 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 23 Mar 2023 07:20:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:20:05 GMT
ENV COUCHDB_VERSION=3.3.1
# Thu, 23 Mar 2023 07:20:06 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 23 Mar 2023 07:20:18 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 23 Mar 2023 07:20:18 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 23 Mar 2023 07:20:18 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 28 Mar 2023 21:39:21 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 28 Mar 2023 21:39:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 28 Mar 2023 21:39:21 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 28 Mar 2023 21:39:21 GMT
VOLUME [/opt/couchdb/data]
# Tue, 28 Mar 2023 21:39:21 GMT
EXPOSE 4369 5984 9100
# Tue, 28 Mar 2023 21:39:21 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1618330853d06ff84cee3f0710edfa89620b7487477fe25b6b9b4c9b5aa6ecbb`  
		Last Modified: Thu, 23 Mar 2023 07:21:43 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25bf7f910cfd6147a589be1daa4d2747b9e79d4b1d620411cfa8b04f76fd78e6`  
		Last Modified: Thu, 23 Mar 2023 07:21:41 GMT  
		Size: 5.2 MB (5209441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8294faa460f96deaf9b020aa5d39f46693755c3e5d8e8e4021da77fd768966c`  
		Last Modified: Thu, 23 Mar 2023 07:21:41 GMT  
		Size: 566.2 KB (566228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99ddcc79770483aa72f62fe1c7042aa2e477e62db34074fbf35070ba0ce4d93`  
		Last Modified: Thu, 23 Mar 2023 07:21:41 GMT  
		Size: 294.3 KB (294251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b9d4aebd4a140d75fee1de8edabce6c8429a4598bdff86308bafb92d7d2722`  
		Last Modified: Thu, 23 Mar 2023 07:21:40 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bd5745764bcdb5b3c74099f609a4f68ed855974ce55b5f5c3e0999ddf36c12`  
		Last Modified: Thu, 23 Mar 2023 07:21:43 GMT  
		Size: 52.5 MB (52530318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea0a2deba7b340cab49bd537bf108fe1d34fd11b565d39b074edece47dddd8c`  
		Last Modified: Thu, 23 Mar 2023 07:21:39 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1132ca9468038cb38834f462df91e0b09daaf709a9b937bc51839654e94c7cdf`  
		Last Modified: Thu, 23 Mar 2023 07:21:39 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e6dda382f5b7956361954059b4221ebc90e5f87e2ebc7d06595856f820fdad`  
		Last Modified: Tue, 28 Mar 2023 21:39:34 GMT  
		Size: 2.2 KB (2223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc09b0172825078f89e56cb53b8b4244542b21acf87f46a1f8a84c6198671feb`  
		Last Modified: Tue, 28 Mar 2023 21:39:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3` - linux; ppc64le

```console
$ docker pull couchdb@sha256:5e55ccae68b16be2f006024bd6fe20d7e360ecd3a593bdc58cbfa4d7890cd9d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.8 MB (95828939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0d438d66e59e61a0215d65cac76fc59d710d226a36ee012fd5515f21d0eaadd`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 23 Mar 2023 01:19:48 GMT
ADD file:fbd36b7667327dd30171fc49b8e028b8371fdbc7d30ee673808d508557f78bf1 in / 
# Thu, 23 Mar 2023 01:19:49 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:28:20 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 23 Mar 2023 13:28:21 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 23 Mar 2023 13:28:39 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:28:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Thu, 23 Mar 2023 13:28:46 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 23 Mar 2023 13:28:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:28:57 GMT
ENV COUCHDB_VERSION=3.3.1
# Thu, 23 Mar 2023 13:28:58 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 23 Mar 2023 13:29:21 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 23 Mar 2023 13:29:23 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 23 Mar 2023 13:29:23 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 28 Mar 2023 22:16:24 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 28 Mar 2023 22:16:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 28 Mar 2023 22:16:25 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 28 Mar 2023 22:16:25 GMT
VOLUME [/opt/couchdb/data]
# Tue, 28 Mar 2023 22:16:26 GMT
EXPOSE 4369 5984 9100
# Tue, 28 Mar 2023 22:16:26 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:8f472ad0a3fa58b4e304d1a974f25615d5bd3b7a99dff9c8202bd30facef0155`  
		Last Modified: Thu, 23 Mar 2023 01:24:22 GMT  
		Size: 35.3 MB (35288050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5c7bf4c8ed82b56f645f6dd5aef795b2ebaf5ad9b12975fd4dc50d3b628832`  
		Last Modified: Thu, 23 Mar 2023 13:30:19 GMT  
		Size: 3.4 KB (3407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5bb5aa4fc53a24f4d3c36f1ec2657044eb895eafc16d3f2d40984403310d682`  
		Last Modified: Thu, 23 Mar 2023 13:30:19 GMT  
		Size: 6.0 MB (6043906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593ab4aa61259780aec8601aa2e5cb0d1890c9fb72572f36731ca410c39ed987`  
		Last Modified: Thu, 23 Mar 2023 13:30:17 GMT  
		Size: 662.0 KB (661975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98e8db79171155dcffbbda14008a110076ea43e1558c06b12047967e48ce9b7`  
		Last Modified: Thu, 23 Mar 2023 13:30:17 GMT  
		Size: 294.2 KB (294213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7edda1bfbb4044153d412476d8d1c3e0ec7e5b7c37abc6bae358c21d80f4c8ca`  
		Last Modified: Thu, 23 Mar 2023 13:30:17 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84d062db9934f420046117f415d6341c3456e5c410555dbfcbf6b2e0f7921cc`  
		Last Modified: Thu, 23 Mar 2023 13:30:24 GMT  
		Size: 53.5 MB (53533380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f78e4dc952cdcc9c77fe3044eea84c6dba34374cda602d50ec9ece0d6a55913`  
		Last Modified: Thu, 23 Mar 2023 13:30:15 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6fa201c8642622fbd3a9430eab8b6e769c4fd523830e5ef0f34f786f6c1b01`  
		Last Modified: Thu, 23 Mar 2023 13:30:15 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bccd1544b83d012a35e53196df3b474db7c88911964af7648fdb7c520803aa9`  
		Last Modified: Tue, 28 Mar 2023 22:16:41 GMT  
		Size: 2.2 KB (2228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b1dd1214b7c873d5119e167b6674ff08970c879fb33604314e473a5b80833f`  
		Last Modified: Tue, 28 Mar 2023 22:16:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.3.1`

```console
$ docker pull couchdb@sha256:8ce476fe6b8b35ce832975e5d939b549bac95758180c67a8e8e8c6865f742086
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:942b2819b96e3cad608505e0d8b61c214458eaceb385af57c257ca6f69f1c300
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90222373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c0e30e9019e2508b12ee524ce325482a6fd58d3c6a0fdc9ea99b2d337e8e52a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:13:24 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 23 Mar 2023 06:13:24 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 23 Mar 2023 06:13:31 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:13:34 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Thu, 23 Mar 2023 06:13:34 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 23 Mar 2023 06:13:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:13:39 GMT
ENV COUCHDB_VERSION=3.3.1
# Thu, 23 Mar 2023 06:13:40 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 23 Mar 2023 06:13:52 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 23 Mar 2023 06:13:52 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 23 Mar 2023 06:13:52 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 28 Mar 2023 21:19:31 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 28 Mar 2023 21:19:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 28 Mar 2023 21:19:31 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 28 Mar 2023 21:19:31 GMT
VOLUME [/opt/couchdb/data]
# Tue, 28 Mar 2023 21:19:32 GMT
EXPOSE 4369 5984 9100
# Tue, 28 Mar 2023 21:19:32 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba7ecd554a3d4cf20e4ee469e50a84ca5ead219a9332ac2c6513b786ab45a20`  
		Last Modified: Thu, 23 Mar 2023 06:15:32 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf01ea1c10cd75a87cff41983af228c45207a118df39f5dd2acb35eb6e18493`  
		Last Modified: Thu, 23 Mar 2023 06:15:31 GMT  
		Size: 5.2 MB (5224316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1fbbca32dec7f4366b57f47aacb4a53e29dd34d19a1d2669ad8af5d98124f7f`  
		Last Modified: Thu, 23 Mar 2023 06:15:30 GMT  
		Size: 610.2 KB (610176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e4e83c342a4a54e132a73b8675b297b02519b678488148700ffa6a3170b6c3`  
		Last Modified: Thu, 23 Mar 2023 06:15:30 GMT  
		Size: 294.3 KB (294302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ccd3165750d901110930a16292f5edaba6dd5399dec993874714e8f23c1f50`  
		Last Modified: Thu, 23 Mar 2023 06:15:30 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed541acd6911a891764e6cdc4031f6f68a387f76a1f5a5878e152debaafe714`  
		Last Modified: Thu, 23 Mar 2023 06:15:33 GMT  
		Size: 52.7 MB (52674763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf4cde9fd11e08968ce2cc685f120862e2d15da31b8168fb33c0c1ff434d48c`  
		Last Modified: Thu, 23 Mar 2023 06:15:28 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de559f5eb2fdb1986baf60340fd174b8acb2c179d27512a14469a241159f7d3`  
		Last Modified: Thu, 23 Mar 2023 06:15:28 GMT  
		Size: 999.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359fb838be8a71de551cb09fc37132882b763aa0ea031c05b6d7338781393237`  
		Last Modified: Tue, 28 Mar 2023 21:19:47 GMT  
		Size: 2.2 KB (2225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb77a1648ee0a099a1c369d785d5cd5352a58de70a8f0294bfcececafd759718`  
		Last Modified: Tue, 28 Mar 2023 21:19:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:4b60ada569d87db6ccc751c48c1af2b7fa32c104f63eb2d01a164ec3d0c76c46
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88670375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6be0e185d26400b7885515277bb9ccf533d0857fe9229ec9ba5610a141630bcf`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:19:52 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 23 Mar 2023 07:19:53 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 23 Mar 2023 07:19:58 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:20:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Thu, 23 Mar 2023 07:20:01 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 23 Mar 2023 07:20:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:20:05 GMT
ENV COUCHDB_VERSION=3.3.1
# Thu, 23 Mar 2023 07:20:06 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 23 Mar 2023 07:20:18 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 23 Mar 2023 07:20:18 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 23 Mar 2023 07:20:18 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 28 Mar 2023 21:39:21 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 28 Mar 2023 21:39:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 28 Mar 2023 21:39:21 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 28 Mar 2023 21:39:21 GMT
VOLUME [/opt/couchdb/data]
# Tue, 28 Mar 2023 21:39:21 GMT
EXPOSE 4369 5984 9100
# Tue, 28 Mar 2023 21:39:21 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1618330853d06ff84cee3f0710edfa89620b7487477fe25b6b9b4c9b5aa6ecbb`  
		Last Modified: Thu, 23 Mar 2023 07:21:43 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25bf7f910cfd6147a589be1daa4d2747b9e79d4b1d620411cfa8b04f76fd78e6`  
		Last Modified: Thu, 23 Mar 2023 07:21:41 GMT  
		Size: 5.2 MB (5209441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8294faa460f96deaf9b020aa5d39f46693755c3e5d8e8e4021da77fd768966c`  
		Last Modified: Thu, 23 Mar 2023 07:21:41 GMT  
		Size: 566.2 KB (566228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99ddcc79770483aa72f62fe1c7042aa2e477e62db34074fbf35070ba0ce4d93`  
		Last Modified: Thu, 23 Mar 2023 07:21:41 GMT  
		Size: 294.3 KB (294251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b9d4aebd4a140d75fee1de8edabce6c8429a4598bdff86308bafb92d7d2722`  
		Last Modified: Thu, 23 Mar 2023 07:21:40 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bd5745764bcdb5b3c74099f609a4f68ed855974ce55b5f5c3e0999ddf36c12`  
		Last Modified: Thu, 23 Mar 2023 07:21:43 GMT  
		Size: 52.5 MB (52530318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea0a2deba7b340cab49bd537bf108fe1d34fd11b565d39b074edece47dddd8c`  
		Last Modified: Thu, 23 Mar 2023 07:21:39 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1132ca9468038cb38834f462df91e0b09daaf709a9b937bc51839654e94c7cdf`  
		Last Modified: Thu, 23 Mar 2023 07:21:39 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e6dda382f5b7956361954059b4221ebc90e5f87e2ebc7d06595856f820fdad`  
		Last Modified: Tue, 28 Mar 2023 21:39:34 GMT  
		Size: 2.2 KB (2223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc09b0172825078f89e56cb53b8b4244542b21acf87f46a1f8a84c6198671feb`  
		Last Modified: Tue, 28 Mar 2023 21:39:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3.1` - linux; ppc64le

```console
$ docker pull couchdb@sha256:5e55ccae68b16be2f006024bd6fe20d7e360ecd3a593bdc58cbfa4d7890cd9d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.8 MB (95828939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0d438d66e59e61a0215d65cac76fc59d710d226a36ee012fd5515f21d0eaadd`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 23 Mar 2023 01:19:48 GMT
ADD file:fbd36b7667327dd30171fc49b8e028b8371fdbc7d30ee673808d508557f78bf1 in / 
# Thu, 23 Mar 2023 01:19:49 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:28:20 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 23 Mar 2023 13:28:21 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 23 Mar 2023 13:28:39 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:28:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Thu, 23 Mar 2023 13:28:46 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 23 Mar 2023 13:28:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:28:57 GMT
ENV COUCHDB_VERSION=3.3.1
# Thu, 23 Mar 2023 13:28:58 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 23 Mar 2023 13:29:21 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 23 Mar 2023 13:29:23 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 23 Mar 2023 13:29:23 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 28 Mar 2023 22:16:24 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 28 Mar 2023 22:16:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 28 Mar 2023 22:16:25 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 28 Mar 2023 22:16:25 GMT
VOLUME [/opt/couchdb/data]
# Tue, 28 Mar 2023 22:16:26 GMT
EXPOSE 4369 5984 9100
# Tue, 28 Mar 2023 22:16:26 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:8f472ad0a3fa58b4e304d1a974f25615d5bd3b7a99dff9c8202bd30facef0155`  
		Last Modified: Thu, 23 Mar 2023 01:24:22 GMT  
		Size: 35.3 MB (35288050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5c7bf4c8ed82b56f645f6dd5aef795b2ebaf5ad9b12975fd4dc50d3b628832`  
		Last Modified: Thu, 23 Mar 2023 13:30:19 GMT  
		Size: 3.4 KB (3407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5bb5aa4fc53a24f4d3c36f1ec2657044eb895eafc16d3f2d40984403310d682`  
		Last Modified: Thu, 23 Mar 2023 13:30:19 GMT  
		Size: 6.0 MB (6043906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593ab4aa61259780aec8601aa2e5cb0d1890c9fb72572f36731ca410c39ed987`  
		Last Modified: Thu, 23 Mar 2023 13:30:17 GMT  
		Size: 662.0 KB (661975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98e8db79171155dcffbbda14008a110076ea43e1558c06b12047967e48ce9b7`  
		Last Modified: Thu, 23 Mar 2023 13:30:17 GMT  
		Size: 294.2 KB (294213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7edda1bfbb4044153d412476d8d1c3e0ec7e5b7c37abc6bae358c21d80f4c8ca`  
		Last Modified: Thu, 23 Mar 2023 13:30:17 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84d062db9934f420046117f415d6341c3456e5c410555dbfcbf6b2e0f7921cc`  
		Last Modified: Thu, 23 Mar 2023 13:30:24 GMT  
		Size: 53.5 MB (53533380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f78e4dc952cdcc9c77fe3044eea84c6dba34374cda602d50ec9ece0d6a55913`  
		Last Modified: Thu, 23 Mar 2023 13:30:15 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6fa201c8642622fbd3a9430eab8b6e769c4fd523830e5ef0f34f786f6c1b01`  
		Last Modified: Thu, 23 Mar 2023 13:30:15 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bccd1544b83d012a35e53196df3b474db7c88911964af7648fdb7c520803aa9`  
		Last Modified: Tue, 28 Mar 2023 22:16:41 GMT  
		Size: 2.2 KB (2228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b1dd1214b7c873d5119e167b6674ff08970c879fb33604314e473a5b80833f`  
		Last Modified: Tue, 28 Mar 2023 22:16:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:latest`

```console
$ docker pull couchdb@sha256:8ce476fe6b8b35ce832975e5d939b549bac95758180c67a8e8e8c6865f742086
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:942b2819b96e3cad608505e0d8b61c214458eaceb385af57c257ca6f69f1c300
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90222373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c0e30e9019e2508b12ee524ce325482a6fd58d3c6a0fdc9ea99b2d337e8e52a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:13:24 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 23 Mar 2023 06:13:24 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 23 Mar 2023 06:13:31 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:13:34 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Thu, 23 Mar 2023 06:13:34 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 23 Mar 2023 06:13:39 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:13:39 GMT
ENV COUCHDB_VERSION=3.3.1
# Thu, 23 Mar 2023 06:13:40 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 23 Mar 2023 06:13:52 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 23 Mar 2023 06:13:52 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 23 Mar 2023 06:13:52 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 28 Mar 2023 21:19:31 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 28 Mar 2023 21:19:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 28 Mar 2023 21:19:31 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 28 Mar 2023 21:19:31 GMT
VOLUME [/opt/couchdb/data]
# Tue, 28 Mar 2023 21:19:32 GMT
EXPOSE 4369 5984 9100
# Tue, 28 Mar 2023 21:19:32 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba7ecd554a3d4cf20e4ee469e50a84ca5ead219a9332ac2c6513b786ab45a20`  
		Last Modified: Thu, 23 Mar 2023 06:15:32 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf01ea1c10cd75a87cff41983af228c45207a118df39f5dd2acb35eb6e18493`  
		Last Modified: Thu, 23 Mar 2023 06:15:31 GMT  
		Size: 5.2 MB (5224316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1fbbca32dec7f4366b57f47aacb4a53e29dd34d19a1d2669ad8af5d98124f7f`  
		Last Modified: Thu, 23 Mar 2023 06:15:30 GMT  
		Size: 610.2 KB (610176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e4e83c342a4a54e132a73b8675b297b02519b678488148700ffa6a3170b6c3`  
		Last Modified: Thu, 23 Mar 2023 06:15:30 GMT  
		Size: 294.3 KB (294302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ccd3165750d901110930a16292f5edaba6dd5399dec993874714e8f23c1f50`  
		Last Modified: Thu, 23 Mar 2023 06:15:30 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed541acd6911a891764e6cdc4031f6f68a387f76a1f5a5878e152debaafe714`  
		Last Modified: Thu, 23 Mar 2023 06:15:33 GMT  
		Size: 52.7 MB (52674763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf4cde9fd11e08968ce2cc685f120862e2d15da31b8168fb33c0c1ff434d48c`  
		Last Modified: Thu, 23 Mar 2023 06:15:28 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de559f5eb2fdb1986baf60340fd174b8acb2c179d27512a14469a241159f7d3`  
		Last Modified: Thu, 23 Mar 2023 06:15:28 GMT  
		Size: 999.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359fb838be8a71de551cb09fc37132882b763aa0ea031c05b6d7338781393237`  
		Last Modified: Tue, 28 Mar 2023 21:19:47 GMT  
		Size: 2.2 KB (2225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb77a1648ee0a099a1c369d785d5cd5352a58de70a8f0294bfcececafd759718`  
		Last Modified: Tue, 28 Mar 2023 21:19:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:4b60ada569d87db6ccc751c48c1af2b7fa32c104f63eb2d01a164ec3d0c76c46
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88670375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6be0e185d26400b7885515277bb9ccf533d0857fe9229ec9ba5610a141630bcf`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 07:19:52 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 23 Mar 2023 07:19:53 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 23 Mar 2023 07:19:58 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:20:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Thu, 23 Mar 2023 07:20:01 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 23 Mar 2023 07:20:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 07:20:05 GMT
ENV COUCHDB_VERSION=3.3.1
# Thu, 23 Mar 2023 07:20:06 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 23 Mar 2023 07:20:18 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 23 Mar 2023 07:20:18 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 23 Mar 2023 07:20:18 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 28 Mar 2023 21:39:21 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 28 Mar 2023 21:39:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 28 Mar 2023 21:39:21 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 28 Mar 2023 21:39:21 GMT
VOLUME [/opt/couchdb/data]
# Tue, 28 Mar 2023 21:39:21 GMT
EXPOSE 4369 5984 9100
# Tue, 28 Mar 2023 21:39:21 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1618330853d06ff84cee3f0710edfa89620b7487477fe25b6b9b4c9b5aa6ecbb`  
		Last Modified: Thu, 23 Mar 2023 07:21:43 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25bf7f910cfd6147a589be1daa4d2747b9e79d4b1d620411cfa8b04f76fd78e6`  
		Last Modified: Thu, 23 Mar 2023 07:21:41 GMT  
		Size: 5.2 MB (5209441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8294faa460f96deaf9b020aa5d39f46693755c3e5d8e8e4021da77fd768966c`  
		Last Modified: Thu, 23 Mar 2023 07:21:41 GMT  
		Size: 566.2 KB (566228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99ddcc79770483aa72f62fe1c7042aa2e477e62db34074fbf35070ba0ce4d93`  
		Last Modified: Thu, 23 Mar 2023 07:21:41 GMT  
		Size: 294.3 KB (294251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b9d4aebd4a140d75fee1de8edabce6c8429a4598bdff86308bafb92d7d2722`  
		Last Modified: Thu, 23 Mar 2023 07:21:40 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bd5745764bcdb5b3c74099f609a4f68ed855974ce55b5f5c3e0999ddf36c12`  
		Last Modified: Thu, 23 Mar 2023 07:21:43 GMT  
		Size: 52.5 MB (52530318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ea0a2deba7b340cab49bd537bf108fe1d34fd11b565d39b074edece47dddd8c`  
		Last Modified: Thu, 23 Mar 2023 07:21:39 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1132ca9468038cb38834f462df91e0b09daaf709a9b937bc51839654e94c7cdf`  
		Last Modified: Thu, 23 Mar 2023 07:21:39 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e6dda382f5b7956361954059b4221ebc90e5f87e2ebc7d06595856f820fdad`  
		Last Modified: Tue, 28 Mar 2023 21:39:34 GMT  
		Size: 2.2 KB (2223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc09b0172825078f89e56cb53b8b4244542b21acf87f46a1f8a84c6198671feb`  
		Last Modified: Tue, 28 Mar 2023 21:39:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; ppc64le

```console
$ docker pull couchdb@sha256:5e55ccae68b16be2f006024bd6fe20d7e360ecd3a593bdc58cbfa4d7890cd9d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.8 MB (95828939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0d438d66e59e61a0215d65cac76fc59d710d226a36ee012fd5515f21d0eaadd`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 23 Mar 2023 01:19:48 GMT
ADD file:fbd36b7667327dd30171fc49b8e028b8371fdbc7d30ee673808d508557f78bf1 in / 
# Thu, 23 Mar 2023 01:19:49 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:28:20 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 23 Mar 2023 13:28:21 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 23 Mar 2023 13:28:39 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:28:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Thu, 23 Mar 2023 13:28:46 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 23 Mar 2023 13:28:57 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:28:57 GMT
ENV COUCHDB_VERSION=3.3.1
# Thu, 23 Mar 2023 13:28:58 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 23 Mar 2023 13:29:21 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 23 Mar 2023 13:29:23 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 23 Mar 2023 13:29:23 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 28 Mar 2023 22:16:24 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 28 Mar 2023 22:16:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 28 Mar 2023 22:16:25 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 28 Mar 2023 22:16:25 GMT
VOLUME [/opt/couchdb/data]
# Tue, 28 Mar 2023 22:16:26 GMT
EXPOSE 4369 5984 9100
# Tue, 28 Mar 2023 22:16:26 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:8f472ad0a3fa58b4e304d1a974f25615d5bd3b7a99dff9c8202bd30facef0155`  
		Last Modified: Thu, 23 Mar 2023 01:24:22 GMT  
		Size: 35.3 MB (35288050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5c7bf4c8ed82b56f645f6dd5aef795b2ebaf5ad9b12975fd4dc50d3b628832`  
		Last Modified: Thu, 23 Mar 2023 13:30:19 GMT  
		Size: 3.4 KB (3407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5bb5aa4fc53a24f4d3c36f1ec2657044eb895eafc16d3f2d40984403310d682`  
		Last Modified: Thu, 23 Mar 2023 13:30:19 GMT  
		Size: 6.0 MB (6043906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593ab4aa61259780aec8601aa2e5cb0d1890c9fb72572f36731ca410c39ed987`  
		Last Modified: Thu, 23 Mar 2023 13:30:17 GMT  
		Size: 662.0 KB (661975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98e8db79171155dcffbbda14008a110076ea43e1558c06b12047967e48ce9b7`  
		Last Modified: Thu, 23 Mar 2023 13:30:17 GMT  
		Size: 294.2 KB (294213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7edda1bfbb4044153d412476d8d1c3e0ec7e5b7c37abc6bae358c21d80f4c8ca`  
		Last Modified: Thu, 23 Mar 2023 13:30:17 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84d062db9934f420046117f415d6341c3456e5c410555dbfcbf6b2e0f7921cc`  
		Last Modified: Thu, 23 Mar 2023 13:30:24 GMT  
		Size: 53.5 MB (53533380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f78e4dc952cdcc9c77fe3044eea84c6dba34374cda602d50ec9ece0d6a55913`  
		Last Modified: Thu, 23 Mar 2023 13:30:15 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6fa201c8642622fbd3a9430eab8b6e769c4fd523830e5ef0f34f786f6c1b01`  
		Last Modified: Thu, 23 Mar 2023 13:30:15 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bccd1544b83d012a35e53196df3b474db7c88911964af7648fdb7c520803aa9`  
		Last Modified: Tue, 28 Mar 2023 22:16:41 GMT  
		Size: 2.2 KB (2228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b1dd1214b7c873d5119e167b6674ff08970c879fb33604314e473a5b80833f`  
		Last Modified: Tue, 28 Mar 2023 22:16:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
