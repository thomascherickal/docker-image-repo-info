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
$ docker pull couchdb@sha256:77e2dd5c39336387efc6e3f9381d0f7bf74461733d121b0f1b9bbe6f271f47ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2` - linux; amd64

```console
$ docker pull couchdb@sha256:f00fa296cbd0f10526356b265b0824774d97e45d93ef344ca502ba708e936c40
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84538927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39085525a132628f4a60c2a8ccbb94ac8ac7c22af508c40a80ed238e47870fc1`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Mar 2023 04:10:22 GMT
ADD file:2254e48bf53907be7a0b1744bc4fcd7805a627672793cf5f86a01ac751a1b24d in / 
# Wed, 01 Mar 2023 04:10:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:57:29 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Mar 2023 04:57:30 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Mar 2023 04:57:38 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:57:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Mar 2023 04:57:42 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Mar 2023 04:57:48 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:58:10 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 01 Mar 2023 04:58:11 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Mar 2023 04:58:29 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Mar 2023 04:58:29 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Mar 2023 04:58:29 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 01 Mar 2023 04:58:29 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 01 Mar 2023 04:58:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Mar 2023 04:58:30 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 04:58:30 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Mar 2023 04:58:30 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Mar 2023 04:58:30 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:8fd419aca81cfd3987d61550e700546537628562693bc01acc9f85468f483706`  
		Last Modified: Wed, 01 Mar 2023 04:15:04 GMT  
		Size: 27.1 MB (27139882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3381c1268083c6f22290329c5445e6bdd0d24301dbe0499de5c3b39c43e6a837`  
		Last Modified: Wed, 01 Mar 2023 04:59:23 GMT  
		Size: 3.4 KB (3415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd80bd75fe65477bba2d539bc9e5e36f67000b64d7090024c548384eaaed1c9a`  
		Last Modified: Wed, 01 Mar 2023 04:59:22 GMT  
		Size: 6.7 MB (6705930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac77c9625dab9ea7df1d54ebd8e3c4e7b603e00f5ab2a83e4631631aa7f28797`  
		Last Modified: Wed, 01 Mar 2023 04:59:21 GMT  
		Size: 1.3 MB (1259600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bda150e57a9a14bfbde395fa9ae9838bb488a7ad4990455bf9df265d69bea56`  
		Last Modified: Wed, 01 Mar 2023 04:59:21 GMT  
		Size: 294.4 KB (294355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721b5a4b16de8b99e4ddee9d018035a4a60663d93f2c764f612fb34dfda44597`  
		Last Modified: Wed, 01 Mar 2023 04:59:35 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd94bdc5adc2d30a569c12f937e9bbaaf7ea83c01fe830f07f974b84d2b33ad`  
		Last Modified: Wed, 01 Mar 2023 04:59:39 GMT  
		Size: 49.1 MB (49132144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c390e14a6265b20a844647eaf7ed464dd270bb5a4c8b8ad9d87c7c44ea46a09c`  
		Last Modified: Wed, 01 Mar 2023 04:59:33 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c12b03ed830f425d2ca6239332392aa2cd342f85d2ef5855d5a15a3925cfbcc`  
		Last Modified: Wed, 01 Mar 2023 04:59:33 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51274e515eb0e24f0ff3d10302bee9884b68bf8607bdc8255079e8b8504a65e0`  
		Last Modified: Wed, 01 Mar 2023 04:59:33 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dcaf5f59e6a480f794e59ab9cd6e40f191ccc6fdae41419af23d7023408a91b`  
		Last Modified: Wed, 01 Mar 2023 04:59:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:18ebb64f4ca27a098d8d0e7c5c91ffdd08acc7cb65a17d8282500bef740f5cb8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72995208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b43cee9fd6b7e4b99034b01169a4b19bf076a06acb57b76544c7467756004a9`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:59 GMT
ADD file:442c85d39a4dbb97fb311e1f30e76f5d197339db3967532742e299fa73410f89 in / 
# Thu, 09 Feb 2023 03:58:59 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 13:38:19 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 09 Feb 2023 13:38:19 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 09 Feb 2023 13:38:25 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 13:38:29 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 09 Feb 2023 13:38:29 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 09 Feb 2023 13:38:35 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 13:38:52 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Thu, 09 Feb 2023 13:38:52 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 09 Feb 2023 13:39:04 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 09 Feb 2023 13:39:04 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Thu, 09 Feb 2023 13:39:04 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 09 Feb 2023 13:39:04 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Thu, 09 Feb 2023 13:39:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 09 Feb 2023 13:39:05 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 13:39:05 GMT
VOLUME [/opt/couchdb/data]
# Thu, 09 Feb 2023 13:39:05 GMT
EXPOSE 4369 5984 9100
# Thu, 09 Feb 2023 13:39:05 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ebcd4e3db076a77234a526ba23bdac8b205f7d74fd052a936cfa190b42cf49aa`  
		Last Modified: Thu, 09 Feb 2023 04:03:14 GMT  
		Size: 25.9 MB (25922825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aee1b8a3c1042190ef5a7ad2017145c92c8500e06474c874a014231b3316aa9`  
		Last Modified: Thu, 09 Feb 2023 13:39:58 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a79a4eead140ecb1871f08ef0f7a36d0c49c13175525de21c6d867a6515177`  
		Last Modified: Thu, 09 Feb 2023 13:39:57 GMT  
		Size: 6.6 MB (6577109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baca3ba0dd68bdf1d65bde8e42c9cfd435f1f0cdb2d234f69fb61bf5590f52c2`  
		Last Modified: Thu, 09 Feb 2023 13:39:57 GMT  
		Size: 1.2 MB (1164507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad75529a1f5bd861854989809c93483e2267245c535df80e7156c83b44d8723`  
		Last Modified: Thu, 09 Feb 2023 13:39:56 GMT  
		Size: 294.2 KB (294169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01784a8cc55d7c2aad75202929ce4bbd31b68b3a5310d668295b57a1f1e9b668`  
		Last Modified: Thu, 09 Feb 2023 13:40:09 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf10def1e72089b84a2e0cf189913a1df3bb063af2cc8394baec9dfaf7dd508`  
		Last Modified: Thu, 09 Feb 2023 13:40:11 GMT  
		Size: 39.0 MB (39029555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:021bcabf1b011cbf1c4ddac97d55197ff6b0965d39a09644eea7fb92ed491680`  
		Last Modified: Thu, 09 Feb 2023 13:40:07 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0e1f0663c8d87d858a66753ed7d1f6572f2d06bd5a526a95b36d98594f81a5`  
		Last Modified: Thu, 09 Feb 2023 13:40:07 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87e3147f28b75c3ea28728a9b2af2d39410fed52577222b78e7c9ea325c429e`  
		Last Modified: Thu, 09 Feb 2023 13:40:07 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbe67db724b32b783545bae3febd5050d2255443f0a8c379739f4a7c149f293`  
		Last Modified: Thu, 09 Feb 2023 13:40:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3`

```console
$ docker pull couchdb@sha256:77e2dd5c39336387efc6e3f9381d0f7bf74461733d121b0f1b9bbe6f271f47ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:f00fa296cbd0f10526356b265b0824774d97e45d93ef344ca502ba708e936c40
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84538927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39085525a132628f4a60c2a8ccbb94ac8ac7c22af508c40a80ed238e47870fc1`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Mar 2023 04:10:22 GMT
ADD file:2254e48bf53907be7a0b1744bc4fcd7805a627672793cf5f86a01ac751a1b24d in / 
# Wed, 01 Mar 2023 04:10:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:57:29 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Mar 2023 04:57:30 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Mar 2023 04:57:38 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:57:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Mar 2023 04:57:42 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Mar 2023 04:57:48 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:58:10 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 01 Mar 2023 04:58:11 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Mar 2023 04:58:29 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Mar 2023 04:58:29 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Mar 2023 04:58:29 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 01 Mar 2023 04:58:29 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 01 Mar 2023 04:58:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Mar 2023 04:58:30 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 04:58:30 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Mar 2023 04:58:30 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Mar 2023 04:58:30 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:8fd419aca81cfd3987d61550e700546537628562693bc01acc9f85468f483706`  
		Last Modified: Wed, 01 Mar 2023 04:15:04 GMT  
		Size: 27.1 MB (27139882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3381c1268083c6f22290329c5445e6bdd0d24301dbe0499de5c3b39c43e6a837`  
		Last Modified: Wed, 01 Mar 2023 04:59:23 GMT  
		Size: 3.4 KB (3415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd80bd75fe65477bba2d539bc9e5e36f67000b64d7090024c548384eaaed1c9a`  
		Last Modified: Wed, 01 Mar 2023 04:59:22 GMT  
		Size: 6.7 MB (6705930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac77c9625dab9ea7df1d54ebd8e3c4e7b603e00f5ab2a83e4631631aa7f28797`  
		Last Modified: Wed, 01 Mar 2023 04:59:21 GMT  
		Size: 1.3 MB (1259600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bda150e57a9a14bfbde395fa9ae9838bb488a7ad4990455bf9df265d69bea56`  
		Last Modified: Wed, 01 Mar 2023 04:59:21 GMT  
		Size: 294.4 KB (294355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721b5a4b16de8b99e4ddee9d018035a4a60663d93f2c764f612fb34dfda44597`  
		Last Modified: Wed, 01 Mar 2023 04:59:35 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd94bdc5adc2d30a569c12f937e9bbaaf7ea83c01fe830f07f974b84d2b33ad`  
		Last Modified: Wed, 01 Mar 2023 04:59:39 GMT  
		Size: 49.1 MB (49132144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c390e14a6265b20a844647eaf7ed464dd270bb5a4c8b8ad9d87c7c44ea46a09c`  
		Last Modified: Wed, 01 Mar 2023 04:59:33 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c12b03ed830f425d2ca6239332392aa2cd342f85d2ef5855d5a15a3925cfbcc`  
		Last Modified: Wed, 01 Mar 2023 04:59:33 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51274e515eb0e24f0ff3d10302bee9884b68bf8607bdc8255079e8b8504a65e0`  
		Last Modified: Wed, 01 Mar 2023 04:59:33 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dcaf5f59e6a480f794e59ab9cd6e40f191ccc6fdae41419af23d7023408a91b`  
		Last Modified: Wed, 01 Mar 2023 04:59:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:18ebb64f4ca27a098d8d0e7c5c91ffdd08acc7cb65a17d8282500bef740f5cb8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72995208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b43cee9fd6b7e4b99034b01169a4b19bf076a06acb57b76544c7467756004a9`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:59 GMT
ADD file:442c85d39a4dbb97fb311e1f30e76f5d197339db3967532742e299fa73410f89 in / 
# Thu, 09 Feb 2023 03:58:59 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 13:38:19 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 09 Feb 2023 13:38:19 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 09 Feb 2023 13:38:25 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 13:38:29 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 09 Feb 2023 13:38:29 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 09 Feb 2023 13:38:35 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 13:38:52 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Thu, 09 Feb 2023 13:38:52 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 09 Feb 2023 13:39:04 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 09 Feb 2023 13:39:04 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Thu, 09 Feb 2023 13:39:04 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 09 Feb 2023 13:39:04 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Thu, 09 Feb 2023 13:39:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 09 Feb 2023 13:39:05 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 13:39:05 GMT
VOLUME [/opt/couchdb/data]
# Thu, 09 Feb 2023 13:39:05 GMT
EXPOSE 4369 5984 9100
# Thu, 09 Feb 2023 13:39:05 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ebcd4e3db076a77234a526ba23bdac8b205f7d74fd052a936cfa190b42cf49aa`  
		Last Modified: Thu, 09 Feb 2023 04:03:14 GMT  
		Size: 25.9 MB (25922825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aee1b8a3c1042190ef5a7ad2017145c92c8500e06474c874a014231b3316aa9`  
		Last Modified: Thu, 09 Feb 2023 13:39:58 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a79a4eead140ecb1871f08ef0f7a36d0c49c13175525de21c6d867a6515177`  
		Last Modified: Thu, 09 Feb 2023 13:39:57 GMT  
		Size: 6.6 MB (6577109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baca3ba0dd68bdf1d65bde8e42c9cfd435f1f0cdb2d234f69fb61bf5590f52c2`  
		Last Modified: Thu, 09 Feb 2023 13:39:57 GMT  
		Size: 1.2 MB (1164507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad75529a1f5bd861854989809c93483e2267245c535df80e7156c83b44d8723`  
		Last Modified: Thu, 09 Feb 2023 13:39:56 GMT  
		Size: 294.2 KB (294169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01784a8cc55d7c2aad75202929ce4bbd31b68b3a5310d668295b57a1f1e9b668`  
		Last Modified: Thu, 09 Feb 2023 13:40:09 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf10def1e72089b84a2e0cf189913a1df3bb063af2cc8394baec9dfaf7dd508`  
		Last Modified: Thu, 09 Feb 2023 13:40:11 GMT  
		Size: 39.0 MB (39029555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:021bcabf1b011cbf1c4ddac97d55197ff6b0965d39a09644eea7fb92ed491680`  
		Last Modified: Thu, 09 Feb 2023 13:40:07 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0e1f0663c8d87d858a66753ed7d1f6572f2d06bd5a526a95b36d98594f81a5`  
		Last Modified: Thu, 09 Feb 2023 13:40:07 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87e3147f28b75c3ea28728a9b2af2d39410fed52577222b78e7c9ea325c429e`  
		Last Modified: Thu, 09 Feb 2023 13:40:07 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbe67db724b32b783545bae3febd5050d2255443f0a8c379739f4a7c149f293`  
		Last Modified: Thu, 09 Feb 2023 13:40:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3.1`

```console
$ docker pull couchdb@sha256:77e2dd5c39336387efc6e3f9381d0f7bf74461733d121b0f1b9bbe6f271f47ad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:f00fa296cbd0f10526356b265b0824774d97e45d93ef344ca502ba708e936c40
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84538927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39085525a132628f4a60c2a8ccbb94ac8ac7c22af508c40a80ed238e47870fc1`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Mar 2023 04:10:22 GMT
ADD file:2254e48bf53907be7a0b1744bc4fcd7805a627672793cf5f86a01ac751a1b24d in / 
# Wed, 01 Mar 2023 04:10:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:57:29 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Mar 2023 04:57:30 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Mar 2023 04:57:38 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:57:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Mar 2023 04:57:42 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Mar 2023 04:57:48 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:58:10 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 01 Mar 2023 04:58:11 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Mar 2023 04:58:29 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Mar 2023 04:58:29 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Mar 2023 04:58:29 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 01 Mar 2023 04:58:29 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 01 Mar 2023 04:58:30 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Mar 2023 04:58:30 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 04:58:30 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Mar 2023 04:58:30 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Mar 2023 04:58:30 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:8fd419aca81cfd3987d61550e700546537628562693bc01acc9f85468f483706`  
		Last Modified: Wed, 01 Mar 2023 04:15:04 GMT  
		Size: 27.1 MB (27139882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3381c1268083c6f22290329c5445e6bdd0d24301dbe0499de5c3b39c43e6a837`  
		Last Modified: Wed, 01 Mar 2023 04:59:23 GMT  
		Size: 3.4 KB (3415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd80bd75fe65477bba2d539bc9e5e36f67000b64d7090024c548384eaaed1c9a`  
		Last Modified: Wed, 01 Mar 2023 04:59:22 GMT  
		Size: 6.7 MB (6705930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac77c9625dab9ea7df1d54ebd8e3c4e7b603e00f5ab2a83e4631631aa7f28797`  
		Last Modified: Wed, 01 Mar 2023 04:59:21 GMT  
		Size: 1.3 MB (1259600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bda150e57a9a14bfbde395fa9ae9838bb488a7ad4990455bf9df265d69bea56`  
		Last Modified: Wed, 01 Mar 2023 04:59:21 GMT  
		Size: 294.4 KB (294355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721b5a4b16de8b99e4ddee9d018035a4a60663d93f2c764f612fb34dfda44597`  
		Last Modified: Wed, 01 Mar 2023 04:59:35 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd94bdc5adc2d30a569c12f937e9bbaaf7ea83c01fe830f07f974b84d2b33ad`  
		Last Modified: Wed, 01 Mar 2023 04:59:39 GMT  
		Size: 49.1 MB (49132144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c390e14a6265b20a844647eaf7ed464dd270bb5a4c8b8ad9d87c7c44ea46a09c`  
		Last Modified: Wed, 01 Mar 2023 04:59:33 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c12b03ed830f425d2ca6239332392aa2cd342f85d2ef5855d5a15a3925cfbcc`  
		Last Modified: Wed, 01 Mar 2023 04:59:33 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51274e515eb0e24f0ff3d10302bee9884b68bf8607bdc8255079e8b8504a65e0`  
		Last Modified: Wed, 01 Mar 2023 04:59:33 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dcaf5f59e6a480f794e59ab9cd6e40f191ccc6fdae41419af23d7023408a91b`  
		Last Modified: Wed, 01 Mar 2023 04:59:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:18ebb64f4ca27a098d8d0e7c5c91ffdd08acc7cb65a17d8282500bef740f5cb8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72995208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b43cee9fd6b7e4b99034b01169a4b19bf076a06acb57b76544c7467756004a9`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:59 GMT
ADD file:442c85d39a4dbb97fb311e1f30e76f5d197339db3967532742e299fa73410f89 in / 
# Thu, 09 Feb 2023 03:58:59 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 13:38:19 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 09 Feb 2023 13:38:19 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 09 Feb 2023 13:38:25 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 13:38:29 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 09 Feb 2023 13:38:29 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 09 Feb 2023 13:38:35 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 13:38:52 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Thu, 09 Feb 2023 13:38:52 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 09 Feb 2023 13:39:04 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 09 Feb 2023 13:39:04 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Thu, 09 Feb 2023 13:39:04 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 09 Feb 2023 13:39:04 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Thu, 09 Feb 2023 13:39:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 09 Feb 2023 13:39:05 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 13:39:05 GMT
VOLUME [/opt/couchdb/data]
# Thu, 09 Feb 2023 13:39:05 GMT
EXPOSE 4369 5984 9100
# Thu, 09 Feb 2023 13:39:05 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ebcd4e3db076a77234a526ba23bdac8b205f7d74fd052a936cfa190b42cf49aa`  
		Last Modified: Thu, 09 Feb 2023 04:03:14 GMT  
		Size: 25.9 MB (25922825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aee1b8a3c1042190ef5a7ad2017145c92c8500e06474c874a014231b3316aa9`  
		Last Modified: Thu, 09 Feb 2023 13:39:58 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a79a4eead140ecb1871f08ef0f7a36d0c49c13175525de21c6d867a6515177`  
		Last Modified: Thu, 09 Feb 2023 13:39:57 GMT  
		Size: 6.6 MB (6577109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baca3ba0dd68bdf1d65bde8e42c9cfd435f1f0cdb2d234f69fb61bf5590f52c2`  
		Last Modified: Thu, 09 Feb 2023 13:39:57 GMT  
		Size: 1.2 MB (1164507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad75529a1f5bd861854989809c93483e2267245c535df80e7156c83b44d8723`  
		Last Modified: Thu, 09 Feb 2023 13:39:56 GMT  
		Size: 294.2 KB (294169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01784a8cc55d7c2aad75202929ce4bbd31b68b3a5310d668295b57a1f1e9b668`  
		Last Modified: Thu, 09 Feb 2023 13:40:09 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf10def1e72089b84a2e0cf189913a1df3bb063af2cc8394baec9dfaf7dd508`  
		Last Modified: Thu, 09 Feb 2023 13:40:11 GMT  
		Size: 39.0 MB (39029555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:021bcabf1b011cbf1c4ddac97d55197ff6b0965d39a09644eea7fb92ed491680`  
		Last Modified: Thu, 09 Feb 2023 13:40:07 GMT  
		Size: 384.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0e1f0663c8d87d858a66753ed7d1f6572f2d06bd5a526a95b36d98594f81a5`  
		Last Modified: Thu, 09 Feb 2023 13:40:07 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87e3147f28b75c3ea28728a9b2af2d39410fed52577222b78e7c9ea325c429e`  
		Last Modified: Thu, 09 Feb 2023 13:40:07 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbe67db724b32b783545bae3febd5050d2255443f0a8c379739f4a7c149f293`  
		Last Modified: Thu, 09 Feb 2023 13:40:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3`

```console
$ docker pull couchdb@sha256:77b6a90206ba433e59878efddc39a694500e2baf4684aadc6265f2b3d2e78b4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3` - linux; amd64

```console
$ docker pull couchdb@sha256:dee3f17fa11aa1d43c0bd60c282d68b95f2cb0ea10582055a712be2c323cf481
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91168508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c023ab20b99cef1ccbfa589fb35f923d1048860f5f55217e69ba05e18e39631a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:56:29 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Mar 2023 04:56:29 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Mar 2023 04:56:37 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:56:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Mar 2023 04:56:41 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Mar 2023 04:56:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:56:46 GMT
ENV COUCHDB_VERSION=3.3.1
# Wed, 01 Mar 2023 04:56:47 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Mar 2023 04:57:00 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Mar 2023 04:57:00 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Mar 2023 04:57:00 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 01 Mar 2023 04:57:00 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 01 Mar 2023 04:57:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Mar 2023 04:57:01 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 04:57:01 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Mar 2023 04:57:01 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Mar 2023 04:57:01 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6637e7f130a96ee279b7cd93c77afc7a28fd7f831b19520de38e2b6b45ba2939`  
		Last Modified: Wed, 01 Mar 2023 04:58:49 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4dc9bd71357404364ed9c84296ea0170e4b13240b108fc598fcbc0400a3880`  
		Last Modified: Wed, 01 Mar 2023 04:58:48 GMT  
		Size: 5.2 MB (5224334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bde3e5409fa60225a360de6fc7cff74d8fdf8e3744088a5d03c3a9f8f22a12e`  
		Last Modified: Wed, 01 Mar 2023 04:58:48 GMT  
		Size: 1.6 MB (1553317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e818344b5f6306fba9c7fd2a9425930d01c149a178358a242bae48ac6fec38`  
		Last Modified: Wed, 01 Mar 2023 04:58:47 GMT  
		Size: 295.6 KB (295619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd0506641807b420c32835a9af376fe4810365cc6932f83148cf11374bf4bdd`  
		Last Modified: Wed, 01 Mar 2023 04:58:47 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6e0fd8fcee53fd180b1f321220a7b173c73c189d01741c93f21d83b664dcf1`  
		Last Modified: Wed, 01 Mar 2023 04:58:51 GMT  
		Size: 52.7 MB (52676453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f243172300bd45fa27ff12f5b283e411a5825f2ae436f9545f9c30fbdcf1031`  
		Last Modified: Wed, 01 Mar 2023 04:58:45 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdece4117c4fa382060db81e46bea365c1dc59ce1b4371caf5036535c9846134`  
		Last Modified: Wed, 01 Mar 2023 04:58:45 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e870857342e5e9d5e0441a5d7eefc223938f717850bb9228d9aa5840386ef4c`  
		Last Modified: Wed, 01 Mar 2023 04:58:45 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64097a0563ea7989e391d5759e050d96127903a994698b8d099486bad2502afb`  
		Last Modified: Wed, 01 Mar 2023 04:58:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:1e5ae5c1018aa7ffac0a966f0b93f626fe1c3ecd2eb74027df90f835fc44df03
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.5 MB (89542496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62c82e36049948ec0642106125f326a103110fa86398d11b0ef673476de21774`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 13:37:29 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 09 Feb 2023 13:37:29 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 09 Feb 2023 13:37:36 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 13:37:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 09 Feb 2023 13:37:38 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 09 Feb 2023 13:37:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 13:37:43 GMT
ENV COUCHDB_VERSION=3.3.1
# Thu, 09 Feb 2023 13:37:43 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 09 Feb 2023 13:37:55 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 09 Feb 2023 13:37:55 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 09 Feb 2023 13:37:55 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Thu, 09 Feb 2023 13:37:55 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Thu, 09 Feb 2023 13:37:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 09 Feb 2023 13:37:56 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 13:37:56 GMT
VOLUME [/opt/couchdb/data]
# Thu, 09 Feb 2023 13:37:56 GMT
EXPOSE 4369 5984 9100
# Thu, 09 Feb 2023 13:37:56 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6091f9f6c73b4b952be2bbc2cd89a8fc504064bf7483b83b7ea81f13fa4d54`  
		Last Modified: Thu, 09 Feb 2023 13:39:26 GMT  
		Size: 3.4 KB (3439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e00b3493fef81fb1cab07d097825491e38cb83abd318e8c4d1ee8c5b856710`  
		Last Modified: Thu, 09 Feb 2023 13:39:26 GMT  
		Size: 5.2 MB (5209406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0f2fc9cbc7001e7f9e0948436f0dd3a05468c357b0bee7bab813dec0619529`  
		Last Modified: Thu, 09 Feb 2023 13:39:25 GMT  
		Size: 1.4 MB (1435933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806951d526ba39c29e24fec1009ff647797fc0fab6abec6327d5cdb57cac82c8`  
		Last Modified: Thu, 09 Feb 2023 13:39:24 GMT  
		Size: 295.5 KB (295507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700f98b31af11297aaa7eb2cd0d795ff8b2741e8b5386b6b2af6ef7b9a0b1699`  
		Last Modified: Thu, 09 Feb 2023 13:39:24 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e964753acddc0f3887bebeeeb9d2f59a9c599626089435b5c304abaa33ace7a`  
		Last Modified: Thu, 09 Feb 2023 13:39:27 GMT  
		Size: 52.5 MB (52531739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3865d8e42284b4b7956e56adf6c7437adbb519a75369988c47ced075375078`  
		Last Modified: Thu, 09 Feb 2023 13:39:22 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa1ed4d8adeb2b889db515882b22a39b2a844eeaacaeb24b7a716274085e2db`  
		Last Modified: Thu, 09 Feb 2023 13:39:22 GMT  
		Size: 999.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42068c71f1e69e3289401c91c462dbbcd14fcb04a5a3f230bcec583dbde39a2`  
		Last Modified: Thu, 09 Feb 2023 13:39:23 GMT  
		Size: 2.2 KB (2188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b380f7228b5b2b7bd574dfac69b654e94c0a45880dbcde5d48db0e90ac1d8d`  
		Last Modified: Thu, 09 Feb 2023 13:39:22 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; ppc64le

```console
$ docker pull couchdb@sha256:aa9693a4ea6a67e2d48c99e32ac51914c414b4332b30be1c9b2bd42c2a616074
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.7 MB (96679233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74ec5c87509de09ccb8fe5339cfd2c6265f9d69bd7aa889186ee6306ad81311c`
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
# Wed, 01 Mar 2023 05:43:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Mar 2023 05:43:59 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Mar 2023 05:44:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:44:16 GMT
ENV COUCHDB_VERSION=3.3.1
# Wed, 01 Mar 2023 05:44:17 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Mar 2023 05:44:48 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Mar 2023 05:44:51 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Mar 2023 05:44:51 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 01 Mar 2023 05:44:52 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 01 Mar 2023 05:44:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Mar 2023 05:44:55 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 05:44:56 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Mar 2023 05:44:57 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Mar 2023 05:44:58 GMT
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
	-	`sha256:cbef0173a07bc581e30e85a57b1e68802fcc0a024f244fa68c5b459d9c237577`  
		Last Modified: Wed, 01 Mar 2023 05:46:04 GMT  
		Size: 1.5 MB (1509253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553cf561c481aa0f831976d5481d1c2f5564fded0f487d629e780599b8b950cb`  
		Last Modified: Wed, 01 Mar 2023 05:46:04 GMT  
		Size: 295.6 KB (295602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57156270861ebec15e15824b98ce258087d77093da47aa2505c0f10323dbf576`  
		Last Modified: Wed, 01 Mar 2023 05:46:03 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170b2c08141c093d2a5f59fade4fed001a14775b4ae0553f26009520440c5074`  
		Last Modified: Wed, 01 Mar 2023 05:46:12 GMT  
		Size: 53.5 MB (53534942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0690b576b7faaf6377d377ccda31c9f40557af57ac472a66e767d1c2003508cf`  
		Last Modified: Wed, 01 Mar 2023 05:46:01 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05de86fd9c9910a4e1ed03a633ffd1f982abc032eddc6482211b9e52712fc457`  
		Last Modified: Wed, 01 Mar 2023 05:46:01 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:332b0bd48c4b5ddcdc504dd68272e7cffed2eeb6543dbf6c2766ee2190566153`  
		Last Modified: Wed, 01 Mar 2023 05:46:01 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3fbf8e1caf707e5e47d41e751e4316e5a73e5c95cbb2b8b717847eb2807b8e`  
		Last Modified: Wed, 01 Mar 2023 05:46:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1`

```console
$ docker pull couchdb@sha256:f112e1d5075a3cc48ca518fe56b22b083c8bc0514c2158598c09454d8e82d4c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:be908c1b586be1c5633621a3aa135ae30190014deb6b0d5998c119199724c9f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80026341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79064f60a232ebcc1807a42c78b66c75b943a335579e9e8bc7cb03010069de82`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Mar 2023 04:10:22 GMT
ADD file:2254e48bf53907be7a0b1744bc4fcd7805a627672793cf5f86a01ac751a1b24d in / 
# Wed, 01 Mar 2023 04:10:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:57:29 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Mar 2023 04:57:30 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Mar 2023 04:57:38 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:57:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Mar 2023 04:57:42 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Mar 2023 04:57:48 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:57:48 GMT
ENV COUCHDB_VERSION=3.1.2
# Wed, 01 Mar 2023 04:57:49 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Mar 2023 04:58:02 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Mar 2023 04:58:03 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Mar 2023 04:58:03 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 01 Mar 2023 04:58:03 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 01 Mar 2023 04:58:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Mar 2023 04:58:04 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 04:58:04 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Mar 2023 04:58:04 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Mar 2023 04:58:04 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:8fd419aca81cfd3987d61550e700546537628562693bc01acc9f85468f483706`  
		Last Modified: Wed, 01 Mar 2023 04:15:04 GMT  
		Size: 27.1 MB (27139882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3381c1268083c6f22290329c5445e6bdd0d24301dbe0499de5c3b39c43e6a837`  
		Last Modified: Wed, 01 Mar 2023 04:59:23 GMT  
		Size: 3.4 KB (3415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd80bd75fe65477bba2d539bc9e5e36f67000b64d7090024c548384eaaed1c9a`  
		Last Modified: Wed, 01 Mar 2023 04:59:22 GMT  
		Size: 6.7 MB (6705930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac77c9625dab9ea7df1d54ebd8e3c4e7b603e00f5ab2a83e4631631aa7f28797`  
		Last Modified: Wed, 01 Mar 2023 04:59:21 GMT  
		Size: 1.3 MB (1259600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bda150e57a9a14bfbde395fa9ae9838bb488a7ad4990455bf9df265d69bea56`  
		Last Modified: Wed, 01 Mar 2023 04:59:21 GMT  
		Size: 294.4 KB (294355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dea979ca4ebb90a90a89878291feea493733f5318c4d0264c38db50cd0095ad`  
		Last Modified: Wed, 01 Mar 2023 04:59:21 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a17435058b174559c6dd62ef7958d24be86a8d7e649d6a55fbf2330405a323b`  
		Last Modified: Wed, 01 Mar 2023 04:59:24 GMT  
		Size: 44.6 MB (44619554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7df995c3f74ff9b041d920545b7451c510a48acf3c55ce68a29ac74635ae546`  
		Last Modified: Wed, 01 Mar 2023 04:59:19 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d69b8d9e468b7b50efc01be45f0d5ada072a78850abd7d21180fb918f7816d`  
		Last Modified: Wed, 01 Mar 2023 04:59:19 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9185dec2968e2084b7f11871f446afd513d7af246f6f2ec666ac7d2f7529938f`  
		Last Modified: Wed, 01 Mar 2023 04:59:19 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3a1c990f13bd06299f57c8bd8959051c2bfe8c1281efd077269c2505c8b31f`  
		Last Modified: Wed, 01 Mar 2023 04:59:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:2614c0d3ccb7c1229ca94ce47d2fbdd875bbd5c3fd63e04c9850712fe35ddac0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75090010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1242bca72c16a2b53e0aa124453d05a5d03e68ed74e52ecf8f6f683602b2ef45`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:59 GMT
ADD file:442c85d39a4dbb97fb311e1f30e76f5d197339db3967532742e299fa73410f89 in / 
# Thu, 09 Feb 2023 03:58:59 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 13:38:19 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 09 Feb 2023 13:38:19 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 09 Feb 2023 13:38:25 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 13:38:29 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 09 Feb 2023 13:38:29 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 09 Feb 2023 13:38:35 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 13:38:35 GMT
ENV COUCHDB_VERSION=3.1.2
# Thu, 09 Feb 2023 13:38:36 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 09 Feb 2023 13:38:47 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 09 Feb 2023 13:38:47 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 09 Feb 2023 13:38:47 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 09 Feb 2023 13:38:47 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Thu, 09 Feb 2023 13:38:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 09 Feb 2023 13:38:48 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 13:38:48 GMT
VOLUME [/opt/couchdb/data]
# Thu, 09 Feb 2023 13:38:48 GMT
EXPOSE 4369 5984 9100
# Thu, 09 Feb 2023 13:38:48 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ebcd4e3db076a77234a526ba23bdac8b205f7d74fd052a936cfa190b42cf49aa`  
		Last Modified: Thu, 09 Feb 2023 04:03:14 GMT  
		Size: 25.9 MB (25922825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aee1b8a3c1042190ef5a7ad2017145c92c8500e06474c874a014231b3316aa9`  
		Last Modified: Thu, 09 Feb 2023 13:39:58 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a79a4eead140ecb1871f08ef0f7a36d0c49c13175525de21c6d867a6515177`  
		Last Modified: Thu, 09 Feb 2023 13:39:57 GMT  
		Size: 6.6 MB (6577109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baca3ba0dd68bdf1d65bde8e42c9cfd435f1f0cdb2d234f69fb61bf5590f52c2`  
		Last Modified: Thu, 09 Feb 2023 13:39:57 GMT  
		Size: 1.2 MB (1164507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad75529a1f5bd861854989809c93483e2267245c535df80e7156c83b44d8723`  
		Last Modified: Thu, 09 Feb 2023 13:39:56 GMT  
		Size: 294.2 KB (294169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:300a4ac8415bd2527731c5b0acef7953cee519e39f6e8bbdbf01752515411503`  
		Last Modified: Thu, 09 Feb 2023 13:39:56 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc0ff1e5a6a14cbac4daca81d8ebcccff30ba548d866a298a3e8e0799f3b664`  
		Last Modified: Thu, 09 Feb 2023 13:39:58 GMT  
		Size: 41.1 MB (41124362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb880062322fc3acb0f1a5ae4480dd3cc87ed64f05a956e45451cc54132f1284`  
		Last Modified: Thu, 09 Feb 2023 13:39:54 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93a3e35751822aed6de6d16280a01e24c984938e1bc01a674fd7b4e88df16311`  
		Last Modified: Thu, 09 Feb 2023 13:39:54 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5a8ed414348edf3155cd80647c851ad48b1c26a1324bfea3a0e687ed2f2e19`  
		Last Modified: Thu, 09 Feb 2023 13:39:54 GMT  
		Size: 2.1 KB (2062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e82e4c4100d5154460d7d35d085ff1dd2d36160e09d709b5b5492f14617fa1`  
		Last Modified: Thu, 09 Feb 2023 13:39:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1.2`

```console
$ docker pull couchdb@sha256:f112e1d5075a3cc48ca518fe56b22b083c8bc0514c2158598c09454d8e82d4c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1.2` - linux; amd64

```console
$ docker pull couchdb@sha256:be908c1b586be1c5633621a3aa135ae30190014deb6b0d5998c119199724c9f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.0 MB (80026341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79064f60a232ebcc1807a42c78b66c75b943a335579e9e8bc7cb03010069de82`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Mar 2023 04:10:22 GMT
ADD file:2254e48bf53907be7a0b1744bc4fcd7805a627672793cf5f86a01ac751a1b24d in / 
# Wed, 01 Mar 2023 04:10:22 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:57:29 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Mar 2023 04:57:30 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Mar 2023 04:57:38 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:57:42 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Mar 2023 04:57:42 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Mar 2023 04:57:48 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:57:48 GMT
ENV COUCHDB_VERSION=3.1.2
# Wed, 01 Mar 2023 04:57:49 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Mar 2023 04:58:02 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Mar 2023 04:58:03 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Mar 2023 04:58:03 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 01 Mar 2023 04:58:03 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 01 Mar 2023 04:58:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Mar 2023 04:58:04 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 04:58:04 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Mar 2023 04:58:04 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Mar 2023 04:58:04 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:8fd419aca81cfd3987d61550e700546537628562693bc01acc9f85468f483706`  
		Last Modified: Wed, 01 Mar 2023 04:15:04 GMT  
		Size: 27.1 MB (27139882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3381c1268083c6f22290329c5445e6bdd0d24301dbe0499de5c3b39c43e6a837`  
		Last Modified: Wed, 01 Mar 2023 04:59:23 GMT  
		Size: 3.4 KB (3415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd80bd75fe65477bba2d539bc9e5e36f67000b64d7090024c548384eaaed1c9a`  
		Last Modified: Wed, 01 Mar 2023 04:59:22 GMT  
		Size: 6.7 MB (6705930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac77c9625dab9ea7df1d54ebd8e3c4e7b603e00f5ab2a83e4631631aa7f28797`  
		Last Modified: Wed, 01 Mar 2023 04:59:21 GMT  
		Size: 1.3 MB (1259600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bda150e57a9a14bfbde395fa9ae9838bb488a7ad4990455bf9df265d69bea56`  
		Last Modified: Wed, 01 Mar 2023 04:59:21 GMT  
		Size: 294.4 KB (294355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dea979ca4ebb90a90a89878291feea493733f5318c4d0264c38db50cd0095ad`  
		Last Modified: Wed, 01 Mar 2023 04:59:21 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a17435058b174559c6dd62ef7958d24be86a8d7e649d6a55fbf2330405a323b`  
		Last Modified: Wed, 01 Mar 2023 04:59:24 GMT  
		Size: 44.6 MB (44619554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7df995c3f74ff9b041d920545b7451c510a48acf3c55ce68a29ac74635ae546`  
		Last Modified: Wed, 01 Mar 2023 04:59:19 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d69b8d9e468b7b50efc01be45f0d5ada072a78850abd7d21180fb918f7816d`  
		Last Modified: Wed, 01 Mar 2023 04:59:19 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9185dec2968e2084b7f11871f446afd513d7af246f6f2ec666ac7d2f7529938f`  
		Last Modified: Wed, 01 Mar 2023 04:59:19 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c3a1c990f13bd06299f57c8bd8959051c2bfe8c1281efd077269c2505c8b31f`  
		Last Modified: Wed, 01 Mar 2023 04:59:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:2614c0d3ccb7c1229ca94ce47d2fbdd875bbd5c3fd63e04c9850712fe35ddac0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75090010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1242bca72c16a2b53e0aa124453d05a5d03e68ed74e52ecf8f6f683602b2ef45`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:59 GMT
ADD file:442c85d39a4dbb97fb311e1f30e76f5d197339db3967532742e299fa73410f89 in / 
# Thu, 09 Feb 2023 03:58:59 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 13:38:19 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 09 Feb 2023 13:38:19 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 09 Feb 2023 13:38:25 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 13:38:29 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 09 Feb 2023 13:38:29 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 09 Feb 2023 13:38:35 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 13:38:35 GMT
ENV COUCHDB_VERSION=3.1.2
# Thu, 09 Feb 2023 13:38:36 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 09 Feb 2023 13:38:47 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 09 Feb 2023 13:38:47 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 09 Feb 2023 13:38:47 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 09 Feb 2023 13:38:47 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Thu, 09 Feb 2023 13:38:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 09 Feb 2023 13:38:48 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 13:38:48 GMT
VOLUME [/opt/couchdb/data]
# Thu, 09 Feb 2023 13:38:48 GMT
EXPOSE 4369 5984 9100
# Thu, 09 Feb 2023 13:38:48 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:ebcd4e3db076a77234a526ba23bdac8b205f7d74fd052a936cfa190b42cf49aa`  
		Last Modified: Thu, 09 Feb 2023 04:03:14 GMT  
		Size: 25.9 MB (25922825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aee1b8a3c1042190ef5a7ad2017145c92c8500e06474c874a014231b3316aa9`  
		Last Modified: Thu, 09 Feb 2023 13:39:58 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a79a4eead140ecb1871f08ef0f7a36d0c49c13175525de21c6d867a6515177`  
		Last Modified: Thu, 09 Feb 2023 13:39:57 GMT  
		Size: 6.6 MB (6577109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baca3ba0dd68bdf1d65bde8e42c9cfd435f1f0cdb2d234f69fb61bf5590f52c2`  
		Last Modified: Thu, 09 Feb 2023 13:39:57 GMT  
		Size: 1.2 MB (1164507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad75529a1f5bd861854989809c93483e2267245c535df80e7156c83b44d8723`  
		Last Modified: Thu, 09 Feb 2023 13:39:56 GMT  
		Size: 294.2 KB (294169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:300a4ac8415bd2527731c5b0acef7953cee519e39f6e8bbdbf01752515411503`  
		Last Modified: Thu, 09 Feb 2023 13:39:56 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc0ff1e5a6a14cbac4daca81d8ebcccff30ba548d866a298a3e8e0799f3b664`  
		Last Modified: Thu, 09 Feb 2023 13:39:58 GMT  
		Size: 41.1 MB (41124362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb880062322fc3acb0f1a5ae4480dd3cc87ed64f05a956e45451cc54132f1284`  
		Last Modified: Thu, 09 Feb 2023 13:39:54 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93a3e35751822aed6de6d16280a01e24c984938e1bc01a674fd7b4e88df16311`  
		Last Modified: Thu, 09 Feb 2023 13:39:54 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5a8ed414348edf3155cd80647c851ad48b1c26a1324bfea3a0e687ed2f2e19`  
		Last Modified: Thu, 09 Feb 2023 13:39:54 GMT  
		Size: 2.1 KB (2062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e82e4c4100d5154460d7d35d085ff1dd2d36160e09d709b5b5492f14617fa1`  
		Last Modified: Thu, 09 Feb 2023 13:39:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2`

```console
$ docker pull couchdb@sha256:a23cc803820a9fd57cef21c2d777d89e905a461b01908f985b9d27e4fd212c36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2` - linux; amd64

```console
$ docker pull couchdb@sha256:c19738d414c68d642761754f7722e951f9f9b61cfe10abee235ef14aa220a80e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87538923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2958c1a2f02e17c9b2091a820af930f1bfcf9baac6f99f422364c5599f69c663`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:56:29 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Mar 2023 04:56:29 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Mar 2023 04:56:37 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:56:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Mar 2023 04:56:41 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Mar 2023 04:56:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:57:10 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Wed, 01 Mar 2023 04:57:10 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Mar 2023 04:57:23 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Mar 2023 04:57:23 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Mar 2023 04:57:23 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 01 Mar 2023 04:57:23 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 01 Mar 2023 04:57:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Mar 2023 04:57:24 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 04:57:24 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Mar 2023 04:57:24 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Mar 2023 04:57:24 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6637e7f130a96ee279b7cd93c77afc7a28fd7f831b19520de38e2b6b45ba2939`  
		Last Modified: Wed, 01 Mar 2023 04:58:49 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4dc9bd71357404364ed9c84296ea0170e4b13240b108fc598fcbc0400a3880`  
		Last Modified: Wed, 01 Mar 2023 04:58:48 GMT  
		Size: 5.2 MB (5224334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bde3e5409fa60225a360de6fc7cff74d8fdf8e3744088a5d03c3a9f8f22a12e`  
		Last Modified: Wed, 01 Mar 2023 04:58:48 GMT  
		Size: 1.6 MB (1553317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e818344b5f6306fba9c7fd2a9425930d01c149a178358a242bae48ac6fec38`  
		Last Modified: Wed, 01 Mar 2023 04:58:47 GMT  
		Size: 295.6 KB (295619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9eab40b1a4155afe9258d02a26fb6d5eb5a9b2ae2b6610573e071b0e6d419e6`  
		Last Modified: Wed, 01 Mar 2023 04:59:07 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e83a5471e8e5bac7dd5130fcdbad25ed5ac5469c46e6b518671d1cc11df24d`  
		Last Modified: Wed, 01 Mar 2023 04:59:10 GMT  
		Size: 49.0 MB (49047109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f8b4a8cba587b7f91cbaacaa2d1eef2747c8d54c580ea4e7239ef111b4ea3b`  
		Last Modified: Wed, 01 Mar 2023 04:59:05 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2850017aae386fac5c0507c14be2ee49fddfe3dc3f2e14bba79f5480ac7d2bc2`  
		Last Modified: Wed, 01 Mar 2023 04:59:05 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18f1503e1f33858dc96ebc2d0100d5770d532fca48d057d28258145db547190`  
		Last Modified: Wed, 01 Mar 2023 04:59:05 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce387e8260bd073472b122c9e811807ab1c48ab390e0618b2dc6202ef7ae9b7e`  
		Last Modified: Wed, 01 Mar 2023 04:59:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:e09252bc88975c7f52bafe3a2e2bc2f79ba509e2891de13cb51d04167943844d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.1 MB (86076271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2679e193fc928827801c98ea02247a5c3b6606e3ac59832f591ea86012b3c33a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 13:37:29 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 09 Feb 2023 13:37:29 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 09 Feb 2023 13:37:36 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 13:37:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 09 Feb 2023 13:37:38 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 09 Feb 2023 13:37:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 13:38:02 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Thu, 09 Feb 2023 13:38:03 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 09 Feb 2023 13:38:14 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 09 Feb 2023 13:38:14 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 09 Feb 2023 13:38:14 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 09 Feb 2023 13:38:14 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Thu, 09 Feb 2023 13:38:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 09 Feb 2023 13:38:15 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 13:38:15 GMT
VOLUME [/opt/couchdb/data]
# Thu, 09 Feb 2023 13:38:15 GMT
EXPOSE 4369 5984 9100
# Thu, 09 Feb 2023 13:38:15 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6091f9f6c73b4b952be2bbc2cd89a8fc504064bf7483b83b7ea81f13fa4d54`  
		Last Modified: Thu, 09 Feb 2023 13:39:26 GMT  
		Size: 3.4 KB (3439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e00b3493fef81fb1cab07d097825491e38cb83abd318e8c4d1ee8c5b856710`  
		Last Modified: Thu, 09 Feb 2023 13:39:26 GMT  
		Size: 5.2 MB (5209406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0f2fc9cbc7001e7f9e0948436f0dd3a05468c357b0bee7bab813dec0619529`  
		Last Modified: Thu, 09 Feb 2023 13:39:25 GMT  
		Size: 1.4 MB (1435933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806951d526ba39c29e24fec1009ff647797fc0fab6abec6327d5cdb57cac82c8`  
		Last Modified: Thu, 09 Feb 2023 13:39:24 GMT  
		Size: 295.5 KB (295507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c5e45cf7407e8d3896cb247de03485145ab396bc34c225dd1844753b519ab5`  
		Last Modified: Thu, 09 Feb 2023 13:39:43 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:820e16ea29bdd62cc638fc0342880a10e15a42bcf7c9204ee1455e5672c68466`  
		Last Modified: Thu, 09 Feb 2023 13:39:45 GMT  
		Size: 49.1 MB (49065739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f478eeb7f76e27f61153bd21bba550550e850fe249fbf8ffe7bd0630a2fdfc6`  
		Last Modified: Thu, 09 Feb 2023 13:39:41 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2bb052e262042a1f075479da668387adae41bfe4c39ba2892fbecf2dc14e2a1`  
		Last Modified: Thu, 09 Feb 2023 13:39:41 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffacc2efe7df09092aaad8ddbb7926352252be834f0ffd0294420960156eadb6`  
		Last Modified: Thu, 09 Feb 2023 13:39:41 GMT  
		Size: 2.2 KB (2191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38cf9faae45da9338c72ca39b478127c47b11cc4c62da439fc8c4e5068d0715b`  
		Last Modified: Thu, 09 Feb 2023 13:39:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2` - linux; ppc64le

```console
$ docker pull couchdb@sha256:c399bf2156b7112b21119165223d1e9a2d34e6a8301b07cc94a2a412eeb4f3e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93230624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6db186358f76c416c7cdb96c50bf21052c524ebecbc30cee46c42beb24fca00`
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
# Wed, 01 Mar 2023 05:43:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Mar 2023 05:43:59 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Mar 2023 05:44:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:45:05 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Wed, 01 Mar 2023 05:45:06 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Mar 2023 05:45:34 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Mar 2023 05:45:36 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Mar 2023 05:45:37 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 01 Mar 2023 05:45:37 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 01 Mar 2023 05:45:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Mar 2023 05:45:39 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 05:45:39 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Mar 2023 05:45:40 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Mar 2023 05:45:40 GMT
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
	-	`sha256:cbef0173a07bc581e30e85a57b1e68802fcc0a024f244fa68c5b459d9c237577`  
		Last Modified: Wed, 01 Mar 2023 05:46:04 GMT  
		Size: 1.5 MB (1509253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553cf561c481aa0f831976d5481d1c2f5564fded0f487d629e780599b8b950cb`  
		Last Modified: Wed, 01 Mar 2023 05:46:04 GMT  
		Size: 295.6 KB (295602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca762f444998d4bd3016122f9886d4e7c14da812ddbc7f7de8e575f4b2bae68`  
		Last Modified: Wed, 01 Mar 2023 05:46:35 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e71af86e7969357b8a270a9d615903fb9a2cc829c6371012bdd30c6b8651ea1`  
		Last Modified: Wed, 01 Mar 2023 05:46:43 GMT  
		Size: 50.1 MB (50086567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a98c3c152489f0d0fe21ceac6aa20723c329bb4301b0947aa29ee6f923a0e52`  
		Last Modified: Wed, 01 Mar 2023 05:46:34 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b42d18f1c4c133b6947441af70f66a78abd7ccadb1f7044e040252a24615781`  
		Last Modified: Wed, 01 Mar 2023 05:46:34 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fc695927445d03aad064debcfbc03a0347a572662d7710e2e5aab06ded9f1b`  
		Last Modified: Wed, 01 Mar 2023 05:46:34 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd64d5384a509a49a41e2a092f9ced334fba5563ff436cd3177217ce7d8fc3b2`  
		Last Modified: Wed, 01 Mar 2023 05:46:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.2.2`

```console
$ docker pull couchdb@sha256:a23cc803820a9fd57cef21c2d777d89e905a461b01908f985b9d27e4fd212c36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.2.2` - linux; amd64

```console
$ docker pull couchdb@sha256:c19738d414c68d642761754f7722e951f9f9b61cfe10abee235ef14aa220a80e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.5 MB (87538923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2958c1a2f02e17c9b2091a820af930f1bfcf9baac6f99f422364c5599f69c663`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:56:29 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Mar 2023 04:56:29 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Mar 2023 04:56:37 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:56:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Mar 2023 04:56:41 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Mar 2023 04:56:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:57:10 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Wed, 01 Mar 2023 04:57:10 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Mar 2023 04:57:23 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Mar 2023 04:57:23 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Mar 2023 04:57:23 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 01 Mar 2023 04:57:23 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 01 Mar 2023 04:57:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Mar 2023 04:57:24 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 04:57:24 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Mar 2023 04:57:24 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Mar 2023 04:57:24 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6637e7f130a96ee279b7cd93c77afc7a28fd7f831b19520de38e2b6b45ba2939`  
		Last Modified: Wed, 01 Mar 2023 04:58:49 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4dc9bd71357404364ed9c84296ea0170e4b13240b108fc598fcbc0400a3880`  
		Last Modified: Wed, 01 Mar 2023 04:58:48 GMT  
		Size: 5.2 MB (5224334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bde3e5409fa60225a360de6fc7cff74d8fdf8e3744088a5d03c3a9f8f22a12e`  
		Last Modified: Wed, 01 Mar 2023 04:58:48 GMT  
		Size: 1.6 MB (1553317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e818344b5f6306fba9c7fd2a9425930d01c149a178358a242bae48ac6fec38`  
		Last Modified: Wed, 01 Mar 2023 04:58:47 GMT  
		Size: 295.6 KB (295619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9eab40b1a4155afe9258d02a26fb6d5eb5a9b2ae2b6610573e071b0e6d419e6`  
		Last Modified: Wed, 01 Mar 2023 04:59:07 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e83a5471e8e5bac7dd5130fcdbad25ed5ac5469c46e6b518671d1cc11df24d`  
		Last Modified: Wed, 01 Mar 2023 04:59:10 GMT  
		Size: 49.0 MB (49047109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f8b4a8cba587b7f91cbaacaa2d1eef2747c8d54c580ea4e7239ef111b4ea3b`  
		Last Modified: Wed, 01 Mar 2023 04:59:05 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2850017aae386fac5c0507c14be2ee49fddfe3dc3f2e14bba79f5480ac7d2bc2`  
		Last Modified: Wed, 01 Mar 2023 04:59:05 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18f1503e1f33858dc96ebc2d0100d5770d532fca48d057d28258145db547190`  
		Last Modified: Wed, 01 Mar 2023 04:59:05 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce387e8260bd073472b122c9e811807ab1c48ab390e0618b2dc6202ef7ae9b7e`  
		Last Modified: Wed, 01 Mar 2023 04:59:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2.2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:e09252bc88975c7f52bafe3a2e2bc2f79ba509e2891de13cb51d04167943844d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.1 MB (86076271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2679e193fc928827801c98ea02247a5c3b6606e3ac59832f591ea86012b3c33a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 13:37:29 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 09 Feb 2023 13:37:29 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 09 Feb 2023 13:37:36 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 13:37:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 09 Feb 2023 13:37:38 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 09 Feb 2023 13:37:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 13:38:02 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Thu, 09 Feb 2023 13:38:03 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 09 Feb 2023 13:38:14 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 09 Feb 2023 13:38:14 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 09 Feb 2023 13:38:14 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 09 Feb 2023 13:38:14 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Thu, 09 Feb 2023 13:38:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 09 Feb 2023 13:38:15 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 13:38:15 GMT
VOLUME [/opt/couchdb/data]
# Thu, 09 Feb 2023 13:38:15 GMT
EXPOSE 4369 5984 9100
# Thu, 09 Feb 2023 13:38:15 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6091f9f6c73b4b952be2bbc2cd89a8fc504064bf7483b83b7ea81f13fa4d54`  
		Last Modified: Thu, 09 Feb 2023 13:39:26 GMT  
		Size: 3.4 KB (3439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e00b3493fef81fb1cab07d097825491e38cb83abd318e8c4d1ee8c5b856710`  
		Last Modified: Thu, 09 Feb 2023 13:39:26 GMT  
		Size: 5.2 MB (5209406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0f2fc9cbc7001e7f9e0948436f0dd3a05468c357b0bee7bab813dec0619529`  
		Last Modified: Thu, 09 Feb 2023 13:39:25 GMT  
		Size: 1.4 MB (1435933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806951d526ba39c29e24fec1009ff647797fc0fab6abec6327d5cdb57cac82c8`  
		Last Modified: Thu, 09 Feb 2023 13:39:24 GMT  
		Size: 295.5 KB (295507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c5e45cf7407e8d3896cb247de03485145ab396bc34c225dd1844753b519ab5`  
		Last Modified: Thu, 09 Feb 2023 13:39:43 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:820e16ea29bdd62cc638fc0342880a10e15a42bcf7c9204ee1455e5672c68466`  
		Last Modified: Thu, 09 Feb 2023 13:39:45 GMT  
		Size: 49.1 MB (49065739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f478eeb7f76e27f61153bd21bba550550e850fe249fbf8ffe7bd0630a2fdfc6`  
		Last Modified: Thu, 09 Feb 2023 13:39:41 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2bb052e262042a1f075479da668387adae41bfe4c39ba2892fbecf2dc14e2a1`  
		Last Modified: Thu, 09 Feb 2023 13:39:41 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffacc2efe7df09092aaad8ddbb7926352252be834f0ffd0294420960156eadb6`  
		Last Modified: Thu, 09 Feb 2023 13:39:41 GMT  
		Size: 2.2 KB (2191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38cf9faae45da9338c72ca39b478127c47b11cc4c62da439fc8c4e5068d0715b`  
		Last Modified: Thu, 09 Feb 2023 13:39:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.2.2` - linux; ppc64le

```console
$ docker pull couchdb@sha256:c399bf2156b7112b21119165223d1e9a2d34e6a8301b07cc94a2a412eeb4f3e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93230624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6db186358f76c416c7cdb96c50bf21052c524ebecbc30cee46c42beb24fca00`
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
# Wed, 01 Mar 2023 05:43:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Mar 2023 05:43:59 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Mar 2023 05:44:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:45:05 GMT
ENV COUCHDB_VERSION=3.2.2-1
# Wed, 01 Mar 2023 05:45:06 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Mar 2023 05:45:34 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Mar 2023 05:45:36 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Mar 2023 05:45:37 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 01 Mar 2023 05:45:37 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 01 Mar 2023 05:45:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Mar 2023 05:45:39 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 05:45:39 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Mar 2023 05:45:40 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Mar 2023 05:45:40 GMT
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
	-	`sha256:cbef0173a07bc581e30e85a57b1e68802fcc0a024f244fa68c5b459d9c237577`  
		Last Modified: Wed, 01 Mar 2023 05:46:04 GMT  
		Size: 1.5 MB (1509253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553cf561c481aa0f831976d5481d1c2f5564fded0f487d629e780599b8b950cb`  
		Last Modified: Wed, 01 Mar 2023 05:46:04 GMT  
		Size: 295.6 KB (295602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca762f444998d4bd3016122f9886d4e7c14da812ddbc7f7de8e575f4b2bae68`  
		Last Modified: Wed, 01 Mar 2023 05:46:35 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e71af86e7969357b8a270a9d615903fb9a2cc829c6371012bdd30c6b8651ea1`  
		Last Modified: Wed, 01 Mar 2023 05:46:43 GMT  
		Size: 50.1 MB (50086567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a98c3c152489f0d0fe21ceac6aa20723c329bb4301b0947aa29ee6f923a0e52`  
		Last Modified: Wed, 01 Mar 2023 05:46:34 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b42d18f1c4c133b6947441af70f66a78abd7ccadb1f7044e040252a24615781`  
		Last Modified: Wed, 01 Mar 2023 05:46:34 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fc695927445d03aad064debcfbc03a0347a572662d7710e2e5aab06ded9f1b`  
		Last Modified: Wed, 01 Mar 2023 05:46:34 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd64d5384a509a49a41e2a092f9ced334fba5563ff436cd3177217ce7d8fc3b2`  
		Last Modified: Wed, 01 Mar 2023 05:46:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.3`

```console
$ docker pull couchdb@sha256:77b6a90206ba433e59878efddc39a694500e2baf4684aadc6265f2b3d2e78b4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.3` - linux; amd64

```console
$ docker pull couchdb@sha256:dee3f17fa11aa1d43c0bd60c282d68b95f2cb0ea10582055a712be2c323cf481
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91168508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c023ab20b99cef1ccbfa589fb35f923d1048860f5f55217e69ba05e18e39631a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:56:29 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Mar 2023 04:56:29 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Mar 2023 04:56:37 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:56:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Mar 2023 04:56:41 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Mar 2023 04:56:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:56:46 GMT
ENV COUCHDB_VERSION=3.3.1
# Wed, 01 Mar 2023 04:56:47 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Mar 2023 04:57:00 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Mar 2023 04:57:00 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Mar 2023 04:57:00 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 01 Mar 2023 04:57:00 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 01 Mar 2023 04:57:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Mar 2023 04:57:01 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 04:57:01 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Mar 2023 04:57:01 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Mar 2023 04:57:01 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6637e7f130a96ee279b7cd93c77afc7a28fd7f831b19520de38e2b6b45ba2939`  
		Last Modified: Wed, 01 Mar 2023 04:58:49 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4dc9bd71357404364ed9c84296ea0170e4b13240b108fc598fcbc0400a3880`  
		Last Modified: Wed, 01 Mar 2023 04:58:48 GMT  
		Size: 5.2 MB (5224334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bde3e5409fa60225a360de6fc7cff74d8fdf8e3744088a5d03c3a9f8f22a12e`  
		Last Modified: Wed, 01 Mar 2023 04:58:48 GMT  
		Size: 1.6 MB (1553317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e818344b5f6306fba9c7fd2a9425930d01c149a178358a242bae48ac6fec38`  
		Last Modified: Wed, 01 Mar 2023 04:58:47 GMT  
		Size: 295.6 KB (295619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd0506641807b420c32835a9af376fe4810365cc6932f83148cf11374bf4bdd`  
		Last Modified: Wed, 01 Mar 2023 04:58:47 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6e0fd8fcee53fd180b1f321220a7b173c73c189d01741c93f21d83b664dcf1`  
		Last Modified: Wed, 01 Mar 2023 04:58:51 GMT  
		Size: 52.7 MB (52676453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f243172300bd45fa27ff12f5b283e411a5825f2ae436f9545f9c30fbdcf1031`  
		Last Modified: Wed, 01 Mar 2023 04:58:45 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdece4117c4fa382060db81e46bea365c1dc59ce1b4371caf5036535c9846134`  
		Last Modified: Wed, 01 Mar 2023 04:58:45 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e870857342e5e9d5e0441a5d7eefc223938f717850bb9228d9aa5840386ef4c`  
		Last Modified: Wed, 01 Mar 2023 04:58:45 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64097a0563ea7989e391d5759e050d96127903a994698b8d099486bad2502afb`  
		Last Modified: Wed, 01 Mar 2023 04:58:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:1e5ae5c1018aa7ffac0a966f0b93f626fe1c3ecd2eb74027df90f835fc44df03
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.5 MB (89542496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62c82e36049948ec0642106125f326a103110fa86398d11b0ef673476de21774`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 13:37:29 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 09 Feb 2023 13:37:29 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 09 Feb 2023 13:37:36 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 13:37:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 09 Feb 2023 13:37:38 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 09 Feb 2023 13:37:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 13:37:43 GMT
ENV COUCHDB_VERSION=3.3.1
# Thu, 09 Feb 2023 13:37:43 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 09 Feb 2023 13:37:55 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 09 Feb 2023 13:37:55 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 09 Feb 2023 13:37:55 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Thu, 09 Feb 2023 13:37:55 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Thu, 09 Feb 2023 13:37:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 09 Feb 2023 13:37:56 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 13:37:56 GMT
VOLUME [/opt/couchdb/data]
# Thu, 09 Feb 2023 13:37:56 GMT
EXPOSE 4369 5984 9100
# Thu, 09 Feb 2023 13:37:56 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6091f9f6c73b4b952be2bbc2cd89a8fc504064bf7483b83b7ea81f13fa4d54`  
		Last Modified: Thu, 09 Feb 2023 13:39:26 GMT  
		Size: 3.4 KB (3439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e00b3493fef81fb1cab07d097825491e38cb83abd318e8c4d1ee8c5b856710`  
		Last Modified: Thu, 09 Feb 2023 13:39:26 GMT  
		Size: 5.2 MB (5209406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0f2fc9cbc7001e7f9e0948436f0dd3a05468c357b0bee7bab813dec0619529`  
		Last Modified: Thu, 09 Feb 2023 13:39:25 GMT  
		Size: 1.4 MB (1435933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806951d526ba39c29e24fec1009ff647797fc0fab6abec6327d5cdb57cac82c8`  
		Last Modified: Thu, 09 Feb 2023 13:39:24 GMT  
		Size: 295.5 KB (295507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700f98b31af11297aaa7eb2cd0d795ff8b2741e8b5386b6b2af6ef7b9a0b1699`  
		Last Modified: Thu, 09 Feb 2023 13:39:24 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e964753acddc0f3887bebeeeb9d2f59a9c599626089435b5c304abaa33ace7a`  
		Last Modified: Thu, 09 Feb 2023 13:39:27 GMT  
		Size: 52.5 MB (52531739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3865d8e42284b4b7956e56adf6c7437adbb519a75369988c47ced075375078`  
		Last Modified: Thu, 09 Feb 2023 13:39:22 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa1ed4d8adeb2b889db515882b22a39b2a844eeaacaeb24b7a716274085e2db`  
		Last Modified: Thu, 09 Feb 2023 13:39:22 GMT  
		Size: 999.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42068c71f1e69e3289401c91c462dbbcd14fcb04a5a3f230bcec583dbde39a2`  
		Last Modified: Thu, 09 Feb 2023 13:39:23 GMT  
		Size: 2.2 KB (2188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b380f7228b5b2b7bd574dfac69b654e94c0a45880dbcde5d48db0e90ac1d8d`  
		Last Modified: Thu, 09 Feb 2023 13:39:22 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3` - linux; ppc64le

```console
$ docker pull couchdb@sha256:aa9693a4ea6a67e2d48c99e32ac51914c414b4332b30be1c9b2bd42c2a616074
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.7 MB (96679233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74ec5c87509de09ccb8fe5339cfd2c6265f9d69bd7aa889186ee6306ad81311c`
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
# Wed, 01 Mar 2023 05:43:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Mar 2023 05:43:59 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Mar 2023 05:44:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:44:16 GMT
ENV COUCHDB_VERSION=3.3.1
# Wed, 01 Mar 2023 05:44:17 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Mar 2023 05:44:48 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Mar 2023 05:44:51 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Mar 2023 05:44:51 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 01 Mar 2023 05:44:52 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 01 Mar 2023 05:44:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Mar 2023 05:44:55 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 05:44:56 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Mar 2023 05:44:57 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Mar 2023 05:44:58 GMT
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
	-	`sha256:cbef0173a07bc581e30e85a57b1e68802fcc0a024f244fa68c5b459d9c237577`  
		Last Modified: Wed, 01 Mar 2023 05:46:04 GMT  
		Size: 1.5 MB (1509253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553cf561c481aa0f831976d5481d1c2f5564fded0f487d629e780599b8b950cb`  
		Last Modified: Wed, 01 Mar 2023 05:46:04 GMT  
		Size: 295.6 KB (295602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57156270861ebec15e15824b98ce258087d77093da47aa2505c0f10323dbf576`  
		Last Modified: Wed, 01 Mar 2023 05:46:03 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170b2c08141c093d2a5f59fade4fed001a14775b4ae0553f26009520440c5074`  
		Last Modified: Wed, 01 Mar 2023 05:46:12 GMT  
		Size: 53.5 MB (53534942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0690b576b7faaf6377d377ccda31c9f40557af57ac472a66e767d1c2003508cf`  
		Last Modified: Wed, 01 Mar 2023 05:46:01 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05de86fd9c9910a4e1ed03a633ffd1f982abc032eddc6482211b9e52712fc457`  
		Last Modified: Wed, 01 Mar 2023 05:46:01 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:332b0bd48c4b5ddcdc504dd68272e7cffed2eeb6543dbf6c2766ee2190566153`  
		Last Modified: Wed, 01 Mar 2023 05:46:01 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3fbf8e1caf707e5e47d41e751e4316e5a73e5c95cbb2b8b717847eb2807b8e`  
		Last Modified: Wed, 01 Mar 2023 05:46:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.3.1`

```console
$ docker pull couchdb@sha256:77b6a90206ba433e59878efddc39a694500e2baf4684aadc6265f2b3d2e78b4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:3.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:dee3f17fa11aa1d43c0bd60c282d68b95f2cb0ea10582055a712be2c323cf481
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91168508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c023ab20b99cef1ccbfa589fb35f923d1048860f5f55217e69ba05e18e39631a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:56:29 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Mar 2023 04:56:29 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Mar 2023 04:56:37 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:56:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Mar 2023 04:56:41 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Mar 2023 04:56:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:56:46 GMT
ENV COUCHDB_VERSION=3.3.1
# Wed, 01 Mar 2023 04:56:47 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Mar 2023 04:57:00 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Mar 2023 04:57:00 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Mar 2023 04:57:00 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 01 Mar 2023 04:57:00 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 01 Mar 2023 04:57:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Mar 2023 04:57:01 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 04:57:01 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Mar 2023 04:57:01 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Mar 2023 04:57:01 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6637e7f130a96ee279b7cd93c77afc7a28fd7f831b19520de38e2b6b45ba2939`  
		Last Modified: Wed, 01 Mar 2023 04:58:49 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4dc9bd71357404364ed9c84296ea0170e4b13240b108fc598fcbc0400a3880`  
		Last Modified: Wed, 01 Mar 2023 04:58:48 GMT  
		Size: 5.2 MB (5224334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bde3e5409fa60225a360de6fc7cff74d8fdf8e3744088a5d03c3a9f8f22a12e`  
		Last Modified: Wed, 01 Mar 2023 04:58:48 GMT  
		Size: 1.6 MB (1553317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e818344b5f6306fba9c7fd2a9425930d01c149a178358a242bae48ac6fec38`  
		Last Modified: Wed, 01 Mar 2023 04:58:47 GMT  
		Size: 295.6 KB (295619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd0506641807b420c32835a9af376fe4810365cc6932f83148cf11374bf4bdd`  
		Last Modified: Wed, 01 Mar 2023 04:58:47 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6e0fd8fcee53fd180b1f321220a7b173c73c189d01741c93f21d83b664dcf1`  
		Last Modified: Wed, 01 Mar 2023 04:58:51 GMT  
		Size: 52.7 MB (52676453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f243172300bd45fa27ff12f5b283e411a5825f2ae436f9545f9c30fbdcf1031`  
		Last Modified: Wed, 01 Mar 2023 04:58:45 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdece4117c4fa382060db81e46bea365c1dc59ce1b4371caf5036535c9846134`  
		Last Modified: Wed, 01 Mar 2023 04:58:45 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e870857342e5e9d5e0441a5d7eefc223938f717850bb9228d9aa5840386ef4c`  
		Last Modified: Wed, 01 Mar 2023 04:58:45 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64097a0563ea7989e391d5759e050d96127903a994698b8d099486bad2502afb`  
		Last Modified: Wed, 01 Mar 2023 04:58:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:1e5ae5c1018aa7ffac0a966f0b93f626fe1c3ecd2eb74027df90f835fc44df03
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.5 MB (89542496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62c82e36049948ec0642106125f326a103110fa86398d11b0ef673476de21774`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 13:37:29 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 09 Feb 2023 13:37:29 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 09 Feb 2023 13:37:36 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 13:37:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 09 Feb 2023 13:37:38 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 09 Feb 2023 13:37:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 13:37:43 GMT
ENV COUCHDB_VERSION=3.3.1
# Thu, 09 Feb 2023 13:37:43 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 09 Feb 2023 13:37:55 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 09 Feb 2023 13:37:55 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 09 Feb 2023 13:37:55 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Thu, 09 Feb 2023 13:37:55 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Thu, 09 Feb 2023 13:37:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 09 Feb 2023 13:37:56 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 13:37:56 GMT
VOLUME [/opt/couchdb/data]
# Thu, 09 Feb 2023 13:37:56 GMT
EXPOSE 4369 5984 9100
# Thu, 09 Feb 2023 13:37:56 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6091f9f6c73b4b952be2bbc2cd89a8fc504064bf7483b83b7ea81f13fa4d54`  
		Last Modified: Thu, 09 Feb 2023 13:39:26 GMT  
		Size: 3.4 KB (3439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e00b3493fef81fb1cab07d097825491e38cb83abd318e8c4d1ee8c5b856710`  
		Last Modified: Thu, 09 Feb 2023 13:39:26 GMT  
		Size: 5.2 MB (5209406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0f2fc9cbc7001e7f9e0948436f0dd3a05468c357b0bee7bab813dec0619529`  
		Last Modified: Thu, 09 Feb 2023 13:39:25 GMT  
		Size: 1.4 MB (1435933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806951d526ba39c29e24fec1009ff647797fc0fab6abec6327d5cdb57cac82c8`  
		Last Modified: Thu, 09 Feb 2023 13:39:24 GMT  
		Size: 295.5 KB (295507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700f98b31af11297aaa7eb2cd0d795ff8b2741e8b5386b6b2af6ef7b9a0b1699`  
		Last Modified: Thu, 09 Feb 2023 13:39:24 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e964753acddc0f3887bebeeeb9d2f59a9c599626089435b5c304abaa33ace7a`  
		Last Modified: Thu, 09 Feb 2023 13:39:27 GMT  
		Size: 52.5 MB (52531739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3865d8e42284b4b7956e56adf6c7437adbb519a75369988c47ced075375078`  
		Last Modified: Thu, 09 Feb 2023 13:39:22 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa1ed4d8adeb2b889db515882b22a39b2a844eeaacaeb24b7a716274085e2db`  
		Last Modified: Thu, 09 Feb 2023 13:39:22 GMT  
		Size: 999.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42068c71f1e69e3289401c91c462dbbcd14fcb04a5a3f230bcec583dbde39a2`  
		Last Modified: Thu, 09 Feb 2023 13:39:23 GMT  
		Size: 2.2 KB (2188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b380f7228b5b2b7bd574dfac69b654e94c0a45880dbcde5d48db0e90ac1d8d`  
		Last Modified: Thu, 09 Feb 2023 13:39:22 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.3.1` - linux; ppc64le

```console
$ docker pull couchdb@sha256:aa9693a4ea6a67e2d48c99e32ac51914c414b4332b30be1c9b2bd42c2a616074
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.7 MB (96679233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74ec5c87509de09ccb8fe5339cfd2c6265f9d69bd7aa889186ee6306ad81311c`
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
# Wed, 01 Mar 2023 05:43:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Mar 2023 05:43:59 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Mar 2023 05:44:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:44:16 GMT
ENV COUCHDB_VERSION=3.3.1
# Wed, 01 Mar 2023 05:44:17 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Mar 2023 05:44:48 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Mar 2023 05:44:51 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Mar 2023 05:44:51 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 01 Mar 2023 05:44:52 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 01 Mar 2023 05:44:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Mar 2023 05:44:55 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 05:44:56 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Mar 2023 05:44:57 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Mar 2023 05:44:58 GMT
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
	-	`sha256:cbef0173a07bc581e30e85a57b1e68802fcc0a024f244fa68c5b459d9c237577`  
		Last Modified: Wed, 01 Mar 2023 05:46:04 GMT  
		Size: 1.5 MB (1509253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553cf561c481aa0f831976d5481d1c2f5564fded0f487d629e780599b8b950cb`  
		Last Modified: Wed, 01 Mar 2023 05:46:04 GMT  
		Size: 295.6 KB (295602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57156270861ebec15e15824b98ce258087d77093da47aa2505c0f10323dbf576`  
		Last Modified: Wed, 01 Mar 2023 05:46:03 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170b2c08141c093d2a5f59fade4fed001a14775b4ae0553f26009520440c5074`  
		Last Modified: Wed, 01 Mar 2023 05:46:12 GMT  
		Size: 53.5 MB (53534942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0690b576b7faaf6377d377ccda31c9f40557af57ac472a66e767d1c2003508cf`  
		Last Modified: Wed, 01 Mar 2023 05:46:01 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05de86fd9c9910a4e1ed03a633ffd1f982abc032eddc6482211b9e52712fc457`  
		Last Modified: Wed, 01 Mar 2023 05:46:01 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:332b0bd48c4b5ddcdc504dd68272e7cffed2eeb6543dbf6c2766ee2190566153`  
		Last Modified: Wed, 01 Mar 2023 05:46:01 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3fbf8e1caf707e5e47d41e751e4316e5a73e5c95cbb2b8b717847eb2807b8e`  
		Last Modified: Wed, 01 Mar 2023 05:46:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:latest`

```console
$ docker pull couchdb@sha256:77b6a90206ba433e59878efddc39a694500e2baf4684aadc6265f2b3d2e78b4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; ppc64le

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:dee3f17fa11aa1d43c0bd60c282d68b95f2cb0ea10582055a712be2c323cf481
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91168508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c023ab20b99cef1ccbfa589fb35f923d1048860f5f55217e69ba05e18e39631a`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:56:29 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 01 Mar 2023 04:56:29 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 01 Mar 2023 04:56:37 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:56:40 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Mar 2023 04:56:41 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Mar 2023 04:56:46 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:56:46 GMT
ENV COUCHDB_VERSION=3.3.1
# Wed, 01 Mar 2023 04:56:47 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Mar 2023 04:57:00 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Mar 2023 04:57:00 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Mar 2023 04:57:00 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 01 Mar 2023 04:57:00 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 01 Mar 2023 04:57:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Mar 2023 04:57:01 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 04:57:01 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Mar 2023 04:57:01 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Mar 2023 04:57:01 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6637e7f130a96ee279b7cd93c77afc7a28fd7f831b19520de38e2b6b45ba2939`  
		Last Modified: Wed, 01 Mar 2023 04:58:49 GMT  
		Size: 3.4 KB (3412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4dc9bd71357404364ed9c84296ea0170e4b13240b108fc598fcbc0400a3880`  
		Last Modified: Wed, 01 Mar 2023 04:58:48 GMT  
		Size: 5.2 MB (5224334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bde3e5409fa60225a360de6fc7cff74d8fdf8e3744088a5d03c3a9f8f22a12e`  
		Last Modified: Wed, 01 Mar 2023 04:58:48 GMT  
		Size: 1.6 MB (1553317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e818344b5f6306fba9c7fd2a9425930d01c149a178358a242bae48ac6fec38`  
		Last Modified: Wed, 01 Mar 2023 04:58:47 GMT  
		Size: 295.6 KB (295619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd0506641807b420c32835a9af376fe4810365cc6932f83148cf11374bf4bdd`  
		Last Modified: Wed, 01 Mar 2023 04:58:47 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6e0fd8fcee53fd180b1f321220a7b173c73c189d01741c93f21d83b664dcf1`  
		Last Modified: Wed, 01 Mar 2023 04:58:51 GMT  
		Size: 52.7 MB (52676453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f243172300bd45fa27ff12f5b283e411a5825f2ae436f9545f9c30fbdcf1031`  
		Last Modified: Wed, 01 Mar 2023 04:58:45 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdece4117c4fa382060db81e46bea365c1dc59ce1b4371caf5036535c9846134`  
		Last Modified: Wed, 01 Mar 2023 04:58:45 GMT  
		Size: 1.0 KB (1001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e870857342e5e9d5e0441a5d7eefc223938f717850bb9228d9aa5840386ef4c`  
		Last Modified: Wed, 01 Mar 2023 04:58:45 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64097a0563ea7989e391d5759e050d96127903a994698b8d099486bad2502afb`  
		Last Modified: Wed, 01 Mar 2023 04:58:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:1e5ae5c1018aa7ffac0a966f0b93f626fe1c3ecd2eb74027df90f835fc44df03
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.5 MB (89542496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62c82e36049948ec0642106125f326a103110fa86398d11b0ef673476de21774`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 13:37:29 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Thu, 09 Feb 2023 13:37:29 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Thu, 09 Feb 2023 13:37:36 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 13:37:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 09 Feb 2023 13:37:38 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 09 Feb 2023 13:37:43 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 13:37:43 GMT
ENV COUCHDB_VERSION=3.3.1
# Thu, 09 Feb 2023 13:37:43 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 09 Feb 2023 13:37:55 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 09 Feb 2023 13:37:55 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 09 Feb 2023 13:37:55 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Thu, 09 Feb 2023 13:37:55 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Thu, 09 Feb 2023 13:37:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 09 Feb 2023 13:37:56 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 09 Feb 2023 13:37:56 GMT
VOLUME [/opt/couchdb/data]
# Thu, 09 Feb 2023 13:37:56 GMT
EXPOSE 4369 5984 9100
# Thu, 09 Feb 2023 13:37:56 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6091f9f6c73b4b952be2bbc2cd89a8fc504064bf7483b83b7ea81f13fa4d54`  
		Last Modified: Thu, 09 Feb 2023 13:39:26 GMT  
		Size: 3.4 KB (3439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e00b3493fef81fb1cab07d097825491e38cb83abd318e8c4d1ee8c5b856710`  
		Last Modified: Thu, 09 Feb 2023 13:39:26 GMT  
		Size: 5.2 MB (5209406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0f2fc9cbc7001e7f9e0948436f0dd3a05468c357b0bee7bab813dec0619529`  
		Last Modified: Thu, 09 Feb 2023 13:39:25 GMT  
		Size: 1.4 MB (1435933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806951d526ba39c29e24fec1009ff647797fc0fab6abec6327d5cdb57cac82c8`  
		Last Modified: Thu, 09 Feb 2023 13:39:24 GMT  
		Size: 295.5 KB (295507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700f98b31af11297aaa7eb2cd0d795ff8b2741e8b5386b6b2af6ef7b9a0b1699`  
		Last Modified: Thu, 09 Feb 2023 13:39:24 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e964753acddc0f3887bebeeeb9d2f59a9c599626089435b5c304abaa33ace7a`  
		Last Modified: Thu, 09 Feb 2023 13:39:27 GMT  
		Size: 52.5 MB (52531739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3865d8e42284b4b7956e56adf6c7437adbb519a75369988c47ced075375078`  
		Last Modified: Thu, 09 Feb 2023 13:39:22 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa1ed4d8adeb2b889db515882b22a39b2a844eeaacaeb24b7a716274085e2db`  
		Last Modified: Thu, 09 Feb 2023 13:39:22 GMT  
		Size: 999.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42068c71f1e69e3289401c91c462dbbcd14fcb04a5a3f230bcec583dbde39a2`  
		Last Modified: Thu, 09 Feb 2023 13:39:23 GMT  
		Size: 2.2 KB (2188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b380f7228b5b2b7bd574dfac69b654e94c0a45880dbcde5d48db0e90ac1d8d`  
		Last Modified: Thu, 09 Feb 2023 13:39:22 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; ppc64le

```console
$ docker pull couchdb@sha256:aa9693a4ea6a67e2d48c99e32ac51914c414b4332b30be1c9b2bd42c2a616074
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.7 MB (96679233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74ec5c87509de09ccb8fe5339cfd2c6265f9d69bd7aa889186ee6306ad81311c`
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
# Wed, 01 Mar 2023 05:43:58 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 01 Mar 2023 05:43:59 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 01 Mar 2023 05:44:15 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 05:44:16 GMT
ENV COUCHDB_VERSION=3.3.1
# Wed, 01 Mar 2023 05:44:17 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 01 Mar 2023 05:44:48 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~bullseye     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 01 Mar 2023 05:44:51 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 01 Mar 2023 05:44:51 GMT
COPY --chown=couchdb:couchdbfile:ef998123ee941cb75b9e8f8c244fd9e244aff7d6394013d8db7515f50882f0cd in /opt/couchdb/etc/ 
# Wed, 01 Mar 2023 05:44:52 GMT
COPY file:0a26a859e55e89f8409b5ab4022d28cfe05edddfe16a742ba28c73ecdbcff9c1 in /usr/local/bin 
# Wed, 01 Mar 2023 05:44:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 01 Mar 2023 05:44:55 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 01 Mar 2023 05:44:56 GMT
VOLUME [/opt/couchdb/data]
# Wed, 01 Mar 2023 05:44:57 GMT
EXPOSE 4369 5984 9100
# Wed, 01 Mar 2023 05:44:58 GMT
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
	-	`sha256:cbef0173a07bc581e30e85a57b1e68802fcc0a024f244fa68c5b459d9c237577`  
		Last Modified: Wed, 01 Mar 2023 05:46:04 GMT  
		Size: 1.5 MB (1509253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553cf561c481aa0f831976d5481d1c2f5564fded0f487d629e780599b8b950cb`  
		Last Modified: Wed, 01 Mar 2023 05:46:04 GMT  
		Size: 295.6 KB (295602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57156270861ebec15e15824b98ce258087d77093da47aa2505c0f10323dbf576`  
		Last Modified: Wed, 01 Mar 2023 05:46:03 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170b2c08141c093d2a5f59fade4fed001a14775b4ae0553f26009520440c5074`  
		Last Modified: Wed, 01 Mar 2023 05:46:12 GMT  
		Size: 53.5 MB (53534942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0690b576b7faaf6377d377ccda31c9f40557af57ac472a66e767d1c2003508cf`  
		Last Modified: Wed, 01 Mar 2023 05:46:01 GMT  
		Size: 383.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05de86fd9c9910a4e1ed03a633ffd1f982abc032eddc6482211b9e52712fc457`  
		Last Modified: Wed, 01 Mar 2023 05:46:01 GMT  
		Size: 1000.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:332b0bd48c4b5ddcdc504dd68272e7cffed2eeb6543dbf6c2766ee2190566153`  
		Last Modified: Wed, 01 Mar 2023 05:46:01 GMT  
		Size: 2.2 KB (2186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3fbf8e1caf707e5e47d41e751e4316e5a73e5c95cbb2b8b717847eb2807b8e`  
		Last Modified: Wed, 01 Mar 2023 05:46:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
