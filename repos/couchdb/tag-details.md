<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `couchdb`

-	[`couchdb:2`](#couchdb2)
-	[`couchdb:2.3`](#couchdb23)
-	[`couchdb:2.3.1`](#couchdb231)
-	[`couchdb:3`](#couchdb3)
-	[`couchdb:3.1`](#couchdb31)
-	[`couchdb:3.1.2`](#couchdb312)
-	[`couchdb:3.2`](#couchdb32)
-	[`couchdb:3.2.0`](#couchdb320)
-	[`couchdb:latest`](#couchdblatest)

## `couchdb:2`

```console
$ docker pull couchdb@sha256:5c11c1b07e3f34b477c6b2a6c9beab86847234d146243a3176d78d2dbcf96a73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2` - linux; amd64

```console
$ docker pull couchdb@sha256:d88f859b0e2d27a94bd6862849a6a0fba3d10d7b2c0aeb79b8c2c5ac2dabf651
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84502946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82ec8a29dd01e00c0d102328f515fe8adc9bda383e5a3db59d5d0fb3c1038879`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 12:32:07 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 12 Oct 2021 12:32:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 12 Oct 2021 12:32:18 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:32:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 12 Oct 2021 12:32:22 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 12 Oct 2021 12:32:29 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:33:14 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 12 Oct 2021 12:33:15 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 12 Oct 2021 12:33:33 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 12 Oct 2021 12:33:34 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 12 Oct 2021 12:33:34 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 12 Oct 2021 12:33:34 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 12 Oct 2021 12:33:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 12 Oct 2021 12:33:35 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 12:33:36 GMT
VOLUME [/opt/couchdb/data]
# Tue, 12 Oct 2021 12:33:36 GMT
EXPOSE 4369 5984 9100
# Tue, 12 Oct 2021 12:33:36 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a46377fe8ce67057386a4c7aa933b926be606ba3070c3342e42f63e68d052c`  
		Last Modified: Tue, 12 Oct 2021 12:34:00 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4bf1b8a9bee200ee03e321a3d81949a87a559329ccffe9da773bd2d9d09fab`  
		Last Modified: Tue, 12 Oct 2021 12:34:00 GMT  
		Size: 6.7 MB (6691348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59081fa6a5d78e2274b9368f09dff77dc9e27812416dc235da1682d043b6129d`  
		Last Modified: Tue, 12 Oct 2021 12:33:58 GMT  
		Size: 1.3 MB (1258348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc87af85d712b9d439d847c5575c30770dcd0910cd5aea578135b4a2d4e5f16e`  
		Last Modified: Tue, 12 Oct 2021 12:33:58 GMT  
		Size: 293.0 KB (292995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81eb406db451bbcfa9ec9d447c1262d9b9d20b830136f5310aa2af479e7c8612`  
		Last Modified: Tue, 12 Oct 2021 12:34:35 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc319e2994b8d2619b9216755ca3e9950d86fa85073fce0b349fa8b385640a0`  
		Last Modified: Tue, 12 Oct 2021 12:34:40 GMT  
		Size: 49.1 MB (49113726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d21da0b575b0674310c4d5f47ed094df2abac3d16714fe1e4f1cf77a86264bf`  
		Last Modified: Tue, 12 Oct 2021 12:34:33 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c546c3ea3ffcd2faa2227c1e3effe181f868847e8e06e0851a2c9dbfabad510`  
		Last Modified: Tue, 12 Oct 2021 12:34:33 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc90b95b675d3c59325b31adebcf8db7d307f6219ecdf4261d2dbb0d726fb9c6`  
		Last Modified: Tue, 12 Oct 2021 12:34:33 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707fc9e3679465e141fed2979b76f9e3f5cc9e21a12f0e1c875ea0e5a341eca6`  
		Last Modified: Tue, 12 Oct 2021 12:34:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:d3eb044e7a1d13ce4195c3451c110c48ef3076438dc61d111670f83966e65bfa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72934615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:590cae5e85151c6228ca646e239503f7fedc56335a729b21cc4419ca32c70350`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:12:13 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 12 Oct 2021 16:12:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 12 Oct 2021 16:12:21 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:12:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 12 Oct 2021 16:12:25 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 12 Oct 2021 16:12:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:13:15 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 12 Oct 2021 16:13:16 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 12 Oct 2021 16:13:28 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 12 Oct 2021 16:13:29 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 12 Oct 2021 16:13:29 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 12 Oct 2021 16:13:29 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 12 Oct 2021 16:13:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 12 Oct 2021 16:13:30 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 16:13:30 GMT
VOLUME [/opt/couchdb/data]
# Tue, 12 Oct 2021 16:13:30 GMT
EXPOSE 4369 5984 9100
# Tue, 12 Oct 2021 16:13:31 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c646791d9868995e805f149bec168431525d3c31b3d0c73124e5a37e4afa76f`  
		Last Modified: Tue, 12 Oct 2021 16:14:03 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836357709ccd6570063bff28686a586c566ca7145e0adb10db6ca88966f4095e`  
		Last Modified: Tue, 12 Oct 2021 16:14:03 GMT  
		Size: 6.6 MB (6550798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7164389db8f0224aead9715f7478a90fb8d0612a43377991018342353359def`  
		Last Modified: Tue, 12 Oct 2021 16:14:02 GMT  
		Size: 1.2 MB (1163463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4097cf55145d3e6941810229afc94a987195c0631cc4d532dd62be1d1db8cae4`  
		Last Modified: Tue, 12 Oct 2021 16:14:01 GMT  
		Size: 292.9 KB (292852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819833447177af7e5beef2f993dd07950e209f2e7b8dd0bfcaf8ef739bc088a0`  
		Last Modified: Tue, 12 Oct 2021 16:14:43 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768c44619b6333fe354d3dcde3d3d7da5ace8c1c76182d6f142aa1dac4801bb9`  
		Last Modified: Tue, 12 Oct 2021 16:14:46 GMT  
		Size: 39.0 MB (39011980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ea5fc0628a1cc34aa10c0c42a21cc83abb67d3d90816c3c55278d58a3d0bb7`  
		Last Modified: Tue, 12 Oct 2021 16:14:40 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927ce1cccfe88f86c96cdcb9b630eabdbee8c1af572172401ec4899f84cc7ca8`  
		Last Modified: Tue, 12 Oct 2021 16:14:40 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989a6997d79c5f14c8b41d4c66a51de7b22c3ba365f72d4047f9b3f0062a0e1c`  
		Last Modified: Tue, 12 Oct 2021 16:14:41 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6104cd0db80895a588fa6f86859fe0d9590821f0911a4e262cf2afa998c137`  
		Last Modified: Tue, 12 Oct 2021 16:14:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3`

```console
$ docker pull couchdb@sha256:5c11c1b07e3f34b477c6b2a6c9beab86847234d146243a3176d78d2dbcf96a73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:d88f859b0e2d27a94bd6862849a6a0fba3d10d7b2c0aeb79b8c2c5ac2dabf651
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84502946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82ec8a29dd01e00c0d102328f515fe8adc9bda383e5a3db59d5d0fb3c1038879`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 12:32:07 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 12 Oct 2021 12:32:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 12 Oct 2021 12:32:18 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:32:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 12 Oct 2021 12:32:22 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 12 Oct 2021 12:32:29 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:33:14 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 12 Oct 2021 12:33:15 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 12 Oct 2021 12:33:33 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 12 Oct 2021 12:33:34 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 12 Oct 2021 12:33:34 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 12 Oct 2021 12:33:34 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 12 Oct 2021 12:33:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 12 Oct 2021 12:33:35 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 12:33:36 GMT
VOLUME [/opt/couchdb/data]
# Tue, 12 Oct 2021 12:33:36 GMT
EXPOSE 4369 5984 9100
# Tue, 12 Oct 2021 12:33:36 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a46377fe8ce67057386a4c7aa933b926be606ba3070c3342e42f63e68d052c`  
		Last Modified: Tue, 12 Oct 2021 12:34:00 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4bf1b8a9bee200ee03e321a3d81949a87a559329ccffe9da773bd2d9d09fab`  
		Last Modified: Tue, 12 Oct 2021 12:34:00 GMT  
		Size: 6.7 MB (6691348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59081fa6a5d78e2274b9368f09dff77dc9e27812416dc235da1682d043b6129d`  
		Last Modified: Tue, 12 Oct 2021 12:33:58 GMT  
		Size: 1.3 MB (1258348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc87af85d712b9d439d847c5575c30770dcd0910cd5aea578135b4a2d4e5f16e`  
		Last Modified: Tue, 12 Oct 2021 12:33:58 GMT  
		Size: 293.0 KB (292995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81eb406db451bbcfa9ec9d447c1262d9b9d20b830136f5310aa2af479e7c8612`  
		Last Modified: Tue, 12 Oct 2021 12:34:35 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc319e2994b8d2619b9216755ca3e9950d86fa85073fce0b349fa8b385640a0`  
		Last Modified: Tue, 12 Oct 2021 12:34:40 GMT  
		Size: 49.1 MB (49113726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d21da0b575b0674310c4d5f47ed094df2abac3d16714fe1e4f1cf77a86264bf`  
		Last Modified: Tue, 12 Oct 2021 12:34:33 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c546c3ea3ffcd2faa2227c1e3effe181f868847e8e06e0851a2c9dbfabad510`  
		Last Modified: Tue, 12 Oct 2021 12:34:33 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc90b95b675d3c59325b31adebcf8db7d307f6219ecdf4261d2dbb0d726fb9c6`  
		Last Modified: Tue, 12 Oct 2021 12:34:33 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707fc9e3679465e141fed2979b76f9e3f5cc9e21a12f0e1c875ea0e5a341eca6`  
		Last Modified: Tue, 12 Oct 2021 12:34:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:d3eb044e7a1d13ce4195c3451c110c48ef3076438dc61d111670f83966e65bfa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72934615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:590cae5e85151c6228ca646e239503f7fedc56335a729b21cc4419ca32c70350`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:12:13 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 12 Oct 2021 16:12:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 12 Oct 2021 16:12:21 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:12:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 12 Oct 2021 16:12:25 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 12 Oct 2021 16:12:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:13:15 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 12 Oct 2021 16:13:16 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 12 Oct 2021 16:13:28 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 12 Oct 2021 16:13:29 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 12 Oct 2021 16:13:29 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 12 Oct 2021 16:13:29 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 12 Oct 2021 16:13:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 12 Oct 2021 16:13:30 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 16:13:30 GMT
VOLUME [/opt/couchdb/data]
# Tue, 12 Oct 2021 16:13:30 GMT
EXPOSE 4369 5984 9100
# Tue, 12 Oct 2021 16:13:31 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c646791d9868995e805f149bec168431525d3c31b3d0c73124e5a37e4afa76f`  
		Last Modified: Tue, 12 Oct 2021 16:14:03 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836357709ccd6570063bff28686a586c566ca7145e0adb10db6ca88966f4095e`  
		Last Modified: Tue, 12 Oct 2021 16:14:03 GMT  
		Size: 6.6 MB (6550798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7164389db8f0224aead9715f7478a90fb8d0612a43377991018342353359def`  
		Last Modified: Tue, 12 Oct 2021 16:14:02 GMT  
		Size: 1.2 MB (1163463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4097cf55145d3e6941810229afc94a987195c0631cc4d532dd62be1d1db8cae4`  
		Last Modified: Tue, 12 Oct 2021 16:14:01 GMT  
		Size: 292.9 KB (292852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819833447177af7e5beef2f993dd07950e209f2e7b8dd0bfcaf8ef739bc088a0`  
		Last Modified: Tue, 12 Oct 2021 16:14:43 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768c44619b6333fe354d3dcde3d3d7da5ace8c1c76182d6f142aa1dac4801bb9`  
		Last Modified: Tue, 12 Oct 2021 16:14:46 GMT  
		Size: 39.0 MB (39011980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ea5fc0628a1cc34aa10c0c42a21cc83abb67d3d90816c3c55278d58a3d0bb7`  
		Last Modified: Tue, 12 Oct 2021 16:14:40 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927ce1cccfe88f86c96cdcb9b630eabdbee8c1af572172401ec4899f84cc7ca8`  
		Last Modified: Tue, 12 Oct 2021 16:14:40 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989a6997d79c5f14c8b41d4c66a51de7b22c3ba365f72d4047f9b3f0062a0e1c`  
		Last Modified: Tue, 12 Oct 2021 16:14:41 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6104cd0db80895a588fa6f86859fe0d9590821f0911a4e262cf2afa998c137`  
		Last Modified: Tue, 12 Oct 2021 16:14:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3.1`

```console
$ docker pull couchdb@sha256:5c11c1b07e3f34b477c6b2a6c9beab86847234d146243a3176d78d2dbcf96a73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:d88f859b0e2d27a94bd6862849a6a0fba3d10d7b2c0aeb79b8c2c5ac2dabf651
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84502946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82ec8a29dd01e00c0d102328f515fe8adc9bda383e5a3db59d5d0fb3c1038879`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 12:32:07 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 12 Oct 2021 12:32:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 12 Oct 2021 12:32:18 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:32:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 12 Oct 2021 12:32:22 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 12 Oct 2021 12:32:29 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:33:14 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 12 Oct 2021 12:33:15 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 12 Oct 2021 12:33:33 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 12 Oct 2021 12:33:34 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 12 Oct 2021 12:33:34 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 12 Oct 2021 12:33:34 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 12 Oct 2021 12:33:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 12 Oct 2021 12:33:35 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 12:33:36 GMT
VOLUME [/opt/couchdb/data]
# Tue, 12 Oct 2021 12:33:36 GMT
EXPOSE 4369 5984 9100
# Tue, 12 Oct 2021 12:33:36 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a46377fe8ce67057386a4c7aa933b926be606ba3070c3342e42f63e68d052c`  
		Last Modified: Tue, 12 Oct 2021 12:34:00 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4bf1b8a9bee200ee03e321a3d81949a87a559329ccffe9da773bd2d9d09fab`  
		Last Modified: Tue, 12 Oct 2021 12:34:00 GMT  
		Size: 6.7 MB (6691348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59081fa6a5d78e2274b9368f09dff77dc9e27812416dc235da1682d043b6129d`  
		Last Modified: Tue, 12 Oct 2021 12:33:58 GMT  
		Size: 1.3 MB (1258348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc87af85d712b9d439d847c5575c30770dcd0910cd5aea578135b4a2d4e5f16e`  
		Last Modified: Tue, 12 Oct 2021 12:33:58 GMT  
		Size: 293.0 KB (292995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81eb406db451bbcfa9ec9d447c1262d9b9d20b830136f5310aa2af479e7c8612`  
		Last Modified: Tue, 12 Oct 2021 12:34:35 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc319e2994b8d2619b9216755ca3e9950d86fa85073fce0b349fa8b385640a0`  
		Last Modified: Tue, 12 Oct 2021 12:34:40 GMT  
		Size: 49.1 MB (49113726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d21da0b575b0674310c4d5f47ed094df2abac3d16714fe1e4f1cf77a86264bf`  
		Last Modified: Tue, 12 Oct 2021 12:34:33 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c546c3ea3ffcd2faa2227c1e3effe181f868847e8e06e0851a2c9dbfabad510`  
		Last Modified: Tue, 12 Oct 2021 12:34:33 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc90b95b675d3c59325b31adebcf8db7d307f6219ecdf4261d2dbb0d726fb9c6`  
		Last Modified: Tue, 12 Oct 2021 12:34:33 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707fc9e3679465e141fed2979b76f9e3f5cc9e21a12f0e1c875ea0e5a341eca6`  
		Last Modified: Tue, 12 Oct 2021 12:34:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:d3eb044e7a1d13ce4195c3451c110c48ef3076438dc61d111670f83966e65bfa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72934615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:590cae5e85151c6228ca646e239503f7fedc56335a729b21cc4419ca32c70350`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:12:13 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 12 Oct 2021 16:12:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 12 Oct 2021 16:12:21 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:12:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 12 Oct 2021 16:12:25 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 12 Oct 2021 16:12:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:13:15 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 12 Oct 2021 16:13:16 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 12 Oct 2021 16:13:28 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 12 Oct 2021 16:13:29 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 12 Oct 2021 16:13:29 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 12 Oct 2021 16:13:29 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 12 Oct 2021 16:13:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 12 Oct 2021 16:13:30 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 16:13:30 GMT
VOLUME [/opt/couchdb/data]
# Tue, 12 Oct 2021 16:13:30 GMT
EXPOSE 4369 5984 9100
# Tue, 12 Oct 2021 16:13:31 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c646791d9868995e805f149bec168431525d3c31b3d0c73124e5a37e4afa76f`  
		Last Modified: Tue, 12 Oct 2021 16:14:03 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836357709ccd6570063bff28686a586c566ca7145e0adb10db6ca88966f4095e`  
		Last Modified: Tue, 12 Oct 2021 16:14:03 GMT  
		Size: 6.6 MB (6550798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7164389db8f0224aead9715f7478a90fb8d0612a43377991018342353359def`  
		Last Modified: Tue, 12 Oct 2021 16:14:02 GMT  
		Size: 1.2 MB (1163463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4097cf55145d3e6941810229afc94a987195c0631cc4d532dd62be1d1db8cae4`  
		Last Modified: Tue, 12 Oct 2021 16:14:01 GMT  
		Size: 292.9 KB (292852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819833447177af7e5beef2f993dd07950e209f2e7b8dd0bfcaf8ef739bc088a0`  
		Last Modified: Tue, 12 Oct 2021 16:14:43 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768c44619b6333fe354d3dcde3d3d7da5ace8c1c76182d6f142aa1dac4801bb9`  
		Last Modified: Tue, 12 Oct 2021 16:14:46 GMT  
		Size: 39.0 MB (39011980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ea5fc0628a1cc34aa10c0c42a21cc83abb67d3d90816c3c55278d58a3d0bb7`  
		Last Modified: Tue, 12 Oct 2021 16:14:40 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927ce1cccfe88f86c96cdcb9b630eabdbee8c1af572172401ec4899f84cc7ca8`  
		Last Modified: Tue, 12 Oct 2021 16:14:40 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989a6997d79c5f14c8b41d4c66a51de7b22c3ba365f72d4047f9b3f0062a0e1c`  
		Last Modified: Tue, 12 Oct 2021 16:14:41 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6104cd0db80895a588fa6f86859fe0d9590821f0911a4e262cf2afa998c137`  
		Last Modified: Tue, 12 Oct 2021 16:14:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3`

```console
$ docker pull couchdb@sha256:6d9aea691cf15e0b185f8b0c245e3693cb1f367a502a24a5fb2d9a97ed45a076
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3` - linux; amd64

```console
$ docker pull couchdb@sha256:e150f08d4781b3d0ba2b2328896615436add41ebbc1ae8f46dbba0d5b50ef756
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.5 MB (80541108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2fff885de6eb95e7060e056bff8a68415b76592d6a9a799dac45ba5989085b`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 12:32:07 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 12 Oct 2021 12:32:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 12 Oct 2021 12:32:18 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:32:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 12 Oct 2021 12:32:22 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 12 Oct 2021 12:32:29 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:32:29 GMT
ENV COUCHDB_VERSION=3.2.0
# Tue, 12 Oct 2021 12:32:30 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 12 Oct 2021 12:32:44 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 12 Oct 2021 12:32:45 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 12 Oct 2021 12:32:45 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 12 Oct 2021 12:32:45 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 12 Oct 2021 12:32:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 12 Oct 2021 12:32:46 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 12:32:46 GMT
VOLUME [/opt/couchdb/data]
# Tue, 12 Oct 2021 12:32:46 GMT
EXPOSE 4369 5984 9100
# Tue, 12 Oct 2021 12:32:47 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a46377fe8ce67057386a4c7aa933b926be606ba3070c3342e42f63e68d052c`  
		Last Modified: Tue, 12 Oct 2021 12:34:00 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4bf1b8a9bee200ee03e321a3d81949a87a559329ccffe9da773bd2d9d09fab`  
		Last Modified: Tue, 12 Oct 2021 12:34:00 GMT  
		Size: 6.7 MB (6691348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59081fa6a5d78e2274b9368f09dff77dc9e27812416dc235da1682d043b6129d`  
		Last Modified: Tue, 12 Oct 2021 12:33:58 GMT  
		Size: 1.3 MB (1258348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc87af85d712b9d439d847c5575c30770dcd0910cd5aea578135b4a2d4e5f16e`  
		Last Modified: Tue, 12 Oct 2021 12:33:58 GMT  
		Size: 293.0 KB (292995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f937941c5ec804af4fe48f885c0f4a7cf4bb52686fa4f351789e0822a0a53010`  
		Last Modified: Tue, 12 Oct 2021 12:33:58 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9def6a2a7f7afb329b52aa79f6e7e364e4c0b1fc5f6456560d340092b1b11c1`  
		Last Modified: Tue, 12 Oct 2021 12:34:01 GMT  
		Size: 45.2 MB (45151893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ab67db1541e933f5d72714f7addf00e24526db1fb69a90ee4a23eb797acf32`  
		Last Modified: Tue, 12 Oct 2021 12:33:56 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80723a7fbea8d1f758f276151c162b1bc34bcb58360f6056c219e4fab23328fc`  
		Last Modified: Tue, 12 Oct 2021 12:33:56 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57f490f20804c696113a543f5d12073356e77950f65b8da9b5e95546e7dd0a5`  
		Last Modified: Tue, 12 Oct 2021 12:33:55 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceefecb83d7b123a6fa5a0374e5bea18fba9de64bcedacdc4f36d1160d93c528`  
		Last Modified: Tue, 12 Oct 2021 12:33:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:7b32c474698f734ff5c42be52ce150bc856f587316fe391b789278bbaf452cc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75645542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d439facf9dca9ce3276743e44eef177c831b96f9a58c4611aa95eccdb37280f`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:12:13 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 12 Oct 2021 16:12:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 12 Oct 2021 16:12:21 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:12:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 12 Oct 2021 16:12:25 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 12 Oct 2021 16:12:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:12:32 GMT
ENV COUCHDB_VERSION=3.2.0
# Tue, 12 Oct 2021 16:12:33 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 12 Oct 2021 16:12:46 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 12 Oct 2021 16:12:46 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 12 Oct 2021 16:12:46 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 12 Oct 2021 16:12:46 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 12 Oct 2021 16:12:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 12 Oct 2021 16:12:47 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 16:12:47 GMT
VOLUME [/opt/couchdb/data]
# Tue, 12 Oct 2021 16:12:48 GMT
EXPOSE 4369 5984 9100
# Tue, 12 Oct 2021 16:12:48 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c646791d9868995e805f149bec168431525d3c31b3d0c73124e5a37e4afa76f`  
		Last Modified: Tue, 12 Oct 2021 16:14:03 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836357709ccd6570063bff28686a586c566ca7145e0adb10db6ca88966f4095e`  
		Last Modified: Tue, 12 Oct 2021 16:14:03 GMT  
		Size: 6.6 MB (6550798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7164389db8f0224aead9715f7478a90fb8d0612a43377991018342353359def`  
		Last Modified: Tue, 12 Oct 2021 16:14:02 GMT  
		Size: 1.2 MB (1163463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4097cf55145d3e6941810229afc94a987195c0631cc4d532dd62be1d1db8cae4`  
		Last Modified: Tue, 12 Oct 2021 16:14:01 GMT  
		Size: 292.9 KB (292852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6cdff452cdb1cbe7c743d23568c7c2f36970b360d7719f5cdc94e6b556c99d`  
		Last Modified: Tue, 12 Oct 2021 16:14:01 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2157f9eb628e6f0866a1288e2621b0f615e47020dba33d47a194c7ecdbc346cb`  
		Last Modified: Tue, 12 Oct 2021 16:14:04 GMT  
		Size: 41.7 MB (41722916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7ec62e0fb1cdc2de91fb8de6822acfa15e206691554d6134c7ff6d75f53c3e`  
		Last Modified: Tue, 12 Oct 2021 16:13:59 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61af5e9d1ae116230517b15c801cb3dc7fe42e88a30222ef9b88b947327512d4`  
		Last Modified: Tue, 12 Oct 2021 16:13:59 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d296d0af30fbebf70e062435b833f7acdbbcdc6714124ccc0a43b9c6e1b8e9`  
		Last Modified: Tue, 12 Oct 2021 16:13:58 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431e5a96bee9235b1db52994b56b5dd4ed5b22987684ea1e3c4fae3cc40d55b5`  
		Last Modified: Tue, 12 Oct 2021 16:13:59 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1`

```console
$ docker pull couchdb@sha256:5062586e9199d531d8db3aa9d0c187db52fa1d4eb77815896b951a5b8d2cd444
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:e22d9bb30b308002f721172b041de5f0e0f0c3d878f46f6953bec061d4f874a1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (79988449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be61a4391f21295d1d0190e854f76d8b92a30b0bd8a74a7576a9e98251805756`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 12:32:07 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 12 Oct 2021 12:32:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 12 Oct 2021 12:32:18 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:32:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 12 Oct 2021 12:32:22 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 12 Oct 2021 12:32:29 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:32:54 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 12 Oct 2021 12:32:55 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 12 Oct 2021 12:33:09 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 12 Oct 2021 12:33:10 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 12 Oct 2021 12:33:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 12 Oct 2021 12:33:10 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 12 Oct 2021 12:33:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 12 Oct 2021 12:33:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 12:33:11 GMT
VOLUME [/opt/couchdb/data]
# Tue, 12 Oct 2021 12:33:12 GMT
EXPOSE 4369 5984 9100
# Tue, 12 Oct 2021 12:33:12 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a46377fe8ce67057386a4c7aa933b926be606ba3070c3342e42f63e68d052c`  
		Last Modified: Tue, 12 Oct 2021 12:34:00 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4bf1b8a9bee200ee03e321a3d81949a87a559329ccffe9da773bd2d9d09fab`  
		Last Modified: Tue, 12 Oct 2021 12:34:00 GMT  
		Size: 6.7 MB (6691348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59081fa6a5d78e2274b9368f09dff77dc9e27812416dc235da1682d043b6129d`  
		Last Modified: Tue, 12 Oct 2021 12:33:58 GMT  
		Size: 1.3 MB (1258348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc87af85d712b9d439d847c5575c30770dcd0910cd5aea578135b4a2d4e5f16e`  
		Last Modified: Tue, 12 Oct 2021 12:33:58 GMT  
		Size: 293.0 KB (292995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8d680eceb1e6eac3a2c1dc667249e8f684e9cb3bc60b720c8e818d7f56097e`  
		Last Modified: Tue, 12 Oct 2021 12:34:19 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a822819d8da2a339ec86da95dcf6f3e3596417fa067abd578ce85ccdb37773`  
		Last Modified: Tue, 12 Oct 2021 12:34:23 GMT  
		Size: 44.6 MB (44599232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a3ca2015db31129d6082d2c9b5fbab4c6872e8ba658a94ced052ebb634e799`  
		Last Modified: Tue, 12 Oct 2021 12:34:17 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62fddea528a9a4c5cdbb27e5e7aaa6f26061b166bfc48392c98e2201ad7e6bbd`  
		Last Modified: Tue, 12 Oct 2021 12:34:17 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87e1db98c95c74f8321c8188ed21d1c538f7c6fa389f4a74511c46dc59f0b2c3`  
		Last Modified: Tue, 12 Oct 2021 12:34:17 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5b3f121da878e849adde075e83e34836c2496d85b085efff24da11d1f1b027`  
		Last Modified: Tue, 12 Oct 2021 12:34:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:e4b92784472e2fad2de21a594c369a6e794821066b1f31688d2a93b403c1ba92
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (75023942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58fe7aead20c1eed32422c116192eff5d75fc0ce6fd9047b35886b272ff0ea63`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:12:13 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 12 Oct 2021 16:12:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 12 Oct 2021 16:12:21 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:12:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 12 Oct 2021 16:12:25 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 12 Oct 2021 16:12:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:12:55 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 12 Oct 2021 16:12:55 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 12 Oct 2021 16:13:08 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 12 Oct 2021 16:13:08 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 12 Oct 2021 16:13:09 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 12 Oct 2021 16:13:09 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 12 Oct 2021 16:13:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 12 Oct 2021 16:13:10 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 16:13:10 GMT
VOLUME [/opt/couchdb/data]
# Tue, 12 Oct 2021 16:13:10 GMT
EXPOSE 4369 5984 9100
# Tue, 12 Oct 2021 16:13:10 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c646791d9868995e805f149bec168431525d3c31b3d0c73124e5a37e4afa76f`  
		Last Modified: Tue, 12 Oct 2021 16:14:03 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836357709ccd6570063bff28686a586c566ca7145e0adb10db6ca88966f4095e`  
		Last Modified: Tue, 12 Oct 2021 16:14:03 GMT  
		Size: 6.6 MB (6550798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7164389db8f0224aead9715f7478a90fb8d0612a43377991018342353359def`  
		Last Modified: Tue, 12 Oct 2021 16:14:02 GMT  
		Size: 1.2 MB (1163463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4097cf55145d3e6941810229afc94a987195c0631cc4d532dd62be1d1db8cae4`  
		Last Modified: Tue, 12 Oct 2021 16:14:01 GMT  
		Size: 292.9 KB (292852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957ddaedc55a721db3da503a66202719faccce0779426e23fe4809d27a117ff3`  
		Last Modified: Tue, 12 Oct 2021 16:14:26 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ef013ac8c51b30090e7d3c0d3e531e04004d9ad6b05c1f9f9dc52d4ff05f7d`  
		Last Modified: Tue, 12 Oct 2021 16:14:29 GMT  
		Size: 41.1 MB (41101314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c1ac0db87b1954b1ff630986ce8157c5d87efcc59bdec0810fe30f2bc35501`  
		Last Modified: Tue, 12 Oct 2021 16:14:23 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a3ad7c337139285d121fb1fb07bb4186ff653362e316bdc31f5c895e22a746`  
		Last Modified: Tue, 12 Oct 2021 16:14:24 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48f493f0f462d3a5ce25afee0fb52f06537eb139c4a1443299b7fb7a8b141fc`  
		Last Modified: Tue, 12 Oct 2021 16:14:27 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0fc4885797a0698a8d68473460075cd36408640761afc7371b408592f03cca`  
		Last Modified: Tue, 12 Oct 2021 16:14:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1.2`

```console
$ docker pull couchdb@sha256:5062586e9199d531d8db3aa9d0c187db52fa1d4eb77815896b951a5b8d2cd444
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1.2` - linux; amd64

```console
$ docker pull couchdb@sha256:e22d9bb30b308002f721172b041de5f0e0f0c3d878f46f6953bec061d4f874a1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (79988449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be61a4391f21295d1d0190e854f76d8b92a30b0bd8a74a7576a9e98251805756`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 12:32:07 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 12 Oct 2021 12:32:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 12 Oct 2021 12:32:18 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:32:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 12 Oct 2021 12:32:22 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 12 Oct 2021 12:32:29 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:32:54 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 12 Oct 2021 12:32:55 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 12 Oct 2021 12:33:09 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 12 Oct 2021 12:33:10 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 12 Oct 2021 12:33:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 12 Oct 2021 12:33:10 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 12 Oct 2021 12:33:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 12 Oct 2021 12:33:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 12:33:11 GMT
VOLUME [/opt/couchdb/data]
# Tue, 12 Oct 2021 12:33:12 GMT
EXPOSE 4369 5984 9100
# Tue, 12 Oct 2021 12:33:12 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a46377fe8ce67057386a4c7aa933b926be606ba3070c3342e42f63e68d052c`  
		Last Modified: Tue, 12 Oct 2021 12:34:00 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4bf1b8a9bee200ee03e321a3d81949a87a559329ccffe9da773bd2d9d09fab`  
		Last Modified: Tue, 12 Oct 2021 12:34:00 GMT  
		Size: 6.7 MB (6691348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59081fa6a5d78e2274b9368f09dff77dc9e27812416dc235da1682d043b6129d`  
		Last Modified: Tue, 12 Oct 2021 12:33:58 GMT  
		Size: 1.3 MB (1258348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc87af85d712b9d439d847c5575c30770dcd0910cd5aea578135b4a2d4e5f16e`  
		Last Modified: Tue, 12 Oct 2021 12:33:58 GMT  
		Size: 293.0 KB (292995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8d680eceb1e6eac3a2c1dc667249e8f684e9cb3bc60b720c8e818d7f56097e`  
		Last Modified: Tue, 12 Oct 2021 12:34:19 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a822819d8da2a339ec86da95dcf6f3e3596417fa067abd578ce85ccdb37773`  
		Last Modified: Tue, 12 Oct 2021 12:34:23 GMT  
		Size: 44.6 MB (44599232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a3ca2015db31129d6082d2c9b5fbab4c6872e8ba658a94ced052ebb634e799`  
		Last Modified: Tue, 12 Oct 2021 12:34:17 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62fddea528a9a4c5cdbb27e5e7aaa6f26061b166bfc48392c98e2201ad7e6bbd`  
		Last Modified: Tue, 12 Oct 2021 12:34:17 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87e1db98c95c74f8321c8188ed21d1c538f7c6fa389f4a74511c46dc59f0b2c3`  
		Last Modified: Tue, 12 Oct 2021 12:34:17 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5b3f121da878e849adde075e83e34836c2496d85b085efff24da11d1f1b027`  
		Last Modified: Tue, 12 Oct 2021 12:34:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:e4b92784472e2fad2de21a594c369a6e794821066b1f31688d2a93b403c1ba92
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (75023942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58fe7aead20c1eed32422c116192eff5d75fc0ce6fd9047b35886b272ff0ea63`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:12:13 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 12 Oct 2021 16:12:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 12 Oct 2021 16:12:21 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:12:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 12 Oct 2021 16:12:25 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 12 Oct 2021 16:12:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:12:55 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 12 Oct 2021 16:12:55 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 12 Oct 2021 16:13:08 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 12 Oct 2021 16:13:08 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 12 Oct 2021 16:13:09 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 12 Oct 2021 16:13:09 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 12 Oct 2021 16:13:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 12 Oct 2021 16:13:10 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 16:13:10 GMT
VOLUME [/opt/couchdb/data]
# Tue, 12 Oct 2021 16:13:10 GMT
EXPOSE 4369 5984 9100
# Tue, 12 Oct 2021 16:13:10 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c646791d9868995e805f149bec168431525d3c31b3d0c73124e5a37e4afa76f`  
		Last Modified: Tue, 12 Oct 2021 16:14:03 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836357709ccd6570063bff28686a586c566ca7145e0adb10db6ca88966f4095e`  
		Last Modified: Tue, 12 Oct 2021 16:14:03 GMT  
		Size: 6.6 MB (6550798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7164389db8f0224aead9715f7478a90fb8d0612a43377991018342353359def`  
		Last Modified: Tue, 12 Oct 2021 16:14:02 GMT  
		Size: 1.2 MB (1163463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4097cf55145d3e6941810229afc94a987195c0631cc4d532dd62be1d1db8cae4`  
		Last Modified: Tue, 12 Oct 2021 16:14:01 GMT  
		Size: 292.9 KB (292852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957ddaedc55a721db3da503a66202719faccce0779426e23fe4809d27a117ff3`  
		Last Modified: Tue, 12 Oct 2021 16:14:26 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ef013ac8c51b30090e7d3c0d3e531e04004d9ad6b05c1f9f9dc52d4ff05f7d`  
		Last Modified: Tue, 12 Oct 2021 16:14:29 GMT  
		Size: 41.1 MB (41101314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c1ac0db87b1954b1ff630986ce8157c5d87efcc59bdec0810fe30f2bc35501`  
		Last Modified: Tue, 12 Oct 2021 16:14:23 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a3ad7c337139285d121fb1fb07bb4186ff653362e316bdc31f5c895e22a746`  
		Last Modified: Tue, 12 Oct 2021 16:14:24 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48f493f0f462d3a5ce25afee0fb52f06537eb139c4a1443299b7fb7a8b141fc`  
		Last Modified: Tue, 12 Oct 2021 16:14:27 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0fc4885797a0698a8d68473460075cd36408640761afc7371b408592f03cca`  
		Last Modified: Tue, 12 Oct 2021 16:14:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2`

```console
$ docker pull couchdb@sha256:6d9aea691cf15e0b185f8b0c245e3693cb1f367a502a24a5fb2d9a97ed45a076
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.2` - linux; amd64

```console
$ docker pull couchdb@sha256:e150f08d4781b3d0ba2b2328896615436add41ebbc1ae8f46dbba0d5b50ef756
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.5 MB (80541108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2fff885de6eb95e7060e056bff8a68415b76592d6a9a799dac45ba5989085b`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 12:32:07 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 12 Oct 2021 12:32:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 12 Oct 2021 12:32:18 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:32:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 12 Oct 2021 12:32:22 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 12 Oct 2021 12:32:29 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:32:29 GMT
ENV COUCHDB_VERSION=3.2.0
# Tue, 12 Oct 2021 12:32:30 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 12 Oct 2021 12:32:44 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 12 Oct 2021 12:32:45 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 12 Oct 2021 12:32:45 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 12 Oct 2021 12:32:45 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 12 Oct 2021 12:32:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 12 Oct 2021 12:32:46 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 12:32:46 GMT
VOLUME [/opt/couchdb/data]
# Tue, 12 Oct 2021 12:32:46 GMT
EXPOSE 4369 5984 9100
# Tue, 12 Oct 2021 12:32:47 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a46377fe8ce67057386a4c7aa933b926be606ba3070c3342e42f63e68d052c`  
		Last Modified: Tue, 12 Oct 2021 12:34:00 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4bf1b8a9bee200ee03e321a3d81949a87a559329ccffe9da773bd2d9d09fab`  
		Last Modified: Tue, 12 Oct 2021 12:34:00 GMT  
		Size: 6.7 MB (6691348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59081fa6a5d78e2274b9368f09dff77dc9e27812416dc235da1682d043b6129d`  
		Last Modified: Tue, 12 Oct 2021 12:33:58 GMT  
		Size: 1.3 MB (1258348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc87af85d712b9d439d847c5575c30770dcd0910cd5aea578135b4a2d4e5f16e`  
		Last Modified: Tue, 12 Oct 2021 12:33:58 GMT  
		Size: 293.0 KB (292995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f937941c5ec804af4fe48f885c0f4a7cf4bb52686fa4f351789e0822a0a53010`  
		Last Modified: Tue, 12 Oct 2021 12:33:58 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9def6a2a7f7afb329b52aa79f6e7e364e4c0b1fc5f6456560d340092b1b11c1`  
		Last Modified: Tue, 12 Oct 2021 12:34:01 GMT  
		Size: 45.2 MB (45151893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ab67db1541e933f5d72714f7addf00e24526db1fb69a90ee4a23eb797acf32`  
		Last Modified: Tue, 12 Oct 2021 12:33:56 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80723a7fbea8d1f758f276151c162b1bc34bcb58360f6056c219e4fab23328fc`  
		Last Modified: Tue, 12 Oct 2021 12:33:56 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57f490f20804c696113a543f5d12073356e77950f65b8da9b5e95546e7dd0a5`  
		Last Modified: Tue, 12 Oct 2021 12:33:55 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceefecb83d7b123a6fa5a0374e5bea18fba9de64bcedacdc4f36d1160d93c528`  
		Last Modified: Tue, 12 Oct 2021 12:33:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:7b32c474698f734ff5c42be52ce150bc856f587316fe391b789278bbaf452cc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75645542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d439facf9dca9ce3276743e44eef177c831b96f9a58c4611aa95eccdb37280f`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:12:13 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 12 Oct 2021 16:12:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 12 Oct 2021 16:12:21 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:12:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 12 Oct 2021 16:12:25 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 12 Oct 2021 16:12:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:12:32 GMT
ENV COUCHDB_VERSION=3.2.0
# Tue, 12 Oct 2021 16:12:33 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 12 Oct 2021 16:12:46 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 12 Oct 2021 16:12:46 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 12 Oct 2021 16:12:46 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 12 Oct 2021 16:12:46 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 12 Oct 2021 16:12:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 12 Oct 2021 16:12:47 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 16:12:47 GMT
VOLUME [/opt/couchdb/data]
# Tue, 12 Oct 2021 16:12:48 GMT
EXPOSE 4369 5984 9100
# Tue, 12 Oct 2021 16:12:48 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c646791d9868995e805f149bec168431525d3c31b3d0c73124e5a37e4afa76f`  
		Last Modified: Tue, 12 Oct 2021 16:14:03 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836357709ccd6570063bff28686a586c566ca7145e0adb10db6ca88966f4095e`  
		Last Modified: Tue, 12 Oct 2021 16:14:03 GMT  
		Size: 6.6 MB (6550798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7164389db8f0224aead9715f7478a90fb8d0612a43377991018342353359def`  
		Last Modified: Tue, 12 Oct 2021 16:14:02 GMT  
		Size: 1.2 MB (1163463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4097cf55145d3e6941810229afc94a987195c0631cc4d532dd62be1d1db8cae4`  
		Last Modified: Tue, 12 Oct 2021 16:14:01 GMT  
		Size: 292.9 KB (292852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6cdff452cdb1cbe7c743d23568c7c2f36970b360d7719f5cdc94e6b556c99d`  
		Last Modified: Tue, 12 Oct 2021 16:14:01 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2157f9eb628e6f0866a1288e2621b0f615e47020dba33d47a194c7ecdbc346cb`  
		Last Modified: Tue, 12 Oct 2021 16:14:04 GMT  
		Size: 41.7 MB (41722916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7ec62e0fb1cdc2de91fb8de6822acfa15e206691554d6134c7ff6d75f53c3e`  
		Last Modified: Tue, 12 Oct 2021 16:13:59 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61af5e9d1ae116230517b15c801cb3dc7fe42e88a30222ef9b88b947327512d4`  
		Last Modified: Tue, 12 Oct 2021 16:13:59 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d296d0af30fbebf70e062435b833f7acdbbcdc6714124ccc0a43b9c6e1b8e9`  
		Last Modified: Tue, 12 Oct 2021 16:13:58 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431e5a96bee9235b1db52994b56b5dd4ed5b22987684ea1e3c4fae3cc40d55b5`  
		Last Modified: Tue, 12 Oct 2021 16:13:59 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2.0`

```console
$ docker pull couchdb@sha256:6d9aea691cf15e0b185f8b0c245e3693cb1f367a502a24a5fb2d9a97ed45a076
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.2.0` - linux; amd64

```console
$ docker pull couchdb@sha256:e150f08d4781b3d0ba2b2328896615436add41ebbc1ae8f46dbba0d5b50ef756
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.5 MB (80541108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2fff885de6eb95e7060e056bff8a68415b76592d6a9a799dac45ba5989085b`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 12:32:07 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 12 Oct 2021 12:32:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 12 Oct 2021 12:32:18 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:32:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 12 Oct 2021 12:32:22 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 12 Oct 2021 12:32:29 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:32:29 GMT
ENV COUCHDB_VERSION=3.2.0
# Tue, 12 Oct 2021 12:32:30 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 12 Oct 2021 12:32:44 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 12 Oct 2021 12:32:45 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 12 Oct 2021 12:32:45 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 12 Oct 2021 12:32:45 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 12 Oct 2021 12:32:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 12 Oct 2021 12:32:46 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 12:32:46 GMT
VOLUME [/opt/couchdb/data]
# Tue, 12 Oct 2021 12:32:46 GMT
EXPOSE 4369 5984 9100
# Tue, 12 Oct 2021 12:32:47 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a46377fe8ce67057386a4c7aa933b926be606ba3070c3342e42f63e68d052c`  
		Last Modified: Tue, 12 Oct 2021 12:34:00 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4bf1b8a9bee200ee03e321a3d81949a87a559329ccffe9da773bd2d9d09fab`  
		Last Modified: Tue, 12 Oct 2021 12:34:00 GMT  
		Size: 6.7 MB (6691348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59081fa6a5d78e2274b9368f09dff77dc9e27812416dc235da1682d043b6129d`  
		Last Modified: Tue, 12 Oct 2021 12:33:58 GMT  
		Size: 1.3 MB (1258348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc87af85d712b9d439d847c5575c30770dcd0910cd5aea578135b4a2d4e5f16e`  
		Last Modified: Tue, 12 Oct 2021 12:33:58 GMT  
		Size: 293.0 KB (292995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f937941c5ec804af4fe48f885c0f4a7cf4bb52686fa4f351789e0822a0a53010`  
		Last Modified: Tue, 12 Oct 2021 12:33:58 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9def6a2a7f7afb329b52aa79f6e7e364e4c0b1fc5f6456560d340092b1b11c1`  
		Last Modified: Tue, 12 Oct 2021 12:34:01 GMT  
		Size: 45.2 MB (45151893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ab67db1541e933f5d72714f7addf00e24526db1fb69a90ee4a23eb797acf32`  
		Last Modified: Tue, 12 Oct 2021 12:33:56 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80723a7fbea8d1f758f276151c162b1bc34bcb58360f6056c219e4fab23328fc`  
		Last Modified: Tue, 12 Oct 2021 12:33:56 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57f490f20804c696113a543f5d12073356e77950f65b8da9b5e95546e7dd0a5`  
		Last Modified: Tue, 12 Oct 2021 12:33:55 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceefecb83d7b123a6fa5a0374e5bea18fba9de64bcedacdc4f36d1160d93c528`  
		Last Modified: Tue, 12 Oct 2021 12:33:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2.0` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:7b32c474698f734ff5c42be52ce150bc856f587316fe391b789278bbaf452cc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75645542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d439facf9dca9ce3276743e44eef177c831b96f9a58c4611aa95eccdb37280f`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:12:13 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 12 Oct 2021 16:12:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 12 Oct 2021 16:12:21 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:12:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 12 Oct 2021 16:12:25 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 12 Oct 2021 16:12:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:12:32 GMT
ENV COUCHDB_VERSION=3.2.0
# Tue, 12 Oct 2021 16:12:33 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 12 Oct 2021 16:12:46 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 12 Oct 2021 16:12:46 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 12 Oct 2021 16:12:46 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 12 Oct 2021 16:12:46 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 12 Oct 2021 16:12:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 12 Oct 2021 16:12:47 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 16:12:47 GMT
VOLUME [/opt/couchdb/data]
# Tue, 12 Oct 2021 16:12:48 GMT
EXPOSE 4369 5984 9100
# Tue, 12 Oct 2021 16:12:48 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c646791d9868995e805f149bec168431525d3c31b3d0c73124e5a37e4afa76f`  
		Last Modified: Tue, 12 Oct 2021 16:14:03 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836357709ccd6570063bff28686a586c566ca7145e0adb10db6ca88966f4095e`  
		Last Modified: Tue, 12 Oct 2021 16:14:03 GMT  
		Size: 6.6 MB (6550798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7164389db8f0224aead9715f7478a90fb8d0612a43377991018342353359def`  
		Last Modified: Tue, 12 Oct 2021 16:14:02 GMT  
		Size: 1.2 MB (1163463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4097cf55145d3e6941810229afc94a987195c0631cc4d532dd62be1d1db8cae4`  
		Last Modified: Tue, 12 Oct 2021 16:14:01 GMT  
		Size: 292.9 KB (292852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6cdff452cdb1cbe7c743d23568c7c2f36970b360d7719f5cdc94e6b556c99d`  
		Last Modified: Tue, 12 Oct 2021 16:14:01 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2157f9eb628e6f0866a1288e2621b0f615e47020dba33d47a194c7ecdbc346cb`  
		Last Modified: Tue, 12 Oct 2021 16:14:04 GMT  
		Size: 41.7 MB (41722916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7ec62e0fb1cdc2de91fb8de6822acfa15e206691554d6134c7ff6d75f53c3e`  
		Last Modified: Tue, 12 Oct 2021 16:13:59 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61af5e9d1ae116230517b15c801cb3dc7fe42e88a30222ef9b88b947327512d4`  
		Last Modified: Tue, 12 Oct 2021 16:13:59 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d296d0af30fbebf70e062435b833f7acdbbcdc6714124ccc0a43b9c6e1b8e9`  
		Last Modified: Tue, 12 Oct 2021 16:13:58 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431e5a96bee9235b1db52994b56b5dd4ed5b22987684ea1e3c4fae3cc40d55b5`  
		Last Modified: Tue, 12 Oct 2021 16:13:59 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:latest`

```console
$ docker pull couchdb@sha256:6d9aea691cf15e0b185f8b0c245e3693cb1f367a502a24a5fb2d9a97ed45a076
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:e150f08d4781b3d0ba2b2328896615436add41ebbc1ae8f46dbba0d5b50ef756
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.5 MB (80541108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2fff885de6eb95e7060e056bff8a68415b76592d6a9a799dac45ba5989085b`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:05 GMT
ADD file:910392427fdf089bc26b64d6dc450ff3d020c7c1a474d85b2f9298134d0007bd in / 
# Tue, 12 Oct 2021 01:21:05 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 12:32:07 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 12 Oct 2021 12:32:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 12 Oct 2021 12:32:18 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:32:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 12 Oct 2021 12:32:22 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 12 Oct 2021 12:32:29 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 12:32:29 GMT
ENV COUCHDB_VERSION=3.2.0
# Tue, 12 Oct 2021 12:32:30 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 12 Oct 2021 12:32:44 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 12 Oct 2021 12:32:45 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 12 Oct 2021 12:32:45 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 12 Oct 2021 12:32:45 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 12 Oct 2021 12:32:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 12 Oct 2021 12:32:46 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 12:32:46 GMT
VOLUME [/opt/couchdb/data]
# Tue, 12 Oct 2021 12:32:46 GMT
EXPOSE 4369 5984 9100
# Tue, 12 Oct 2021 12:32:47 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b380bbd43752f83945df8b5d1074fef8dd044820e7d3aef33b655a2483e030c7`  
		Last Modified: Tue, 12 Oct 2021 01:26:51 GMT  
		Size: 27.1 MB (27139510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a46377fe8ce67057386a4c7aa933b926be606ba3070c3342e42f63e68d052c`  
		Last Modified: Tue, 12 Oct 2021 12:34:00 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4bf1b8a9bee200ee03e321a3d81949a87a559329ccffe9da773bd2d9d09fab`  
		Last Modified: Tue, 12 Oct 2021 12:34:00 GMT  
		Size: 6.7 MB (6691348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59081fa6a5d78e2274b9368f09dff77dc9e27812416dc235da1682d043b6129d`  
		Last Modified: Tue, 12 Oct 2021 12:33:58 GMT  
		Size: 1.3 MB (1258348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc87af85d712b9d439d847c5575c30770dcd0910cd5aea578135b4a2d4e5f16e`  
		Last Modified: Tue, 12 Oct 2021 12:33:58 GMT  
		Size: 293.0 KB (292995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f937941c5ec804af4fe48f885c0f4a7cf4bb52686fa4f351789e0822a0a53010`  
		Last Modified: Tue, 12 Oct 2021 12:33:58 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9def6a2a7f7afb329b52aa79f6e7e364e4c0b1fc5f6456560d340092b1b11c1`  
		Last Modified: Tue, 12 Oct 2021 12:34:01 GMT  
		Size: 45.2 MB (45151893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ab67db1541e933f5d72714f7addf00e24526db1fb69a90ee4a23eb797acf32`  
		Last Modified: Tue, 12 Oct 2021 12:33:56 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80723a7fbea8d1f758f276151c162b1bc34bcb58360f6056c219e4fab23328fc`  
		Last Modified: Tue, 12 Oct 2021 12:33:56 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57f490f20804c696113a543f5d12073356e77950f65b8da9b5e95546e7dd0a5`  
		Last Modified: Tue, 12 Oct 2021 12:33:55 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceefecb83d7b123a6fa5a0374e5bea18fba9de64bcedacdc4f36d1160d93c528`  
		Last Modified: Tue, 12 Oct 2021 12:33:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:7b32c474698f734ff5c42be52ce150bc856f587316fe391b789278bbaf452cc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75645542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d439facf9dca9ce3276743e44eef177c831b96f9a58c4611aa95eccdb37280f`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:42 GMT
ADD file:f0d53027a7ba594477674127971aa477af3a2bc6bcddef6c0aa174953a5f2db0 in / 
# Tue, 12 Oct 2021 01:41:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:12:13 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 12 Oct 2021 16:12:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 12 Oct 2021 16:12:21 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:12:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 12 Oct 2021 16:12:25 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 12 Oct 2021 16:12:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:12:32 GMT
ENV COUCHDB_VERSION=3.2.0
# Tue, 12 Oct 2021 16:12:33 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 12 Oct 2021 16:12:46 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 12 Oct 2021 16:12:46 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 12 Oct 2021 16:12:46 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 12 Oct 2021 16:12:46 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 12 Oct 2021 16:12:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 12 Oct 2021 16:12:47 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 12 Oct 2021 16:12:47 GMT
VOLUME [/opt/couchdb/data]
# Tue, 12 Oct 2021 16:12:48 GMT
EXPOSE 4369 5984 9100
# Tue, 12 Oct 2021 16:12:48 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:02b45931a436a68cadb742684148ed6aacbbf9aa21447b467c11bac97f92eb46`  
		Last Modified: Tue, 12 Oct 2021 01:49:07 GMT  
		Size: 25.9 MB (25908479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c646791d9868995e805f149bec168431525d3c31b3d0c73124e5a37e4afa76f`  
		Last Modified: Tue, 12 Oct 2021 16:14:03 GMT  
		Size: 3.4 KB (3435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836357709ccd6570063bff28686a586c566ca7145e0adb10db6ca88966f4095e`  
		Last Modified: Tue, 12 Oct 2021 16:14:03 GMT  
		Size: 6.6 MB (6550798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7164389db8f0224aead9715f7478a90fb8d0612a43377991018342353359def`  
		Last Modified: Tue, 12 Oct 2021 16:14:02 GMT  
		Size: 1.2 MB (1163463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4097cf55145d3e6941810229afc94a987195c0631cc4d532dd62be1d1db8cae4`  
		Last Modified: Tue, 12 Oct 2021 16:14:01 GMT  
		Size: 292.9 KB (292852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6cdff452cdb1cbe7c743d23568c7c2f36970b360d7719f5cdc94e6b556c99d`  
		Last Modified: Tue, 12 Oct 2021 16:14:01 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2157f9eb628e6f0866a1288e2621b0f615e47020dba33d47a194c7ecdbc346cb`  
		Last Modified: Tue, 12 Oct 2021 16:14:04 GMT  
		Size: 41.7 MB (41722916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f7ec62e0fb1cdc2de91fb8de6822acfa15e206691554d6134c7ff6d75f53c3e`  
		Last Modified: Tue, 12 Oct 2021 16:13:59 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61af5e9d1ae116230517b15c801cb3dc7fe42e88a30222ef9b88b947327512d4`  
		Last Modified: Tue, 12 Oct 2021 16:13:59 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d296d0af30fbebf70e062435b833f7acdbbcdc6714124ccc0a43b9c6e1b8e9`  
		Last Modified: Tue, 12 Oct 2021 16:13:58 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431e5a96bee9235b1db52994b56b5dd4ed5b22987684ea1e3c4fae3cc40d55b5`  
		Last Modified: Tue, 12 Oct 2021 16:13:59 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
