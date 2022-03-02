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
$ docker pull couchdb@sha256:4ef104f0a97f4016f48dea1056742f19863df2184af6db88b83b39d5306a9608
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2` - linux; amd64

```console
$ docker pull couchdb@sha256:847e1795b0a0d237d9f94be94629e33d811e0104c8c508897958440e1bdcf06c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84517807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10596e5ba2cc278725271cb50463f181896f424dbf4b06da88ce36c6ac59fd18`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:56 GMT
ADD file:702017714ad3e1567b4f60b688750f8b631d91088e4dcf41351c4bb07749c579 in / 
# Tue, 01 Mar 2022 02:13:56 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 05:43:51 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 01 Mar 2022 05:43:52 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 01 Mar 2022 05:44:01 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 05:44:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 01 Mar 2022 05:44:05 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 01 Mar 2022 05:44:13 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 05:44:31 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 01 Mar 2022 05:44:32 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 01 Mar 2022 05:44:50 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 01 Mar 2022 05:44:50 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 01 Mar 2022 05:44:50 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 01 Mar 2022 05:44:50 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 01 Mar 2022 05:44:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 05:44:51 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 01 Mar 2022 05:44:51 GMT
VOLUME [/opt/couchdb/data]
# Tue, 01 Mar 2022 05:44:51 GMT
EXPOSE 4369 5984 9100
# Tue, 01 Mar 2022 05:44:51 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:15115158dd02a1bf2fd28724e3c1024394033fb0e9a5d3e451ed2715b6ae312d`  
		Last Modified: Tue, 01 Mar 2022 02:20:08 GMT  
		Size: 27.2 MB (27153737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e132993eb143d25686acdeb919d14985e8a65255f56170cc91230c350b203efa`  
		Last Modified: Tue, 01 Mar 2022 05:45:35 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50404ca1e1b3d297bb3c53a42e386f090eaa10f2d4db26fa324c39a836a18ea2`  
		Last Modified: Tue, 01 Mar 2022 05:45:34 GMT  
		Size: 6.7 MB (6691238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185b4237a163f4ee3d4cbb14cccd38dbfff817f923da22f90651149905d5957f`  
		Last Modified: Tue, 01 Mar 2022 05:45:33 GMT  
		Size: 1.3 MB (1258328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3a7c7c6b65c07b5de14a76f367630dcdc1f47fb75f959826b67e019b0617ec2`  
		Last Modified: Tue, 01 Mar 2022 05:45:33 GMT  
		Size: 293.0 KB (293032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10737976dd7f04dffd2c8080cb3ea3718e864fb550e1f8e3354886937546574`  
		Last Modified: Tue, 01 Mar 2022 05:45:48 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a11c8284534d8d62c430ef5edd0b754f191ed08eb41a89dd12c88cc42f8876e`  
		Last Modified: Tue, 01 Mar 2022 05:45:52 GMT  
		Size: 49.1 MB (49114456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54d99378c788f80c9ecc1d468356b808769ef6e72ba204e99075047a72d9401`  
		Last Modified: Tue, 01 Mar 2022 05:45:47 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8f2f19f0705503827a4fdc361a6f99896e1875fb4fddbf33721a673720aef6`  
		Last Modified: Tue, 01 Mar 2022 05:45:46 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bef14bec9c81959285cc9e53e3d5699eabb9be169611e2c125bbfd9f261c52b`  
		Last Modified: Tue, 01 Mar 2022 05:45:46 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd86d7a071c031c015596ab2ec6dcfe4cfdf70bd5082935f1016dc604a66c4f`  
		Last Modified: Tue, 01 Mar 2022 05:45:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:d5faeab69938596cc25f9c1b52105c67801c5187b3fa64fd5a40d539e40427d9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72522813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f49a6ea2840b6fad1f61ac250caadcda9144931bf249c8044548022a19566fad`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:57 GMT
ADD file:7d35162eea06441e7115c6fd9508802eafee00f64b11a7529a8f125bc67fa95e in / 
# Tue, 01 Mar 2022 02:11:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:55:17 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 01 Mar 2022 10:55:18 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 01 Mar 2022 10:55:26 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:55:31 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 01 Mar 2022 10:55:32 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 01 Mar 2022 10:55:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:56:18 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 01 Mar 2022 10:56:19 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 01 Mar 2022 10:56:38 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 01 Mar 2022 10:56:39 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 01 Mar 2022 10:56:40 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 01 Mar 2022 10:56:41 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 01 Mar 2022 10:56:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 10:56:42 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 01 Mar 2022 10:56:43 GMT
VOLUME [/opt/couchdb/data]
# Tue, 01 Mar 2022 10:56:44 GMT
EXPOSE 4369 5984 9100
# Tue, 01 Mar 2022 10:56:45 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:69bf0018a85cc0775a59a4dbda1b2f2e71086a2d817473f72336bf4d0a83b9d0`  
		Last Modified: Tue, 01 Mar 2022 02:19:15 GMT  
		Size: 25.9 MB (25923140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f3b0034185f805a7eca8287a2a7e1c7083a4a3803aa2ff831381977e362fdd`  
		Last Modified: Tue, 01 Mar 2022 10:57:38 GMT  
		Size: 3.3 KB (3321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b11afb5df4d7ceb32be036fdf972d3345cdb7577b89ee1e2f5718768554a3b3`  
		Last Modified: Tue, 01 Mar 2022 10:57:37 GMT  
		Size: 6.5 MB (6549945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01d9cba25fe10102232e70e1e262509477dcbda240c129c62ff2a79c6870918`  
		Last Modified: Tue, 01 Mar 2022 10:57:36 GMT  
		Size: 951.2 KB (951181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75a3508d3b60b5de298e4411ecdd1e54e257ebe20f94a95023c85b62a5c2ad3`  
		Last Modified: Tue, 01 Mar 2022 10:57:36 GMT  
		Size: 79.9 KB (79885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b102dd0eb55f11c90904fccef03a986e2109c1c15ab98820ba9c5821bfe7e07`  
		Last Modified: Tue, 01 Mar 2022 10:57:52 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84f7d5462854b7642f779f2acad5f45f22257a80b41ed8846f7416e79785332`  
		Last Modified: Tue, 01 Mar 2022 10:57:55 GMT  
		Size: 39.0 MB (39011744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f95c1a2438170f86f990ad088f83767ba8e419f1ac96cdb294ff40c617a7d3`  
		Last Modified: Tue, 01 Mar 2022 10:57:50 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7614832d184c7d5e6c6fb96776cbcd809045a5a10fce32f263ac293ff39195`  
		Last Modified: Tue, 01 Mar 2022 10:57:50 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e269a34ba04007a35b2fa7baec856b1c30f30c697671b8540c393e84a631d49`  
		Last Modified: Tue, 01 Mar 2022 10:57:50 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d4b074057a622e81c2cc34c78ffb522085c5f499dd352f356ccb5ab44f33f7`  
		Last Modified: Tue, 01 Mar 2022 10:57:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3`

```console
$ docker pull couchdb@sha256:4ef104f0a97f4016f48dea1056742f19863df2184af6db88b83b39d5306a9608
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:847e1795b0a0d237d9f94be94629e33d811e0104c8c508897958440e1bdcf06c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84517807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10596e5ba2cc278725271cb50463f181896f424dbf4b06da88ce36c6ac59fd18`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:56 GMT
ADD file:702017714ad3e1567b4f60b688750f8b631d91088e4dcf41351c4bb07749c579 in / 
# Tue, 01 Mar 2022 02:13:56 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 05:43:51 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 01 Mar 2022 05:43:52 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 01 Mar 2022 05:44:01 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 05:44:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 01 Mar 2022 05:44:05 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 01 Mar 2022 05:44:13 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 05:44:31 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 01 Mar 2022 05:44:32 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 01 Mar 2022 05:44:50 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 01 Mar 2022 05:44:50 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 01 Mar 2022 05:44:50 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 01 Mar 2022 05:44:50 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 01 Mar 2022 05:44:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 05:44:51 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 01 Mar 2022 05:44:51 GMT
VOLUME [/opt/couchdb/data]
# Tue, 01 Mar 2022 05:44:51 GMT
EXPOSE 4369 5984 9100
# Tue, 01 Mar 2022 05:44:51 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:15115158dd02a1bf2fd28724e3c1024394033fb0e9a5d3e451ed2715b6ae312d`  
		Last Modified: Tue, 01 Mar 2022 02:20:08 GMT  
		Size: 27.2 MB (27153737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e132993eb143d25686acdeb919d14985e8a65255f56170cc91230c350b203efa`  
		Last Modified: Tue, 01 Mar 2022 05:45:35 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50404ca1e1b3d297bb3c53a42e386f090eaa10f2d4db26fa324c39a836a18ea2`  
		Last Modified: Tue, 01 Mar 2022 05:45:34 GMT  
		Size: 6.7 MB (6691238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185b4237a163f4ee3d4cbb14cccd38dbfff817f923da22f90651149905d5957f`  
		Last Modified: Tue, 01 Mar 2022 05:45:33 GMT  
		Size: 1.3 MB (1258328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3a7c7c6b65c07b5de14a76f367630dcdc1f47fb75f959826b67e019b0617ec2`  
		Last Modified: Tue, 01 Mar 2022 05:45:33 GMT  
		Size: 293.0 KB (293032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10737976dd7f04dffd2c8080cb3ea3718e864fb550e1f8e3354886937546574`  
		Last Modified: Tue, 01 Mar 2022 05:45:48 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a11c8284534d8d62c430ef5edd0b754f191ed08eb41a89dd12c88cc42f8876e`  
		Last Modified: Tue, 01 Mar 2022 05:45:52 GMT  
		Size: 49.1 MB (49114456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54d99378c788f80c9ecc1d468356b808769ef6e72ba204e99075047a72d9401`  
		Last Modified: Tue, 01 Mar 2022 05:45:47 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8f2f19f0705503827a4fdc361a6f99896e1875fb4fddbf33721a673720aef6`  
		Last Modified: Tue, 01 Mar 2022 05:45:46 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bef14bec9c81959285cc9e53e3d5699eabb9be169611e2c125bbfd9f261c52b`  
		Last Modified: Tue, 01 Mar 2022 05:45:46 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd86d7a071c031c015596ab2ec6dcfe4cfdf70bd5082935f1016dc604a66c4f`  
		Last Modified: Tue, 01 Mar 2022 05:45:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:d5faeab69938596cc25f9c1b52105c67801c5187b3fa64fd5a40d539e40427d9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72522813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f49a6ea2840b6fad1f61ac250caadcda9144931bf249c8044548022a19566fad`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:57 GMT
ADD file:7d35162eea06441e7115c6fd9508802eafee00f64b11a7529a8f125bc67fa95e in / 
# Tue, 01 Mar 2022 02:11:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:55:17 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 01 Mar 2022 10:55:18 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 01 Mar 2022 10:55:26 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:55:31 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 01 Mar 2022 10:55:32 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 01 Mar 2022 10:55:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:56:18 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 01 Mar 2022 10:56:19 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 01 Mar 2022 10:56:38 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 01 Mar 2022 10:56:39 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 01 Mar 2022 10:56:40 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 01 Mar 2022 10:56:41 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 01 Mar 2022 10:56:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 10:56:42 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 01 Mar 2022 10:56:43 GMT
VOLUME [/opt/couchdb/data]
# Tue, 01 Mar 2022 10:56:44 GMT
EXPOSE 4369 5984 9100
# Tue, 01 Mar 2022 10:56:45 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:69bf0018a85cc0775a59a4dbda1b2f2e71086a2d817473f72336bf4d0a83b9d0`  
		Last Modified: Tue, 01 Mar 2022 02:19:15 GMT  
		Size: 25.9 MB (25923140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f3b0034185f805a7eca8287a2a7e1c7083a4a3803aa2ff831381977e362fdd`  
		Last Modified: Tue, 01 Mar 2022 10:57:38 GMT  
		Size: 3.3 KB (3321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b11afb5df4d7ceb32be036fdf972d3345cdb7577b89ee1e2f5718768554a3b3`  
		Last Modified: Tue, 01 Mar 2022 10:57:37 GMT  
		Size: 6.5 MB (6549945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01d9cba25fe10102232e70e1e262509477dcbda240c129c62ff2a79c6870918`  
		Last Modified: Tue, 01 Mar 2022 10:57:36 GMT  
		Size: 951.2 KB (951181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75a3508d3b60b5de298e4411ecdd1e54e257ebe20f94a95023c85b62a5c2ad3`  
		Last Modified: Tue, 01 Mar 2022 10:57:36 GMT  
		Size: 79.9 KB (79885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b102dd0eb55f11c90904fccef03a986e2109c1c15ab98820ba9c5821bfe7e07`  
		Last Modified: Tue, 01 Mar 2022 10:57:52 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84f7d5462854b7642f779f2acad5f45f22257a80b41ed8846f7416e79785332`  
		Last Modified: Tue, 01 Mar 2022 10:57:55 GMT  
		Size: 39.0 MB (39011744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f95c1a2438170f86f990ad088f83767ba8e419f1ac96cdb294ff40c617a7d3`  
		Last Modified: Tue, 01 Mar 2022 10:57:50 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7614832d184c7d5e6c6fb96776cbcd809045a5a10fce32f263ac293ff39195`  
		Last Modified: Tue, 01 Mar 2022 10:57:50 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e269a34ba04007a35b2fa7baec856b1c30f30c697671b8540c393e84a631d49`  
		Last Modified: Tue, 01 Mar 2022 10:57:50 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d4b074057a622e81c2cc34c78ffb522085c5f499dd352f356ccb5ab44f33f7`  
		Last Modified: Tue, 01 Mar 2022 10:57:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3.1`

```console
$ docker pull couchdb@sha256:4ef104f0a97f4016f48dea1056742f19863df2184af6db88b83b39d5306a9608
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:847e1795b0a0d237d9f94be94629e33d811e0104c8c508897958440e1bdcf06c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84517807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10596e5ba2cc278725271cb50463f181896f424dbf4b06da88ce36c6ac59fd18`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:56 GMT
ADD file:702017714ad3e1567b4f60b688750f8b631d91088e4dcf41351c4bb07749c579 in / 
# Tue, 01 Mar 2022 02:13:56 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 05:43:51 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 01 Mar 2022 05:43:52 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 01 Mar 2022 05:44:01 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 05:44:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 01 Mar 2022 05:44:05 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 01 Mar 2022 05:44:13 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 05:44:31 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 01 Mar 2022 05:44:32 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 01 Mar 2022 05:44:50 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 01 Mar 2022 05:44:50 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 01 Mar 2022 05:44:50 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 01 Mar 2022 05:44:50 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 01 Mar 2022 05:44:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 05:44:51 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 01 Mar 2022 05:44:51 GMT
VOLUME [/opt/couchdb/data]
# Tue, 01 Mar 2022 05:44:51 GMT
EXPOSE 4369 5984 9100
# Tue, 01 Mar 2022 05:44:51 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:15115158dd02a1bf2fd28724e3c1024394033fb0e9a5d3e451ed2715b6ae312d`  
		Last Modified: Tue, 01 Mar 2022 02:20:08 GMT  
		Size: 27.2 MB (27153737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e132993eb143d25686acdeb919d14985e8a65255f56170cc91230c350b203efa`  
		Last Modified: Tue, 01 Mar 2022 05:45:35 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50404ca1e1b3d297bb3c53a42e386f090eaa10f2d4db26fa324c39a836a18ea2`  
		Last Modified: Tue, 01 Mar 2022 05:45:34 GMT  
		Size: 6.7 MB (6691238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185b4237a163f4ee3d4cbb14cccd38dbfff817f923da22f90651149905d5957f`  
		Last Modified: Tue, 01 Mar 2022 05:45:33 GMT  
		Size: 1.3 MB (1258328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3a7c7c6b65c07b5de14a76f367630dcdc1f47fb75f959826b67e019b0617ec2`  
		Last Modified: Tue, 01 Mar 2022 05:45:33 GMT  
		Size: 293.0 KB (293032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10737976dd7f04dffd2c8080cb3ea3718e864fb550e1f8e3354886937546574`  
		Last Modified: Tue, 01 Mar 2022 05:45:48 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a11c8284534d8d62c430ef5edd0b754f191ed08eb41a89dd12c88cc42f8876e`  
		Last Modified: Tue, 01 Mar 2022 05:45:52 GMT  
		Size: 49.1 MB (49114456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54d99378c788f80c9ecc1d468356b808769ef6e72ba204e99075047a72d9401`  
		Last Modified: Tue, 01 Mar 2022 05:45:47 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8f2f19f0705503827a4fdc361a6f99896e1875fb4fddbf33721a673720aef6`  
		Last Modified: Tue, 01 Mar 2022 05:45:46 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bef14bec9c81959285cc9e53e3d5699eabb9be169611e2c125bbfd9f261c52b`  
		Last Modified: Tue, 01 Mar 2022 05:45:46 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd86d7a071c031c015596ab2ec6dcfe4cfdf70bd5082935f1016dc604a66c4f`  
		Last Modified: Tue, 01 Mar 2022 05:45:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:d5faeab69938596cc25f9c1b52105c67801c5187b3fa64fd5a40d539e40427d9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.5 MB (72522813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f49a6ea2840b6fad1f61ac250caadcda9144931bf249c8044548022a19566fad`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:57 GMT
ADD file:7d35162eea06441e7115c6fd9508802eafee00f64b11a7529a8f125bc67fa95e in / 
# Tue, 01 Mar 2022 02:11:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:55:17 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 01 Mar 2022 10:55:18 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 01 Mar 2022 10:55:26 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:55:31 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 01 Mar 2022 10:55:32 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 01 Mar 2022 10:55:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:56:18 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 01 Mar 2022 10:56:19 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 01 Mar 2022 10:56:38 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 01 Mar 2022 10:56:39 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 01 Mar 2022 10:56:40 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 01 Mar 2022 10:56:41 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 01 Mar 2022 10:56:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 10:56:42 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 01 Mar 2022 10:56:43 GMT
VOLUME [/opt/couchdb/data]
# Tue, 01 Mar 2022 10:56:44 GMT
EXPOSE 4369 5984 9100
# Tue, 01 Mar 2022 10:56:45 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:69bf0018a85cc0775a59a4dbda1b2f2e71086a2d817473f72336bf4d0a83b9d0`  
		Last Modified: Tue, 01 Mar 2022 02:19:15 GMT  
		Size: 25.9 MB (25923140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f3b0034185f805a7eca8287a2a7e1c7083a4a3803aa2ff831381977e362fdd`  
		Last Modified: Tue, 01 Mar 2022 10:57:38 GMT  
		Size: 3.3 KB (3321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b11afb5df4d7ceb32be036fdf972d3345cdb7577b89ee1e2f5718768554a3b3`  
		Last Modified: Tue, 01 Mar 2022 10:57:37 GMT  
		Size: 6.5 MB (6549945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01d9cba25fe10102232e70e1e262509477dcbda240c129c62ff2a79c6870918`  
		Last Modified: Tue, 01 Mar 2022 10:57:36 GMT  
		Size: 951.2 KB (951181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75a3508d3b60b5de298e4411ecdd1e54e257ebe20f94a95023c85b62a5c2ad3`  
		Last Modified: Tue, 01 Mar 2022 10:57:36 GMT  
		Size: 79.9 KB (79885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b102dd0eb55f11c90904fccef03a986e2109c1c15ab98820ba9c5821bfe7e07`  
		Last Modified: Tue, 01 Mar 2022 10:57:52 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84f7d5462854b7642f779f2acad5f45f22257a80b41ed8846f7416e79785332`  
		Last Modified: Tue, 01 Mar 2022 10:57:55 GMT  
		Size: 39.0 MB (39011744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f95c1a2438170f86f990ad088f83767ba8e419f1ac96cdb294ff40c617a7d3`  
		Last Modified: Tue, 01 Mar 2022 10:57:50 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7614832d184c7d5e6c6fb96776cbcd809045a5a10fce32f263ac293ff39195`  
		Last Modified: Tue, 01 Mar 2022 10:57:50 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e269a34ba04007a35b2fa7baec856b1c30f30c697671b8540c393e84a631d49`  
		Last Modified: Tue, 01 Mar 2022 10:57:50 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d4b074057a622e81c2cc34c78ffb522085c5f499dd352f356ccb5ab44f33f7`  
		Last Modified: Tue, 01 Mar 2022 10:57:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3`

```console
$ docker pull couchdb@sha256:d275d11cad8ce62d8c41bc221e71e7635eae899609f519b673e36754e0106f72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3` - linux; amd64

```console
$ docker pull couchdb@sha256:822d0f6a1fa1a4468bc77928901cd80cfb9b0679382255660da873c4570f0ea0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.4 MB (87438641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f265241b13e4aafb4f0fda52c6626eb1885d026244944902e2188c4765c30f0`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 05:43:11 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 01 Mar 2022 05:43:11 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 01 Mar 2022 05:43:19 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 05:43:23 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 01 Mar 2022 05:43:23 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 01 Mar 2022 05:43:28 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 05:43:28 GMT
ENV COUCHDB_VERSION=3.2.1-1
# Tue, 01 Mar 2022 05:43:29 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 01 Mar 2022 05:43:42 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 01 Mar 2022 05:43:42 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 01 Mar 2022 05:43:42 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 01 Mar 2022 05:43:43 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 01 Mar 2022 05:43:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 05:43:43 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 01 Mar 2022 05:43:43 GMT
VOLUME [/opt/couchdb/data]
# Tue, 01 Mar 2022 05:43:44 GMT
EXPOSE 4369 5984 9100
# Tue, 01 Mar 2022 05:43:44 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f736067abe3ec6aa7995ab61efa1d9a2b46b4c6a43e237fb15d6ba10bccc8a0`  
		Last Modified: Tue, 01 Mar 2022 05:45:13 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89cf0cd8366d641805527862400e1bce25dfe0e4d75301bfca351f6cb51adf42`  
		Last Modified: Tue, 01 Mar 2022 05:45:12 GMT  
		Size: 5.2 MB (5223244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6765d7966078499cee66919d4eae6c448903398520afd4a9af50e628602308dd`  
		Last Modified: Tue, 01 Mar 2022 05:45:11 GMT  
		Size: 1.6 MB (1553184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0aa553e191057af86f122b236ee318ab2840b814e55f6ed1f843dbf2734c3df`  
		Last Modified: Tue, 01 Mar 2022 05:45:11 GMT  
		Size: 295.5 KB (295513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6836a13a921ed1c7d33495e61fbf8c4110efd124ba364aa65719668d915df6`  
		Last Modified: Tue, 01 Mar 2022 05:45:11 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3670b70ba1f6cf592b77e0fbb8feefaa5d19731d115a8f40e5d7ad276b7572c0`  
		Last Modified: Tue, 01 Mar 2022 05:45:15 GMT  
		Size: 49.0 MB (48993167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6abf74c316c94beb45bf67044c6219f3205152bbc1a595080a4d646cad125055`  
		Last Modified: Tue, 01 Mar 2022 05:45:09 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91336f088c386950fab72a2eff4fb6e543ea167051299e920860f25763ddad4c`  
		Last Modified: Tue, 01 Mar 2022 05:45:09 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec02748684ecc64a7c390d3f95f2556ed75c995c0018dca6d3a5bcb4f10222e`  
		Last Modified: Tue, 01 Mar 2022 05:45:09 GMT  
		Size: 2.2 KB (2184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50b0fab1478c6789e174467f18aec4753c1a77109436988456425cef86c95aa`  
		Last Modified: Tue, 01 Mar 2022 05:45:09 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:3e6dc6d0db2d323fddb035a9432235b94c05601e90dede631eef8984dfbd59c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.6 MB (85578848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49ed81158960a991bcb8edcedb33f3bb86af2b2248ff74cadb7932938493c341`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:29 GMT
ADD file:9816c9c29627693c34afda4fa5e1a5e8a0f5aa3c5d5cfd920a4d89c77aab997d in / 
# Tue, 01 Mar 2022 02:11:30 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:54:16 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 01 Mar 2022 10:54:17 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 01 Mar 2022 10:54:25 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:54:29 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 01 Mar 2022 10:54:30 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 01 Mar 2022 10:54:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:54:37 GMT
ENV COUCHDB_VERSION=3.2.1-1
# Tue, 01 Mar 2022 10:54:38 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 01 Mar 2022 10:54:59 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 01 Mar 2022 10:55:00 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 01 Mar 2022 10:55:01 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 01 Mar 2022 10:55:02 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 01 Mar 2022 10:55:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 10:55:03 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 01 Mar 2022 10:55:04 GMT
VOLUME [/opt/couchdb/data]
# Tue, 01 Mar 2022 10:55:05 GMT
EXPOSE 4369 5984 9100
# Tue, 01 Mar 2022 10:55:06 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:279a020076a7fbddfc996e4c55e605a8f322810c3eca21cdedbcb06beb0e1305`  
		Last Modified: Tue, 01 Mar 2022 02:18:24 GMT  
		Size: 30.1 MB (30057008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfcff81d5bffc5f578ce75b1352bd0ec1fbc72e64741076e33fec78f31f8251`  
		Last Modified: Tue, 01 Mar 2022 10:57:14 GMT  
		Size: 3.3 KB (3321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd324560c127ebd17fc2f7dadad8e82385cada679ffe92bba01f0ac0dc1147c`  
		Last Modified: Tue, 01 Mar 2022 10:57:13 GMT  
		Size: 5.2 MB (5208018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b903e5b6f9f94a6b822e164537f5fce3c6b17d856646c5ed96bb2ca39b5d4d3a`  
		Last Modified: Tue, 01 Mar 2022 10:57:12 GMT  
		Size: 1.2 MB (1221005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c16dea62989609f7bd2a55428c40adcb00d517c47c9c52e0ec5e76d3e1af6ee`  
		Last Modified: Tue, 01 Mar 2022 10:57:12 GMT  
		Size: 79.1 KB (79098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66b3299f2b80a371f9445b89065781cb0070d916bc4cb9cfabc1d747159652cd`  
		Last Modified: Tue, 01 Mar 2022 10:57:12 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4ee9c5380651ad3aa998731b2c7cfceaff37464c95ab95dfb1880628869f77`  
		Last Modified: Tue, 01 Mar 2022 10:57:16 GMT  
		Size: 49.0 MB (49006666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce8d37b711b0d0f9efce1b36bb75dc4823a4d16b320d261e0b1f4aa51cee6c3`  
		Last Modified: Tue, 01 Mar 2022 10:57:10 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4daebd54e61f91fc444be8b7157fd4bbc43c96e578f49ac98381094e38ffc7a2`  
		Last Modified: Tue, 01 Mar 2022 10:57:10 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76d8dbd3035c9da1363c7be373af9100c55b68b887d37581e4ea815d31fcef7`  
		Last Modified: Tue, 01 Mar 2022 10:57:10 GMT  
		Size: 2.2 KB (2187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772c4d8177aba4266c7d6008fd9345bca757dc38dbdeeee5eda1b255e2a92b38`  
		Last Modified: Tue, 01 Mar 2022 10:57:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; ppc64le

```console
$ docker pull couchdb@sha256:910fc1e2c4c95579028118dd6ac80d60b5e34135807caae0b3b759bbd3f7558f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93156878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0af7fca6e0cc3d261c23d2b84ee250be1f1b53921c4e9e0cbe68619f6680d109`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 01 Mar 2022 02:05:07 GMT
ADD file:fc0989685aecf50ec36795d73893c30d9ddd4f946f8c5f4a6d10963f8ab41168 in / 
# Tue, 01 Mar 2022 02:05:12 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 07:26:33 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 02 Mar 2022 07:26:42 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 02 Mar 2022 07:27:18 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 07:27:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 02 Mar 2022 07:27:33 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 02 Mar 2022 07:27:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 07:27:58 GMT
ENV COUCHDB_VERSION=3.2.1-1
# Wed, 02 Mar 2022 07:28:03 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 02 Mar 2022 07:28:45 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 02 Mar 2022 07:28:49 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 02 Mar 2022 07:28:49 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 02 Mar 2022 07:28:51 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 02 Mar 2022 07:28:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 02 Mar 2022 07:28:56 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 02 Mar 2022 07:28:58 GMT
VOLUME [/opt/couchdb/data]
# Wed, 02 Mar 2022 07:29:00 GMT
EXPOSE 4369 5984 9100
# Wed, 02 Mar 2022 07:29:02 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:1dde9239ed493e1fe68971baa3f162c734ef0f461ad109e48aeb5b56daa55cc2`  
		Last Modified: Tue, 01 Mar 2022 02:15:19 GMT  
		Size: 35.3 MB (35272910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8e3b76def43005a4bad42db196a1af1f2e2a7571c562c402c6d5fab6b670fa`  
		Last Modified: Wed, 02 Mar 2022 07:29:28 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0b0be0220579d9a54e06e2c75add9959107db00f235745c5094280a38a0d66`  
		Last Modified: Wed, 02 Mar 2022 07:29:28 GMT  
		Size: 6.0 MB (6043478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8512718ccfd18b0d0555389092336b2345a224cf8741ecacd8cf0aefc13b56ad`  
		Last Modified: Wed, 02 Mar 2022 07:29:27 GMT  
		Size: 1.5 MB (1509175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0d3da23acf1804501e1d63f82b765ae6fff0d46daf6a85271bcd6485a2ac20`  
		Last Modified: Wed, 02 Mar 2022 07:29:26 GMT  
		Size: 295.6 KB (295572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079334cb185001d3836b007108d00ae394390595a59b51c946ddd3d6dcf748a0`  
		Last Modified: Wed, 02 Mar 2022 07:29:26 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92f960d7dfa5dfa0ceedc8b12ecda5b51ee8a82a42811c576537fc6009f5741`  
		Last Modified: Wed, 02 Mar 2022 07:29:31 GMT  
		Size: 50.0 MB (50028599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:618b23d01fac8298a56be32af0a4f1e0bf7e2e80a89587293ae671d5da9499b9`  
		Last Modified: Wed, 02 Mar 2022 07:29:24 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6739034ddd8a12ca87e41304cc52cea8bd9691c386759d8e336397f0e513e7`  
		Last Modified: Wed, 02 Mar 2022 07:29:24 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4641352460d612b4811a827f1e46eaca3d2bee21b5a9fe04e849a4461856173c`  
		Last Modified: Wed, 02 Mar 2022 07:29:24 GMT  
		Size: 2.2 KB (2185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dea3c3c346c9f62d3d3be2c25ca691732d97c66ac1dd786e1befc38de0d67a1`  
		Last Modified: Wed, 02 Mar 2022 07:29:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1`

```console
$ docker pull couchdb@sha256:59d2c2a05e2e5bc6bf773d686777e07870b63b229e9909281e1d7087b083f74a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:ca79518cf7009d4d0f0469fddac30481acbbc5c04dd9e4f68698c9fb209b2379
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80003576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52bd847d3676edaaf93238ec7616aeef0990d0d366c26034bf10cefa563907f7`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:56 GMT
ADD file:702017714ad3e1567b4f60b688750f8b631d91088e4dcf41351c4bb07749c579 in / 
# Tue, 01 Mar 2022 02:13:56 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 05:43:51 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 01 Mar 2022 05:43:52 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 01 Mar 2022 05:44:01 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 05:44:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 01 Mar 2022 05:44:05 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 01 Mar 2022 05:44:13 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 05:44:13 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 01 Mar 2022 05:44:14 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 01 Mar 2022 05:44:27 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 01 Mar 2022 05:44:28 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 01 Mar 2022 05:44:28 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 01 Mar 2022 05:44:28 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 01 Mar 2022 05:44:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 05:44:29 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 01 Mar 2022 05:44:29 GMT
VOLUME [/opt/couchdb/data]
# Tue, 01 Mar 2022 05:44:29 GMT
EXPOSE 4369 5984 9100
# Tue, 01 Mar 2022 05:44:29 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:15115158dd02a1bf2fd28724e3c1024394033fb0e9a5d3e451ed2715b6ae312d`  
		Last Modified: Tue, 01 Mar 2022 02:20:08 GMT  
		Size: 27.2 MB (27153737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e132993eb143d25686acdeb919d14985e8a65255f56170cc91230c350b203efa`  
		Last Modified: Tue, 01 Mar 2022 05:45:35 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50404ca1e1b3d297bb3c53a42e386f090eaa10f2d4db26fa324c39a836a18ea2`  
		Last Modified: Tue, 01 Mar 2022 05:45:34 GMT  
		Size: 6.7 MB (6691238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185b4237a163f4ee3d4cbb14cccd38dbfff817f923da22f90651149905d5957f`  
		Last Modified: Tue, 01 Mar 2022 05:45:33 GMT  
		Size: 1.3 MB (1258328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3a7c7c6b65c07b5de14a76f367630dcdc1f47fb75f959826b67e019b0617ec2`  
		Last Modified: Tue, 01 Mar 2022 05:45:33 GMT  
		Size: 293.0 KB (293032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30360495bdc30a76fa2b700246ad48767cacf9d445a76c0a5794bb67ffe1ff8a`  
		Last Modified: Tue, 01 Mar 2022 05:45:32 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c66f25dd672892d6a4f8fe8ada5c2761d4e92d82b846c1b3c0c324f20736ea7`  
		Last Modified: Tue, 01 Mar 2022 05:45:36 GMT  
		Size: 44.6 MB (44600228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0fa53bb7e951e99619bfc60a13fe5fdb4627934cd960bfa56b8d32e1f7f7ff4`  
		Last Modified: Tue, 01 Mar 2022 05:45:30 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ec6b081df4af00c592f2a0bb9b8d16a2e164dbc88510fac16341ee519f518f`  
		Last Modified: Tue, 01 Mar 2022 05:45:30 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bae1344cc973a946de72a34a50f850ee96245021b199d90b188174ded7f00e3`  
		Last Modified: Tue, 01 Mar 2022 05:45:30 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc978b9768eef46e866245b0df9c77957340e1ec7cc6935b34d15c38ce7623f5`  
		Last Modified: Tue, 01 Mar 2022 05:45:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:5f8dac4539f06028cd3ebb23990a6ccc41654b62c7a7c9839d46d8b1064104f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74612104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96626e4e6b82ff4ca1ff8ca3d3eda6acd2c1edb16fc68c307509a39302d31b0b`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:57 GMT
ADD file:7d35162eea06441e7115c6fd9508802eafee00f64b11a7529a8f125bc67fa95e in / 
# Tue, 01 Mar 2022 02:11:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:55:17 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 01 Mar 2022 10:55:18 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 01 Mar 2022 10:55:26 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:55:31 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 01 Mar 2022 10:55:32 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 01 Mar 2022 10:55:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:55:39 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 01 Mar 2022 10:55:40 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 01 Mar 2022 10:56:00 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 01 Mar 2022 10:56:01 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 01 Mar 2022 10:56:02 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 01 Mar 2022 10:56:03 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 01 Mar 2022 10:56:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 10:56:04 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 01 Mar 2022 10:56:05 GMT
VOLUME [/opt/couchdb/data]
# Tue, 01 Mar 2022 10:56:06 GMT
EXPOSE 4369 5984 9100
# Tue, 01 Mar 2022 10:56:07 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:69bf0018a85cc0775a59a4dbda1b2f2e71086a2d817473f72336bf4d0a83b9d0`  
		Last Modified: Tue, 01 Mar 2022 02:19:15 GMT  
		Size: 25.9 MB (25923140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f3b0034185f805a7eca8287a2a7e1c7083a4a3803aa2ff831381977e362fdd`  
		Last Modified: Tue, 01 Mar 2022 10:57:38 GMT  
		Size: 3.3 KB (3321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b11afb5df4d7ceb32be036fdf972d3345cdb7577b89ee1e2f5718768554a3b3`  
		Last Modified: Tue, 01 Mar 2022 10:57:37 GMT  
		Size: 6.5 MB (6549945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01d9cba25fe10102232e70e1e262509477dcbda240c129c62ff2a79c6870918`  
		Last Modified: Tue, 01 Mar 2022 10:57:36 GMT  
		Size: 951.2 KB (951181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75a3508d3b60b5de298e4411ecdd1e54e257ebe20f94a95023c85b62a5c2ad3`  
		Last Modified: Tue, 01 Mar 2022 10:57:36 GMT  
		Size: 79.9 KB (79885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fd20e0726ac6872eb93ae32931222420923cddc35a82d1837bce297f9a1c688`  
		Last Modified: Tue, 01 Mar 2022 10:57:36 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8567e8d6ec7c59ba98a6eb76aebda0812faad30e413650fbef6e472d2df467`  
		Last Modified: Tue, 01 Mar 2022 10:57:39 GMT  
		Size: 41.1 MB (41101035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b812b68765debb885ecc8cfbf4d04e83765c46ce0aedc425b31aeb639b15e2`  
		Last Modified: Tue, 01 Mar 2022 10:57:34 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cd704848b3b3a7577ef01bdc35a296be3225c307b4a590cb45a492395bfaec`  
		Last Modified: Tue, 01 Mar 2022 10:57:34 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c866c2a179409d96705fafdac1defc3fd36da15d4134ddb7723ca83aa03797f3`  
		Last Modified: Tue, 01 Mar 2022 10:57:34 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e167116d1ad782a3daab07acadb106fb1dd956fbb7bf7698577c2fdef9c54f3`  
		Last Modified: Tue, 01 Mar 2022 10:57:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1.2`

```console
$ docker pull couchdb@sha256:59d2c2a05e2e5bc6bf773d686777e07870b63b229e9909281e1d7087b083f74a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1.2` - linux; amd64

```console
$ docker pull couchdb@sha256:ca79518cf7009d4d0f0469fddac30481acbbc5c04dd9e4f68698c9fb209b2379
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80003576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52bd847d3676edaaf93238ec7616aeef0990d0d366c26034bf10cefa563907f7`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:56 GMT
ADD file:702017714ad3e1567b4f60b688750f8b631d91088e4dcf41351c4bb07749c579 in / 
# Tue, 01 Mar 2022 02:13:56 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 05:43:51 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 01 Mar 2022 05:43:52 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 01 Mar 2022 05:44:01 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 05:44:05 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 01 Mar 2022 05:44:05 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 01 Mar 2022 05:44:13 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 05:44:13 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 01 Mar 2022 05:44:14 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 01 Mar 2022 05:44:27 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 01 Mar 2022 05:44:28 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 01 Mar 2022 05:44:28 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 01 Mar 2022 05:44:28 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 01 Mar 2022 05:44:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 05:44:29 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 01 Mar 2022 05:44:29 GMT
VOLUME [/opt/couchdb/data]
# Tue, 01 Mar 2022 05:44:29 GMT
EXPOSE 4369 5984 9100
# Tue, 01 Mar 2022 05:44:29 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:15115158dd02a1bf2fd28724e3c1024394033fb0e9a5d3e451ed2715b6ae312d`  
		Last Modified: Tue, 01 Mar 2022 02:20:08 GMT  
		Size: 27.2 MB (27153737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e132993eb143d25686acdeb919d14985e8a65255f56170cc91230c350b203efa`  
		Last Modified: Tue, 01 Mar 2022 05:45:35 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50404ca1e1b3d297bb3c53a42e386f090eaa10f2d4db26fa324c39a836a18ea2`  
		Last Modified: Tue, 01 Mar 2022 05:45:34 GMT  
		Size: 6.7 MB (6691238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185b4237a163f4ee3d4cbb14cccd38dbfff817f923da22f90651149905d5957f`  
		Last Modified: Tue, 01 Mar 2022 05:45:33 GMT  
		Size: 1.3 MB (1258328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3a7c7c6b65c07b5de14a76f367630dcdc1f47fb75f959826b67e019b0617ec2`  
		Last Modified: Tue, 01 Mar 2022 05:45:33 GMT  
		Size: 293.0 KB (293032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30360495bdc30a76fa2b700246ad48767cacf9d445a76c0a5794bb67ffe1ff8a`  
		Last Modified: Tue, 01 Mar 2022 05:45:32 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c66f25dd672892d6a4f8fe8ada5c2761d4e92d82b846c1b3c0c324f20736ea7`  
		Last Modified: Tue, 01 Mar 2022 05:45:36 GMT  
		Size: 44.6 MB (44600228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0fa53bb7e951e99619bfc60a13fe5fdb4627934cd960bfa56b8d32e1f7f7ff4`  
		Last Modified: Tue, 01 Mar 2022 05:45:30 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ec6b081df4af00c592f2a0bb9b8d16a2e164dbc88510fac16341ee519f518f`  
		Last Modified: Tue, 01 Mar 2022 05:45:30 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bae1344cc973a946de72a34a50f850ee96245021b199d90b188174ded7f00e3`  
		Last Modified: Tue, 01 Mar 2022 05:45:30 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc978b9768eef46e866245b0df9c77957340e1ec7cc6935b34d15c38ce7623f5`  
		Last Modified: Tue, 01 Mar 2022 05:45:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:5f8dac4539f06028cd3ebb23990a6ccc41654b62c7a7c9839d46d8b1064104f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74612104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96626e4e6b82ff4ca1ff8ca3d3eda6acd2c1edb16fc68c307509a39302d31b0b`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:57 GMT
ADD file:7d35162eea06441e7115c6fd9508802eafee00f64b11a7529a8f125bc67fa95e in / 
# Tue, 01 Mar 2022 02:11:57 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:55:17 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 01 Mar 2022 10:55:18 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 01 Mar 2022 10:55:26 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:55:31 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 01 Mar 2022 10:55:32 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 01 Mar 2022 10:55:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:55:39 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 01 Mar 2022 10:55:40 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 01 Mar 2022 10:56:00 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 01 Mar 2022 10:56:01 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 01 Mar 2022 10:56:02 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 01 Mar 2022 10:56:03 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 01 Mar 2022 10:56:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 10:56:04 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 01 Mar 2022 10:56:05 GMT
VOLUME [/opt/couchdb/data]
# Tue, 01 Mar 2022 10:56:06 GMT
EXPOSE 4369 5984 9100
# Tue, 01 Mar 2022 10:56:07 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:69bf0018a85cc0775a59a4dbda1b2f2e71086a2d817473f72336bf4d0a83b9d0`  
		Last Modified: Tue, 01 Mar 2022 02:19:15 GMT  
		Size: 25.9 MB (25923140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f3b0034185f805a7eca8287a2a7e1c7083a4a3803aa2ff831381977e362fdd`  
		Last Modified: Tue, 01 Mar 2022 10:57:38 GMT  
		Size: 3.3 KB (3321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b11afb5df4d7ceb32be036fdf972d3345cdb7577b89ee1e2f5718768554a3b3`  
		Last Modified: Tue, 01 Mar 2022 10:57:37 GMT  
		Size: 6.5 MB (6549945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01d9cba25fe10102232e70e1e262509477dcbda240c129c62ff2a79c6870918`  
		Last Modified: Tue, 01 Mar 2022 10:57:36 GMT  
		Size: 951.2 KB (951181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75a3508d3b60b5de298e4411ecdd1e54e257ebe20f94a95023c85b62a5c2ad3`  
		Last Modified: Tue, 01 Mar 2022 10:57:36 GMT  
		Size: 79.9 KB (79885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fd20e0726ac6872eb93ae32931222420923cddc35a82d1837bce297f9a1c688`  
		Last Modified: Tue, 01 Mar 2022 10:57:36 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8567e8d6ec7c59ba98a6eb76aebda0812faad30e413650fbef6e472d2df467`  
		Last Modified: Tue, 01 Mar 2022 10:57:39 GMT  
		Size: 41.1 MB (41101035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b812b68765debb885ecc8cfbf4d04e83765c46ce0aedc425b31aeb639b15e2`  
		Last Modified: Tue, 01 Mar 2022 10:57:34 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cd704848b3b3a7577ef01bdc35a296be3225c307b4a590cb45a492395bfaec`  
		Last Modified: Tue, 01 Mar 2022 10:57:34 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c866c2a179409d96705fafdac1defc3fd36da15d4134ddb7723ca83aa03797f3`  
		Last Modified: Tue, 01 Mar 2022 10:57:34 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e167116d1ad782a3daab07acadb106fb1dd956fbb7bf7698577c2fdef9c54f3`  
		Last Modified: Tue, 01 Mar 2022 10:57:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2`

```console
$ docker pull couchdb@sha256:d275d11cad8ce62d8c41bc221e71e7635eae899609f519b673e36754e0106f72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2` - linux; amd64

```console
$ docker pull couchdb@sha256:822d0f6a1fa1a4468bc77928901cd80cfb9b0679382255660da873c4570f0ea0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.4 MB (87438641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f265241b13e4aafb4f0fda52c6626eb1885d026244944902e2188c4765c30f0`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 05:43:11 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 01 Mar 2022 05:43:11 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 01 Mar 2022 05:43:19 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 05:43:23 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 01 Mar 2022 05:43:23 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 01 Mar 2022 05:43:28 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 05:43:28 GMT
ENV COUCHDB_VERSION=3.2.1-1
# Tue, 01 Mar 2022 05:43:29 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 01 Mar 2022 05:43:42 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 01 Mar 2022 05:43:42 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 01 Mar 2022 05:43:42 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 01 Mar 2022 05:43:43 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 01 Mar 2022 05:43:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 05:43:43 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 01 Mar 2022 05:43:43 GMT
VOLUME [/opt/couchdb/data]
# Tue, 01 Mar 2022 05:43:44 GMT
EXPOSE 4369 5984 9100
# Tue, 01 Mar 2022 05:43:44 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f736067abe3ec6aa7995ab61efa1d9a2b46b4c6a43e237fb15d6ba10bccc8a0`  
		Last Modified: Tue, 01 Mar 2022 05:45:13 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89cf0cd8366d641805527862400e1bce25dfe0e4d75301bfca351f6cb51adf42`  
		Last Modified: Tue, 01 Mar 2022 05:45:12 GMT  
		Size: 5.2 MB (5223244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6765d7966078499cee66919d4eae6c448903398520afd4a9af50e628602308dd`  
		Last Modified: Tue, 01 Mar 2022 05:45:11 GMT  
		Size: 1.6 MB (1553184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0aa553e191057af86f122b236ee318ab2840b814e55f6ed1f843dbf2734c3df`  
		Last Modified: Tue, 01 Mar 2022 05:45:11 GMT  
		Size: 295.5 KB (295513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6836a13a921ed1c7d33495e61fbf8c4110efd124ba364aa65719668d915df6`  
		Last Modified: Tue, 01 Mar 2022 05:45:11 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3670b70ba1f6cf592b77e0fbb8feefaa5d19731d115a8f40e5d7ad276b7572c0`  
		Last Modified: Tue, 01 Mar 2022 05:45:15 GMT  
		Size: 49.0 MB (48993167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6abf74c316c94beb45bf67044c6219f3205152bbc1a595080a4d646cad125055`  
		Last Modified: Tue, 01 Mar 2022 05:45:09 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91336f088c386950fab72a2eff4fb6e543ea167051299e920860f25763ddad4c`  
		Last Modified: Tue, 01 Mar 2022 05:45:09 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec02748684ecc64a7c390d3f95f2556ed75c995c0018dca6d3a5bcb4f10222e`  
		Last Modified: Tue, 01 Mar 2022 05:45:09 GMT  
		Size: 2.2 KB (2184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50b0fab1478c6789e174467f18aec4753c1a77109436988456425cef86c95aa`  
		Last Modified: Tue, 01 Mar 2022 05:45:09 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:3e6dc6d0db2d323fddb035a9432235b94c05601e90dede631eef8984dfbd59c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.6 MB (85578848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49ed81158960a991bcb8edcedb33f3bb86af2b2248ff74cadb7932938493c341`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:29 GMT
ADD file:9816c9c29627693c34afda4fa5e1a5e8a0f5aa3c5d5cfd920a4d89c77aab997d in / 
# Tue, 01 Mar 2022 02:11:30 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:54:16 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 01 Mar 2022 10:54:17 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 01 Mar 2022 10:54:25 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:54:29 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 01 Mar 2022 10:54:30 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 01 Mar 2022 10:54:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:54:37 GMT
ENV COUCHDB_VERSION=3.2.1-1
# Tue, 01 Mar 2022 10:54:38 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 01 Mar 2022 10:54:59 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 01 Mar 2022 10:55:00 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 01 Mar 2022 10:55:01 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 01 Mar 2022 10:55:02 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 01 Mar 2022 10:55:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 10:55:03 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 01 Mar 2022 10:55:04 GMT
VOLUME [/opt/couchdb/data]
# Tue, 01 Mar 2022 10:55:05 GMT
EXPOSE 4369 5984 9100
# Tue, 01 Mar 2022 10:55:06 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:279a020076a7fbddfc996e4c55e605a8f322810c3eca21cdedbcb06beb0e1305`  
		Last Modified: Tue, 01 Mar 2022 02:18:24 GMT  
		Size: 30.1 MB (30057008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfcff81d5bffc5f578ce75b1352bd0ec1fbc72e64741076e33fec78f31f8251`  
		Last Modified: Tue, 01 Mar 2022 10:57:14 GMT  
		Size: 3.3 KB (3321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd324560c127ebd17fc2f7dadad8e82385cada679ffe92bba01f0ac0dc1147c`  
		Last Modified: Tue, 01 Mar 2022 10:57:13 GMT  
		Size: 5.2 MB (5208018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b903e5b6f9f94a6b822e164537f5fce3c6b17d856646c5ed96bb2ca39b5d4d3a`  
		Last Modified: Tue, 01 Mar 2022 10:57:12 GMT  
		Size: 1.2 MB (1221005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c16dea62989609f7bd2a55428c40adcb00d517c47c9c52e0ec5e76d3e1af6ee`  
		Last Modified: Tue, 01 Mar 2022 10:57:12 GMT  
		Size: 79.1 KB (79098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66b3299f2b80a371f9445b89065781cb0070d916bc4cb9cfabc1d747159652cd`  
		Last Modified: Tue, 01 Mar 2022 10:57:12 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4ee9c5380651ad3aa998731b2c7cfceaff37464c95ab95dfb1880628869f77`  
		Last Modified: Tue, 01 Mar 2022 10:57:16 GMT  
		Size: 49.0 MB (49006666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce8d37b711b0d0f9efce1b36bb75dc4823a4d16b320d261e0b1f4aa51cee6c3`  
		Last Modified: Tue, 01 Mar 2022 10:57:10 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4daebd54e61f91fc444be8b7157fd4bbc43c96e578f49ac98381094e38ffc7a2`  
		Last Modified: Tue, 01 Mar 2022 10:57:10 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76d8dbd3035c9da1363c7be373af9100c55b68b887d37581e4ea815d31fcef7`  
		Last Modified: Tue, 01 Mar 2022 10:57:10 GMT  
		Size: 2.2 KB (2187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772c4d8177aba4266c7d6008fd9345bca757dc38dbdeeee5eda1b255e2a92b38`  
		Last Modified: Tue, 01 Mar 2022 10:57:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; ppc64le

```console
$ docker pull couchdb@sha256:910fc1e2c4c95579028118dd6ac80d60b5e34135807caae0b3b759bbd3f7558f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93156878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0af7fca6e0cc3d261c23d2b84ee250be1f1b53921c4e9e0cbe68619f6680d109`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 01 Mar 2022 02:05:07 GMT
ADD file:fc0989685aecf50ec36795d73893c30d9ddd4f946f8c5f4a6d10963f8ab41168 in / 
# Tue, 01 Mar 2022 02:05:12 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 07:26:33 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 02 Mar 2022 07:26:42 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 02 Mar 2022 07:27:18 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 07:27:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 02 Mar 2022 07:27:33 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 02 Mar 2022 07:27:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 07:27:58 GMT
ENV COUCHDB_VERSION=3.2.1-1
# Wed, 02 Mar 2022 07:28:03 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 02 Mar 2022 07:28:45 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 02 Mar 2022 07:28:49 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 02 Mar 2022 07:28:49 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 02 Mar 2022 07:28:51 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 02 Mar 2022 07:28:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 02 Mar 2022 07:28:56 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 02 Mar 2022 07:28:58 GMT
VOLUME [/opt/couchdb/data]
# Wed, 02 Mar 2022 07:29:00 GMT
EXPOSE 4369 5984 9100
# Wed, 02 Mar 2022 07:29:02 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:1dde9239ed493e1fe68971baa3f162c734ef0f461ad109e48aeb5b56daa55cc2`  
		Last Modified: Tue, 01 Mar 2022 02:15:19 GMT  
		Size: 35.3 MB (35272910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8e3b76def43005a4bad42db196a1af1f2e2a7571c562c402c6d5fab6b670fa`  
		Last Modified: Wed, 02 Mar 2022 07:29:28 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0b0be0220579d9a54e06e2c75add9959107db00f235745c5094280a38a0d66`  
		Last Modified: Wed, 02 Mar 2022 07:29:28 GMT  
		Size: 6.0 MB (6043478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8512718ccfd18b0d0555389092336b2345a224cf8741ecacd8cf0aefc13b56ad`  
		Last Modified: Wed, 02 Mar 2022 07:29:27 GMT  
		Size: 1.5 MB (1509175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0d3da23acf1804501e1d63f82b765ae6fff0d46daf6a85271bcd6485a2ac20`  
		Last Modified: Wed, 02 Mar 2022 07:29:26 GMT  
		Size: 295.6 KB (295572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079334cb185001d3836b007108d00ae394390595a59b51c946ddd3d6dcf748a0`  
		Last Modified: Wed, 02 Mar 2022 07:29:26 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92f960d7dfa5dfa0ceedc8b12ecda5b51ee8a82a42811c576537fc6009f5741`  
		Last Modified: Wed, 02 Mar 2022 07:29:31 GMT  
		Size: 50.0 MB (50028599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:618b23d01fac8298a56be32af0a4f1e0bf7e2e80a89587293ae671d5da9499b9`  
		Last Modified: Wed, 02 Mar 2022 07:29:24 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6739034ddd8a12ca87e41304cc52cea8bd9691c386759d8e336397f0e513e7`  
		Last Modified: Wed, 02 Mar 2022 07:29:24 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4641352460d612b4811a827f1e46eaca3d2bee21b5a9fe04e849a4461856173c`  
		Last Modified: Wed, 02 Mar 2022 07:29:24 GMT  
		Size: 2.2 KB (2185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dea3c3c346c9f62d3d3be2c25ca691732d97c66ac1dd786e1befc38de0d67a1`  
		Last Modified: Wed, 02 Mar 2022 07:29:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2.1`

```console
$ docker pull couchdb@sha256:d275d11cad8ce62d8c41bc221e71e7635eae899609f519b673e36754e0106f72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2.1` - linux; amd64

```console
$ docker pull couchdb@sha256:822d0f6a1fa1a4468bc77928901cd80cfb9b0679382255660da873c4570f0ea0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.4 MB (87438641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f265241b13e4aafb4f0fda52c6626eb1885d026244944902e2188c4765c30f0`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 05:43:11 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 01 Mar 2022 05:43:11 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 01 Mar 2022 05:43:19 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 05:43:23 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 01 Mar 2022 05:43:23 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 01 Mar 2022 05:43:28 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 05:43:28 GMT
ENV COUCHDB_VERSION=3.2.1-1
# Tue, 01 Mar 2022 05:43:29 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 01 Mar 2022 05:43:42 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 01 Mar 2022 05:43:42 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 01 Mar 2022 05:43:42 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 01 Mar 2022 05:43:43 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 01 Mar 2022 05:43:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 05:43:43 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 01 Mar 2022 05:43:43 GMT
VOLUME [/opt/couchdb/data]
# Tue, 01 Mar 2022 05:43:44 GMT
EXPOSE 4369 5984 9100
# Tue, 01 Mar 2022 05:43:44 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f736067abe3ec6aa7995ab61efa1d9a2b46b4c6a43e237fb15d6ba10bccc8a0`  
		Last Modified: Tue, 01 Mar 2022 05:45:13 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89cf0cd8366d641805527862400e1bce25dfe0e4d75301bfca351f6cb51adf42`  
		Last Modified: Tue, 01 Mar 2022 05:45:12 GMT  
		Size: 5.2 MB (5223244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6765d7966078499cee66919d4eae6c448903398520afd4a9af50e628602308dd`  
		Last Modified: Tue, 01 Mar 2022 05:45:11 GMT  
		Size: 1.6 MB (1553184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0aa553e191057af86f122b236ee318ab2840b814e55f6ed1f843dbf2734c3df`  
		Last Modified: Tue, 01 Mar 2022 05:45:11 GMT  
		Size: 295.5 KB (295513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6836a13a921ed1c7d33495e61fbf8c4110efd124ba364aa65719668d915df6`  
		Last Modified: Tue, 01 Mar 2022 05:45:11 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3670b70ba1f6cf592b77e0fbb8feefaa5d19731d115a8f40e5d7ad276b7572c0`  
		Last Modified: Tue, 01 Mar 2022 05:45:15 GMT  
		Size: 49.0 MB (48993167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6abf74c316c94beb45bf67044c6219f3205152bbc1a595080a4d646cad125055`  
		Last Modified: Tue, 01 Mar 2022 05:45:09 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91336f088c386950fab72a2eff4fb6e543ea167051299e920860f25763ddad4c`  
		Last Modified: Tue, 01 Mar 2022 05:45:09 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec02748684ecc64a7c390d3f95f2556ed75c995c0018dca6d3a5bcb4f10222e`  
		Last Modified: Tue, 01 Mar 2022 05:45:09 GMT  
		Size: 2.2 KB (2184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50b0fab1478c6789e174467f18aec4753c1a77109436988456425cef86c95aa`  
		Last Modified: Tue, 01 Mar 2022 05:45:09 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:3e6dc6d0db2d323fddb035a9432235b94c05601e90dede631eef8984dfbd59c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.6 MB (85578848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49ed81158960a991bcb8edcedb33f3bb86af2b2248ff74cadb7932938493c341`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:29 GMT
ADD file:9816c9c29627693c34afda4fa5e1a5e8a0f5aa3c5d5cfd920a4d89c77aab997d in / 
# Tue, 01 Mar 2022 02:11:30 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:54:16 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 01 Mar 2022 10:54:17 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 01 Mar 2022 10:54:25 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:54:29 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 01 Mar 2022 10:54:30 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 01 Mar 2022 10:54:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:54:37 GMT
ENV COUCHDB_VERSION=3.2.1-1
# Tue, 01 Mar 2022 10:54:38 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 01 Mar 2022 10:54:59 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 01 Mar 2022 10:55:00 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 01 Mar 2022 10:55:01 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 01 Mar 2022 10:55:02 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 01 Mar 2022 10:55:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 10:55:03 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 01 Mar 2022 10:55:04 GMT
VOLUME [/opt/couchdb/data]
# Tue, 01 Mar 2022 10:55:05 GMT
EXPOSE 4369 5984 9100
# Tue, 01 Mar 2022 10:55:06 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:279a020076a7fbddfc996e4c55e605a8f322810c3eca21cdedbcb06beb0e1305`  
		Last Modified: Tue, 01 Mar 2022 02:18:24 GMT  
		Size: 30.1 MB (30057008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfcff81d5bffc5f578ce75b1352bd0ec1fbc72e64741076e33fec78f31f8251`  
		Last Modified: Tue, 01 Mar 2022 10:57:14 GMT  
		Size: 3.3 KB (3321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd324560c127ebd17fc2f7dadad8e82385cada679ffe92bba01f0ac0dc1147c`  
		Last Modified: Tue, 01 Mar 2022 10:57:13 GMT  
		Size: 5.2 MB (5208018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b903e5b6f9f94a6b822e164537f5fce3c6b17d856646c5ed96bb2ca39b5d4d3a`  
		Last Modified: Tue, 01 Mar 2022 10:57:12 GMT  
		Size: 1.2 MB (1221005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c16dea62989609f7bd2a55428c40adcb00d517c47c9c52e0ec5e76d3e1af6ee`  
		Last Modified: Tue, 01 Mar 2022 10:57:12 GMT  
		Size: 79.1 KB (79098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66b3299f2b80a371f9445b89065781cb0070d916bc4cb9cfabc1d747159652cd`  
		Last Modified: Tue, 01 Mar 2022 10:57:12 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4ee9c5380651ad3aa998731b2c7cfceaff37464c95ab95dfb1880628869f77`  
		Last Modified: Tue, 01 Mar 2022 10:57:16 GMT  
		Size: 49.0 MB (49006666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce8d37b711b0d0f9efce1b36bb75dc4823a4d16b320d261e0b1f4aa51cee6c3`  
		Last Modified: Tue, 01 Mar 2022 10:57:10 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4daebd54e61f91fc444be8b7157fd4bbc43c96e578f49ac98381094e38ffc7a2`  
		Last Modified: Tue, 01 Mar 2022 10:57:10 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76d8dbd3035c9da1363c7be373af9100c55b68b887d37581e4ea815d31fcef7`  
		Last Modified: Tue, 01 Mar 2022 10:57:10 GMT  
		Size: 2.2 KB (2187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772c4d8177aba4266c7d6008fd9345bca757dc38dbdeeee5eda1b255e2a92b38`  
		Last Modified: Tue, 01 Mar 2022 10:57:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2.1` - linux; ppc64le

```console
$ docker pull couchdb@sha256:910fc1e2c4c95579028118dd6ac80d60b5e34135807caae0b3b759bbd3f7558f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93156878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0af7fca6e0cc3d261c23d2b84ee250be1f1b53921c4e9e0cbe68619f6680d109`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 01 Mar 2022 02:05:07 GMT
ADD file:fc0989685aecf50ec36795d73893c30d9ddd4f946f8c5f4a6d10963f8ab41168 in / 
# Tue, 01 Mar 2022 02:05:12 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 07:26:33 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 02 Mar 2022 07:26:42 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 02 Mar 2022 07:27:18 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 07:27:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 02 Mar 2022 07:27:33 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 02 Mar 2022 07:27:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 07:27:58 GMT
ENV COUCHDB_VERSION=3.2.1-1
# Wed, 02 Mar 2022 07:28:03 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 02 Mar 2022 07:28:45 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 02 Mar 2022 07:28:49 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 02 Mar 2022 07:28:49 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 02 Mar 2022 07:28:51 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 02 Mar 2022 07:28:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 02 Mar 2022 07:28:56 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 02 Mar 2022 07:28:58 GMT
VOLUME [/opt/couchdb/data]
# Wed, 02 Mar 2022 07:29:00 GMT
EXPOSE 4369 5984 9100
# Wed, 02 Mar 2022 07:29:02 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:1dde9239ed493e1fe68971baa3f162c734ef0f461ad109e48aeb5b56daa55cc2`  
		Last Modified: Tue, 01 Mar 2022 02:15:19 GMT  
		Size: 35.3 MB (35272910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8e3b76def43005a4bad42db196a1af1f2e2a7571c562c402c6d5fab6b670fa`  
		Last Modified: Wed, 02 Mar 2022 07:29:28 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0b0be0220579d9a54e06e2c75add9959107db00f235745c5094280a38a0d66`  
		Last Modified: Wed, 02 Mar 2022 07:29:28 GMT  
		Size: 6.0 MB (6043478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8512718ccfd18b0d0555389092336b2345a224cf8741ecacd8cf0aefc13b56ad`  
		Last Modified: Wed, 02 Mar 2022 07:29:27 GMT  
		Size: 1.5 MB (1509175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0d3da23acf1804501e1d63f82b765ae6fff0d46daf6a85271bcd6485a2ac20`  
		Last Modified: Wed, 02 Mar 2022 07:29:26 GMT  
		Size: 295.6 KB (295572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079334cb185001d3836b007108d00ae394390595a59b51c946ddd3d6dcf748a0`  
		Last Modified: Wed, 02 Mar 2022 07:29:26 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92f960d7dfa5dfa0ceedc8b12ecda5b51ee8a82a42811c576537fc6009f5741`  
		Last Modified: Wed, 02 Mar 2022 07:29:31 GMT  
		Size: 50.0 MB (50028599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:618b23d01fac8298a56be32af0a4f1e0bf7e2e80a89587293ae671d5da9499b9`  
		Last Modified: Wed, 02 Mar 2022 07:29:24 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6739034ddd8a12ca87e41304cc52cea8bd9691c386759d8e336397f0e513e7`  
		Last Modified: Wed, 02 Mar 2022 07:29:24 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4641352460d612b4811a827f1e46eaca3d2bee21b5a9fe04e849a4461856173c`  
		Last Modified: Wed, 02 Mar 2022 07:29:24 GMT  
		Size: 2.2 KB (2185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dea3c3c346c9f62d3d3be2c25ca691732d97c66ac1dd786e1befc38de0d67a1`  
		Last Modified: Wed, 02 Mar 2022 07:29:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:latest`

```console
$ docker pull couchdb@sha256:d275d11cad8ce62d8c41bc221e71e7635eae899609f519b673e36754e0106f72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:822d0f6a1fa1a4468bc77928901cd80cfb9b0679382255660da873c4570f0ea0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.4 MB (87438641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f265241b13e4aafb4f0fda52c6626eb1885d026244944902e2188c4765c30f0`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 05:43:11 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 01 Mar 2022 05:43:11 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 01 Mar 2022 05:43:19 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 05:43:23 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 01 Mar 2022 05:43:23 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 01 Mar 2022 05:43:28 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 05:43:28 GMT
ENV COUCHDB_VERSION=3.2.1-1
# Tue, 01 Mar 2022 05:43:29 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 01 Mar 2022 05:43:42 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 01 Mar 2022 05:43:42 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 01 Mar 2022 05:43:42 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 01 Mar 2022 05:43:43 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 01 Mar 2022 05:43:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 05:43:43 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 01 Mar 2022 05:43:43 GMT
VOLUME [/opt/couchdb/data]
# Tue, 01 Mar 2022 05:43:44 GMT
EXPOSE 4369 5984 9100
# Tue, 01 Mar 2022 05:43:44 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f736067abe3ec6aa7995ab61efa1d9a2b46b4c6a43e237fb15d6ba10bccc8a0`  
		Last Modified: Tue, 01 Mar 2022 05:45:13 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89cf0cd8366d641805527862400e1bce25dfe0e4d75301bfca351f6cb51adf42`  
		Last Modified: Tue, 01 Mar 2022 05:45:12 GMT  
		Size: 5.2 MB (5223244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6765d7966078499cee66919d4eae6c448903398520afd4a9af50e628602308dd`  
		Last Modified: Tue, 01 Mar 2022 05:45:11 GMT  
		Size: 1.6 MB (1553184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0aa553e191057af86f122b236ee318ab2840b814e55f6ed1f843dbf2734c3df`  
		Last Modified: Tue, 01 Mar 2022 05:45:11 GMT  
		Size: 295.5 KB (295513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6836a13a921ed1c7d33495e61fbf8c4110efd124ba364aa65719668d915df6`  
		Last Modified: Tue, 01 Mar 2022 05:45:11 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3670b70ba1f6cf592b77e0fbb8feefaa5d19731d115a8f40e5d7ad276b7572c0`  
		Last Modified: Tue, 01 Mar 2022 05:45:15 GMT  
		Size: 49.0 MB (48993167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6abf74c316c94beb45bf67044c6219f3205152bbc1a595080a4d646cad125055`  
		Last Modified: Tue, 01 Mar 2022 05:45:09 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91336f088c386950fab72a2eff4fb6e543ea167051299e920860f25763ddad4c`  
		Last Modified: Tue, 01 Mar 2022 05:45:09 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec02748684ecc64a7c390d3f95f2556ed75c995c0018dca6d3a5bcb4f10222e`  
		Last Modified: Tue, 01 Mar 2022 05:45:09 GMT  
		Size: 2.2 KB (2184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50b0fab1478c6789e174467f18aec4753c1a77109436988456425cef86c95aa`  
		Last Modified: Tue, 01 Mar 2022 05:45:09 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:3e6dc6d0db2d323fddb035a9432235b94c05601e90dede631eef8984dfbd59c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.6 MB (85578848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49ed81158960a991bcb8edcedb33f3bb86af2b2248ff74cadb7932938493c341`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:29 GMT
ADD file:9816c9c29627693c34afda4fa5e1a5e8a0f5aa3c5d5cfd920a4d89c77aab997d in / 
# Tue, 01 Mar 2022 02:11:30 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:54:16 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 01 Mar 2022 10:54:17 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 01 Mar 2022 10:54:25 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:54:29 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 01 Mar 2022 10:54:30 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 01 Mar 2022 10:54:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:54:37 GMT
ENV COUCHDB_VERSION=3.2.1-1
# Tue, 01 Mar 2022 10:54:38 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 01 Mar 2022 10:54:59 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 01 Mar 2022 10:55:00 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 01 Mar 2022 10:55:01 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 01 Mar 2022 10:55:02 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Tue, 01 Mar 2022 10:55:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 01 Mar 2022 10:55:03 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 01 Mar 2022 10:55:04 GMT
VOLUME [/opt/couchdb/data]
# Tue, 01 Mar 2022 10:55:05 GMT
EXPOSE 4369 5984 9100
# Tue, 01 Mar 2022 10:55:06 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:279a020076a7fbddfc996e4c55e605a8f322810c3eca21cdedbcb06beb0e1305`  
		Last Modified: Tue, 01 Mar 2022 02:18:24 GMT  
		Size: 30.1 MB (30057008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfcff81d5bffc5f578ce75b1352bd0ec1fbc72e64741076e33fec78f31f8251`  
		Last Modified: Tue, 01 Mar 2022 10:57:14 GMT  
		Size: 3.3 KB (3321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd324560c127ebd17fc2f7dadad8e82385cada679ffe92bba01f0ac0dc1147c`  
		Last Modified: Tue, 01 Mar 2022 10:57:13 GMT  
		Size: 5.2 MB (5208018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b903e5b6f9f94a6b822e164537f5fce3c6b17d856646c5ed96bb2ca39b5d4d3a`  
		Last Modified: Tue, 01 Mar 2022 10:57:12 GMT  
		Size: 1.2 MB (1221005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c16dea62989609f7bd2a55428c40adcb00d517c47c9c52e0ec5e76d3e1af6ee`  
		Last Modified: Tue, 01 Mar 2022 10:57:12 GMT  
		Size: 79.1 KB (79098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66b3299f2b80a371f9445b89065781cb0070d916bc4cb9cfabc1d747159652cd`  
		Last Modified: Tue, 01 Mar 2022 10:57:12 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4ee9c5380651ad3aa998731b2c7cfceaff37464c95ab95dfb1880628869f77`  
		Last Modified: Tue, 01 Mar 2022 10:57:16 GMT  
		Size: 49.0 MB (49006666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce8d37b711b0d0f9efce1b36bb75dc4823a4d16b320d261e0b1f4aa51cee6c3`  
		Last Modified: Tue, 01 Mar 2022 10:57:10 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4daebd54e61f91fc444be8b7157fd4bbc43c96e578f49ac98381094e38ffc7a2`  
		Last Modified: Tue, 01 Mar 2022 10:57:10 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76d8dbd3035c9da1363c7be373af9100c55b68b887d37581e4ea815d31fcef7`  
		Last Modified: Tue, 01 Mar 2022 10:57:10 GMT  
		Size: 2.2 KB (2187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772c4d8177aba4266c7d6008fd9345bca757dc38dbdeeee5eda1b255e2a92b38`  
		Last Modified: Tue, 01 Mar 2022 10:57:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; ppc64le

```console
$ docker pull couchdb@sha256:910fc1e2c4c95579028118dd6ac80d60b5e34135807caae0b3b759bbd3f7558f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93156878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0af7fca6e0cc3d261c23d2b84ee250be1f1b53921c4e9e0cbe68619f6680d109`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 01 Mar 2022 02:05:07 GMT
ADD file:fc0989685aecf50ec36795d73893c30d9ddd4f946f8c5f4a6d10963f8ab41168 in / 
# Tue, 01 Mar 2022 02:05:12 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 07:26:33 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 02 Mar 2022 07:26:42 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 02 Mar 2022 07:27:18 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 07:27:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 02 Mar 2022 07:27:33 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 02 Mar 2022 07:27:56 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 07:27:58 GMT
ENV COUCHDB_VERSION=3.2.1-1
# Wed, 02 Mar 2022 07:28:03 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 02 Mar 2022 07:28:45 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 02 Mar 2022 07:28:49 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 02 Mar 2022 07:28:49 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 02 Mar 2022 07:28:51 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 02 Mar 2022 07:28:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 02 Mar 2022 07:28:56 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 02 Mar 2022 07:28:58 GMT
VOLUME [/opt/couchdb/data]
# Wed, 02 Mar 2022 07:29:00 GMT
EXPOSE 4369 5984 9100
# Wed, 02 Mar 2022 07:29:02 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:1dde9239ed493e1fe68971baa3f162c734ef0f461ad109e48aeb5b56daa55cc2`  
		Last Modified: Tue, 01 Mar 2022 02:15:19 GMT  
		Size: 35.3 MB (35272910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8e3b76def43005a4bad42db196a1af1f2e2a7571c562c402c6d5fab6b670fa`  
		Last Modified: Wed, 02 Mar 2022 07:29:28 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0b0be0220579d9a54e06e2c75add9959107db00f235745c5094280a38a0d66`  
		Last Modified: Wed, 02 Mar 2022 07:29:28 GMT  
		Size: 6.0 MB (6043478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8512718ccfd18b0d0555389092336b2345a224cf8741ecacd8cf0aefc13b56ad`  
		Last Modified: Wed, 02 Mar 2022 07:29:27 GMT  
		Size: 1.5 MB (1509175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0d3da23acf1804501e1d63f82b765ae6fff0d46daf6a85271bcd6485a2ac20`  
		Last Modified: Wed, 02 Mar 2022 07:29:26 GMT  
		Size: 295.6 KB (295572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079334cb185001d3836b007108d00ae394390595a59b51c946ddd3d6dcf748a0`  
		Last Modified: Wed, 02 Mar 2022 07:29:26 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92f960d7dfa5dfa0ceedc8b12ecda5b51ee8a82a42811c576537fc6009f5741`  
		Last Modified: Wed, 02 Mar 2022 07:29:31 GMT  
		Size: 50.0 MB (50028599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:618b23d01fac8298a56be32af0a4f1e0bf7e2e80a89587293ae671d5da9499b9`  
		Last Modified: Wed, 02 Mar 2022 07:29:24 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6739034ddd8a12ca87e41304cc52cea8bd9691c386759d8e336397f0e513e7`  
		Last Modified: Wed, 02 Mar 2022 07:29:24 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4641352460d612b4811a827f1e46eaca3d2bee21b5a9fe04e849a4461856173c`  
		Last Modified: Wed, 02 Mar 2022 07:29:24 GMT  
		Size: 2.2 KB (2185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dea3c3c346c9f62d3d3be2c25ca691732d97c66ac1dd786e1befc38de0d67a1`  
		Last Modified: Wed, 02 Mar 2022 07:29:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
