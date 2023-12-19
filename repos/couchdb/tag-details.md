<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `couchdb`

-	[`couchdb:2`](#couchdb2)
-	[`couchdb:2.3`](#couchdb23)
-	[`couchdb:2.3.1`](#couchdb231)
-	[`couchdb:3`](#couchdb3)
-	[`couchdb:3.1`](#couchdb31)
-	[`couchdb:3.1.2`](#couchdb312)
-	[`couchdb:3.2`](#couchdb32)
-	[`couchdb:3.2.3`](#couchdb323)
-	[`couchdb:3.3`](#couchdb33)
-	[`couchdb:3.3.3`](#couchdb333)
-	[`couchdb:latest`](#couchdblatest)

## `couchdb:2`

```console
$ docker pull couchdb@sha256:50ad9c59ebd5f43e19bce82149a7eab2e487e0342a38f5b21fd1aa7419a6b785
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2` - linux; amd64

```console
$ docker pull couchdb@sha256:09f0f5ee98dab4f14dfa0948e7959a182f73a5fb28462c0550ede691f518957b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.6 MB (84603754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ba66eb6710e44595d821b1c799bcf4d5d092bc6dd3fa42386457618eb2a7434`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:12 GMT
ADD file:ae5c65eea20f7ddcf93a0aa255b6a08a906ac1a1a65cd2c4b5d1529bf9f6eaf8 in / 
# Tue, 19 Dec 2023 01:21:13 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 06:48:09 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 19 Dec 2023 06:48:09 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 19 Dec 2023 06:48:18 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:48:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 19 Dec 2023 06:48:22 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 19 Dec 2023 06:48:29 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:48:50 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 19 Dec 2023 06:48:50 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 19 Dec 2023 06:49:09 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 19 Dec 2023 06:49:10 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 19 Dec 2023 06:49:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 19 Dec 2023 06:49:10 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 19 Dec 2023 06:49:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 19 Dec 2023 06:49:10 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 06:49:11 GMT
VOLUME [/opt/couchdb/data]
# Tue, 19 Dec 2023 06:49:11 GMT
EXPOSE 4369 5984 9100
# Tue, 19 Dec 2023 06:49:11 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:faac0b3889808c27af96e662a1082eef35772c35dcee1c7334f5f5a22b4149d7`  
		Last Modified: Tue, 19 Dec 2023 01:26:21 GMT  
		Size: 27.2 MB (27188221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7166d4cfe5df555a7729929a6d911ba456e010fabf8a64909232e00ead121bc`  
		Last Modified: Tue, 19 Dec 2023 06:49:59 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4b104d263a43ff5771a1387a20124227ad1f5673c6e0db8dc73314fb604c36`  
		Last Modified: Tue, 19 Dec 2023 06:49:58 GMT  
		Size: 6.7 MB (6704570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d9bda983dd893f88c5ac99cfecbd7008f925b865f7d0684189a6224b0c6de8`  
		Last Modified: Tue, 19 Dec 2023 06:49:57 GMT  
		Size: 1.3 MB (1259894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab85e8861aa6e17e21bcde34afc7866fecfbb5fae39616bcaf635fc5ef14fb24`  
		Last Modified: Tue, 19 Dec 2023 06:49:57 GMT  
		Size: 294.6 KB (294555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89d6563e8c3b10aff1a57fa8336cd27e627cd802ad4080a165dd18fe76bf2ea`  
		Last Modified: Tue, 19 Dec 2023 06:50:11 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d577c04040648c253601c8988f5ce21fd1e69b05720ecc993886b8ce7e92af`  
		Last Modified: Tue, 19 Dec 2023 06:50:15 GMT  
		Size: 49.1 MB (49149495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4bbe2da817b6638fd544411743245fcc3026c70514b44c7f734d25f62b504ed`  
		Last Modified: Tue, 19 Dec 2023 06:50:09 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1cd4ed0cc7ca429112deb3a9c807f11a2716fbeef17f10fdc6061e1153ef19`  
		Last Modified: Tue, 19 Dec 2023 06:50:09 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c48e0c302b1fa8a286b4011d3f6e249602f32f99ec2184ae7eea9d1921e581f`  
		Last Modified: Tue, 19 Dec 2023 06:50:09 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1127283dd5b4a3c263aa5a7ed2b4b10fa99a8b61de96e789daec4a40b8c4da5d`  
		Last Modified: Tue, 19 Dec 2023 06:50:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:f6c2eb09ebaa599f0a93c7f28e5f47185121416af39120dd80ee27ae42e90a63
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (73042770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0ab83c5db3e862a9904f8a1d3e4821e2ab1d2eb563d33313ac79316b544b348`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:34 GMT
ADD file:475e94b9a8f65c7cd4d4156af31e83190240ff35d8038f3fa86ad124d4d5d299 in / 
# Tue, 21 Nov 2023 06:27:35 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:53:23 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Nov 2023 07:53:24 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Nov 2023 07:53:33 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:53:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 21 Nov 2023 07:53:37 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Nov 2023 07:53:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:54:03 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 21 Nov 2023 07:54:04 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Nov 2023 07:54:15 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Nov 2023 07:54:16 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Nov 2023 07:54:16 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 21 Nov 2023 07:54:16 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 21 Nov 2023 07:54:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Nov 2023 07:54:16 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Nov 2023 07:54:16 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Nov 2023 07:54:17 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Nov 2023 07:54:17 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:78b429e3efdd9f2b163abf0bca6b1462a25b1c5eddc1dd47f5d3445c6413cfa1`  
		Last Modified: Tue, 21 Nov 2023 06:31:45 GMT  
		Size: 26.0 MB (25967796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3c5bfaccf97ef74c924764aca27d055d3cab8446f6ef59870cd544056d4cec`  
		Last Modified: Tue, 21 Nov 2023 07:54:50 GMT  
		Size: 3.4 KB (3434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff6bf33f9c2e30b4f1ce3f1bf6149231315457866fad15eedffdf007ad01f5e`  
		Last Modified: Tue, 21 Nov 2023 07:54:49 GMT  
		Size: 6.6 MB (6577624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0040bf5cab2106c8e662145f7f764673fdd1f2b1ea63a2f64a94333049636031`  
		Last Modified: Tue, 21 Nov 2023 07:54:48 GMT  
		Size: 1.2 MB (1164833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6ff98dded5f418fecd217598fdeb4a722749c105e50a53dce349adc0872191`  
		Last Modified: Tue, 21 Nov 2023 07:54:48 GMT  
		Size: 294.4 KB (294403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b62b412c39c27d6b0bb77c29580f219e6832aa220a1ed8f0e2bb8ac5e792a8c`  
		Last Modified: Tue, 21 Nov 2023 07:55:00 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb05dfa0bb3aaeb852e7044d0f340c9f2ab0670711209b60bcd59af90662d446`  
		Last Modified: Tue, 21 Nov 2023 07:55:01 GMT  
		Size: 39.0 MB (39031078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0733c721e2ac151b2a04aa4474c02909229c16794206a817831aaf359c3586`  
		Last Modified: Tue, 21 Nov 2023 07:54:58 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898bac72b3df0026173253ea7ec67fdf05a7b81e4b1b35117bbefeeb74161be3`  
		Last Modified: Tue, 21 Nov 2023 07:54:58 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df6dfa461e8b59dabcba0ba599e8cf4ac4467d94a12592cfac6025ae0656cb7`  
		Last Modified: Tue, 21 Nov 2023 07:54:58 GMT  
		Size: 2.1 KB (2056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d16e9798ed2dcc347e66efbb5cc6cb53f4a73440518bf6a3c0adad2ee71cfd`  
		Last Modified: Tue, 21 Nov 2023 07:54:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3`

```console
$ docker pull couchdb@sha256:50ad9c59ebd5f43e19bce82149a7eab2e487e0342a38f5b21fd1aa7419a6b785
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:09f0f5ee98dab4f14dfa0948e7959a182f73a5fb28462c0550ede691f518957b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.6 MB (84603754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ba66eb6710e44595d821b1c799bcf4d5d092bc6dd3fa42386457618eb2a7434`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:12 GMT
ADD file:ae5c65eea20f7ddcf93a0aa255b6a08a906ac1a1a65cd2c4b5d1529bf9f6eaf8 in / 
# Tue, 19 Dec 2023 01:21:13 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 06:48:09 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 19 Dec 2023 06:48:09 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 19 Dec 2023 06:48:18 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:48:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 19 Dec 2023 06:48:22 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 19 Dec 2023 06:48:29 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:48:50 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 19 Dec 2023 06:48:50 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 19 Dec 2023 06:49:09 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 19 Dec 2023 06:49:10 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 19 Dec 2023 06:49:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 19 Dec 2023 06:49:10 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 19 Dec 2023 06:49:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 19 Dec 2023 06:49:10 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 06:49:11 GMT
VOLUME [/opt/couchdb/data]
# Tue, 19 Dec 2023 06:49:11 GMT
EXPOSE 4369 5984 9100
# Tue, 19 Dec 2023 06:49:11 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:faac0b3889808c27af96e662a1082eef35772c35dcee1c7334f5f5a22b4149d7`  
		Last Modified: Tue, 19 Dec 2023 01:26:21 GMT  
		Size: 27.2 MB (27188221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7166d4cfe5df555a7729929a6d911ba456e010fabf8a64909232e00ead121bc`  
		Last Modified: Tue, 19 Dec 2023 06:49:59 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4b104d263a43ff5771a1387a20124227ad1f5673c6e0db8dc73314fb604c36`  
		Last Modified: Tue, 19 Dec 2023 06:49:58 GMT  
		Size: 6.7 MB (6704570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d9bda983dd893f88c5ac99cfecbd7008f925b865f7d0684189a6224b0c6de8`  
		Last Modified: Tue, 19 Dec 2023 06:49:57 GMT  
		Size: 1.3 MB (1259894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab85e8861aa6e17e21bcde34afc7866fecfbb5fae39616bcaf635fc5ef14fb24`  
		Last Modified: Tue, 19 Dec 2023 06:49:57 GMT  
		Size: 294.6 KB (294555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89d6563e8c3b10aff1a57fa8336cd27e627cd802ad4080a165dd18fe76bf2ea`  
		Last Modified: Tue, 19 Dec 2023 06:50:11 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d577c04040648c253601c8988f5ce21fd1e69b05720ecc993886b8ce7e92af`  
		Last Modified: Tue, 19 Dec 2023 06:50:15 GMT  
		Size: 49.1 MB (49149495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4bbe2da817b6638fd544411743245fcc3026c70514b44c7f734d25f62b504ed`  
		Last Modified: Tue, 19 Dec 2023 06:50:09 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1cd4ed0cc7ca429112deb3a9c807f11a2716fbeef17f10fdc6061e1153ef19`  
		Last Modified: Tue, 19 Dec 2023 06:50:09 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c48e0c302b1fa8a286b4011d3f6e249602f32f99ec2184ae7eea9d1921e581f`  
		Last Modified: Tue, 19 Dec 2023 06:50:09 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1127283dd5b4a3c263aa5a7ed2b4b10fa99a8b61de96e789daec4a40b8c4da5d`  
		Last Modified: Tue, 19 Dec 2023 06:50:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:f6c2eb09ebaa599f0a93c7f28e5f47185121416af39120dd80ee27ae42e90a63
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (73042770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0ab83c5db3e862a9904f8a1d3e4821e2ab1d2eb563d33313ac79316b544b348`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:34 GMT
ADD file:475e94b9a8f65c7cd4d4156af31e83190240ff35d8038f3fa86ad124d4d5d299 in / 
# Tue, 21 Nov 2023 06:27:35 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:53:23 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Nov 2023 07:53:24 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Nov 2023 07:53:33 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:53:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 21 Nov 2023 07:53:37 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Nov 2023 07:53:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:54:03 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 21 Nov 2023 07:54:04 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Nov 2023 07:54:15 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Nov 2023 07:54:16 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Nov 2023 07:54:16 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 21 Nov 2023 07:54:16 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 21 Nov 2023 07:54:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Nov 2023 07:54:16 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Nov 2023 07:54:16 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Nov 2023 07:54:17 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Nov 2023 07:54:17 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:78b429e3efdd9f2b163abf0bca6b1462a25b1c5eddc1dd47f5d3445c6413cfa1`  
		Last Modified: Tue, 21 Nov 2023 06:31:45 GMT  
		Size: 26.0 MB (25967796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3c5bfaccf97ef74c924764aca27d055d3cab8446f6ef59870cd544056d4cec`  
		Last Modified: Tue, 21 Nov 2023 07:54:50 GMT  
		Size: 3.4 KB (3434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff6bf33f9c2e30b4f1ce3f1bf6149231315457866fad15eedffdf007ad01f5e`  
		Last Modified: Tue, 21 Nov 2023 07:54:49 GMT  
		Size: 6.6 MB (6577624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0040bf5cab2106c8e662145f7f764673fdd1f2b1ea63a2f64a94333049636031`  
		Last Modified: Tue, 21 Nov 2023 07:54:48 GMT  
		Size: 1.2 MB (1164833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6ff98dded5f418fecd217598fdeb4a722749c105e50a53dce349adc0872191`  
		Last Modified: Tue, 21 Nov 2023 07:54:48 GMT  
		Size: 294.4 KB (294403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b62b412c39c27d6b0bb77c29580f219e6832aa220a1ed8f0e2bb8ac5e792a8c`  
		Last Modified: Tue, 21 Nov 2023 07:55:00 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb05dfa0bb3aaeb852e7044d0f340c9f2ab0670711209b60bcd59af90662d446`  
		Last Modified: Tue, 21 Nov 2023 07:55:01 GMT  
		Size: 39.0 MB (39031078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0733c721e2ac151b2a04aa4474c02909229c16794206a817831aaf359c3586`  
		Last Modified: Tue, 21 Nov 2023 07:54:58 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898bac72b3df0026173253ea7ec67fdf05a7b81e4b1b35117bbefeeb74161be3`  
		Last Modified: Tue, 21 Nov 2023 07:54:58 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df6dfa461e8b59dabcba0ba599e8cf4ac4467d94a12592cfac6025ae0656cb7`  
		Last Modified: Tue, 21 Nov 2023 07:54:58 GMT  
		Size: 2.1 KB (2056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d16e9798ed2dcc347e66efbb5cc6cb53f4a73440518bf6a3c0adad2ee71cfd`  
		Last Modified: Tue, 21 Nov 2023 07:54:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3.1`

```console
$ docker pull couchdb@sha256:50ad9c59ebd5f43e19bce82149a7eab2e487e0342a38f5b21fd1aa7419a6b785
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:09f0f5ee98dab4f14dfa0948e7959a182f73a5fb28462c0550ede691f518957b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.6 MB (84603754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ba66eb6710e44595d821b1c799bcf4d5d092bc6dd3fa42386457618eb2a7434`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:12 GMT
ADD file:ae5c65eea20f7ddcf93a0aa255b6a08a906ac1a1a65cd2c4b5d1529bf9f6eaf8 in / 
# Tue, 19 Dec 2023 01:21:13 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 06:48:09 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 19 Dec 2023 06:48:09 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 19 Dec 2023 06:48:18 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:48:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 19 Dec 2023 06:48:22 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 19 Dec 2023 06:48:29 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:48:50 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 19 Dec 2023 06:48:50 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 19 Dec 2023 06:49:09 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 19 Dec 2023 06:49:10 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 19 Dec 2023 06:49:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 19 Dec 2023 06:49:10 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 19 Dec 2023 06:49:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 19 Dec 2023 06:49:10 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 06:49:11 GMT
VOLUME [/opt/couchdb/data]
# Tue, 19 Dec 2023 06:49:11 GMT
EXPOSE 4369 5984 9100
# Tue, 19 Dec 2023 06:49:11 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:faac0b3889808c27af96e662a1082eef35772c35dcee1c7334f5f5a22b4149d7`  
		Last Modified: Tue, 19 Dec 2023 01:26:21 GMT  
		Size: 27.2 MB (27188221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7166d4cfe5df555a7729929a6d911ba456e010fabf8a64909232e00ead121bc`  
		Last Modified: Tue, 19 Dec 2023 06:49:59 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4b104d263a43ff5771a1387a20124227ad1f5673c6e0db8dc73314fb604c36`  
		Last Modified: Tue, 19 Dec 2023 06:49:58 GMT  
		Size: 6.7 MB (6704570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d9bda983dd893f88c5ac99cfecbd7008f925b865f7d0684189a6224b0c6de8`  
		Last Modified: Tue, 19 Dec 2023 06:49:57 GMT  
		Size: 1.3 MB (1259894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab85e8861aa6e17e21bcde34afc7866fecfbb5fae39616bcaf635fc5ef14fb24`  
		Last Modified: Tue, 19 Dec 2023 06:49:57 GMT  
		Size: 294.6 KB (294555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89d6563e8c3b10aff1a57fa8336cd27e627cd802ad4080a165dd18fe76bf2ea`  
		Last Modified: Tue, 19 Dec 2023 06:50:11 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d577c04040648c253601c8988f5ce21fd1e69b05720ecc993886b8ce7e92af`  
		Last Modified: Tue, 19 Dec 2023 06:50:15 GMT  
		Size: 49.1 MB (49149495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4bbe2da817b6638fd544411743245fcc3026c70514b44c7f734d25f62b504ed`  
		Last Modified: Tue, 19 Dec 2023 06:50:09 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1cd4ed0cc7ca429112deb3a9c807f11a2716fbeef17f10fdc6061e1153ef19`  
		Last Modified: Tue, 19 Dec 2023 06:50:09 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c48e0c302b1fa8a286b4011d3f6e249602f32f99ec2184ae7eea9d1921e581f`  
		Last Modified: Tue, 19 Dec 2023 06:50:09 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1127283dd5b4a3c263aa5a7ed2b4b10fa99a8b61de96e789daec4a40b8c4da5d`  
		Last Modified: Tue, 19 Dec 2023 06:50:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:f6c2eb09ebaa599f0a93c7f28e5f47185121416af39120dd80ee27ae42e90a63
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (73042770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0ab83c5db3e862a9904f8a1d3e4821e2ab1d2eb563d33313ac79316b544b348`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:34 GMT
ADD file:475e94b9a8f65c7cd4d4156af31e83190240ff35d8038f3fa86ad124d4d5d299 in / 
# Tue, 21 Nov 2023 06:27:35 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:53:23 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Nov 2023 07:53:24 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Nov 2023 07:53:33 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:53:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 21 Nov 2023 07:53:37 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Nov 2023 07:53:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:54:03 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Tue, 21 Nov 2023 07:54:04 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Nov 2023 07:54:15 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Nov 2023 07:54:16 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Nov 2023 07:54:16 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 21 Nov 2023 07:54:16 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Tue, 21 Nov 2023 07:54:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Nov 2023 07:54:16 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Nov 2023 07:54:16 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Nov 2023 07:54:17 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Nov 2023 07:54:17 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:78b429e3efdd9f2b163abf0bca6b1462a25b1c5eddc1dd47f5d3445c6413cfa1`  
		Last Modified: Tue, 21 Nov 2023 06:31:45 GMT  
		Size: 26.0 MB (25967796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3c5bfaccf97ef74c924764aca27d055d3cab8446f6ef59870cd544056d4cec`  
		Last Modified: Tue, 21 Nov 2023 07:54:50 GMT  
		Size: 3.4 KB (3434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff6bf33f9c2e30b4f1ce3f1bf6149231315457866fad15eedffdf007ad01f5e`  
		Last Modified: Tue, 21 Nov 2023 07:54:49 GMT  
		Size: 6.6 MB (6577624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0040bf5cab2106c8e662145f7f764673fdd1f2b1ea63a2f64a94333049636031`  
		Last Modified: Tue, 21 Nov 2023 07:54:48 GMT  
		Size: 1.2 MB (1164833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6ff98dded5f418fecd217598fdeb4a722749c105e50a53dce349adc0872191`  
		Last Modified: Tue, 21 Nov 2023 07:54:48 GMT  
		Size: 294.4 KB (294403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b62b412c39c27d6b0bb77c29580f219e6832aa220a1ed8f0e2bb8ac5e792a8c`  
		Last Modified: Tue, 21 Nov 2023 07:55:00 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb05dfa0bb3aaeb852e7044d0f340c9f2ab0670711209b60bcd59af90662d446`  
		Last Modified: Tue, 21 Nov 2023 07:55:01 GMT  
		Size: 39.0 MB (39031078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0733c721e2ac151b2a04aa4474c02909229c16794206a817831aaf359c3586`  
		Last Modified: Tue, 21 Nov 2023 07:54:58 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898bac72b3df0026173253ea7ec67fdf05a7b81e4b1b35117bbefeeb74161be3`  
		Last Modified: Tue, 21 Nov 2023 07:54:58 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df6dfa461e8b59dabcba0ba599e8cf4ac4467d94a12592cfac6025ae0656cb7`  
		Last Modified: Tue, 21 Nov 2023 07:54:58 GMT  
		Size: 2.1 KB (2056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d16e9798ed2dcc347e66efbb5cc6cb53f4a73440518bf6a3c0adad2ee71cfd`  
		Last Modified: Tue, 21 Nov 2023 07:54:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3`

```console
$ docker pull couchdb@sha256:a2dc0a7ba1239ddc25b4f29931cee7ef6377554f88dd5b5bfd07019a6790e033
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `couchdb:3` - linux; amd64

```console
$ docker pull couchdb@sha256:84cc1a070b6ed5057c2539ce9ac0729140211317bfd4c3f8c6af6a972f866fec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.3 MB (90281758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f410d452fcd2d0f4feb71f132b5e4571b9097692fa5ee7bfe55846fffb1b7e3`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:50 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Tue, 19 Dec 2023 01:20:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 06:47:07 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 19 Dec 2023 06:47:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 19 Dec 2023 06:47:16 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:47:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 19 Dec 2023 06:47:20 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 19 Dec 2023 06:47:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:47:25 GMT
ENV COUCHDB_VERSION=3.3.3
# Tue, 19 Dec 2023 06:47:26 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 19 Dec 2023 06:47:39 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 19 Dec 2023 06:47:39 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 19 Dec 2023 06:47:39 GMT
COPY --chown=couchdb:couchdbfile:e5db3ae8229456931b3901d8737d15bbebc21bae345eb60dc63b3edc7a03cfbc in /opt/couchdb/etc/ 
# Tue, 19 Dec 2023 06:47:40 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 19 Dec 2023 06:47:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 19 Dec 2023 06:47:40 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 06:47:40 GMT
VOLUME [/opt/couchdb/data]
# Tue, 19 Dec 2023 06:47:40 GMT
EXPOSE 4369 5984 9100
# Tue, 19 Dec 2023 06:47:40 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23f4f070a8876f3b9f2d6536e694e3c435dd993aa89811b93afe3bacdd39de9`  
		Last Modified: Tue, 19 Dec 2023 06:49:26 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e164d5f405aaa07b15f82f3f61b6dbd1cbdc900af32846793054982af6bebe8`  
		Last Modified: Tue, 19 Dec 2023 06:49:25 GMT  
		Size: 5.2 MB (5226586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1dfb4acdebdde82699f2071917a04403c86391036145bbe0ed6d0088656a5c`  
		Last Modified: Tue, 19 Dec 2023 06:49:24 GMT  
		Size: 610.9 KB (610876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1881a771df37f7280e9f36e60d2bf31e1aa682bc897cc46f6048ac2968810ba`  
		Last Modified: Tue, 19 Dec 2023 06:49:24 GMT  
		Size: 295.1 KB (295141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43749cff0c55900c892efc75594212cdfa3d8250f5e733ad3d7992578c888a53`  
		Last Modified: Tue, 19 Dec 2023 06:49:24 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73826e46a52089a5eb9572f0c4af2e15b3acdb046351f947055ebcf4a9738e8`  
		Last Modified: Tue, 19 Dec 2023 06:49:27 GMT  
		Size: 52.7 MB (52723616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d947e97cc2e724ae946a0a9c7d7acb1c2d25392cadd8502765bf22263aeb7c`  
		Last Modified: Tue, 19 Dec 2023 06:49:22 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7faf03e411f35a5287f56dfccb92efe76a20e4c74a82b7a72829c26175f8213f`  
		Last Modified: Tue, 19 Dec 2023 06:49:22 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0ad2880bdae49be7450333cca29ee638cc9391120e38cc468595f5860297d4`  
		Last Modified: Tue, 19 Dec 2023 06:49:22 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b3dcd02b547118831d71c582730baa714d3fa17b91ec09f7e73ad145fff73d`  
		Last Modified: Tue, 19 Dec 2023 06:49:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:665b281f4faefaa7f8859d9586a6a708c422903079ef2f4ccfe6a14564a886f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88720918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54871336972f9328fcec06bfc3e450d64daa6333ee69a45f0da14d120f8d2c05`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:52:39 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Nov 2023 07:52:39 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Nov 2023 07:52:45 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:52:48 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 21 Nov 2023 07:52:48 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Nov 2023 07:52:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 06 Dec 2023 00:39:25 GMT
ENV COUCHDB_VERSION=3.3.3
# Wed, 06 Dec 2023 00:39:26 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 06 Dec 2023 00:39:39 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 06 Dec 2023 00:39:39 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 06 Dec 2023 00:39:39 GMT
COPY --chown=couchdb:couchdbfile:e5db3ae8229456931b3901d8737d15bbebc21bae345eb60dc63b3edc7a03cfbc in /opt/couchdb/etc/ 
# Wed, 06 Dec 2023 00:39:40 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 06 Dec 2023 00:39:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 06 Dec 2023 00:39:40 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 06 Dec 2023 00:39:40 GMT
VOLUME [/opt/couchdb/data]
# Wed, 06 Dec 2023 00:39:40 GMT
EXPOSE 4369 5984 9100
# Wed, 06 Dec 2023 00:39:40 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a831f10e5df507c8f1e02bf16d8431aea07447742165f87bac8012c02082c5c1`  
		Last Modified: Tue, 21 Nov 2023 07:54:32 GMT  
		Size: 3.4 KB (3431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4f74c0ee547299d86d3b6de1a1b677264a77024288fe76a0459fe1596e94b0`  
		Last Modified: Tue, 21 Nov 2023 07:54:31 GMT  
		Size: 5.2 MB (5210800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a278347563aa0aac229a39ef7f2d07a6925c6a95f1eca2dc9335921b7b75f3`  
		Last Modified: Tue, 21 Nov 2023 07:54:31 GMT  
		Size: 567.0 KB (567042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479409bd9ad96512a7ba2074dabd9869a645ffa5edcc2ed2838022c816bae08d`  
		Last Modified: Tue, 21 Nov 2023 07:54:30 GMT  
		Size: 295.0 KB (295025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a142d67d1e29c92e5e8b3e869e9b175983fc8595ab6a96682dcf62381bfb7dcb`  
		Last Modified: Wed, 06 Dec 2023 00:40:09 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97468cc1d2c014c7d261b8ec053090497120e5fa58def003932cd6e2639f6fe8`  
		Last Modified: Wed, 06 Dec 2023 00:40:12 GMT  
		Size: 52.6 MB (52576241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f55ad37c5c976a16532ce2f3417578564432a3dae4959d764e63b301e6776c`  
		Last Modified: Wed, 06 Dec 2023 00:40:07 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab04edd67f8e979a7dd59173cfccc23a76d20fb11d745f273740d9954a48b1a3`  
		Last Modified: Wed, 06 Dec 2023 00:40:07 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e21f0bbd368632977373281a49f7c290995e50445f19302d538837ead8892cb`  
		Last Modified: Wed, 06 Dec 2023 00:40:07 GMT  
		Size: 2.2 KB (2228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559798cd9ec997b9e4aef8bf3ad255005563cab30e1be4f26ebdfdcad8b43c15`  
		Last Modified: Wed, 06 Dec 2023 00:40:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; ppc64le

```console
$ docker pull couchdb@sha256:753b8176a7aef04da37381fd019c1b2fa6681010e801fc9036e3024e18715ca5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.0 MB (96006838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d353bf91590bd557c4b0d1b956dfe7e1e6fa4e21024715d5368e4a2c0d40cb23`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 19 Dec 2023 01:22:19 GMT
ADD file:1cb772a6ad8ca6301624db3141029490564de7673bc0f2d4bedb5a1578ea85bd in / 
# Tue, 19 Dec 2023 01:22:21 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 06:11:17 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 19 Dec 2023 06:11:20 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 19 Dec 2023 06:11:35 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:11:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 19 Dec 2023 06:11:40 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 19 Dec 2023 06:11:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:11:50 GMT
ENV COUCHDB_VERSION=3.3.3
# Tue, 19 Dec 2023 06:11:51 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 19 Dec 2023 06:12:12 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 19 Dec 2023 06:12:14 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 19 Dec 2023 06:12:15 GMT
COPY --chown=couchdb:couchdbfile:e5db3ae8229456931b3901d8737d15bbebc21bae345eb60dc63b3edc7a03cfbc in /opt/couchdb/etc/ 
# Tue, 19 Dec 2023 06:12:15 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 19 Dec 2023 06:12:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 19 Dec 2023 06:12:16 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 06:12:17 GMT
VOLUME [/opt/couchdb/data]
# Tue, 19 Dec 2023 06:12:17 GMT
EXPOSE 4369 5984 9100
# Tue, 19 Dec 2023 06:12:18 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:c9f6fac7f65cfc65b7f8de8bc377b135ca95e45a3246cf2bd1bb90922679553e`  
		Last Modified: Tue, 19 Dec 2023 01:27:11 GMT  
		Size: 35.3 MB (35293807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7577d3224ba65ea8b4b80082d021e485704e429a94e948187c117ef600a0bef`  
		Last Modified: Tue, 19 Dec 2023 06:12:58 GMT  
		Size: 3.4 KB (3417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf8166072b100e13640179c785cd4218b6a2e957ec0e129d0bde7e3834b4dfd`  
		Last Modified: Tue, 19 Dec 2023 06:12:57 GMT  
		Size: 6.0 MB (6046157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c850ad28a78cd961b2a762a88d0451864228709b98ab4b853b228ab4c0800ff7`  
		Last Modified: Tue, 19 Dec 2023 06:12:56 GMT  
		Size: 662.9 KB (662861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95514ebca6987967313a81e9311e31cd8685e3e37bbae279e5d699953a929caf`  
		Last Modified: Tue, 19 Dec 2023 06:12:56 GMT  
		Size: 295.0 KB (295041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c19fb87d01555598a6d01afad8ee27bbe66f165aba43c2b7371a8992104b49`  
		Last Modified: Tue, 19 Dec 2023 06:12:56 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f88c0665db50b85ec902075ad54db3b289b00cc710d7e4392ad1a54d2b30b67`  
		Last Modified: Tue, 19 Dec 2023 06:13:00 GMT  
		Size: 53.7 MB (53701301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4418e5805fb7f6139789891c3e29e2e88f5edc1316d9ba290f5b787f7875b4b4`  
		Last Modified: Tue, 19 Dec 2023 06:12:54 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1d3278e0d5e4065ead7e595ecf8e930b3d840461de896a6764408ca3c217f3`  
		Last Modified: Tue, 19 Dec 2023 06:12:54 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7656c58286888136b4d0eeadba3ffe94124aea9339b8f188674a7d9f08e23bb8`  
		Last Modified: Tue, 19 Dec 2023 06:12:54 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00ff0e342ac6c64e01a93d5a7e5b8141b7afc11273eaf4e03414f7cea7ea31f`  
		Last Modified: Tue, 19 Dec 2023 06:12:54 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; s390x

```console
$ docker pull couchdb@sha256:2c22df2955be2202b336377102e40ba9df2110d2de473c1e15d4f47d6f349dd4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.0 MB (87020308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b385379393ba611686bcc3b50163b72e3d734b0d4de65bfe22aabcad3464918`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Nov 2023 05:05:18 GMT
ADD file:a545f27075704ce13e33e539170d3f47007424d2cc2bea5aecfd2608a5194151 in / 
# Tue, 21 Nov 2023 05:05:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:20:22 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Nov 2023 06:20:22 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Nov 2023 06:20:28 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:20:31 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 21 Nov 2023 06:20:31 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Nov 2023 06:20:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 06 Dec 2023 02:02:06 GMT
ENV COUCHDB_VERSION=3.3.3
# Wed, 06 Dec 2023 02:02:07 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 06 Dec 2023 02:02:23 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 06 Dec 2023 02:02:25 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 06 Dec 2023 02:02:25 GMT
COPY --chown=couchdb:couchdbfile:e5db3ae8229456931b3901d8737d15bbebc21bae345eb60dc63b3edc7a03cfbc in /opt/couchdb/etc/ 
# Wed, 06 Dec 2023 02:02:25 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 06 Dec 2023 02:02:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 06 Dec 2023 02:02:26 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 06 Dec 2023 02:02:26 GMT
VOLUME [/opt/couchdb/data]
# Wed, 06 Dec 2023 02:02:26 GMT
EXPOSE 4369 5984 9100
# Wed, 06 Dec 2023 02:02:26 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b114072f1cab66b7376d690985b12816aebab2e4e41fc170e32f111df27951dc`  
		Last Modified: Tue, 21 Nov 2023 05:10:48 GMT  
		Size: 29.7 MB (29656938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72dba253785a5e917fdd9064f61b676b4080ff3073424ff387308d70579c728b`  
		Last Modified: Tue, 21 Nov 2023 06:21:15 GMT  
		Size: 3.4 KB (3431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a299cd04ea14bbc3034e11001a1ec06dd4b5e1aaa78317dc803570f8a4c6437`  
		Last Modified: Tue, 21 Nov 2023 06:21:15 GMT  
		Size: 5.1 MB (5111719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c684e5bcbb93c8f0c9da5b81b4a1d19274f7ad0c7e3b17eb12cbe45cd2514989`  
		Last Modified: Tue, 21 Nov 2023 06:21:14 GMT  
		Size: 573.6 KB (573635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d916370cd04b7352346fee3edc1ac77bdb9393e24c5bc62c4cb0803a682836`  
		Last Modified: Tue, 21 Nov 2023 06:21:14 GMT  
		Size: 295.1 KB (295096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a1103db371c12bf970b540b2c88218edfbcbb795f44723923250883b44e1bd`  
		Last Modified: Wed, 06 Dec 2023 02:02:43 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b973390785fed3323a0dee86843a01b7fd4619d45b07d56f720944ec44472e`  
		Last Modified: Wed, 06 Dec 2023 02:02:47 GMT  
		Size: 51.4 MB (51375238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4460d75cadbb0c64ba1971daf7b584f7e206f245cf94c11aad8f34cb1ff3dabc`  
		Last Modified: Wed, 06 Dec 2023 02:02:42 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0329d7b8f2445b6e102b78c5fdde312f1124b63342ded38fc3aaea4e0f0df7`  
		Last Modified: Wed, 06 Dec 2023 02:02:42 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0492a0f28b3dfa930e25093cdb69b9d296c5a7eeb676913d57e1e7435073e4`  
		Last Modified: Wed, 06 Dec 2023 02:02:42 GMT  
		Size: 2.2 KB (2230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256de16f96660a155ac66140b318852f2d80a5e0b27520f1f56d4b5d5215e497`  
		Last Modified: Wed, 06 Dec 2023 02:02:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1`

```console
$ docker pull couchdb@sha256:fbf4664ad8ddfaece73013419d797d68caf453a09e36d32e21bb8158ee7190b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:fc5b9fb424a1f29932290b6fe9534d56d25da640f90af8325cfeccf225225569
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.1 MB (80076408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8751799358a2a661a1cc51181313a85f37683a6bf99209b131e54ec5dba0c26`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:12 GMT
ADD file:ae5c65eea20f7ddcf93a0aa255b6a08a906ac1a1a65cd2c4b5d1529bf9f6eaf8 in / 
# Tue, 19 Dec 2023 01:21:13 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 06:48:09 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 19 Dec 2023 06:48:09 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 19 Dec 2023 06:48:18 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:48:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 19 Dec 2023 06:48:22 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 19 Dec 2023 06:48:29 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:48:29 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 19 Dec 2023 06:48:30 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 19 Dec 2023 06:48:43 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 19 Dec 2023 06:48:43 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 19 Dec 2023 06:48:44 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 19 Dec 2023 06:48:44 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 19 Dec 2023 06:48:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 19 Dec 2023 06:48:44 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 06:48:44 GMT
VOLUME [/opt/couchdb/data]
# Tue, 19 Dec 2023 06:48:44 GMT
EXPOSE 4369 5984 9100
# Tue, 19 Dec 2023 06:48:45 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:faac0b3889808c27af96e662a1082eef35772c35dcee1c7334f5f5a22b4149d7`  
		Last Modified: Tue, 19 Dec 2023 01:26:21 GMT  
		Size: 27.2 MB (27188221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7166d4cfe5df555a7729929a6d911ba456e010fabf8a64909232e00ead121bc`  
		Last Modified: Tue, 19 Dec 2023 06:49:59 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4b104d263a43ff5771a1387a20124227ad1f5673c6e0db8dc73314fb604c36`  
		Last Modified: Tue, 19 Dec 2023 06:49:58 GMT  
		Size: 6.7 MB (6704570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d9bda983dd893f88c5ac99cfecbd7008f925b865f7d0684189a6224b0c6de8`  
		Last Modified: Tue, 19 Dec 2023 06:49:57 GMT  
		Size: 1.3 MB (1259894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab85e8861aa6e17e21bcde34afc7866fecfbb5fae39616bcaf635fc5ef14fb24`  
		Last Modified: Tue, 19 Dec 2023 06:49:57 GMT  
		Size: 294.6 KB (294555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97240f92ce4de6aaad4479bd8c3587c9d99063a2f926fa499931ce4fac4e4275`  
		Last Modified: Tue, 19 Dec 2023 06:49:57 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f75ff7bb5081af19002ea75058891e555644d534a6aad9086d653c2190c15aaf`  
		Last Modified: Tue, 19 Dec 2023 06:50:00 GMT  
		Size: 44.6 MB (44622151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afc2dc812cf3929e712fb0aef7b198002b614224c04593709dd30335709edec6`  
		Last Modified: Tue, 19 Dec 2023 06:49:55 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25848513c50e1ddbdfbbd7a52c5ac15ef29db26ec37d2aa18bb659fb70e94618`  
		Last Modified: Tue, 19 Dec 2023 06:49:55 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2305e3f1b72672ec9dc4491426e34bc4891ed116d39359e9b4352f7b701b72a5`  
		Last Modified: Tue, 19 Dec 2023 06:49:55 GMT  
		Size: 2.1 KB (2061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0101d064fe5a27e07e1294fe7d8ea2ce5e4a635da0db0ee5caf3a52fcba907c5`  
		Last Modified: Tue, 19 Dec 2023 06:49:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:37cc498008183d12dd4e01b804cefe36ebab637b48c806c1e209702798d42690
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75138387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c17b5985551eb87f31d003a31f350852ebca8ba78287ed3f55dd68678ec17ca`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:34 GMT
ADD file:475e94b9a8f65c7cd4d4156af31e83190240ff35d8038f3fa86ad124d4d5d299 in / 
# Tue, 21 Nov 2023 06:27:35 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:53:23 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Nov 2023 07:53:24 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Nov 2023 07:53:33 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:53:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 21 Nov 2023 07:53:37 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Nov 2023 07:53:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:53:43 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 21 Nov 2023 07:53:43 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Nov 2023 07:53:55 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Nov 2023 07:53:55 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Nov 2023 07:53:55 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 21 Nov 2023 07:53:56 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 21 Nov 2023 07:53:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Nov 2023 07:53:56 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Nov 2023 07:53:56 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Nov 2023 07:53:56 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Nov 2023 07:53:56 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:78b429e3efdd9f2b163abf0bca6b1462a25b1c5eddc1dd47f5d3445c6413cfa1`  
		Last Modified: Tue, 21 Nov 2023 06:31:45 GMT  
		Size: 26.0 MB (25967796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3c5bfaccf97ef74c924764aca27d055d3cab8446f6ef59870cd544056d4cec`  
		Last Modified: Tue, 21 Nov 2023 07:54:50 GMT  
		Size: 3.4 KB (3434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff6bf33f9c2e30b4f1ce3f1bf6149231315457866fad15eedffdf007ad01f5e`  
		Last Modified: Tue, 21 Nov 2023 07:54:49 GMT  
		Size: 6.6 MB (6577624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0040bf5cab2106c8e662145f7f764673fdd1f2b1ea63a2f64a94333049636031`  
		Last Modified: Tue, 21 Nov 2023 07:54:48 GMT  
		Size: 1.2 MB (1164833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6ff98dded5f418fecd217598fdeb4a722749c105e50a53dce349adc0872191`  
		Last Modified: Tue, 21 Nov 2023 07:54:48 GMT  
		Size: 294.4 KB (294403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b3cf58bd99b2965a4aa657d7191e0436efdee52829d14f4b0e7c830ed26296`  
		Last Modified: Tue, 21 Nov 2023 07:54:48 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50d22884607a48a62a9335825c3f44fe0065a733e89d1c09cdf41fa1f20421d`  
		Last Modified: Tue, 21 Nov 2023 07:54:49 GMT  
		Size: 41.1 MB (41126695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041cbf629fcf79f3a1ae7768c35b231256213eb7a6a245e48871a296ca1c5e1c`  
		Last Modified: Tue, 21 Nov 2023 07:54:46 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092b48f8245b28b3573e94e1d5e6df3c5b930eee14f17cf005f4a43a2baf2ab8`  
		Last Modified: Tue, 21 Nov 2023 07:54:46 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e42c042eb9e348de2b88f5421f8526d33d89321080bf5cb2af402fff160e965`  
		Last Modified: Tue, 21 Nov 2023 07:54:46 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b2de15229ac86dc89469f80ca89c3565745f1a26b772a362d1e55c3d00c65b`  
		Last Modified: Tue, 21 Nov 2023 07:54:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1.2`

```console
$ docker pull couchdb@sha256:fbf4664ad8ddfaece73013419d797d68caf453a09e36d32e21bb8158ee7190b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1.2` - linux; amd64

```console
$ docker pull couchdb@sha256:fc5b9fb424a1f29932290b6fe9534d56d25da640f90af8325cfeccf225225569
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.1 MB (80076408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8751799358a2a661a1cc51181313a85f37683a6bf99209b131e54ec5dba0c26`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:12 GMT
ADD file:ae5c65eea20f7ddcf93a0aa255b6a08a906ac1a1a65cd2c4b5d1529bf9f6eaf8 in / 
# Tue, 19 Dec 2023 01:21:13 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 06:48:09 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 19 Dec 2023 06:48:09 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 19 Dec 2023 06:48:18 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:48:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 19 Dec 2023 06:48:22 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 19 Dec 2023 06:48:29 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:48:29 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 19 Dec 2023 06:48:30 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 19 Dec 2023 06:48:43 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 19 Dec 2023 06:48:43 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 19 Dec 2023 06:48:44 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 19 Dec 2023 06:48:44 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 19 Dec 2023 06:48:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 19 Dec 2023 06:48:44 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 06:48:44 GMT
VOLUME [/opt/couchdb/data]
# Tue, 19 Dec 2023 06:48:44 GMT
EXPOSE 4369 5984 9100
# Tue, 19 Dec 2023 06:48:45 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:faac0b3889808c27af96e662a1082eef35772c35dcee1c7334f5f5a22b4149d7`  
		Last Modified: Tue, 19 Dec 2023 01:26:21 GMT  
		Size: 27.2 MB (27188221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7166d4cfe5df555a7729929a6d911ba456e010fabf8a64909232e00ead121bc`  
		Last Modified: Tue, 19 Dec 2023 06:49:59 GMT  
		Size: 3.4 KB (3414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4b104d263a43ff5771a1387a20124227ad1f5673c6e0db8dc73314fb604c36`  
		Last Modified: Tue, 19 Dec 2023 06:49:58 GMT  
		Size: 6.7 MB (6704570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d9bda983dd893f88c5ac99cfecbd7008f925b865f7d0684189a6224b0c6de8`  
		Last Modified: Tue, 19 Dec 2023 06:49:57 GMT  
		Size: 1.3 MB (1259894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab85e8861aa6e17e21bcde34afc7866fecfbb5fae39616bcaf635fc5ef14fb24`  
		Last Modified: Tue, 19 Dec 2023 06:49:57 GMT  
		Size: 294.6 KB (294555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97240f92ce4de6aaad4479bd8c3587c9d99063a2f926fa499931ce4fac4e4275`  
		Last Modified: Tue, 19 Dec 2023 06:49:57 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f75ff7bb5081af19002ea75058891e555644d534a6aad9086d653c2190c15aaf`  
		Last Modified: Tue, 19 Dec 2023 06:50:00 GMT  
		Size: 44.6 MB (44622151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afc2dc812cf3929e712fb0aef7b198002b614224c04593709dd30335709edec6`  
		Last Modified: Tue, 19 Dec 2023 06:49:55 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25848513c50e1ddbdfbbd7a52c5ac15ef29db26ec37d2aa18bb659fb70e94618`  
		Last Modified: Tue, 19 Dec 2023 06:49:55 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2305e3f1b72672ec9dc4491426e34bc4891ed116d39359e9b4352f7b701b72a5`  
		Last Modified: Tue, 19 Dec 2023 06:49:55 GMT  
		Size: 2.1 KB (2061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0101d064fe5a27e07e1294fe7d8ea2ce5e4a635da0db0ee5caf3a52fcba907c5`  
		Last Modified: Tue, 19 Dec 2023 06:49:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:37cc498008183d12dd4e01b804cefe36ebab637b48c806c1e209702798d42690
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75138387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c17b5985551eb87f31d003a31f350852ebca8ba78287ed3f55dd68678ec17ca`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:34 GMT
ADD file:475e94b9a8f65c7cd4d4156af31e83190240ff35d8038f3fa86ad124d4d5d299 in / 
# Tue, 21 Nov 2023 06:27:35 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:53:23 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Nov 2023 07:53:24 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Nov 2023 07:53:33 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:53:37 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 21 Nov 2023 07:53:37 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Nov 2023 07:53:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:53:43 GMT
ENV COUCHDB_VERSION=3.1.2
# Tue, 21 Nov 2023 07:53:43 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Nov 2023 07:53:55 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Nov 2023 07:53:55 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Nov 2023 07:53:55 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 21 Nov 2023 07:53:56 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 21 Nov 2023 07:53:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Nov 2023 07:53:56 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Nov 2023 07:53:56 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Nov 2023 07:53:56 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Nov 2023 07:53:56 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:78b429e3efdd9f2b163abf0bca6b1462a25b1c5eddc1dd47f5d3445c6413cfa1`  
		Last Modified: Tue, 21 Nov 2023 06:31:45 GMT  
		Size: 26.0 MB (25967796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3c5bfaccf97ef74c924764aca27d055d3cab8446f6ef59870cd544056d4cec`  
		Last Modified: Tue, 21 Nov 2023 07:54:50 GMT  
		Size: 3.4 KB (3434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff6bf33f9c2e30b4f1ce3f1bf6149231315457866fad15eedffdf007ad01f5e`  
		Last Modified: Tue, 21 Nov 2023 07:54:49 GMT  
		Size: 6.6 MB (6577624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0040bf5cab2106c8e662145f7f764673fdd1f2b1ea63a2f64a94333049636031`  
		Last Modified: Tue, 21 Nov 2023 07:54:48 GMT  
		Size: 1.2 MB (1164833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6ff98dded5f418fecd217598fdeb4a722749c105e50a53dce349adc0872191`  
		Last Modified: Tue, 21 Nov 2023 07:54:48 GMT  
		Size: 294.4 KB (294403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b3cf58bd99b2965a4aa657d7191e0436efdee52829d14f4b0e7c830ed26296`  
		Last Modified: Tue, 21 Nov 2023 07:54:48 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50d22884607a48a62a9335825c3f44fe0065a733e89d1c09cdf41fa1f20421d`  
		Last Modified: Tue, 21 Nov 2023 07:54:49 GMT  
		Size: 41.1 MB (41126695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041cbf629fcf79f3a1ae7768c35b231256213eb7a6a245e48871a296ca1c5e1c`  
		Last Modified: Tue, 21 Nov 2023 07:54:46 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092b48f8245b28b3573e94e1d5e6df3c5b930eee14f17cf005f4a43a2baf2ab8`  
		Last Modified: Tue, 21 Nov 2023 07:54:46 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e42c042eb9e348de2b88f5421f8526d33d89321080bf5cb2af402fff160e965`  
		Last Modified: Tue, 21 Nov 2023 07:54:46 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b2de15229ac86dc89469f80ca89c3565745f1a26b772a362d1e55c3d00c65b`  
		Last Modified: Tue, 21 Nov 2023 07:54:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2`

```console
$ docker pull couchdb@sha256:b6fed2756895c2a121867640a043206eb216653175d711eeaf64d4fd234fc794
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2` - linux; amd64

```console
$ docker pull couchdb@sha256:97a8510522e914d2a89b62553f12eb05d78facba87aca42c8c7ad7f217c9cc3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.7 MB (89747360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7867d5f717af65fbeb432fa0300039806f58bc1c8585c1660fe22fb78a166d8`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:50 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Tue, 19 Dec 2023 01:20:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 06:47:07 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 19 Dec 2023 06:47:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 19 Dec 2023 06:47:16 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:47:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 19 Dec 2023 06:47:20 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 19 Dec 2023 06:47:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:47:48 GMT
ENV COUCHDB_VERSION=3.2.3
# Tue, 19 Dec 2023 06:47:49 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 19 Dec 2023 06:48:02 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 19 Dec 2023 06:48:02 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 19 Dec 2023 06:48:03 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 19 Dec 2023 06:48:03 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 19 Dec 2023 06:48:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 19 Dec 2023 06:48:03 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 06:48:03 GMT
VOLUME [/opt/couchdb/data]
# Tue, 19 Dec 2023 06:48:03 GMT
EXPOSE 4369 5984 9100
# Tue, 19 Dec 2023 06:48:04 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23f4f070a8876f3b9f2d6536e694e3c435dd993aa89811b93afe3bacdd39de9`  
		Last Modified: Tue, 19 Dec 2023 06:49:26 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e164d5f405aaa07b15f82f3f61b6dbd1cbdc900af32846793054982af6bebe8`  
		Last Modified: Tue, 19 Dec 2023 06:49:25 GMT  
		Size: 5.2 MB (5226586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1dfb4acdebdde82699f2071917a04403c86391036145bbe0ed6d0088656a5c`  
		Last Modified: Tue, 19 Dec 2023 06:49:24 GMT  
		Size: 610.9 KB (610876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1881a771df37f7280e9f36e60d2bf31e1aa682bc897cc46f6048ac2968810ba`  
		Last Modified: Tue, 19 Dec 2023 06:49:24 GMT  
		Size: 295.1 KB (295141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a5f772a9a428e77320db7958f9bec8de6e19d7439a1daecf6a6e370a0dfd71`  
		Last Modified: Tue, 19 Dec 2023 06:49:43 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8503e53b380d12f249eed7e899655ab7f8a3ac7e0f336c80c2f1a6c29cddd85`  
		Last Modified: Tue, 19 Dec 2023 06:49:46 GMT  
		Size: 52.2 MB (52189462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a68e6f5c21ad4eb62ee1bf2db65655af57173cf5db06b8e072f08302a21522a`  
		Last Modified: Tue, 19 Dec 2023 06:49:41 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d51023e201b1f0f0838c8ad3578ea0ea1ce092fef87c23ff52c1880bb44b1fb`  
		Last Modified: Tue, 19 Dec 2023 06:49:41 GMT  
		Size: 999.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2dc6bf45c477ac7473d9b8716ba020b5dbef88ee2843274a50404cd108acdf6`  
		Last Modified: Tue, 19 Dec 2023 06:49:41 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83fe7b8ff6b4bb08b244a8f4414c8e51089ae9f313086a4e953db6f2df395477`  
		Last Modified: Tue, 19 Dec 2023 06:49:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:960305e9b35826163f173e8b89eab4112410bee3725c3f0773140932dd9f7877
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.2 MB (85205205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:352add31bc606968e9b4695dc003a06de6c7ca3682ea0d3145b972feb8dabfee`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:33:39 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 12 Apr 2023 01:33:39 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 12 Apr 2023 01:33:45 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:33:48 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 12 Apr 2023 01:33:48 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 12 Apr 2023 01:33:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:34:12 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Wed, 12 Apr 2023 01:34:12 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 12 Apr 2023 01:34:24 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 12 Apr 2023 01:34:24 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 12 Apr 2023 01:34:24 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 12 Apr 2023 01:34:24 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 12 Apr 2023 01:34:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 12 Apr 2023 01:34:25 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 01:34:25 GMT
VOLUME [/opt/couchdb/data]
# Wed, 12 Apr 2023 01:34:25 GMT
EXPOSE 4369 5984 9100
# Wed, 12 Apr 2023 01:34:25 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f522824805b9b3818de882a514dd5454399e3c21b512a09e64274bf12d18ab4`  
		Last Modified: Wed, 12 Apr 2023 01:35:29 GMT  
		Size: 3.4 KB (3434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdfaf598c101b0427a73a7b5a1edb3b6229985b64794e6d215eb049125bbd25`  
		Last Modified: Wed, 12 Apr 2023 01:35:27 GMT  
		Size: 5.2 MB (5209561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc33796685833f0fdacecb6c4f2078915729822d8fb7a21aada1b767c48b377`  
		Last Modified: Wed, 12 Apr 2023 01:35:27 GMT  
		Size: 566.3 KB (566295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356323e70f7127294f4bee19c211582a4af79acc6d1f696d70fc94229c84aa52`  
		Last Modified: Wed, 12 Apr 2023 01:35:27 GMT  
		Size: 294.3 KB (294328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9652526d42f149093060de62ac3b39905fb0bfb8457d6148e4314ef71058a153`  
		Last Modified: Wed, 12 Apr 2023 01:35:44 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d95be693dac094ea4fe70ff2bd1f44b66a9ede007474a31cafcb829c361429`  
		Last Modified: Wed, 12 Apr 2023 01:35:47 GMT  
		Size: 49.1 MB (49063995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61eb7f6826c8440901fb275f2b3c5f6be3e97d95482db6770215d5bd31899ed1`  
		Last Modified: Wed, 12 Apr 2023 01:35:42 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d81fa00cdd93053287b1afda2f3cfda4475c6ac6307dc22125a76f843f21415`  
		Last Modified: Wed, 12 Apr 2023 01:35:43 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16e726b19dd008ea8df7bf3ce90fa1947f685d2f6fdd3caa36e1f3b6e40526d0`  
		Last Modified: Wed, 12 Apr 2023 01:35:43 GMT  
		Size: 2.2 KB (2227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c78146fce98da16e884fde6d22f444849c69c3da90555e336827ceb2b6a039`  
		Last Modified: Wed, 12 Apr 2023 01:35:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; ppc64le

```console
$ docker pull couchdb@sha256:90a95123b16f3f08c9e3b862a7e628ead429c8602d5dc110db1b038b5b47db9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.4 MB (92383985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7c0714b286e5789d8b829c846536d1f8a5308d8cf419fa60995af8b91ab3b55`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 12 Apr 2023 00:08:20 GMT
ADD file:63eb52aaff02c15bceabb87a78eb1b36389066ff4774cf8a754160ca7d509816 in / 
# Wed, 12 Apr 2023 00:08:23 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:23:31 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 12 Apr 2023 01:23:35 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 12 Apr 2023 01:23:57 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:24:07 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Wed, 12 Apr 2023 01:24:08 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 12 Apr 2023 01:24:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 01:25:25 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Wed, 12 Apr 2023 01:25:27 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 12 Apr 2023 01:25:58 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 12 Apr 2023 01:26:02 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 12 Apr 2023 01:26:02 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 12 Apr 2023 01:26:03 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 12 Apr 2023 01:26:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 12 Apr 2023 01:26:05 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 12 Apr 2023 01:26:06 GMT
VOLUME [/opt/couchdb/data]
# Wed, 12 Apr 2023 01:26:06 GMT
EXPOSE 4369 5984 9100
# Wed, 12 Apr 2023 01:26:07 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:5b41d5ec640939cf684959234ad3b80909268a32bfd520a31c6720a91521c2fa`  
		Last Modified: Wed, 12 Apr 2023 00:13:13 GMT  
		Size: 35.3 MB (35291995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7569dcea363c11bb071b416ea27193dbe62d8a210fa1f829efabb35b46600dae`  
		Last Modified: Wed, 12 Apr 2023 01:26:25 GMT  
		Size: 3.4 KB (3411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a685c575c0e899abc0410edf84715dd5cf4184fcbd447fdbbcac069795eadd05`  
		Last Modified: Wed, 12 Apr 2023 01:26:26 GMT  
		Size: 6.0 MB (6044117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0283a2882808914c7a35f392d4ad2d2921ccf8b8855ab399e2998c22d061f16e`  
		Last Modified: Wed, 12 Apr 2023 01:26:24 GMT  
		Size: 662.1 KB (662116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17deb4c48f5c43beee592bed99d27502afe8c8f60cde1cb4bebb7dce00e877c`  
		Last Modified: Wed, 12 Apr 2023 01:26:24 GMT  
		Size: 294.3 KB (294319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7661a9384c6767a073bc8e86df2ec2c60bef8bad55fac7ab22d7ecffcdb1f1`  
		Last Modified: Wed, 12 Apr 2023 01:26:48 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74733b44093de42db86284861068e909838a6bca4f3ecf0bfd04eb99d5bf8c79`  
		Last Modified: Wed, 12 Apr 2023 01:26:56 GMT  
		Size: 50.1 MB (50084252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c567dbfb6ac3167b1cd2d6532940fd6fb66d9b5b6a1dedf22d61b92a7b4095eb`  
		Last Modified: Wed, 12 Apr 2023 01:26:46 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf08299e06354b4674e5fabd7e99da65832d26bc98826c051d261e7a03195099`  
		Last Modified: Wed, 12 Apr 2023 01:26:46 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5861e0f3152c23eda58111aaac02f82ed4973711f9a55c51cb55ebb9af6220`  
		Last Modified: Wed, 12 Apr 2023 01:26:46 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54774512e47b4b9a6dee9f79bf7ec483b3c7c234e949bc4f6c96fb22a3e8237`  
		Last Modified: Wed, 12 Apr 2023 01:26:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2.3`

```console
$ docker pull couchdb@sha256:1a2d0ec478dd3c43ac8f9ce2bb58ca379844a12826080d4787687b585a2560d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchdb:3.2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:97a8510522e914d2a89b62553f12eb05d78facba87aca42c8c7ad7f217c9cc3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.7 MB (89747360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7867d5f717af65fbeb432fa0300039806f58bc1c8585c1660fe22fb78a166d8`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:50 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Tue, 19 Dec 2023 01:20:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 06:47:07 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 19 Dec 2023 06:47:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 19 Dec 2023 06:47:16 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:47:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 19 Dec 2023 06:47:20 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 19 Dec 2023 06:47:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:47:48 GMT
ENV COUCHDB_VERSION=3.2.3
# Tue, 19 Dec 2023 06:47:49 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 19 Dec 2023 06:48:02 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 19 Dec 2023 06:48:02 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 19 Dec 2023 06:48:03 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Tue, 19 Dec 2023 06:48:03 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 19 Dec 2023 06:48:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 19 Dec 2023 06:48:03 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 06:48:03 GMT
VOLUME [/opt/couchdb/data]
# Tue, 19 Dec 2023 06:48:03 GMT
EXPOSE 4369 5984 9100
# Tue, 19 Dec 2023 06:48:04 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23f4f070a8876f3b9f2d6536e694e3c435dd993aa89811b93afe3bacdd39de9`  
		Last Modified: Tue, 19 Dec 2023 06:49:26 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e164d5f405aaa07b15f82f3f61b6dbd1cbdc900af32846793054982af6bebe8`  
		Last Modified: Tue, 19 Dec 2023 06:49:25 GMT  
		Size: 5.2 MB (5226586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1dfb4acdebdde82699f2071917a04403c86391036145bbe0ed6d0088656a5c`  
		Last Modified: Tue, 19 Dec 2023 06:49:24 GMT  
		Size: 610.9 KB (610876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1881a771df37f7280e9f36e60d2bf31e1aa682bc897cc46f6048ac2968810ba`  
		Last Modified: Tue, 19 Dec 2023 06:49:24 GMT  
		Size: 295.1 KB (295141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a5f772a9a428e77320db7958f9bec8de6e19d7439a1daecf6a6e370a0dfd71`  
		Last Modified: Tue, 19 Dec 2023 06:49:43 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8503e53b380d12f249eed7e899655ab7f8a3ac7e0f336c80c2f1a6c29cddd85`  
		Last Modified: Tue, 19 Dec 2023 06:49:46 GMT  
		Size: 52.2 MB (52189462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a68e6f5c21ad4eb62ee1bf2db65655af57173cf5db06b8e072f08302a21522a`  
		Last Modified: Tue, 19 Dec 2023 06:49:41 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d51023e201b1f0f0838c8ad3578ea0ea1ce092fef87c23ff52c1880bb44b1fb`  
		Last Modified: Tue, 19 Dec 2023 06:49:41 GMT  
		Size: 999.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2dc6bf45c477ac7473d9b8716ba020b5dbef88ee2843274a50404cd108acdf6`  
		Last Modified: Tue, 19 Dec 2023 06:49:41 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83fe7b8ff6b4bb08b244a8f4414c8e51089ae9f313086a4e953db6f2df395477`  
		Last Modified: Tue, 19 Dec 2023 06:49:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.3`

```console
$ docker pull couchdb@sha256:a2dc0a7ba1239ddc25b4f29931cee7ef6377554f88dd5b5bfd07019a6790e033
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `couchdb:3.3` - linux; amd64

```console
$ docker pull couchdb@sha256:84cc1a070b6ed5057c2539ce9ac0729140211317bfd4c3f8c6af6a972f866fec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.3 MB (90281758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f410d452fcd2d0f4feb71f132b5e4571b9097692fa5ee7bfe55846fffb1b7e3`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:50 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Tue, 19 Dec 2023 01:20:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 06:47:07 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 19 Dec 2023 06:47:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 19 Dec 2023 06:47:16 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:47:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 19 Dec 2023 06:47:20 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 19 Dec 2023 06:47:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:47:25 GMT
ENV COUCHDB_VERSION=3.3.3
# Tue, 19 Dec 2023 06:47:26 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 19 Dec 2023 06:47:39 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 19 Dec 2023 06:47:39 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 19 Dec 2023 06:47:39 GMT
COPY --chown=couchdb:couchdbfile:e5db3ae8229456931b3901d8737d15bbebc21bae345eb60dc63b3edc7a03cfbc in /opt/couchdb/etc/ 
# Tue, 19 Dec 2023 06:47:40 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 19 Dec 2023 06:47:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 19 Dec 2023 06:47:40 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 06:47:40 GMT
VOLUME [/opt/couchdb/data]
# Tue, 19 Dec 2023 06:47:40 GMT
EXPOSE 4369 5984 9100
# Tue, 19 Dec 2023 06:47:40 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23f4f070a8876f3b9f2d6536e694e3c435dd993aa89811b93afe3bacdd39de9`  
		Last Modified: Tue, 19 Dec 2023 06:49:26 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e164d5f405aaa07b15f82f3f61b6dbd1cbdc900af32846793054982af6bebe8`  
		Last Modified: Tue, 19 Dec 2023 06:49:25 GMT  
		Size: 5.2 MB (5226586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1dfb4acdebdde82699f2071917a04403c86391036145bbe0ed6d0088656a5c`  
		Last Modified: Tue, 19 Dec 2023 06:49:24 GMT  
		Size: 610.9 KB (610876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1881a771df37f7280e9f36e60d2bf31e1aa682bc897cc46f6048ac2968810ba`  
		Last Modified: Tue, 19 Dec 2023 06:49:24 GMT  
		Size: 295.1 KB (295141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43749cff0c55900c892efc75594212cdfa3d8250f5e733ad3d7992578c888a53`  
		Last Modified: Tue, 19 Dec 2023 06:49:24 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73826e46a52089a5eb9572f0c4af2e15b3acdb046351f947055ebcf4a9738e8`  
		Last Modified: Tue, 19 Dec 2023 06:49:27 GMT  
		Size: 52.7 MB (52723616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d947e97cc2e724ae946a0a9c7d7acb1c2d25392cadd8502765bf22263aeb7c`  
		Last Modified: Tue, 19 Dec 2023 06:49:22 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7faf03e411f35a5287f56dfccb92efe76a20e4c74a82b7a72829c26175f8213f`  
		Last Modified: Tue, 19 Dec 2023 06:49:22 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0ad2880bdae49be7450333cca29ee638cc9391120e38cc468595f5860297d4`  
		Last Modified: Tue, 19 Dec 2023 06:49:22 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b3dcd02b547118831d71c582730baa714d3fa17b91ec09f7e73ad145fff73d`  
		Last Modified: Tue, 19 Dec 2023 06:49:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:665b281f4faefaa7f8859d9586a6a708c422903079ef2f4ccfe6a14564a886f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88720918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54871336972f9328fcec06bfc3e450d64daa6333ee69a45f0da14d120f8d2c05`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:52:39 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Nov 2023 07:52:39 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Nov 2023 07:52:45 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:52:48 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 21 Nov 2023 07:52:48 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Nov 2023 07:52:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 06 Dec 2023 00:39:25 GMT
ENV COUCHDB_VERSION=3.3.3
# Wed, 06 Dec 2023 00:39:26 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 06 Dec 2023 00:39:39 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 06 Dec 2023 00:39:39 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 06 Dec 2023 00:39:39 GMT
COPY --chown=couchdb:couchdbfile:e5db3ae8229456931b3901d8737d15bbebc21bae345eb60dc63b3edc7a03cfbc in /opt/couchdb/etc/ 
# Wed, 06 Dec 2023 00:39:40 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 06 Dec 2023 00:39:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 06 Dec 2023 00:39:40 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 06 Dec 2023 00:39:40 GMT
VOLUME [/opt/couchdb/data]
# Wed, 06 Dec 2023 00:39:40 GMT
EXPOSE 4369 5984 9100
# Wed, 06 Dec 2023 00:39:40 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a831f10e5df507c8f1e02bf16d8431aea07447742165f87bac8012c02082c5c1`  
		Last Modified: Tue, 21 Nov 2023 07:54:32 GMT  
		Size: 3.4 KB (3431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4f74c0ee547299d86d3b6de1a1b677264a77024288fe76a0459fe1596e94b0`  
		Last Modified: Tue, 21 Nov 2023 07:54:31 GMT  
		Size: 5.2 MB (5210800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a278347563aa0aac229a39ef7f2d07a6925c6a95f1eca2dc9335921b7b75f3`  
		Last Modified: Tue, 21 Nov 2023 07:54:31 GMT  
		Size: 567.0 KB (567042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479409bd9ad96512a7ba2074dabd9869a645ffa5edcc2ed2838022c816bae08d`  
		Last Modified: Tue, 21 Nov 2023 07:54:30 GMT  
		Size: 295.0 KB (295025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a142d67d1e29c92e5e8b3e869e9b175983fc8595ab6a96682dcf62381bfb7dcb`  
		Last Modified: Wed, 06 Dec 2023 00:40:09 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97468cc1d2c014c7d261b8ec053090497120e5fa58def003932cd6e2639f6fe8`  
		Last Modified: Wed, 06 Dec 2023 00:40:12 GMT  
		Size: 52.6 MB (52576241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f55ad37c5c976a16532ce2f3417578564432a3dae4959d764e63b301e6776c`  
		Last Modified: Wed, 06 Dec 2023 00:40:07 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab04edd67f8e979a7dd59173cfccc23a76d20fb11d745f273740d9954a48b1a3`  
		Last Modified: Wed, 06 Dec 2023 00:40:07 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e21f0bbd368632977373281a49f7c290995e50445f19302d538837ead8892cb`  
		Last Modified: Wed, 06 Dec 2023 00:40:07 GMT  
		Size: 2.2 KB (2228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559798cd9ec997b9e4aef8bf3ad255005563cab30e1be4f26ebdfdcad8b43c15`  
		Last Modified: Wed, 06 Dec 2023 00:40:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3` - linux; ppc64le

```console
$ docker pull couchdb@sha256:753b8176a7aef04da37381fd019c1b2fa6681010e801fc9036e3024e18715ca5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.0 MB (96006838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d353bf91590bd557c4b0d1b956dfe7e1e6fa4e21024715d5368e4a2c0d40cb23`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 19 Dec 2023 01:22:19 GMT
ADD file:1cb772a6ad8ca6301624db3141029490564de7673bc0f2d4bedb5a1578ea85bd in / 
# Tue, 19 Dec 2023 01:22:21 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 06:11:17 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 19 Dec 2023 06:11:20 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 19 Dec 2023 06:11:35 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:11:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 19 Dec 2023 06:11:40 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 19 Dec 2023 06:11:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:11:50 GMT
ENV COUCHDB_VERSION=3.3.3
# Tue, 19 Dec 2023 06:11:51 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 19 Dec 2023 06:12:12 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 19 Dec 2023 06:12:14 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 19 Dec 2023 06:12:15 GMT
COPY --chown=couchdb:couchdbfile:e5db3ae8229456931b3901d8737d15bbebc21bae345eb60dc63b3edc7a03cfbc in /opt/couchdb/etc/ 
# Tue, 19 Dec 2023 06:12:15 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 19 Dec 2023 06:12:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 19 Dec 2023 06:12:16 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 06:12:17 GMT
VOLUME [/opt/couchdb/data]
# Tue, 19 Dec 2023 06:12:17 GMT
EXPOSE 4369 5984 9100
# Tue, 19 Dec 2023 06:12:18 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:c9f6fac7f65cfc65b7f8de8bc377b135ca95e45a3246cf2bd1bb90922679553e`  
		Last Modified: Tue, 19 Dec 2023 01:27:11 GMT  
		Size: 35.3 MB (35293807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7577d3224ba65ea8b4b80082d021e485704e429a94e948187c117ef600a0bef`  
		Last Modified: Tue, 19 Dec 2023 06:12:58 GMT  
		Size: 3.4 KB (3417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf8166072b100e13640179c785cd4218b6a2e957ec0e129d0bde7e3834b4dfd`  
		Last Modified: Tue, 19 Dec 2023 06:12:57 GMT  
		Size: 6.0 MB (6046157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c850ad28a78cd961b2a762a88d0451864228709b98ab4b853b228ab4c0800ff7`  
		Last Modified: Tue, 19 Dec 2023 06:12:56 GMT  
		Size: 662.9 KB (662861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95514ebca6987967313a81e9311e31cd8685e3e37bbae279e5d699953a929caf`  
		Last Modified: Tue, 19 Dec 2023 06:12:56 GMT  
		Size: 295.0 KB (295041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c19fb87d01555598a6d01afad8ee27bbe66f165aba43c2b7371a8992104b49`  
		Last Modified: Tue, 19 Dec 2023 06:12:56 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f88c0665db50b85ec902075ad54db3b289b00cc710d7e4392ad1a54d2b30b67`  
		Last Modified: Tue, 19 Dec 2023 06:13:00 GMT  
		Size: 53.7 MB (53701301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4418e5805fb7f6139789891c3e29e2e88f5edc1316d9ba290f5b787f7875b4b4`  
		Last Modified: Tue, 19 Dec 2023 06:12:54 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1d3278e0d5e4065ead7e595ecf8e930b3d840461de896a6764408ca3c217f3`  
		Last Modified: Tue, 19 Dec 2023 06:12:54 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7656c58286888136b4d0eeadba3ffe94124aea9339b8f188674a7d9f08e23bb8`  
		Last Modified: Tue, 19 Dec 2023 06:12:54 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00ff0e342ac6c64e01a93d5a7e5b8141b7afc11273eaf4e03414f7cea7ea31f`  
		Last Modified: Tue, 19 Dec 2023 06:12:54 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3` - linux; s390x

```console
$ docker pull couchdb@sha256:2c22df2955be2202b336377102e40ba9df2110d2de473c1e15d4f47d6f349dd4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.0 MB (87020308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b385379393ba611686bcc3b50163b72e3d734b0d4de65bfe22aabcad3464918`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Nov 2023 05:05:18 GMT
ADD file:a545f27075704ce13e33e539170d3f47007424d2cc2bea5aecfd2608a5194151 in / 
# Tue, 21 Nov 2023 05:05:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:20:22 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Nov 2023 06:20:22 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Nov 2023 06:20:28 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:20:31 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 21 Nov 2023 06:20:31 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Nov 2023 06:20:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 06 Dec 2023 02:02:06 GMT
ENV COUCHDB_VERSION=3.3.3
# Wed, 06 Dec 2023 02:02:07 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 06 Dec 2023 02:02:23 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 06 Dec 2023 02:02:25 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 06 Dec 2023 02:02:25 GMT
COPY --chown=couchdb:couchdbfile:e5db3ae8229456931b3901d8737d15bbebc21bae345eb60dc63b3edc7a03cfbc in /opt/couchdb/etc/ 
# Wed, 06 Dec 2023 02:02:25 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 06 Dec 2023 02:02:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 06 Dec 2023 02:02:26 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 06 Dec 2023 02:02:26 GMT
VOLUME [/opt/couchdb/data]
# Wed, 06 Dec 2023 02:02:26 GMT
EXPOSE 4369 5984 9100
# Wed, 06 Dec 2023 02:02:26 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b114072f1cab66b7376d690985b12816aebab2e4e41fc170e32f111df27951dc`  
		Last Modified: Tue, 21 Nov 2023 05:10:48 GMT  
		Size: 29.7 MB (29656938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72dba253785a5e917fdd9064f61b676b4080ff3073424ff387308d70579c728b`  
		Last Modified: Tue, 21 Nov 2023 06:21:15 GMT  
		Size: 3.4 KB (3431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a299cd04ea14bbc3034e11001a1ec06dd4b5e1aaa78317dc803570f8a4c6437`  
		Last Modified: Tue, 21 Nov 2023 06:21:15 GMT  
		Size: 5.1 MB (5111719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c684e5bcbb93c8f0c9da5b81b4a1d19274f7ad0c7e3b17eb12cbe45cd2514989`  
		Last Modified: Tue, 21 Nov 2023 06:21:14 GMT  
		Size: 573.6 KB (573635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d916370cd04b7352346fee3edc1ac77bdb9393e24c5bc62c4cb0803a682836`  
		Last Modified: Tue, 21 Nov 2023 06:21:14 GMT  
		Size: 295.1 KB (295096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a1103db371c12bf970b540b2c88218edfbcbb795f44723923250883b44e1bd`  
		Last Modified: Wed, 06 Dec 2023 02:02:43 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b973390785fed3323a0dee86843a01b7fd4619d45b07d56f720944ec44472e`  
		Last Modified: Wed, 06 Dec 2023 02:02:47 GMT  
		Size: 51.4 MB (51375238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4460d75cadbb0c64ba1971daf7b584f7e206f245cf94c11aad8f34cb1ff3dabc`  
		Last Modified: Wed, 06 Dec 2023 02:02:42 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0329d7b8f2445b6e102b78c5fdde312f1124b63342ded38fc3aaea4e0f0df7`  
		Last Modified: Wed, 06 Dec 2023 02:02:42 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0492a0f28b3dfa930e25093cdb69b9d296c5a7eeb676913d57e1e7435073e4`  
		Last Modified: Wed, 06 Dec 2023 02:02:42 GMT  
		Size: 2.2 KB (2230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256de16f96660a155ac66140b318852f2d80a5e0b27520f1f56d4b5d5215e497`  
		Last Modified: Wed, 06 Dec 2023 02:02:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.3.3`

```console
$ docker pull couchdb@sha256:a2dc0a7ba1239ddc25b4f29931cee7ef6377554f88dd5b5bfd07019a6790e033
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `couchdb:3.3.3` - linux; amd64

```console
$ docker pull couchdb@sha256:84cc1a070b6ed5057c2539ce9ac0729140211317bfd4c3f8c6af6a972f866fec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.3 MB (90281758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f410d452fcd2d0f4feb71f132b5e4571b9097692fa5ee7bfe55846fffb1b7e3`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:50 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Tue, 19 Dec 2023 01:20:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 06:47:07 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 19 Dec 2023 06:47:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 19 Dec 2023 06:47:16 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:47:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 19 Dec 2023 06:47:20 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 19 Dec 2023 06:47:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:47:25 GMT
ENV COUCHDB_VERSION=3.3.3
# Tue, 19 Dec 2023 06:47:26 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 19 Dec 2023 06:47:39 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 19 Dec 2023 06:47:39 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 19 Dec 2023 06:47:39 GMT
COPY --chown=couchdb:couchdbfile:e5db3ae8229456931b3901d8737d15bbebc21bae345eb60dc63b3edc7a03cfbc in /opt/couchdb/etc/ 
# Tue, 19 Dec 2023 06:47:40 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 19 Dec 2023 06:47:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 19 Dec 2023 06:47:40 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 06:47:40 GMT
VOLUME [/opt/couchdb/data]
# Tue, 19 Dec 2023 06:47:40 GMT
EXPOSE 4369 5984 9100
# Tue, 19 Dec 2023 06:47:40 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23f4f070a8876f3b9f2d6536e694e3c435dd993aa89811b93afe3bacdd39de9`  
		Last Modified: Tue, 19 Dec 2023 06:49:26 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e164d5f405aaa07b15f82f3f61b6dbd1cbdc900af32846793054982af6bebe8`  
		Last Modified: Tue, 19 Dec 2023 06:49:25 GMT  
		Size: 5.2 MB (5226586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1dfb4acdebdde82699f2071917a04403c86391036145bbe0ed6d0088656a5c`  
		Last Modified: Tue, 19 Dec 2023 06:49:24 GMT  
		Size: 610.9 KB (610876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1881a771df37f7280e9f36e60d2bf31e1aa682bc897cc46f6048ac2968810ba`  
		Last Modified: Tue, 19 Dec 2023 06:49:24 GMT  
		Size: 295.1 KB (295141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43749cff0c55900c892efc75594212cdfa3d8250f5e733ad3d7992578c888a53`  
		Last Modified: Tue, 19 Dec 2023 06:49:24 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73826e46a52089a5eb9572f0c4af2e15b3acdb046351f947055ebcf4a9738e8`  
		Last Modified: Tue, 19 Dec 2023 06:49:27 GMT  
		Size: 52.7 MB (52723616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d947e97cc2e724ae946a0a9c7d7acb1c2d25392cadd8502765bf22263aeb7c`  
		Last Modified: Tue, 19 Dec 2023 06:49:22 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7faf03e411f35a5287f56dfccb92efe76a20e4c74a82b7a72829c26175f8213f`  
		Last Modified: Tue, 19 Dec 2023 06:49:22 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0ad2880bdae49be7450333cca29ee638cc9391120e38cc468595f5860297d4`  
		Last Modified: Tue, 19 Dec 2023 06:49:22 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b3dcd02b547118831d71c582730baa714d3fa17b91ec09f7e73ad145fff73d`  
		Last Modified: Tue, 19 Dec 2023 06:49:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:665b281f4faefaa7f8859d9586a6a708c422903079ef2f4ccfe6a14564a886f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88720918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54871336972f9328fcec06bfc3e450d64daa6333ee69a45f0da14d120f8d2c05`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:52:39 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Nov 2023 07:52:39 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Nov 2023 07:52:45 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:52:48 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 21 Nov 2023 07:52:48 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Nov 2023 07:52:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 06 Dec 2023 00:39:25 GMT
ENV COUCHDB_VERSION=3.3.3
# Wed, 06 Dec 2023 00:39:26 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 06 Dec 2023 00:39:39 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 06 Dec 2023 00:39:39 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 06 Dec 2023 00:39:39 GMT
COPY --chown=couchdb:couchdbfile:e5db3ae8229456931b3901d8737d15bbebc21bae345eb60dc63b3edc7a03cfbc in /opt/couchdb/etc/ 
# Wed, 06 Dec 2023 00:39:40 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 06 Dec 2023 00:39:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 06 Dec 2023 00:39:40 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 06 Dec 2023 00:39:40 GMT
VOLUME [/opt/couchdb/data]
# Wed, 06 Dec 2023 00:39:40 GMT
EXPOSE 4369 5984 9100
# Wed, 06 Dec 2023 00:39:40 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a831f10e5df507c8f1e02bf16d8431aea07447742165f87bac8012c02082c5c1`  
		Last Modified: Tue, 21 Nov 2023 07:54:32 GMT  
		Size: 3.4 KB (3431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4f74c0ee547299d86d3b6de1a1b677264a77024288fe76a0459fe1596e94b0`  
		Last Modified: Tue, 21 Nov 2023 07:54:31 GMT  
		Size: 5.2 MB (5210800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a278347563aa0aac229a39ef7f2d07a6925c6a95f1eca2dc9335921b7b75f3`  
		Last Modified: Tue, 21 Nov 2023 07:54:31 GMT  
		Size: 567.0 KB (567042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479409bd9ad96512a7ba2074dabd9869a645ffa5edcc2ed2838022c816bae08d`  
		Last Modified: Tue, 21 Nov 2023 07:54:30 GMT  
		Size: 295.0 KB (295025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a142d67d1e29c92e5e8b3e869e9b175983fc8595ab6a96682dcf62381bfb7dcb`  
		Last Modified: Wed, 06 Dec 2023 00:40:09 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97468cc1d2c014c7d261b8ec053090497120e5fa58def003932cd6e2639f6fe8`  
		Last Modified: Wed, 06 Dec 2023 00:40:12 GMT  
		Size: 52.6 MB (52576241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f55ad37c5c976a16532ce2f3417578564432a3dae4959d764e63b301e6776c`  
		Last Modified: Wed, 06 Dec 2023 00:40:07 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab04edd67f8e979a7dd59173cfccc23a76d20fb11d745f273740d9954a48b1a3`  
		Last Modified: Wed, 06 Dec 2023 00:40:07 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e21f0bbd368632977373281a49f7c290995e50445f19302d538837ead8892cb`  
		Last Modified: Wed, 06 Dec 2023 00:40:07 GMT  
		Size: 2.2 KB (2228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559798cd9ec997b9e4aef8bf3ad255005563cab30e1be4f26ebdfdcad8b43c15`  
		Last Modified: Wed, 06 Dec 2023 00:40:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3.3` - linux; ppc64le

```console
$ docker pull couchdb@sha256:753b8176a7aef04da37381fd019c1b2fa6681010e801fc9036e3024e18715ca5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.0 MB (96006838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d353bf91590bd557c4b0d1b956dfe7e1e6fa4e21024715d5368e4a2c0d40cb23`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 19 Dec 2023 01:22:19 GMT
ADD file:1cb772a6ad8ca6301624db3141029490564de7673bc0f2d4bedb5a1578ea85bd in / 
# Tue, 19 Dec 2023 01:22:21 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 06:11:17 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 19 Dec 2023 06:11:20 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 19 Dec 2023 06:11:35 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:11:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 19 Dec 2023 06:11:40 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 19 Dec 2023 06:11:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:11:50 GMT
ENV COUCHDB_VERSION=3.3.3
# Tue, 19 Dec 2023 06:11:51 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 19 Dec 2023 06:12:12 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 19 Dec 2023 06:12:14 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 19 Dec 2023 06:12:15 GMT
COPY --chown=couchdb:couchdbfile:e5db3ae8229456931b3901d8737d15bbebc21bae345eb60dc63b3edc7a03cfbc in /opt/couchdb/etc/ 
# Tue, 19 Dec 2023 06:12:15 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 19 Dec 2023 06:12:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 19 Dec 2023 06:12:16 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 06:12:17 GMT
VOLUME [/opt/couchdb/data]
# Tue, 19 Dec 2023 06:12:17 GMT
EXPOSE 4369 5984 9100
# Tue, 19 Dec 2023 06:12:18 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:c9f6fac7f65cfc65b7f8de8bc377b135ca95e45a3246cf2bd1bb90922679553e`  
		Last Modified: Tue, 19 Dec 2023 01:27:11 GMT  
		Size: 35.3 MB (35293807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7577d3224ba65ea8b4b80082d021e485704e429a94e948187c117ef600a0bef`  
		Last Modified: Tue, 19 Dec 2023 06:12:58 GMT  
		Size: 3.4 KB (3417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf8166072b100e13640179c785cd4218b6a2e957ec0e129d0bde7e3834b4dfd`  
		Last Modified: Tue, 19 Dec 2023 06:12:57 GMT  
		Size: 6.0 MB (6046157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c850ad28a78cd961b2a762a88d0451864228709b98ab4b853b228ab4c0800ff7`  
		Last Modified: Tue, 19 Dec 2023 06:12:56 GMT  
		Size: 662.9 KB (662861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95514ebca6987967313a81e9311e31cd8685e3e37bbae279e5d699953a929caf`  
		Last Modified: Tue, 19 Dec 2023 06:12:56 GMT  
		Size: 295.0 KB (295041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c19fb87d01555598a6d01afad8ee27bbe66f165aba43c2b7371a8992104b49`  
		Last Modified: Tue, 19 Dec 2023 06:12:56 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f88c0665db50b85ec902075ad54db3b289b00cc710d7e4392ad1a54d2b30b67`  
		Last Modified: Tue, 19 Dec 2023 06:13:00 GMT  
		Size: 53.7 MB (53701301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4418e5805fb7f6139789891c3e29e2e88f5edc1316d9ba290f5b787f7875b4b4`  
		Last Modified: Tue, 19 Dec 2023 06:12:54 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1d3278e0d5e4065ead7e595ecf8e930b3d840461de896a6764408ca3c217f3`  
		Last Modified: Tue, 19 Dec 2023 06:12:54 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7656c58286888136b4d0eeadba3ffe94124aea9339b8f188674a7d9f08e23bb8`  
		Last Modified: Tue, 19 Dec 2023 06:12:54 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00ff0e342ac6c64e01a93d5a7e5b8141b7afc11273eaf4e03414f7cea7ea31f`  
		Last Modified: Tue, 19 Dec 2023 06:12:54 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3.3` - linux; s390x

```console
$ docker pull couchdb@sha256:2c22df2955be2202b336377102e40ba9df2110d2de473c1e15d4f47d6f349dd4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.0 MB (87020308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b385379393ba611686bcc3b50163b72e3d734b0d4de65bfe22aabcad3464918`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Nov 2023 05:05:18 GMT
ADD file:a545f27075704ce13e33e539170d3f47007424d2cc2bea5aecfd2608a5194151 in / 
# Tue, 21 Nov 2023 05:05:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:20:22 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Nov 2023 06:20:22 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Nov 2023 06:20:28 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:20:31 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 21 Nov 2023 06:20:31 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Nov 2023 06:20:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 06 Dec 2023 02:02:06 GMT
ENV COUCHDB_VERSION=3.3.3
# Wed, 06 Dec 2023 02:02:07 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 06 Dec 2023 02:02:23 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 06 Dec 2023 02:02:25 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 06 Dec 2023 02:02:25 GMT
COPY --chown=couchdb:couchdbfile:e5db3ae8229456931b3901d8737d15bbebc21bae345eb60dc63b3edc7a03cfbc in /opt/couchdb/etc/ 
# Wed, 06 Dec 2023 02:02:25 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 06 Dec 2023 02:02:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 06 Dec 2023 02:02:26 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 06 Dec 2023 02:02:26 GMT
VOLUME [/opt/couchdb/data]
# Wed, 06 Dec 2023 02:02:26 GMT
EXPOSE 4369 5984 9100
# Wed, 06 Dec 2023 02:02:26 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b114072f1cab66b7376d690985b12816aebab2e4e41fc170e32f111df27951dc`  
		Last Modified: Tue, 21 Nov 2023 05:10:48 GMT  
		Size: 29.7 MB (29656938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72dba253785a5e917fdd9064f61b676b4080ff3073424ff387308d70579c728b`  
		Last Modified: Tue, 21 Nov 2023 06:21:15 GMT  
		Size: 3.4 KB (3431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a299cd04ea14bbc3034e11001a1ec06dd4b5e1aaa78317dc803570f8a4c6437`  
		Last Modified: Tue, 21 Nov 2023 06:21:15 GMT  
		Size: 5.1 MB (5111719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c684e5bcbb93c8f0c9da5b81b4a1d19274f7ad0c7e3b17eb12cbe45cd2514989`  
		Last Modified: Tue, 21 Nov 2023 06:21:14 GMT  
		Size: 573.6 KB (573635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d916370cd04b7352346fee3edc1ac77bdb9393e24c5bc62c4cb0803a682836`  
		Last Modified: Tue, 21 Nov 2023 06:21:14 GMT  
		Size: 295.1 KB (295096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a1103db371c12bf970b540b2c88218edfbcbb795f44723923250883b44e1bd`  
		Last Modified: Wed, 06 Dec 2023 02:02:43 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b973390785fed3323a0dee86843a01b7fd4619d45b07d56f720944ec44472e`  
		Last Modified: Wed, 06 Dec 2023 02:02:47 GMT  
		Size: 51.4 MB (51375238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4460d75cadbb0c64ba1971daf7b584f7e206f245cf94c11aad8f34cb1ff3dabc`  
		Last Modified: Wed, 06 Dec 2023 02:02:42 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0329d7b8f2445b6e102b78c5fdde312f1124b63342ded38fc3aaea4e0f0df7`  
		Last Modified: Wed, 06 Dec 2023 02:02:42 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0492a0f28b3dfa930e25093cdb69b9d296c5a7eeb676913d57e1e7435073e4`  
		Last Modified: Wed, 06 Dec 2023 02:02:42 GMT  
		Size: 2.2 KB (2230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256de16f96660a155ac66140b318852f2d80a5e0b27520f1f56d4b5d5215e497`  
		Last Modified: Wed, 06 Dec 2023 02:02:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:latest`

```console
$ docker pull couchdb@sha256:a2dc0a7ba1239ddc25b4f29931cee7ef6377554f88dd5b5bfd07019a6790e033
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:84cc1a070b6ed5057c2539ce9ac0729140211317bfd4c3f8c6af6a972f866fec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.3 MB (90281758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f410d452fcd2d0f4feb71f132b5e4571b9097692fa5ee7bfe55846fffb1b7e3`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 19 Dec 2023 01:20:50 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Tue, 19 Dec 2023 01:20:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 06:47:07 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 19 Dec 2023 06:47:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 19 Dec 2023 06:47:16 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:47:19 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 19 Dec 2023 06:47:20 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 19 Dec 2023 06:47:25 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:47:25 GMT
ENV COUCHDB_VERSION=3.3.3
# Tue, 19 Dec 2023 06:47:26 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 19 Dec 2023 06:47:39 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 19 Dec 2023 06:47:39 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 19 Dec 2023 06:47:39 GMT
COPY --chown=couchdb:couchdbfile:e5db3ae8229456931b3901d8737d15bbebc21bae345eb60dc63b3edc7a03cfbc in /opt/couchdb/etc/ 
# Tue, 19 Dec 2023 06:47:40 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 19 Dec 2023 06:47:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 19 Dec 2023 06:47:40 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 06:47:40 GMT
VOLUME [/opt/couchdb/data]
# Tue, 19 Dec 2023 06:47:40 GMT
EXPOSE 4369 5984 9100
# Tue, 19 Dec 2023 06:47:40 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23f4f070a8876f3b9f2d6536e694e3c435dd993aa89811b93afe3bacdd39de9`  
		Last Modified: Tue, 19 Dec 2023 06:49:26 GMT  
		Size: 3.4 KB (3409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e164d5f405aaa07b15f82f3f61b6dbd1cbdc900af32846793054982af6bebe8`  
		Last Modified: Tue, 19 Dec 2023 06:49:25 GMT  
		Size: 5.2 MB (5226586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1dfb4acdebdde82699f2071917a04403c86391036145bbe0ed6d0088656a5c`  
		Last Modified: Tue, 19 Dec 2023 06:49:24 GMT  
		Size: 610.9 KB (610876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1881a771df37f7280e9f36e60d2bf31e1aa682bc897cc46f6048ac2968810ba`  
		Last Modified: Tue, 19 Dec 2023 06:49:24 GMT  
		Size: 295.1 KB (295141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43749cff0c55900c892efc75594212cdfa3d8250f5e733ad3d7992578c888a53`  
		Last Modified: Tue, 19 Dec 2023 06:49:24 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73826e46a52089a5eb9572f0c4af2e15b3acdb046351f947055ebcf4a9738e8`  
		Last Modified: Tue, 19 Dec 2023 06:49:27 GMT  
		Size: 52.7 MB (52723616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d947e97cc2e724ae946a0a9c7d7acb1c2d25392cadd8502765bf22263aeb7c`  
		Last Modified: Tue, 19 Dec 2023 06:49:22 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7faf03e411f35a5287f56dfccb92efe76a20e4c74a82b7a72829c26175f8213f`  
		Last Modified: Tue, 19 Dec 2023 06:49:22 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0ad2880bdae49be7450333cca29ee638cc9391120e38cc468595f5860297d4`  
		Last Modified: Tue, 19 Dec 2023 06:49:22 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b3dcd02b547118831d71c582730baa714d3fa17b91ec09f7e73ad145fff73d`  
		Last Modified: Tue, 19 Dec 2023 06:49:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:665b281f4faefaa7f8859d9586a6a708c422903079ef2f4ccfe6a14564a886f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **88.7 MB (88720918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54871336972f9328fcec06bfc3e450d64daa6333ee69a45f0da14d120f8d2c05`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:52:39 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Nov 2023 07:52:39 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Nov 2023 07:52:45 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 07:52:48 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 21 Nov 2023 07:52:48 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Nov 2023 07:52:52 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 06 Dec 2023 00:39:25 GMT
ENV COUCHDB_VERSION=3.3.3
# Wed, 06 Dec 2023 00:39:26 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 06 Dec 2023 00:39:39 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 06 Dec 2023 00:39:39 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 06 Dec 2023 00:39:39 GMT
COPY --chown=couchdb:couchdbfile:e5db3ae8229456931b3901d8737d15bbebc21bae345eb60dc63b3edc7a03cfbc in /opt/couchdb/etc/ 
# Wed, 06 Dec 2023 00:39:40 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 06 Dec 2023 00:39:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 06 Dec 2023 00:39:40 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 06 Dec 2023 00:39:40 GMT
VOLUME [/opt/couchdb/data]
# Wed, 06 Dec 2023 00:39:40 GMT
EXPOSE 4369 5984 9100
# Wed, 06 Dec 2023 00:39:40 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a831f10e5df507c8f1e02bf16d8431aea07447742165f87bac8012c02082c5c1`  
		Last Modified: Tue, 21 Nov 2023 07:54:32 GMT  
		Size: 3.4 KB (3431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4f74c0ee547299d86d3b6de1a1b677264a77024288fe76a0459fe1596e94b0`  
		Last Modified: Tue, 21 Nov 2023 07:54:31 GMT  
		Size: 5.2 MB (5210800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a278347563aa0aac229a39ef7f2d07a6925c6a95f1eca2dc9335921b7b75f3`  
		Last Modified: Tue, 21 Nov 2023 07:54:31 GMT  
		Size: 567.0 KB (567042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479409bd9ad96512a7ba2074dabd9869a645ffa5edcc2ed2838022c816bae08d`  
		Last Modified: Tue, 21 Nov 2023 07:54:30 GMT  
		Size: 295.0 KB (295025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a142d67d1e29c92e5e8b3e869e9b175983fc8595ab6a96682dcf62381bfb7dcb`  
		Last Modified: Wed, 06 Dec 2023 00:40:09 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97468cc1d2c014c7d261b8ec053090497120e5fa58def003932cd6e2639f6fe8`  
		Last Modified: Wed, 06 Dec 2023 00:40:12 GMT  
		Size: 52.6 MB (52576241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f55ad37c5c976a16532ce2f3417578564432a3dae4959d764e63b301e6776c`  
		Last Modified: Wed, 06 Dec 2023 00:40:07 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab04edd67f8e979a7dd59173cfccc23a76d20fb11d745f273740d9954a48b1a3`  
		Last Modified: Wed, 06 Dec 2023 00:40:07 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e21f0bbd368632977373281a49f7c290995e50445f19302d538837ead8892cb`  
		Last Modified: Wed, 06 Dec 2023 00:40:07 GMT  
		Size: 2.2 KB (2228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559798cd9ec997b9e4aef8bf3ad255005563cab30e1be4f26ebdfdcad8b43c15`  
		Last Modified: Wed, 06 Dec 2023 00:40:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; ppc64le

```console
$ docker pull couchdb@sha256:753b8176a7aef04da37381fd019c1b2fa6681010e801fc9036e3024e18715ca5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.0 MB (96006838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d353bf91590bd557c4b0d1b956dfe7e1e6fa4e21024715d5368e4a2c0d40cb23`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 19 Dec 2023 01:22:19 GMT
ADD file:1cb772a6ad8ca6301624db3141029490564de7673bc0f2d4bedb5a1578ea85bd in / 
# Tue, 19 Dec 2023 01:22:21 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 06:11:17 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 19 Dec 2023 06:11:20 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 19 Dec 2023 06:11:35 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:11:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 19 Dec 2023 06:11:40 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 19 Dec 2023 06:11:50 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 06:11:50 GMT
ENV COUCHDB_VERSION=3.3.3
# Tue, 19 Dec 2023 06:11:51 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 19 Dec 2023 06:12:12 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 19 Dec 2023 06:12:14 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 19 Dec 2023 06:12:15 GMT
COPY --chown=couchdb:couchdbfile:e5db3ae8229456931b3901d8737d15bbebc21bae345eb60dc63b3edc7a03cfbc in /opt/couchdb/etc/ 
# Tue, 19 Dec 2023 06:12:15 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Tue, 19 Dec 2023 06:12:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 19 Dec 2023 06:12:16 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 06:12:17 GMT
VOLUME [/opt/couchdb/data]
# Tue, 19 Dec 2023 06:12:17 GMT
EXPOSE 4369 5984 9100
# Tue, 19 Dec 2023 06:12:18 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:c9f6fac7f65cfc65b7f8de8bc377b135ca95e45a3246cf2bd1bb90922679553e`  
		Last Modified: Tue, 19 Dec 2023 01:27:11 GMT  
		Size: 35.3 MB (35293807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7577d3224ba65ea8b4b80082d021e485704e429a94e948187c117ef600a0bef`  
		Last Modified: Tue, 19 Dec 2023 06:12:58 GMT  
		Size: 3.4 KB (3417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bf8166072b100e13640179c785cd4218b6a2e957ec0e129d0bde7e3834b4dfd`  
		Last Modified: Tue, 19 Dec 2023 06:12:57 GMT  
		Size: 6.0 MB (6046157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c850ad28a78cd961b2a762a88d0451864228709b98ab4b853b228ab4c0800ff7`  
		Last Modified: Tue, 19 Dec 2023 06:12:56 GMT  
		Size: 662.9 KB (662861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95514ebca6987967313a81e9311e31cd8685e3e37bbae279e5d699953a929caf`  
		Last Modified: Tue, 19 Dec 2023 06:12:56 GMT  
		Size: 295.0 KB (295041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c19fb87d01555598a6d01afad8ee27bbe66f165aba43c2b7371a8992104b49`  
		Last Modified: Tue, 19 Dec 2023 06:12:56 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f88c0665db50b85ec902075ad54db3b289b00cc710d7e4392ad1a54d2b30b67`  
		Last Modified: Tue, 19 Dec 2023 06:13:00 GMT  
		Size: 53.7 MB (53701301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4418e5805fb7f6139789891c3e29e2e88f5edc1316d9ba290f5b787f7875b4b4`  
		Last Modified: Tue, 19 Dec 2023 06:12:54 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1d3278e0d5e4065ead7e595ecf8e930b3d840461de896a6764408ca3c217f3`  
		Last Modified: Tue, 19 Dec 2023 06:12:54 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7656c58286888136b4d0eeadba3ffe94124aea9339b8f188674a7d9f08e23bb8`  
		Last Modified: Tue, 19 Dec 2023 06:12:54 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00ff0e342ac6c64e01a93d5a7e5b8141b7afc11273eaf4e03414f7cea7ea31f`  
		Last Modified: Tue, 19 Dec 2023 06:12:54 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; s390x

```console
$ docker pull couchdb@sha256:2c22df2955be2202b336377102e40ba9df2110d2de473c1e15d4f47d6f349dd4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.0 MB (87020308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b385379393ba611686bcc3b50163b72e3d734b0d4de65bfe22aabcad3464918`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Nov 2023 05:05:18 GMT
ADD file:a545f27075704ce13e33e539170d3f47007424d2cc2bea5aecfd2608a5194151 in / 
# Tue, 21 Nov 2023 05:05:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:20:22 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Nov 2023 06:20:22 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Nov 2023 06:20:28 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 06:20:31 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends tini;     rm -rf /var/lib/apt/lists/*;     tini --version
# Tue, 21 Nov 2023 06:20:31 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Nov 2023 06:20:36 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 06 Dec 2023 02:02:06 GMT
ENV COUCHDB_VERSION=3.3.3
# Wed, 06 Dec 2023 02:02:07 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 06 Dec 2023 02:02:23 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 06 Dec 2023 02:02:25 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 06 Dec 2023 02:02:25 GMT
COPY --chown=couchdb:couchdbfile:e5db3ae8229456931b3901d8737d15bbebc21bae345eb60dc63b3edc7a03cfbc in /opt/couchdb/etc/ 
# Wed, 06 Dec 2023 02:02:25 GMT
COPY file:cb88dd5d91ff7eac8d8abd6ec372df4f0e05b7787b7d3622916ee9dbe8ea0c85 in /usr/local/bin 
# Wed, 06 Dec 2023 02:02:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 06 Dec 2023 02:02:26 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 06 Dec 2023 02:02:26 GMT
VOLUME [/opt/couchdb/data]
# Wed, 06 Dec 2023 02:02:26 GMT
EXPOSE 4369 5984 9100
# Wed, 06 Dec 2023 02:02:26 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b114072f1cab66b7376d690985b12816aebab2e4e41fc170e32f111df27951dc`  
		Last Modified: Tue, 21 Nov 2023 05:10:48 GMT  
		Size: 29.7 MB (29656938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72dba253785a5e917fdd9064f61b676b4080ff3073424ff387308d70579c728b`  
		Last Modified: Tue, 21 Nov 2023 06:21:15 GMT  
		Size: 3.4 KB (3431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a299cd04ea14bbc3034e11001a1ec06dd4b5e1aaa78317dc803570f8a4c6437`  
		Last Modified: Tue, 21 Nov 2023 06:21:15 GMT  
		Size: 5.1 MB (5111719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c684e5bcbb93c8f0c9da5b81b4a1d19274f7ad0c7e3b17eb12cbe45cd2514989`  
		Last Modified: Tue, 21 Nov 2023 06:21:14 GMT  
		Size: 573.6 KB (573635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d916370cd04b7352346fee3edc1ac77bdb9393e24c5bc62c4cb0803a682836`  
		Last Modified: Tue, 21 Nov 2023 06:21:14 GMT  
		Size: 295.1 KB (295096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a1103db371c12bf970b540b2c88218edfbcbb795f44723923250883b44e1bd`  
		Last Modified: Wed, 06 Dec 2023 02:02:43 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b973390785fed3323a0dee86843a01b7fd4619d45b07d56f720944ec44472e`  
		Last Modified: Wed, 06 Dec 2023 02:02:47 GMT  
		Size: 51.4 MB (51375238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4460d75cadbb0c64ba1971daf7b584f7e206f245cf94c11aad8f34cb1ff3dabc`  
		Last Modified: Wed, 06 Dec 2023 02:02:42 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0329d7b8f2445b6e102b78c5fdde312f1124b63342ded38fc3aaea4e0f0df7`  
		Last Modified: Wed, 06 Dec 2023 02:02:42 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0492a0f28b3dfa930e25093cdb69b9d296c5a7eeb676913d57e1e7435073e4`  
		Last Modified: Wed, 06 Dec 2023 02:02:42 GMT  
		Size: 2.2 KB (2230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256de16f96660a155ac66140b318852f2d80a5e0b27520f1f56d4b5d5215e497`  
		Last Modified: Wed, 06 Dec 2023 02:02:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
