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
$ docker pull couchdb@sha256:79d0c5ffb99785a6c36ecfa205ae78722254f6282a100c330d4681b5c3bcf6df
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
$ docker pull couchdb@sha256:ea7b89c57661b743d97ce50a81b24533b6ad78eea4c237090b4bb1b4de72da44
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72997261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:071dbafc8ee72b35d2774709ddc014915b1ea4b29f4c914f0ffc76192af2c845`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:56 GMT
ADD file:ab0ca1f1ee3db357c8de06fd63e3d5f0132541162438c121e99f29e6af190bfa in / 
# Wed, 01 Mar 2023 02:20:56 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 13:01:33 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Mar 2023 13:01:33 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Mar 2023 13:01:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 13:01:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Mar 2023 13:01:44 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Mar 2023 13:01:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 13:02:06 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 01 Mar 2023 13:02:07 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Mar 2023 13:02:18 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Mar 2023 13:02:18 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Mar 2023 13:02:18 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 01 Mar 2023 13:02:18 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 01 Mar 2023 13:02:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Mar 2023 13:02:19 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 13:02:19 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Mar 2023 13:02:19 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Mar 2023 13:02:19 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ed22f951ea44cd39f81544a2f0bf196ad60d13c1428cea537535186be61818f7`  
		Last Modified: Wed, 01 Mar 2023 02:24:56 GMT  
		Size: 25.9 MB (25922699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6759d0399eeb0f700a9b9ce8ac2a6434521a39edd2c8d47b8c92c96f16df8457`  
		Last Modified: Wed, 01 Mar 2023 13:03:12 GMT  
		Size: 3.4 KB (3437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fe820e62570423958042a1e3878aac6a571079ee3d518a5e649b0958deeefc`  
		Last Modified: Wed, 01 Mar 2023 13:03:11 GMT  
		Size: 6.6 MB (6579452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a247326076072850c80eb99fb5139cf988dc11020995fccdb020dc57e571c4`  
		Last Modified: Wed, 01 Mar 2023 13:03:11 GMT  
		Size: 1.2 MB (1164552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ace80db58c9be6fa388162aa3678dba8385d28f7022cba310faccebdbccc62b`  
		Last Modified: Wed, 01 Mar 2023 13:03:11 GMT  
		Size: 294.2 KB (294169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5de621ffd97e5656bcca3d5d3e385935ca23892f98767fd83629331975b0718`  
		Last Modified: Wed, 01 Mar 2023 13:03:23 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2acbf36cda8047ccda1da0cb7d771fe3c0bfa2b0676612e74892db968eeaf8ed`  
		Last Modified: Wed, 01 Mar 2023 13:03:24 GMT  
		Size: 39.0 MB (39029350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ef8d5f305333f3b52585331b86e0a4b6ce982ee2e5130cb4d77cd2c5903e1c`  
		Last Modified: Wed, 01 Mar 2023 13:03:21 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09bec3c44ac5d8ec73c5a35785b6f43cebf7fa8e9273d01c43e3aa19aa8fb648`  
		Last Modified: Wed, 01 Mar 2023 13:03:21 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10211858e516ea36fb3c31e5f65541e85397e5daa0e1c3461f7188eab8908a5a`  
		Last Modified: Wed, 01 Mar 2023 13:03:21 GMT  
		Size: 2.1 KB (2055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adabf0b267fbb86f841b2d667849dd0e0443cd81fd3db55ed8893834ddaeb23c`  
		Last Modified: Wed, 01 Mar 2023 13:03:21 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3`

```console
$ docker pull couchdb@sha256:79d0c5ffb99785a6c36ecfa205ae78722254f6282a100c330d4681b5c3bcf6df
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
$ docker pull couchdb@sha256:ea7b89c57661b743d97ce50a81b24533b6ad78eea4c237090b4bb1b4de72da44
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72997261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:071dbafc8ee72b35d2774709ddc014915b1ea4b29f4c914f0ffc76192af2c845`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:56 GMT
ADD file:ab0ca1f1ee3db357c8de06fd63e3d5f0132541162438c121e99f29e6af190bfa in / 
# Wed, 01 Mar 2023 02:20:56 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 13:01:33 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Mar 2023 13:01:33 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Mar 2023 13:01:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 13:01:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Mar 2023 13:01:44 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Mar 2023 13:01:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 13:02:06 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 01 Mar 2023 13:02:07 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Mar 2023 13:02:18 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Mar 2023 13:02:18 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Mar 2023 13:02:18 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 01 Mar 2023 13:02:18 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 01 Mar 2023 13:02:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Mar 2023 13:02:19 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 13:02:19 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Mar 2023 13:02:19 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Mar 2023 13:02:19 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ed22f951ea44cd39f81544a2f0bf196ad60d13c1428cea537535186be61818f7`  
		Last Modified: Wed, 01 Mar 2023 02:24:56 GMT  
		Size: 25.9 MB (25922699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6759d0399eeb0f700a9b9ce8ac2a6434521a39edd2c8d47b8c92c96f16df8457`  
		Last Modified: Wed, 01 Mar 2023 13:03:12 GMT  
		Size: 3.4 KB (3437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fe820e62570423958042a1e3878aac6a571079ee3d518a5e649b0958deeefc`  
		Last Modified: Wed, 01 Mar 2023 13:03:11 GMT  
		Size: 6.6 MB (6579452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a247326076072850c80eb99fb5139cf988dc11020995fccdb020dc57e571c4`  
		Last Modified: Wed, 01 Mar 2023 13:03:11 GMT  
		Size: 1.2 MB (1164552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ace80db58c9be6fa388162aa3678dba8385d28f7022cba310faccebdbccc62b`  
		Last Modified: Wed, 01 Mar 2023 13:03:11 GMT  
		Size: 294.2 KB (294169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5de621ffd97e5656bcca3d5d3e385935ca23892f98767fd83629331975b0718`  
		Last Modified: Wed, 01 Mar 2023 13:03:23 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2acbf36cda8047ccda1da0cb7d771fe3c0bfa2b0676612e74892db968eeaf8ed`  
		Last Modified: Wed, 01 Mar 2023 13:03:24 GMT  
		Size: 39.0 MB (39029350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ef8d5f305333f3b52585331b86e0a4b6ce982ee2e5130cb4d77cd2c5903e1c`  
		Last Modified: Wed, 01 Mar 2023 13:03:21 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09bec3c44ac5d8ec73c5a35785b6f43cebf7fa8e9273d01c43e3aa19aa8fb648`  
		Last Modified: Wed, 01 Mar 2023 13:03:21 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10211858e516ea36fb3c31e5f65541e85397e5daa0e1c3461f7188eab8908a5a`  
		Last Modified: Wed, 01 Mar 2023 13:03:21 GMT  
		Size: 2.1 KB (2055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adabf0b267fbb86f841b2d667849dd0e0443cd81fd3db55ed8893834ddaeb23c`  
		Last Modified: Wed, 01 Mar 2023 13:03:21 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3.1`

```console
$ docker pull couchdb@sha256:79d0c5ffb99785a6c36ecfa205ae78722254f6282a100c330d4681b5c3bcf6df
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
$ docker pull couchdb@sha256:ea7b89c57661b743d97ce50a81b24533b6ad78eea4c237090b4bb1b4de72da44
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72997261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:071dbafc8ee72b35d2774709ddc014915b1ea4b29f4c914f0ffc76192af2c845`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:56 GMT
ADD file:ab0ca1f1ee3db357c8de06fd63e3d5f0132541162438c121e99f29e6af190bfa in / 
# Wed, 01 Mar 2023 02:20:56 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 13:01:33 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Mar 2023 13:01:33 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Mar 2023 13:01:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 13:01:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Mar 2023 13:01:44 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Mar 2023 13:01:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 13:02:06 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 01 Mar 2023 13:02:07 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Mar 2023 13:02:18 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Mar 2023 13:02:18 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Mar 2023 13:02:18 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 01 Mar 2023 13:02:18 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 01 Mar 2023 13:02:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Mar 2023 13:02:19 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 13:02:19 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Mar 2023 13:02:19 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Mar 2023 13:02:19 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ed22f951ea44cd39f81544a2f0bf196ad60d13c1428cea537535186be61818f7`  
		Last Modified: Wed, 01 Mar 2023 02:24:56 GMT  
		Size: 25.9 MB (25922699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6759d0399eeb0f700a9b9ce8ac2a6434521a39edd2c8d47b8c92c96f16df8457`  
		Last Modified: Wed, 01 Mar 2023 13:03:12 GMT  
		Size: 3.4 KB (3437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fe820e62570423958042a1e3878aac6a571079ee3d518a5e649b0958deeefc`  
		Last Modified: Wed, 01 Mar 2023 13:03:11 GMT  
		Size: 6.6 MB (6579452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a247326076072850c80eb99fb5139cf988dc11020995fccdb020dc57e571c4`  
		Last Modified: Wed, 01 Mar 2023 13:03:11 GMT  
		Size: 1.2 MB (1164552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ace80db58c9be6fa388162aa3678dba8385d28f7022cba310faccebdbccc62b`  
		Last Modified: Wed, 01 Mar 2023 13:03:11 GMT  
		Size: 294.2 KB (294169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5de621ffd97e5656bcca3d5d3e385935ca23892f98767fd83629331975b0718`  
		Last Modified: Wed, 01 Mar 2023 13:03:23 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2acbf36cda8047ccda1da0cb7d771fe3c0bfa2b0676612e74892db968eeaf8ed`  
		Last Modified: Wed, 01 Mar 2023 13:03:24 GMT  
		Size: 39.0 MB (39029350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ef8d5f305333f3b52585331b86e0a4b6ce982ee2e5130cb4d77cd2c5903e1c`  
		Last Modified: Wed, 01 Mar 2023 13:03:21 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09bec3c44ac5d8ec73c5a35785b6f43cebf7fa8e9273d01c43e3aa19aa8fb648`  
		Last Modified: Wed, 01 Mar 2023 13:03:21 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10211858e516ea36fb3c31e5f65541e85397e5daa0e1c3461f7188eab8908a5a`  
		Last Modified: Wed, 01 Mar 2023 13:03:21 GMT  
		Size: 2.1 KB (2055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adabf0b267fbb86f841b2d667849dd0e0443cd81fd3db55ed8893834ddaeb23c`  
		Last Modified: Wed, 01 Mar 2023 13:03:21 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3`

```console
$ docker pull couchdb@sha256:6d2bb29aad3d6092f514cb1ce6b0d31f033ec55cb3ca04c37160a1b0cb04d933
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3` - linux; amd64

```console
$ docker pull couchdb@sha256:b72b2cd30fafc137a82a790eeb975d9571ab80a1fb76052383ac8276df3d3adf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90222354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6444bc77edd5ec49ef56b16455e2679e4b0f07e542d31773b8b7bffccd1ebd40`
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
# Thu, 23 Mar 2023 06:13:52 GMT
COPY file:4f56a6457d04af3aef6fcaf07a864b915c40e6514919d19a783d4be98fe5bc89 in /usr/local/bin 
# Thu, 23 Mar 2023 06:13:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 06:13:53 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 06:13:53 GMT
VOLUME [/opt/couchdb/data]
# Thu, 23 Mar 2023 06:13:53 GMT
EXPOSE 4369 5984 9100
# Thu, 23 Mar 2023 06:13:53 GMT
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
	-	`sha256:6e9b6b12f4543e0688de9b6df3d5af367066f54097bdaac8c8f75323550c65e1`  
		Last Modified: Thu, 23 Mar 2023 06:15:28 GMT  
		Size: 2.2 KB (2206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70246ed49013058084013ec8e76bde438cdecc306fb6de20c01acab5a1d2074f`  
		Last Modified: Thu, 23 Mar 2023 06:15:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:5be64acf57d5f2991219ecf2e2e918f4053a6a4da203551e24bfd72c959b947e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88670295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b255331a1a6975bbf99a2262a7fc0d462d3f3c54e4ad114fd1463a0e2fb6e20a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 13:00:43 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Mar 2023 13:00:44 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Mar 2023 13:00:50 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Mon, 20 Mar 2023 22:40:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Mon, 20 Mar 2023 22:40:34 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Mon, 20 Mar 2023 22:40:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Mon, 20 Mar 2023 22:40:38 GMT
ENV COUCHDB_VERSION=3.3.1
# Mon, 20 Mar 2023 22:40:38 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Mon, 20 Mar 2023 22:40:52 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Mon, 20 Mar 2023 22:40:52 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Mon, 20 Mar 2023 22:40:52 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Mon, 20 Mar 2023 22:40:52 GMT
COPY file:4f56a6457d04af3aef6fcaf07a864b915c40e6514919d19a783d4be98fe5bc89 in /usr/local/bin 
# Mon, 20 Mar 2023 22:40:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Mon, 20 Mar 2023 22:40:53 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Mon, 20 Mar 2023 22:40:53 GMT
VOLUME [/opt/couchdb/data]
# Mon, 20 Mar 2023 22:40:53 GMT
EXPOSE 4369 5984 9100
# Mon, 20 Mar 2023 22:40:53 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5062435b3525c590327308b13c7117ff3a0462e7dd8ac2b02b934c832e0b6882`  
		Last Modified: Wed, 01 Mar 2023 13:02:41 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870190223a80d6ce34a8ac53a6aade325a75a20aeca43cbff5549ee2dcd3c1ad`  
		Last Modified: Wed, 01 Mar 2023 13:02:40 GMT  
		Size: 5.2 MB (5209450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e9863e93722978d8dc7bac8f1b64d8c91395ca199c458ffe489ce5be975dab`  
		Last Modified: Mon, 20 Mar 2023 22:41:36 GMT  
		Size: 566.3 KB (566255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7fe9ae8269843a8b140bbc16fe2e7b8db84126d2894b818a46695cf5d98ee9d`  
		Last Modified: Mon, 20 Mar 2023 22:41:36 GMT  
		Size: 294.3 KB (294264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4125d43b64e1ede5061372eac5d8d2b087312f7319996fb20974a85caa1ca2b6`  
		Last Modified: Mon, 20 Mar 2023 22:41:36 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfd880493a9e6cce11f45f67b70d9597f7b7548b6394536119699df09ffcfb0`  
		Last Modified: Mon, 20 Mar 2023 22:41:38 GMT  
		Size: 52.5 MB (52530089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a2dcece77541a2b77d9dfcdfec67a290de44f9aadf8142ef5c0a163ae1dca8`  
		Last Modified: Mon, 20 Mar 2023 22:41:34 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4026f83bc51c9945168f17b4cb18c4978c6854bd15b4df9dd224526d26a928e1`  
		Last Modified: Mon, 20 Mar 2023 22:41:34 GMT  
		Size: 997.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37dde701322e89f3b3989bb60176435c056116b6c1b9db6f4963eb6973b7ee1`  
		Last Modified: Mon, 20 Mar 2023 22:41:34 GMT  
		Size: 2.2 KB (2209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2c60e14e30c82431555c8e47192b288d36688c176e70425db6ee4270399a26`  
		Last Modified: Mon, 20 Mar 2023 22:41:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; ppc64le

```console
$ docker pull couchdb@sha256:a61c3683b0ca2948f3078b89d06c1b75500eef5c74972583d5e44cda377ba776
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.8 MB (95829290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae9642c64a707353006d1cffecd1a7a4da3e2bd27829d533c4a337b10972083c`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:33 GMT
ADD file:6fdf0b2f8ea4be2d01e25a9d85db8f8c7e3b2a641c9c7665e34f4fad771815e0 in / 
# Wed, 01 Mar 2023 04:47:35 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:43:25 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Mar 2023 05:43:26 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Mar 2023 05:43:48 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Mon, 20 Mar 2023 22:16:34 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Mon, 20 Mar 2023 22:16:34 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Mon, 20 Mar 2023 22:16:47 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Mon, 20 Mar 2023 22:16:47 GMT
ENV COUCHDB_VERSION=3.3.1
# Mon, 20 Mar 2023 22:16:48 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Mon, 20 Mar 2023 22:17:13 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Mon, 20 Mar 2023 22:17:14 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Mon, 20 Mar 2023 22:17:15 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Mon, 20 Mar 2023 22:17:15 GMT
COPY file:4f56a6457d04af3aef6fcaf07a864b915c40e6514919d19a783d4be98fe5bc89 in /usr/local/bin 
# Mon, 20 Mar 2023 22:17:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Mon, 20 Mar 2023 22:17:16 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Mon, 20 Mar 2023 22:17:16 GMT
VOLUME [/opt/couchdb/data]
# Mon, 20 Mar 2023 22:17:17 GMT
EXPOSE 4369 5984 9100
# Mon, 20 Mar 2023 22:17:17 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:93ab3a60c2a8cbc1150cb2bd54222db8b79c525c0243534a10d6294ef7ff83ac`  
		Last Modified: Wed, 01 Mar 2023 04:53:54 GMT  
		Size: 35.3 MB (35288103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7db168bb798ef118541ed78f0f09ab50044e5c6830937388a72cc43d78035b4`  
		Last Modified: Wed, 01 Mar 2023 05:46:05 GMT  
		Size: 3.4 KB (3415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b49f4851c4778b84f6d8d20589ed144f5d5aed34469fb055ba5961d658a92d`  
		Last Modified: Wed, 01 Mar 2023 05:46:05 GMT  
		Size: 6.0 MB (6043951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2842ad19ef92a090e8111ad7e88fcbf2c0fb50caec07709f50d634294c4ced5`  
		Last Modified: Mon, 20 Mar 2023 22:18:22 GMT  
		Size: 662.1 KB (662067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54475fcf0a17094179a6d5e3a9e1c1ff6aeb8e8a76da5630da72ba9c7164b9e5`  
		Last Modified: Mon, 20 Mar 2023 22:18:22 GMT  
		Size: 294.3 KB (294302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35f095cf7b5e92264b86d71420ddf1ae59ea1ffd7e653fa4985df3a6b0ef42cf`  
		Last Modified: Mon, 20 Mar 2023 22:18:21 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1625cdce16d9ecdc3ebd8dee77f10730d1b98340f8a79deae3d9c9fbc626e013`  
		Last Modified: Mon, 20 Mar 2023 22:18:29 GMT  
		Size: 53.5 MB (53533461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602d60b8bd03fd76328fee3d9232ce007b6f489bd4186ab1e573332cafb27a55`  
		Last Modified: Mon, 20 Mar 2023 22:18:19 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5371246bf435da2d0007b058ada6946f5bd70333face6dba0a595e9695478eb0`  
		Last Modified: Mon, 20 Mar 2023 22:18:19 GMT  
		Size: 1.0 KB (1002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba84c938a14f7ecd134f28ac7951fcdb3c73179b7713659792f8c4e86a495180`  
		Last Modified: Mon, 20 Mar 2023 22:18:19 GMT  
		Size: 2.2 KB (2210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd777621cdc3f8f9dc7f220ac32bd3f8227860f932bb8462275d2f3597e0829`  
		Last Modified: Mon, 20 Mar 2023 22:18:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1`

```console
$ docker pull couchdb@sha256:f4a375e7017a565e7f1f555aab8635b3fc88aad3ffed2f13402cd4c95b25fe8a
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
$ docker pull couchdb@sha256:0436fea5383841f640f3c67f8e9c180518ee41ffeffc8d9b46ca4ea1ec07809a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75093777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcb0c71e0699b58cbadc26292b9aac02773859d11d528715ab27b352cbce4290`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:56 GMT
ADD file:ab0ca1f1ee3db357c8de06fd63e3d5f0132541162438c121e99f29e6af190bfa in / 
# Wed, 01 Mar 2023 02:20:56 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 13:01:33 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Mar 2023 13:01:33 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Mar 2023 13:01:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 13:01:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Mar 2023 13:01:44 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Mar 2023 13:01:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 13:01:50 GMT
ENV COUCHDB_VERSION=3.1.2
# Wed, 01 Mar 2023 13:01:50 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Mar 2023 13:02:02 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Mar 2023 13:02:02 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Mar 2023 13:02:02 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 01 Mar 2023 13:02:02 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 01 Mar 2023 13:02:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Mar 2023 13:02:03 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 13:02:03 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Mar 2023 13:02:03 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Mar 2023 13:02:03 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ed22f951ea44cd39f81544a2f0bf196ad60d13c1428cea537535186be61818f7`  
		Last Modified: Wed, 01 Mar 2023 02:24:56 GMT  
		Size: 25.9 MB (25922699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6759d0399eeb0f700a9b9ce8ac2a6434521a39edd2c8d47b8c92c96f16df8457`  
		Last Modified: Wed, 01 Mar 2023 13:03:12 GMT  
		Size: 3.4 KB (3437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fe820e62570423958042a1e3878aac6a571079ee3d518a5e649b0958deeefc`  
		Last Modified: Wed, 01 Mar 2023 13:03:11 GMT  
		Size: 6.6 MB (6579452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a247326076072850c80eb99fb5139cf988dc11020995fccdb020dc57e571c4`  
		Last Modified: Wed, 01 Mar 2023 13:03:11 GMT  
		Size: 1.2 MB (1164552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ace80db58c9be6fa388162aa3678dba8385d28f7022cba310faccebdbccc62b`  
		Last Modified: Wed, 01 Mar 2023 13:03:11 GMT  
		Size: 294.2 KB (294169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11d35eeba918575d5c78b08bd873cb609e1dd7de4039ed4e7fde1a9655f6fee`  
		Last Modified: Wed, 01 Mar 2023 13:03:10 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913390e565908a1cde895cd2228112cbb865040a57aafcdbc70f3517216859a8`  
		Last Modified: Wed, 01 Mar 2023 13:03:13 GMT  
		Size: 41.1 MB (41125870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5405f7852d9ad5045236f53e4662f0356b00cada7d223812ab2aedc7e8b30b2e`  
		Last Modified: Wed, 01 Mar 2023 13:03:09 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c39ac9cf22dc7bc4a74a244936a8952f03b8fdf9868d67726adaa8072ba283`  
		Last Modified: Wed, 01 Mar 2023 13:03:09 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a51f93869e0195860058e9e05e4da9ecb1a8220ee4ff2e0454e3e423dc8e77f`  
		Last Modified: Wed, 01 Mar 2023 13:03:09 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e37b09e566e2d6ef8a535b536d4b6481bbc5ef7cb410313006ce11818af20e`  
		Last Modified: Wed, 01 Mar 2023 13:03:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1.2`

```console
$ docker pull couchdb@sha256:f4a375e7017a565e7f1f555aab8635b3fc88aad3ffed2f13402cd4c95b25fe8a
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
$ docker pull couchdb@sha256:0436fea5383841f640f3c67f8e9c180518ee41ffeffc8d9b46ca4ea1ec07809a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75093777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcb0c71e0699b58cbadc26292b9aac02773859d11d528715ab27b352cbce4290`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:56 GMT
ADD file:ab0ca1f1ee3db357c8de06fd63e3d5f0132541162438c121e99f29e6af190bfa in / 
# Wed, 01 Mar 2023 02:20:56 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 13:01:33 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Mar 2023 13:01:33 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Mar 2023 13:01:41 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 13:01:44 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Mar 2023 13:01:44 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Mar 2023 13:01:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 13:01:50 GMT
ENV COUCHDB_VERSION=3.1.2
# Wed, 01 Mar 2023 13:01:50 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Mar 2023 13:02:02 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Mar 2023 13:02:02 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Mar 2023 13:02:02 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 01 Mar 2023 13:02:02 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 01 Mar 2023 13:02:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Mar 2023 13:02:03 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 13:02:03 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Mar 2023 13:02:03 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Mar 2023 13:02:03 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ed22f951ea44cd39f81544a2f0bf196ad60d13c1428cea537535186be61818f7`  
		Last Modified: Wed, 01 Mar 2023 02:24:56 GMT  
		Size: 25.9 MB (25922699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6759d0399eeb0f700a9b9ce8ac2a6434521a39edd2c8d47b8c92c96f16df8457`  
		Last Modified: Wed, 01 Mar 2023 13:03:12 GMT  
		Size: 3.4 KB (3437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fe820e62570423958042a1e3878aac6a571079ee3d518a5e649b0958deeefc`  
		Last Modified: Wed, 01 Mar 2023 13:03:11 GMT  
		Size: 6.6 MB (6579452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a247326076072850c80eb99fb5139cf988dc11020995fccdb020dc57e571c4`  
		Last Modified: Wed, 01 Mar 2023 13:03:11 GMT  
		Size: 1.2 MB (1164552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ace80db58c9be6fa388162aa3678dba8385d28f7022cba310faccebdbccc62b`  
		Last Modified: Wed, 01 Mar 2023 13:03:11 GMT  
		Size: 294.2 KB (294169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b11d35eeba918575d5c78b08bd873cb609e1dd7de4039ed4e7fde1a9655f6fee`  
		Last Modified: Wed, 01 Mar 2023 13:03:10 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913390e565908a1cde895cd2228112cbb865040a57aafcdbc70f3517216859a8`  
		Last Modified: Wed, 01 Mar 2023 13:03:13 GMT  
		Size: 41.1 MB (41125870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5405f7852d9ad5045236f53e4662f0356b00cada7d223812ab2aedc7e8b30b2e`  
		Last Modified: Wed, 01 Mar 2023 13:03:09 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c39ac9cf22dc7bc4a74a244936a8952f03b8fdf9868d67726adaa8072ba283`  
		Last Modified: Wed, 01 Mar 2023 13:03:09 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a51f93869e0195860058e9e05e4da9ecb1a8220ee4ff2e0454e3e423dc8e77f`  
		Last Modified: Wed, 01 Mar 2023 13:03:09 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e37b09e566e2d6ef8a535b536d4b6481bbc5ef7cb410313006ce11818af20e`  
		Last Modified: Wed, 01 Mar 2023 13:03:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2`

```console
$ docker pull couchdb@sha256:b38c2105b1f48eea4d5c9e73261c623520c2473cdb9901f69c1daa9498600cce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2` - linux; amd64

```console
$ docker pull couchdb@sha256:2aa2d4fad1a4a83c698112ba3a184c803e5015e4331a26d3c0dd43189f5312be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.6 MB (86593022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18fe84d4e9112bf81fc6af5e66ca0dcd8191a4adddc3c9a8d2cc0e3af6ee3685`
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
# Thu, 23 Mar 2023 06:14:11 GMT
COPY file:4f56a6457d04af3aef6fcaf07a864b915c40e6514919d19a783d4be98fe5bc89 in /usr/local/bin 
# Thu, 23 Mar 2023 06:14:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 06:14:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 06:14:12 GMT
VOLUME [/opt/couchdb/data]
# Thu, 23 Mar 2023 06:14:12 GMT
EXPOSE 4369 5984 9100
# Thu, 23 Mar 2023 06:14:12 GMT
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
	-	`sha256:787e97e060ac4e06721929197ebc59c32c255aaf00bf063ab51dc6567ebfe47b`  
		Last Modified: Thu, 23 Mar 2023 06:15:46 GMT  
		Size: 2.2 KB (2207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f10bc42743c5df9c947baa99e520dcada340d695b30090676138d9a02a6bb7`  
		Last Modified: Thu, 23 Mar 2023 06:15:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:c7bfa672b9850d10a0ef35eef0e933fea809d69b0ddc5eb3fede8a0a1633415b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.2 MB (85203417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5e723f0e0446fb3ecaf143e4f89b6e1f5a1de1679b062dc561fcf24ad894f5a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 13:00:43 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Mar 2023 13:00:44 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Mar 2023 13:00:50 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Mon, 20 Mar 2023 22:40:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Mon, 20 Mar 2023 22:40:34 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Mon, 20 Mar 2023 22:40:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Mon, 20 Mar 2023 22:40:59 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Mon, 20 Mar 2023 22:40:59 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Mon, 20 Mar 2023 22:41:10 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Mon, 20 Mar 2023 22:41:11 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Mon, 20 Mar 2023 22:41:11 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Mon, 20 Mar 2023 22:41:11 GMT
COPY file:4f56a6457d04af3aef6fcaf07a864b915c40e6514919d19a783d4be98fe5bc89 in /usr/local/bin 
# Mon, 20 Mar 2023 22:41:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Mon, 20 Mar 2023 22:41:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Mon, 20 Mar 2023 22:41:11 GMT
VOLUME [/opt/couchdb/data]
# Mon, 20 Mar 2023 22:41:12 GMT
EXPOSE 4369 5984 9100
# Mon, 20 Mar 2023 22:41:12 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5062435b3525c590327308b13c7117ff3a0462e7dd8ac2b02b934c832e0b6882`  
		Last Modified: Wed, 01 Mar 2023 13:02:41 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870190223a80d6ce34a8ac53a6aade325a75a20aeca43cbff5549ee2dcd3c1ad`  
		Last Modified: Wed, 01 Mar 2023 13:02:40 GMT  
		Size: 5.2 MB (5209450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e9863e93722978d8dc7bac8f1b64d8c91395ca199c458ffe489ce5be975dab`  
		Last Modified: Mon, 20 Mar 2023 22:41:36 GMT  
		Size: 566.3 KB (566255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7fe9ae8269843a8b140bbc16fe2e7b8db84126d2894b818a46695cf5d98ee9d`  
		Last Modified: Mon, 20 Mar 2023 22:41:36 GMT  
		Size: 294.3 KB (294264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11fa14a9dc768becb181b6eaec01357e7e625496b251b350e9f7e942f8a4641`  
		Last Modified: Mon, 20 Mar 2023 22:41:54 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22fbc84a5c7a3a8ecfad0b32c6dad18d008e55f3fd6bfe1b895883542f52a579`  
		Last Modified: Mon, 20 Mar 2023 22:41:56 GMT  
		Size: 49.1 MB (49063448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edff6ca058235d8ee0053b189875e31ad9466c259c5d3f2d3f3e1e219d773a01`  
		Last Modified: Mon, 20 Mar 2023 22:41:52 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85be94c4bdfc428632cfd534ab11ded24868bb8915af233fb75383ac0005e225`  
		Last Modified: Mon, 20 Mar 2023 22:41:52 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51893b49f1d197ad05c80d84d95823c616cc3946c55f9d3acbd49fe57446a59a`  
		Last Modified: Mon, 20 Mar 2023 22:41:52 GMT  
		Size: 2.2 KB (2208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704dfb9e82a1349c8c943679907d4ca82e7153ec12efc5ec4892b61272610e25`  
		Last Modified: Mon, 20 Mar 2023 22:41:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; ppc64le

```console
$ docker pull couchdb@sha256:fdeaf905d8a3b9d06e4e6849f93676f985ab16ac033ba5f5e587a426508baa7f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.4 MB (92380111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9738e44b7a76473ef2f322c46833148b6dace87a1aabe733cf1a302612db6e0e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:33 GMT
ADD file:6fdf0b2f8ea4be2d01e25a9d85db8f8c7e3b2a641c9c7665e34f4fad771815e0 in / 
# Wed, 01 Mar 2023 04:47:35 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:43:25 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Mar 2023 05:43:26 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Mar 2023 05:43:48 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Mon, 20 Mar 2023 22:16:34 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Mon, 20 Mar 2023 22:16:34 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Mon, 20 Mar 2023 22:16:47 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Mon, 20 Mar 2023 22:17:27 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Mon, 20 Mar 2023 22:17:28 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Mon, 20 Mar 2023 22:17:53 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Mon, 20 Mar 2023 22:17:55 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Mon, 20 Mar 2023 22:17:55 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Mon, 20 Mar 2023 22:17:56 GMT
COPY file:4f56a6457d04af3aef6fcaf07a864b915c40e6514919d19a783d4be98fe5bc89 in /usr/local/bin 
# Mon, 20 Mar 2023 22:17:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Mon, 20 Mar 2023 22:17:57 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Mon, 20 Mar 2023 22:17:58 GMT
VOLUME [/opt/couchdb/data]
# Mon, 20 Mar 2023 22:17:58 GMT
EXPOSE 4369 5984 9100
# Mon, 20 Mar 2023 22:17:58 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:93ab3a60c2a8cbc1150cb2bd54222db8b79c525c0243534a10d6294ef7ff83ac`  
		Last Modified: Wed, 01 Mar 2023 04:53:54 GMT  
		Size: 35.3 MB (35288103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7db168bb798ef118541ed78f0f09ab50044e5c6830937388a72cc43d78035b4`  
		Last Modified: Wed, 01 Mar 2023 05:46:05 GMT  
		Size: 3.4 KB (3415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b49f4851c4778b84f6d8d20589ed144f5d5aed34469fb055ba5961d658a92d`  
		Last Modified: Wed, 01 Mar 2023 05:46:05 GMT  
		Size: 6.0 MB (6043951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2842ad19ef92a090e8111ad7e88fcbf2c0fb50caec07709f50d634294c4ced5`  
		Last Modified: Mon, 20 Mar 2023 22:18:22 GMT  
		Size: 662.1 KB (662067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54475fcf0a17094179a6d5e3a9e1c1ff6aeb8e8a76da5630da72ba9c7164b9e5`  
		Last Modified: Mon, 20 Mar 2023 22:18:22 GMT  
		Size: 294.3 KB (294302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1734a252d77fb3688f52be57a07ad38abfe3bd07823ffd18d5a5c9117cd48ec8`  
		Last Modified: Mon, 20 Mar 2023 22:18:49 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350edebe1cd9eeb0ca6a9d595f5ee280a18d46d40285f34325e3ad0fb42b4a00`  
		Last Modified: Mon, 20 Mar 2023 22:18:56 GMT  
		Size: 50.1 MB (50084518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d090c1b025d577eeb6279984259e9d16d0e7abf6e8b476845319dea36ea2c1f1`  
		Last Modified: Mon, 20 Mar 2023 22:18:47 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e18b3fc4ebb659a720ba490d614a15d7eb339e495441e3e172cc20c3e855846`  
		Last Modified: Mon, 20 Mar 2023 22:18:47 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a26506d4fbff34e3d802de1e7be5fcfecd057b1404c7899c659c338d6822e13`  
		Last Modified: Mon, 20 Mar 2023 22:18:47 GMT  
		Size: 2.2 KB (2209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad9598fc836f16ec532e8c06f41968e61c307e00e5293be9aa729eb43f4a471`  
		Last Modified: Mon, 20 Mar 2023 22:18:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2.2`

```console
$ docker pull couchdb@sha256:b38c2105b1f48eea4d5c9e73261c623520c2473cdb9901f69c1daa9498600cce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2.2` - linux; amd64

```console
$ docker pull couchdb@sha256:2aa2d4fad1a4a83c698112ba3a184c803e5015e4331a26d3c0dd43189f5312be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.6 MB (86593022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18fe84d4e9112bf81fc6af5e66ca0dcd8191a4adddc3c9a8d2cc0e3af6ee3685`
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
# Thu, 23 Mar 2023 06:14:11 GMT
COPY file:4f56a6457d04af3aef6fcaf07a864b915c40e6514919d19a783d4be98fe5bc89 in /usr/local/bin 
# Thu, 23 Mar 2023 06:14:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 06:14:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 06:14:12 GMT
VOLUME [/opt/couchdb/data]
# Thu, 23 Mar 2023 06:14:12 GMT
EXPOSE 4369 5984 9100
# Thu, 23 Mar 2023 06:14:12 GMT
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
	-	`sha256:787e97e060ac4e06721929197ebc59c32c255aaf00bf063ab51dc6567ebfe47b`  
		Last Modified: Thu, 23 Mar 2023 06:15:46 GMT  
		Size: 2.2 KB (2207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f10bc42743c5df9c947baa99e520dcada340d695b30090676138d9a02a6bb7`  
		Last Modified: Thu, 23 Mar 2023 06:15:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:c7bfa672b9850d10a0ef35eef0e933fea809d69b0ddc5eb3fede8a0a1633415b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.2 MB (85203417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5e723f0e0446fb3ecaf143e4f89b6e1f5a1de1679b062dc561fcf24ad894f5a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 13:00:43 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Mar 2023 13:00:44 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Mar 2023 13:00:50 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Mon, 20 Mar 2023 22:40:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Mon, 20 Mar 2023 22:40:34 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Mon, 20 Mar 2023 22:40:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Mon, 20 Mar 2023 22:40:59 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Mon, 20 Mar 2023 22:40:59 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Mon, 20 Mar 2023 22:41:10 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Mon, 20 Mar 2023 22:41:11 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Mon, 20 Mar 2023 22:41:11 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Mon, 20 Mar 2023 22:41:11 GMT
COPY file:4f56a6457d04af3aef6fcaf07a864b915c40e6514919d19a783d4be98fe5bc89 in /usr/local/bin 
# Mon, 20 Mar 2023 22:41:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Mon, 20 Mar 2023 22:41:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Mon, 20 Mar 2023 22:41:11 GMT
VOLUME [/opt/couchdb/data]
# Mon, 20 Mar 2023 22:41:12 GMT
EXPOSE 4369 5984 9100
# Mon, 20 Mar 2023 22:41:12 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5062435b3525c590327308b13c7117ff3a0462e7dd8ac2b02b934c832e0b6882`  
		Last Modified: Wed, 01 Mar 2023 13:02:41 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870190223a80d6ce34a8ac53a6aade325a75a20aeca43cbff5549ee2dcd3c1ad`  
		Last Modified: Wed, 01 Mar 2023 13:02:40 GMT  
		Size: 5.2 MB (5209450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e9863e93722978d8dc7bac8f1b64d8c91395ca199c458ffe489ce5be975dab`  
		Last Modified: Mon, 20 Mar 2023 22:41:36 GMT  
		Size: 566.3 KB (566255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7fe9ae8269843a8b140bbc16fe2e7b8db84126d2894b818a46695cf5d98ee9d`  
		Last Modified: Mon, 20 Mar 2023 22:41:36 GMT  
		Size: 294.3 KB (294264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11fa14a9dc768becb181b6eaec01357e7e625496b251b350e9f7e942f8a4641`  
		Last Modified: Mon, 20 Mar 2023 22:41:54 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22fbc84a5c7a3a8ecfad0b32c6dad18d008e55f3fd6bfe1b895883542f52a579`  
		Last Modified: Mon, 20 Mar 2023 22:41:56 GMT  
		Size: 49.1 MB (49063448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edff6ca058235d8ee0053b189875e31ad9466c259c5d3f2d3f3e1e219d773a01`  
		Last Modified: Mon, 20 Mar 2023 22:41:52 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85be94c4bdfc428632cfd534ab11ded24868bb8915af233fb75383ac0005e225`  
		Last Modified: Mon, 20 Mar 2023 22:41:52 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51893b49f1d197ad05c80d84d95823c616cc3946c55f9d3acbd49fe57446a59a`  
		Last Modified: Mon, 20 Mar 2023 22:41:52 GMT  
		Size: 2.2 KB (2208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704dfb9e82a1349c8c943679907d4ca82e7153ec12efc5ec4892b61272610e25`  
		Last Modified: Mon, 20 Mar 2023 22:41:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2.2` - linux; ppc64le

```console
$ docker pull couchdb@sha256:fdeaf905d8a3b9d06e4e6849f93676f985ab16ac033ba5f5e587a426508baa7f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.4 MB (92380111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9738e44b7a76473ef2f322c46833148b6dace87a1aabe733cf1a302612db6e0e`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:33 GMT
ADD file:6fdf0b2f8ea4be2d01e25a9d85db8f8c7e3b2a641c9c7665e34f4fad771815e0 in / 
# Wed, 01 Mar 2023 04:47:35 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:43:25 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Mar 2023 05:43:26 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Mar 2023 05:43:48 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Mon, 20 Mar 2023 22:16:34 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Mon, 20 Mar 2023 22:16:34 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Mon, 20 Mar 2023 22:16:47 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Mon, 20 Mar 2023 22:17:27 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Mon, 20 Mar 2023 22:17:28 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Mon, 20 Mar 2023 22:17:53 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Mon, 20 Mar 2023 22:17:55 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Mon, 20 Mar 2023 22:17:55 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Mon, 20 Mar 2023 22:17:56 GMT
COPY file:4f56a6457d04af3aef6fcaf07a864b915c40e6514919d19a783d4be98fe5bc89 in /usr/local/bin 
# Mon, 20 Mar 2023 22:17:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Mon, 20 Mar 2023 22:17:57 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Mon, 20 Mar 2023 22:17:58 GMT
VOLUME [/opt/couchdb/data]
# Mon, 20 Mar 2023 22:17:58 GMT
EXPOSE 4369 5984 9100
# Mon, 20 Mar 2023 22:17:58 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:93ab3a60c2a8cbc1150cb2bd54222db8b79c525c0243534a10d6294ef7ff83ac`  
		Last Modified: Wed, 01 Mar 2023 04:53:54 GMT  
		Size: 35.3 MB (35288103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7db168bb798ef118541ed78f0f09ab50044e5c6830937388a72cc43d78035b4`  
		Last Modified: Wed, 01 Mar 2023 05:46:05 GMT  
		Size: 3.4 KB (3415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b49f4851c4778b84f6d8d20589ed144f5d5aed34469fb055ba5961d658a92d`  
		Last Modified: Wed, 01 Mar 2023 05:46:05 GMT  
		Size: 6.0 MB (6043951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2842ad19ef92a090e8111ad7e88fcbf2c0fb50caec07709f50d634294c4ced5`  
		Last Modified: Mon, 20 Mar 2023 22:18:22 GMT  
		Size: 662.1 KB (662067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54475fcf0a17094179a6d5e3a9e1c1ff6aeb8e8a76da5630da72ba9c7164b9e5`  
		Last Modified: Mon, 20 Mar 2023 22:18:22 GMT  
		Size: 294.3 KB (294302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1734a252d77fb3688f52be57a07ad38abfe3bd07823ffd18d5a5c9117cd48ec8`  
		Last Modified: Mon, 20 Mar 2023 22:18:49 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350edebe1cd9eeb0ca6a9d595f5ee280a18d46d40285f34325e3ad0fb42b4a00`  
		Last Modified: Mon, 20 Mar 2023 22:18:56 GMT  
		Size: 50.1 MB (50084518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d090c1b025d577eeb6279984259e9d16d0e7abf6e8b476845319dea36ea2c1f1`  
		Last Modified: Mon, 20 Mar 2023 22:18:47 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e18b3fc4ebb659a720ba490d614a15d7eb339e495441e3e172cc20c3e855846`  
		Last Modified: Mon, 20 Mar 2023 22:18:47 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a26506d4fbff34e3d802de1e7be5fcfecd057b1404c7899c659c338d6822e13`  
		Last Modified: Mon, 20 Mar 2023 22:18:47 GMT  
		Size: 2.2 KB (2209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad9598fc836f16ec532e8c06f41968e61c307e00e5293be9aa729eb43f4a471`  
		Last Modified: Mon, 20 Mar 2023 22:18:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.3`

```console
$ docker pull couchdb@sha256:6d2bb29aad3d6092f514cb1ce6b0d31f033ec55cb3ca04c37160a1b0cb04d933
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.3` - linux; amd64

```console
$ docker pull couchdb@sha256:b72b2cd30fafc137a82a790eeb975d9571ab80a1fb76052383ac8276df3d3adf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90222354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6444bc77edd5ec49ef56b16455e2679e4b0f07e542d31773b8b7bffccd1ebd40`
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
# Thu, 23 Mar 2023 06:13:52 GMT
COPY file:4f56a6457d04af3aef6fcaf07a864b915c40e6514919d19a783d4be98fe5bc89 in /usr/local/bin 
# Thu, 23 Mar 2023 06:13:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 06:13:53 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 06:13:53 GMT
VOLUME [/opt/couchdb/data]
# Thu, 23 Mar 2023 06:13:53 GMT
EXPOSE 4369 5984 9100
# Thu, 23 Mar 2023 06:13:53 GMT
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
	-	`sha256:6e9b6b12f4543e0688de9b6df3d5af367066f54097bdaac8c8f75323550c65e1`  
		Last Modified: Thu, 23 Mar 2023 06:15:28 GMT  
		Size: 2.2 KB (2206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70246ed49013058084013ec8e76bde438cdecc306fb6de20c01acab5a1d2074f`  
		Last Modified: Thu, 23 Mar 2023 06:15:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:5be64acf57d5f2991219ecf2e2e918f4053a6a4da203551e24bfd72c959b947e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88670295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b255331a1a6975bbf99a2262a7fc0d462d3f3c54e4ad114fd1463a0e2fb6e20a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 13:00:43 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Mar 2023 13:00:44 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Mar 2023 13:00:50 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Mon, 20 Mar 2023 22:40:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Mon, 20 Mar 2023 22:40:34 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Mon, 20 Mar 2023 22:40:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Mon, 20 Mar 2023 22:40:38 GMT
ENV COUCHDB_VERSION=3.3.1
# Mon, 20 Mar 2023 22:40:38 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Mon, 20 Mar 2023 22:40:52 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Mon, 20 Mar 2023 22:40:52 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Mon, 20 Mar 2023 22:40:52 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Mon, 20 Mar 2023 22:40:52 GMT
COPY file:4f56a6457d04af3aef6fcaf07a864b915c40e6514919d19a783d4be98fe5bc89 in /usr/local/bin 
# Mon, 20 Mar 2023 22:40:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Mon, 20 Mar 2023 22:40:53 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Mon, 20 Mar 2023 22:40:53 GMT
VOLUME [/opt/couchdb/data]
# Mon, 20 Mar 2023 22:40:53 GMT
EXPOSE 4369 5984 9100
# Mon, 20 Mar 2023 22:40:53 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5062435b3525c590327308b13c7117ff3a0462e7dd8ac2b02b934c832e0b6882`  
		Last Modified: Wed, 01 Mar 2023 13:02:41 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870190223a80d6ce34a8ac53a6aade325a75a20aeca43cbff5549ee2dcd3c1ad`  
		Last Modified: Wed, 01 Mar 2023 13:02:40 GMT  
		Size: 5.2 MB (5209450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e9863e93722978d8dc7bac8f1b64d8c91395ca199c458ffe489ce5be975dab`  
		Last Modified: Mon, 20 Mar 2023 22:41:36 GMT  
		Size: 566.3 KB (566255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7fe9ae8269843a8b140bbc16fe2e7b8db84126d2894b818a46695cf5d98ee9d`  
		Last Modified: Mon, 20 Mar 2023 22:41:36 GMT  
		Size: 294.3 KB (294264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4125d43b64e1ede5061372eac5d8d2b087312f7319996fb20974a85caa1ca2b6`  
		Last Modified: Mon, 20 Mar 2023 22:41:36 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfd880493a9e6cce11f45f67b70d9597f7b7548b6394536119699df09ffcfb0`  
		Last Modified: Mon, 20 Mar 2023 22:41:38 GMT  
		Size: 52.5 MB (52530089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a2dcece77541a2b77d9dfcdfec67a290de44f9aadf8142ef5c0a163ae1dca8`  
		Last Modified: Mon, 20 Mar 2023 22:41:34 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4026f83bc51c9945168f17b4cb18c4978c6854bd15b4df9dd224526d26a928e1`  
		Last Modified: Mon, 20 Mar 2023 22:41:34 GMT  
		Size: 997.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37dde701322e89f3b3989bb60176435c056116b6c1b9db6f4963eb6973b7ee1`  
		Last Modified: Mon, 20 Mar 2023 22:41:34 GMT  
		Size: 2.2 KB (2209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2c60e14e30c82431555c8e47192b288d36688c176e70425db6ee4270399a26`  
		Last Modified: Mon, 20 Mar 2023 22:41:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3` - linux; ppc64le

```console
$ docker pull couchdb@sha256:a61c3683b0ca2948f3078b89d06c1b75500eef5c74972583d5e44cda377ba776
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.8 MB (95829290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae9642c64a707353006d1cffecd1a7a4da3e2bd27829d533c4a337b10972083c`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:33 GMT
ADD file:6fdf0b2f8ea4be2d01e25a9d85db8f8c7e3b2a641c9c7665e34f4fad771815e0 in / 
# Wed, 01 Mar 2023 04:47:35 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:43:25 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Mar 2023 05:43:26 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Mar 2023 05:43:48 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Mon, 20 Mar 2023 22:16:34 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Mon, 20 Mar 2023 22:16:34 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Mon, 20 Mar 2023 22:16:47 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Mon, 20 Mar 2023 22:16:47 GMT
ENV COUCHDB_VERSION=3.3.1
# Mon, 20 Mar 2023 22:16:48 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Mon, 20 Mar 2023 22:17:13 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Mon, 20 Mar 2023 22:17:14 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Mon, 20 Mar 2023 22:17:15 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Mon, 20 Mar 2023 22:17:15 GMT
COPY file:4f56a6457d04af3aef6fcaf07a864b915c40e6514919d19a783d4be98fe5bc89 in /usr/local/bin 
# Mon, 20 Mar 2023 22:17:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Mon, 20 Mar 2023 22:17:16 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Mon, 20 Mar 2023 22:17:16 GMT
VOLUME [/opt/couchdb/data]
# Mon, 20 Mar 2023 22:17:17 GMT
EXPOSE 4369 5984 9100
# Mon, 20 Mar 2023 22:17:17 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:93ab3a60c2a8cbc1150cb2bd54222db8b79c525c0243534a10d6294ef7ff83ac`  
		Last Modified: Wed, 01 Mar 2023 04:53:54 GMT  
		Size: 35.3 MB (35288103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7db168bb798ef118541ed78f0f09ab50044e5c6830937388a72cc43d78035b4`  
		Last Modified: Wed, 01 Mar 2023 05:46:05 GMT  
		Size: 3.4 KB (3415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b49f4851c4778b84f6d8d20589ed144f5d5aed34469fb055ba5961d658a92d`  
		Last Modified: Wed, 01 Mar 2023 05:46:05 GMT  
		Size: 6.0 MB (6043951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2842ad19ef92a090e8111ad7e88fcbf2c0fb50caec07709f50d634294c4ced5`  
		Last Modified: Mon, 20 Mar 2023 22:18:22 GMT  
		Size: 662.1 KB (662067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54475fcf0a17094179a6d5e3a9e1c1ff6aeb8e8a76da5630da72ba9c7164b9e5`  
		Last Modified: Mon, 20 Mar 2023 22:18:22 GMT  
		Size: 294.3 KB (294302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35f095cf7b5e92264b86d71420ddf1ae59ea1ffd7e653fa4985df3a6b0ef42cf`  
		Last Modified: Mon, 20 Mar 2023 22:18:21 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1625cdce16d9ecdc3ebd8dee77f10730d1b98340f8a79deae3d9c9fbc626e013`  
		Last Modified: Mon, 20 Mar 2023 22:18:29 GMT  
		Size: 53.5 MB (53533461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602d60b8bd03fd76328fee3d9232ce007b6f489bd4186ab1e573332cafb27a55`  
		Last Modified: Mon, 20 Mar 2023 22:18:19 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5371246bf435da2d0007b058ada6946f5bd70333face6dba0a595e9695478eb0`  
		Last Modified: Mon, 20 Mar 2023 22:18:19 GMT  
		Size: 1.0 KB (1002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba84c938a14f7ecd134f28ac7951fcdb3c73179b7713659792f8c4e86a495180`  
		Last Modified: Mon, 20 Mar 2023 22:18:19 GMT  
		Size: 2.2 KB (2210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd777621cdc3f8f9dc7f220ac32bd3f8227860f932bb8462275d2f3597e0829`  
		Last Modified: Mon, 20 Mar 2023 22:18:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.3.1`

```console
$ docker pull couchdb@sha256:6d2bb29aad3d6092f514cb1ce6b0d31f033ec55cb3ca04c37160a1b0cb04d933
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:b72b2cd30fafc137a82a790eeb975d9571ab80a1fb76052383ac8276df3d3adf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90222354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6444bc77edd5ec49ef56b16455e2679e4b0f07e542d31773b8b7bffccd1ebd40`
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
# Thu, 23 Mar 2023 06:13:52 GMT
COPY file:4f56a6457d04af3aef6fcaf07a864b915c40e6514919d19a783d4be98fe5bc89 in /usr/local/bin 
# Thu, 23 Mar 2023 06:13:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 06:13:53 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 06:13:53 GMT
VOLUME [/opt/couchdb/data]
# Thu, 23 Mar 2023 06:13:53 GMT
EXPOSE 4369 5984 9100
# Thu, 23 Mar 2023 06:13:53 GMT
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
	-	`sha256:6e9b6b12f4543e0688de9b6df3d5af367066f54097bdaac8c8f75323550c65e1`  
		Last Modified: Thu, 23 Mar 2023 06:15:28 GMT  
		Size: 2.2 KB (2206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70246ed49013058084013ec8e76bde438cdecc306fb6de20c01acab5a1d2074f`  
		Last Modified: Thu, 23 Mar 2023 06:15:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:5be64acf57d5f2991219ecf2e2e918f4053a6a4da203551e24bfd72c959b947e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88670295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b255331a1a6975bbf99a2262a7fc0d462d3f3c54e4ad114fd1463a0e2fb6e20a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 13:00:43 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Mar 2023 13:00:44 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Mar 2023 13:00:50 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Mon, 20 Mar 2023 22:40:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Mon, 20 Mar 2023 22:40:34 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Mon, 20 Mar 2023 22:40:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Mon, 20 Mar 2023 22:40:38 GMT
ENV COUCHDB_VERSION=3.3.1
# Mon, 20 Mar 2023 22:40:38 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Mon, 20 Mar 2023 22:40:52 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Mon, 20 Mar 2023 22:40:52 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Mon, 20 Mar 2023 22:40:52 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Mon, 20 Mar 2023 22:40:52 GMT
COPY file:4f56a6457d04af3aef6fcaf07a864b915c40e6514919d19a783d4be98fe5bc89 in /usr/local/bin 
# Mon, 20 Mar 2023 22:40:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Mon, 20 Mar 2023 22:40:53 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Mon, 20 Mar 2023 22:40:53 GMT
VOLUME [/opt/couchdb/data]
# Mon, 20 Mar 2023 22:40:53 GMT
EXPOSE 4369 5984 9100
# Mon, 20 Mar 2023 22:40:53 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5062435b3525c590327308b13c7117ff3a0462e7dd8ac2b02b934c832e0b6882`  
		Last Modified: Wed, 01 Mar 2023 13:02:41 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870190223a80d6ce34a8ac53a6aade325a75a20aeca43cbff5549ee2dcd3c1ad`  
		Last Modified: Wed, 01 Mar 2023 13:02:40 GMT  
		Size: 5.2 MB (5209450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e9863e93722978d8dc7bac8f1b64d8c91395ca199c458ffe489ce5be975dab`  
		Last Modified: Mon, 20 Mar 2023 22:41:36 GMT  
		Size: 566.3 KB (566255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7fe9ae8269843a8b140bbc16fe2e7b8db84126d2894b818a46695cf5d98ee9d`  
		Last Modified: Mon, 20 Mar 2023 22:41:36 GMT  
		Size: 294.3 KB (294264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4125d43b64e1ede5061372eac5d8d2b087312f7319996fb20974a85caa1ca2b6`  
		Last Modified: Mon, 20 Mar 2023 22:41:36 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfd880493a9e6cce11f45f67b70d9597f7b7548b6394536119699df09ffcfb0`  
		Last Modified: Mon, 20 Mar 2023 22:41:38 GMT  
		Size: 52.5 MB (52530089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a2dcece77541a2b77d9dfcdfec67a290de44f9aadf8142ef5c0a163ae1dca8`  
		Last Modified: Mon, 20 Mar 2023 22:41:34 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4026f83bc51c9945168f17b4cb18c4978c6854bd15b4df9dd224526d26a928e1`  
		Last Modified: Mon, 20 Mar 2023 22:41:34 GMT  
		Size: 997.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37dde701322e89f3b3989bb60176435c056116b6c1b9db6f4963eb6973b7ee1`  
		Last Modified: Mon, 20 Mar 2023 22:41:34 GMT  
		Size: 2.2 KB (2209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2c60e14e30c82431555c8e47192b288d36688c176e70425db6ee4270399a26`  
		Last Modified: Mon, 20 Mar 2023 22:41:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3.1` - linux; ppc64le

```console
$ docker pull couchdb@sha256:a61c3683b0ca2948f3078b89d06c1b75500eef5c74972583d5e44cda377ba776
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.8 MB (95829290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae9642c64a707353006d1cffecd1a7a4da3e2bd27829d533c4a337b10972083c`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:33 GMT
ADD file:6fdf0b2f8ea4be2d01e25a9d85db8f8c7e3b2a641c9c7665e34f4fad771815e0 in / 
# Wed, 01 Mar 2023 04:47:35 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:43:25 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Mar 2023 05:43:26 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Mar 2023 05:43:48 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Mon, 20 Mar 2023 22:16:34 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Mon, 20 Mar 2023 22:16:34 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Mon, 20 Mar 2023 22:16:47 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Mon, 20 Mar 2023 22:16:47 GMT
ENV COUCHDB_VERSION=3.3.1
# Mon, 20 Mar 2023 22:16:48 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Mon, 20 Mar 2023 22:17:13 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Mon, 20 Mar 2023 22:17:14 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Mon, 20 Mar 2023 22:17:15 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Mon, 20 Mar 2023 22:17:15 GMT
COPY file:4f56a6457d04af3aef6fcaf07a864b915c40e6514919d19a783d4be98fe5bc89 in /usr/local/bin 
# Mon, 20 Mar 2023 22:17:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Mon, 20 Mar 2023 22:17:16 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Mon, 20 Mar 2023 22:17:16 GMT
VOLUME [/opt/couchdb/data]
# Mon, 20 Mar 2023 22:17:17 GMT
EXPOSE 4369 5984 9100
# Mon, 20 Mar 2023 22:17:17 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:93ab3a60c2a8cbc1150cb2bd54222db8b79c525c0243534a10d6294ef7ff83ac`  
		Last Modified: Wed, 01 Mar 2023 04:53:54 GMT  
		Size: 35.3 MB (35288103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7db168bb798ef118541ed78f0f09ab50044e5c6830937388a72cc43d78035b4`  
		Last Modified: Wed, 01 Mar 2023 05:46:05 GMT  
		Size: 3.4 KB (3415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b49f4851c4778b84f6d8d20589ed144f5d5aed34469fb055ba5961d658a92d`  
		Last Modified: Wed, 01 Mar 2023 05:46:05 GMT  
		Size: 6.0 MB (6043951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2842ad19ef92a090e8111ad7e88fcbf2c0fb50caec07709f50d634294c4ced5`  
		Last Modified: Mon, 20 Mar 2023 22:18:22 GMT  
		Size: 662.1 KB (662067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54475fcf0a17094179a6d5e3a9e1c1ff6aeb8e8a76da5630da72ba9c7164b9e5`  
		Last Modified: Mon, 20 Mar 2023 22:18:22 GMT  
		Size: 294.3 KB (294302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35f095cf7b5e92264b86d71420ddf1ae59ea1ffd7e653fa4985df3a6b0ef42cf`  
		Last Modified: Mon, 20 Mar 2023 22:18:21 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1625cdce16d9ecdc3ebd8dee77f10730d1b98340f8a79deae3d9c9fbc626e013`  
		Last Modified: Mon, 20 Mar 2023 22:18:29 GMT  
		Size: 53.5 MB (53533461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602d60b8bd03fd76328fee3d9232ce007b6f489bd4186ab1e573332cafb27a55`  
		Last Modified: Mon, 20 Mar 2023 22:18:19 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5371246bf435da2d0007b058ada6946f5bd70333face6dba0a595e9695478eb0`  
		Last Modified: Mon, 20 Mar 2023 22:18:19 GMT  
		Size: 1.0 KB (1002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba84c938a14f7ecd134f28ac7951fcdb3c73179b7713659792f8c4e86a495180`  
		Last Modified: Mon, 20 Mar 2023 22:18:19 GMT  
		Size: 2.2 KB (2210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd777621cdc3f8f9dc7f220ac32bd3f8227860f932bb8462275d2f3597e0829`  
		Last Modified: Mon, 20 Mar 2023 22:18:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:latest`

```console
$ docker pull couchdb@sha256:6d2bb29aad3d6092f514cb1ce6b0d31f033ec55cb3ca04c37160a1b0cb04d933
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:b72b2cd30fafc137a82a790eeb975d9571ab80a1fb76052383ac8276df3d3adf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.2 MB (90222354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6444bc77edd5ec49ef56b16455e2679e4b0f07e542d31773b8b7bffccd1ebd40`
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
# Thu, 23 Mar 2023 06:13:52 GMT
COPY file:4f56a6457d04af3aef6fcaf07a864b915c40e6514919d19a783d4be98fe5bc89 in /usr/local/bin 
# Thu, 23 Mar 2023 06:13:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 23 Mar 2023 06:13:53 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 23 Mar 2023 06:13:53 GMT
VOLUME [/opt/couchdb/data]
# Thu, 23 Mar 2023 06:13:53 GMT
EXPOSE 4369 5984 9100
# Thu, 23 Mar 2023 06:13:53 GMT
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
	-	`sha256:6e9b6b12f4543e0688de9b6df3d5af367066f54097bdaac8c8f75323550c65e1`  
		Last Modified: Thu, 23 Mar 2023 06:15:28 GMT  
		Size: 2.2 KB (2206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70246ed49013058084013ec8e76bde438cdecc306fb6de20c01acab5a1d2074f`  
		Last Modified: Thu, 23 Mar 2023 06:15:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:5be64acf57d5f2991219ecf2e2e918f4053a6a4da203551e24bfd72c959b947e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88670295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b255331a1a6975bbf99a2262a7fc0d462d3f3c54e4ad114fd1463a0e2fb6e20a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 13:00:43 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Mar 2023 13:00:44 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Mar 2023 13:00:50 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Mon, 20 Mar 2023 22:40:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Mon, 20 Mar 2023 22:40:34 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Mon, 20 Mar 2023 22:40:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Mon, 20 Mar 2023 22:40:38 GMT
ENV COUCHDB_VERSION=3.3.1
# Mon, 20 Mar 2023 22:40:38 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Mon, 20 Mar 2023 22:40:52 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Mon, 20 Mar 2023 22:40:52 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Mon, 20 Mar 2023 22:40:52 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Mon, 20 Mar 2023 22:40:52 GMT
COPY file:4f56a6457d04af3aef6fcaf07a864b915c40e6514919d19a783d4be98fe5bc89 in /usr/local/bin 
# Mon, 20 Mar 2023 22:40:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Mon, 20 Mar 2023 22:40:53 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Mon, 20 Mar 2023 22:40:53 GMT
VOLUME [/opt/couchdb/data]
# Mon, 20 Mar 2023 22:40:53 GMT
EXPOSE 4369 5984 9100
# Mon, 20 Mar 2023 22:40:53 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5062435b3525c590327308b13c7117ff3a0462e7dd8ac2b02b934c832e0b6882`  
		Last Modified: Wed, 01 Mar 2023 13:02:41 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870190223a80d6ce34a8ac53a6aade325a75a20aeca43cbff5549ee2dcd3c1ad`  
		Last Modified: Wed, 01 Mar 2023 13:02:40 GMT  
		Size: 5.2 MB (5209450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e9863e93722978d8dc7bac8f1b64d8c91395ca199c458ffe489ce5be975dab`  
		Last Modified: Mon, 20 Mar 2023 22:41:36 GMT  
		Size: 566.3 KB (566255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7fe9ae8269843a8b140bbc16fe2e7b8db84126d2894b818a46695cf5d98ee9d`  
		Last Modified: Mon, 20 Mar 2023 22:41:36 GMT  
		Size: 294.3 KB (294264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4125d43b64e1ede5061372eac5d8d2b087312f7319996fb20974a85caa1ca2b6`  
		Last Modified: Mon, 20 Mar 2023 22:41:36 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfd880493a9e6cce11f45f67b70d9597f7b7548b6394536119699df09ffcfb0`  
		Last Modified: Mon, 20 Mar 2023 22:41:38 GMT  
		Size: 52.5 MB (52530089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a2dcece77541a2b77d9dfcdfec67a290de44f9aadf8142ef5c0a163ae1dca8`  
		Last Modified: Mon, 20 Mar 2023 22:41:34 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4026f83bc51c9945168f17b4cb18c4978c6854bd15b4df9dd224526d26a928e1`  
		Last Modified: Mon, 20 Mar 2023 22:41:34 GMT  
		Size: 997.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37dde701322e89f3b3989bb60176435c056116b6c1b9db6f4963eb6973b7ee1`  
		Last Modified: Mon, 20 Mar 2023 22:41:34 GMT  
		Size: 2.2 KB (2209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2c60e14e30c82431555c8e47192b288d36688c176e70425db6ee4270399a26`  
		Last Modified: Mon, 20 Mar 2023 22:41:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; ppc64le

```console
$ docker pull couchdb@sha256:a61c3683b0ca2948f3078b89d06c1b75500eef5c74972583d5e44cda377ba776
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.8 MB (95829290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae9642c64a707353006d1cffecd1a7a4da3e2bd27829d533c4a337b10972083c`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:33 GMT
ADD file:6fdf0b2f8ea4be2d01e25a9d85db8f8c7e3b2a641c9c7665e34f4fad771815e0 in / 
# Wed, 01 Mar 2023 04:47:35 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 05:43:25 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Mar 2023 05:43:26 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Mar 2023 05:43:48 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Mon, 20 Mar 2023 22:16:34 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Mon, 20 Mar 2023 22:16:34 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Mon, 20 Mar 2023 22:16:47 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Mon, 20 Mar 2023 22:16:47 GMT
ENV COUCHDB_VERSION=3.3.1
# Mon, 20 Mar 2023 22:16:48 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Mon, 20 Mar 2023 22:17:13 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Mon, 20 Mar 2023 22:17:14 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Mon, 20 Mar 2023 22:17:15 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Mon, 20 Mar 2023 22:17:15 GMT
COPY file:4f56a6457d04af3aef6fcaf07a864b915c40e6514919d19a783d4be98fe5bc89 in /usr/local/bin 
# Mon, 20 Mar 2023 22:17:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Mon, 20 Mar 2023 22:17:16 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Mon, 20 Mar 2023 22:17:16 GMT
VOLUME [/opt/couchdb/data]
# Mon, 20 Mar 2023 22:17:17 GMT
EXPOSE 4369 5984 9100
# Mon, 20 Mar 2023 22:17:17 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:93ab3a60c2a8cbc1150cb2bd54222db8b79c525c0243534a10d6294ef7ff83ac`  
		Last Modified: Wed, 01 Mar 2023 04:53:54 GMT  
		Size: 35.3 MB (35288103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7db168bb798ef118541ed78f0f09ab50044e5c6830937388a72cc43d78035b4`  
		Last Modified: Wed, 01 Mar 2023 05:46:05 GMT  
		Size: 3.4 KB (3415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b49f4851c4778b84f6d8d20589ed144f5d5aed34469fb055ba5961d658a92d`  
		Last Modified: Wed, 01 Mar 2023 05:46:05 GMT  
		Size: 6.0 MB (6043951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2842ad19ef92a090e8111ad7e88fcbf2c0fb50caec07709f50d634294c4ced5`  
		Last Modified: Mon, 20 Mar 2023 22:18:22 GMT  
		Size: 662.1 KB (662067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54475fcf0a17094179a6d5e3a9e1c1ff6aeb8e8a76da5630da72ba9c7164b9e5`  
		Last Modified: Mon, 20 Mar 2023 22:18:22 GMT  
		Size: 294.3 KB (294302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35f095cf7b5e92264b86d71420ddf1ae59ea1ffd7e653fa4985df3a6b0ef42cf`  
		Last Modified: Mon, 20 Mar 2023 22:18:21 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1625cdce16d9ecdc3ebd8dee77f10730d1b98340f8a79deae3d9c9fbc626e013`  
		Last Modified: Mon, 20 Mar 2023 22:18:29 GMT  
		Size: 53.5 MB (53533461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602d60b8bd03fd76328fee3d9232ce007b6f489bd4186ab1e573332cafb27a55`  
		Last Modified: Mon, 20 Mar 2023 22:18:19 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5371246bf435da2d0007b058ada6946f5bd70333face6dba0a595e9695478eb0`  
		Last Modified: Mon, 20 Mar 2023 22:18:19 GMT  
		Size: 1.0 KB (1002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba84c938a14f7ecd134f28ac7951fcdb3c73179b7713659792f8c4e86a495180`  
		Last Modified: Mon, 20 Mar 2023 22:18:19 GMT  
		Size: 2.2 KB (2210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd777621cdc3f8f9dc7f220ac32bd3f8227860f932bb8462275d2f3597e0829`  
		Last Modified: Mon, 20 Mar 2023 22:18:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
