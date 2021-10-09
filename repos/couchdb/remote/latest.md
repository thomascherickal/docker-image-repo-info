## `couchdb:latest`

```console
$ docker pull couchdb@sha256:e8df47d19b8fadefa959798510d888334a330e13d335d02b10718e8e0c64bc50
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:c1522166bbdb8e0d7b8887b05707a209d12ca70aa5abf09b2eae6416c544823b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.5 MB (80548099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be7c310b6320e9ad3028b724afc20d824fc746d8d413fae292ed6ac94159ab86`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 28 Sep 2021 01:23:09 GMT
ADD file:99db7cfe7952a1c7a7959cc3457af37c1d6facdd43a946bd72313d8b5ede0029 in / 
# Tue, 28 Sep 2021 01:23:10 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:07:35 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 28 Sep 2021 02:07:35 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 28 Sep 2021 02:07:43 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:07:47 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 28 Sep 2021 02:07:47 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 28 Sep 2021 02:07:54 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Sat, 09 Oct 2021 00:19:20 GMT
ENV COUCHDB_VERSION=3.2.0
# Sat, 09 Oct 2021 00:19:20 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Sat, 09 Oct 2021 00:19:34 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Sat, 09 Oct 2021 00:19:34 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Sat, 09 Oct 2021 00:19:35 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Sat, 09 Oct 2021 00:19:35 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Sat, 09 Oct 2021 00:19:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Sat, 09 Oct 2021 00:19:36 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Sat, 09 Oct 2021 00:19:36 GMT
VOLUME [/opt/couchdb/data]
# Sat, 09 Oct 2021 00:19:36 GMT
EXPOSE 4369 5984 9100
# Sat, 09 Oct 2021 00:19:36 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:07aded7c29c6011dfdf02fc98e087c941d3c2661c4e73d134c6491e25231d16c`  
		Last Modified: Tue, 28 Sep 2021 01:29:45 GMT  
		Size: 27.1 MB (27145994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf6d2572e5cb46cd161abd1cad4bfe814861bb79af678e8c8878bfceea39800`  
		Last Modified: Tue, 28 Sep 2021 02:08:58 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c07788136736f89aa055ecaf94d8a84930476f22f9743523ea520a89676871`  
		Last Modified: Tue, 28 Sep 2021 02:08:57 GMT  
		Size: 6.7 MB (6691239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f38611f22a1bf97d622c97f121883635774e7c90a58b732ea6ac173481ed5f`  
		Last Modified: Tue, 28 Sep 2021 02:08:56 GMT  
		Size: 1.3 MB (1258340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b7085d2ce04f2475efd91088b35d5999a9d08265c4b69ff48f3756f569dfc0`  
		Last Modified: Tue, 28 Sep 2021 02:08:56 GMT  
		Size: 293.0 KB (292984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe8c3f84d1ff35f076c03a4720f66d9e64df26c18df7b687e83858a3a4f5e5c`  
		Last Modified: Sat, 09 Oct 2021 00:19:58 GMT  
		Size: 274.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:859414b864a1964e98aca1a872fc1798e261bb42229748668f0856b4403acc7e`  
		Last Modified: Sat, 09 Oct 2021 00:20:01 GMT  
		Size: 45.2 MB (45152529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120839791efe40b609a2f9f617baddf03deab16ef81e7a6c8cbe69b29ba50971`  
		Last Modified: Sat, 09 Oct 2021 00:19:56 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b576c5a18ed3e62d68e58204b0610f2a8beebf0136df15d9dec0bc6ff9bdb35c`  
		Last Modified: Sat, 09 Oct 2021 00:19:56 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55e4c816bda584f02da024703e44fdf5db4e9a7a7d963780f389edf03cb199d`  
		Last Modified: Sat, 09 Oct 2021 00:19:56 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb79b8811c23ac5dc30f9ccf5500dd034853f0dc07b927315e7517a5253f722`  
		Last Modified: Sat, 09 Oct 2021 00:19:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:a6500b9a69dd7649d736440910d269f6c44b82381b65975d25ee107fb65bab5c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75649500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74ae92e937268d84ab86d7800081ab4e3aef19c02e8aab0cac503efe8a3811b5`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 28 Sep 2021 01:41:13 GMT
ADD file:3e2426765cfe2b896fc847bcb435624930753c72ac00b87d2c73f4a81c813fd4 in / 
# Tue, 28 Sep 2021 01:41:13 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 02:13:20 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 28 Sep 2021 02:13:21 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 28 Sep 2021 02:13:28 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 02:13:32 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 28 Sep 2021 02:13:32 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 28 Sep 2021 02:13:38 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Fri, 08 Oct 2021 23:39:23 GMT
ENV COUCHDB_VERSION=3.2.0
# Fri, 08 Oct 2021 23:39:24 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Fri, 08 Oct 2021 23:39:37 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Fri, 08 Oct 2021 23:39:37 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Fri, 08 Oct 2021 23:39:37 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Fri, 08 Oct 2021 23:39:37 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Fri, 08 Oct 2021 23:39:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Fri, 08 Oct 2021 23:39:38 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Fri, 08 Oct 2021 23:39:38 GMT
VOLUME [/opt/couchdb/data]
# Fri, 08 Oct 2021 23:39:39 GMT
EXPOSE 4369 5984 9100
# Fri, 08 Oct 2021 23:39:39 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:896f18f54b28590b15a0f3354b13e8ea2f88a05f13de4117720f88cef30206ee`  
		Last Modified: Tue, 28 Sep 2021 01:49:22 GMT  
		Size: 25.9 MB (25915039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccce50a09ce93b18af732f0cccc8bc50f337920af8abdceb6899462acf0d0f1`  
		Last Modified: Tue, 28 Sep 2021 02:14:49 GMT  
		Size: 3.4 KB (3430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cfe94af3886b0bb198cc647f566a4d700267dd1162f81fd578bd8218a898c01`  
		Last Modified: Tue, 28 Sep 2021 02:14:48 GMT  
		Size: 6.6 MB (6550861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9c0e24b6130ef05d86938e8f18a781c86cbd4b340809dfe0253927c98f2ee4`  
		Last Modified: Tue, 28 Sep 2021 02:14:47 GMT  
		Size: 1.2 MB (1163444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64a60e19b9cb05869c7102040626818240c5cf125ed25c9237bd8b7a36547a6`  
		Last Modified: Tue, 28 Sep 2021 02:14:46 GMT  
		Size: 292.8 KB (292825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548288e8f973bece9d8cf1f3e7cb603dfb20101fc3e89cc3d45d6fcd44f88e9b`  
		Last Modified: Fri, 08 Oct 2021 23:40:16 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc78b96a773b05f4fa42b178b6768370880b5c8b573929a6ad4790a5864d6135`  
		Last Modified: Fri, 08 Oct 2021 23:40:20 GMT  
		Size: 41.7 MB (41720301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce3efd2f4358be175d41ec4a71b2f89f0456b2ad94308d78a74e9fdbd5b96a1e`  
		Last Modified: Fri, 08 Oct 2021 23:40:14 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1e000d414b41f1540610350026b49645f3feb786be6710f97947e12a31509d`  
		Last Modified: Fri, 08 Oct 2021 23:40:15 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcdc6c77c3660993e9d8e1f96ddeaea7479a0eb925942abdf115849fce89ebc8`  
		Last Modified: Fri, 08 Oct 2021 23:40:14 GMT  
		Size: 2.1 KB (2060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285c88dfdc22e30a79414c8eba0487288ad68dce6a23cd00e8996f67439480fd`  
		Last Modified: Fri, 08 Oct 2021 23:40:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
