## `couchdb:latest`

```console
$ docker pull couchdb@sha256:721df2c2a5da1b477e3976f3f10c3d1f015ba3c0101fb49efdcb7062b695a32c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:658ef40b47f068cdbc8e8a069d18e72df1a37c38f26890e7e2543decc24246fe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.6 MB (80555365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ac41a5539f547e479507d3cefa4a9b2a7250cbf6fd0660fbeedd8fee65f9234`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:09:14 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Dec 2021 02:09:14 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Dec 2021 02:09:22 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:09:27 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 21 Dec 2021 02:09:27 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Dec 2021 02:09:33 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:09:33 GMT
ENV COUCHDB_VERSION=3.2.0
# Tue, 21 Dec 2021 02:09:34 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Dec 2021 02:09:48 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Dec 2021 02:09:49 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Dec 2021 02:09:49 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 21 Dec 2021 02:09:49 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 21 Dec 2021 02:09:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Dec 2021 02:09:50 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Dec 2021 02:09:51 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Dec 2021 02:09:51 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Dec 2021 02:09:51 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430d6c754b31c32dd1a76de01ad3420033c05661c724b97d708362a8ec139d42`  
		Last Modified: Tue, 21 Dec 2021 02:10:58 GMT  
		Size: 3.4 KB (3413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3227820103030b5232e32ba7e76de56823a61d47245d450403c0040933f6aebd`  
		Last Modified: Tue, 21 Dec 2021 02:10:58 GMT  
		Size: 6.7 MB (6691223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454611cf9dafef09164a7f64cb967a12ab5d1549d70599c56b74a2c283ae8ef1`  
		Last Modified: Tue, 21 Dec 2021 02:10:56 GMT  
		Size: 1.3 MB (1258346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5993063a8d6d688f066b9d8208c98f7d0dd3d78e7076cbc7a132ab98a975dece`  
		Last Modified: Tue, 21 Dec 2021 02:10:56 GMT  
		Size: 293.0 KB (293029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e1a5cbb187a2701cb1f4f219e175d4903fc4ef19eecfbafaa89efecfe9f350`  
		Last Modified: Tue, 21 Dec 2021 02:10:56 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf5b3b5a34ef74b2afa7c1ab7adc5957d6def0d5cb372796cadbc953023f76e`  
		Last Modified: Tue, 21 Dec 2021 02:10:59 GMT  
		Size: 45.2 MB (45152027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67b48a446b521e34ad7bbbb9989e634a2a7e726f24df622bc933d81cf8c45a7`  
		Last Modified: Tue, 21 Dec 2021 02:10:54 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd626acdd610cc57988f501ff79961f1428c576461bebd4231e6ea26986e247c`  
		Last Modified: Tue, 21 Dec 2021 02:10:54 GMT  
		Size: 763.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c823a8f47edfaf32b423082634aea86cdb7addaf551842be131974000268d72f`  
		Last Modified: Tue, 21 Dec 2021 02:10:54 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920494c25accb2e7113ebc8561d68c1b875ce9ea97b254e7f0b1859d0c42fb85`  
		Last Modified: Tue, 21 Dec 2021 02:10:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:869f47e225975cb48c3eb1031664774c529080c0d6f9a71f3fcb404a698d4a6d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.2 MB (75231146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80c4d8555edeeddd256bfc90afd27fe69187e5be6505a8bfb08ea1bbe088a957`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:48 GMT
ADD file:9810440ab841e71bd153282c21cfcd46d3f40bd5099e60c332e05bf066e390ac in / 
# Tue, 21 Dec 2021 01:42:49 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:44:40 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Tue, 21 Dec 2021 10:44:41 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Tue, 21 Dec 2021 10:44:49 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:44:53 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Tue, 21 Dec 2021 10:44:54 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Tue, 21 Dec 2021 10:45:01 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:45:02 GMT
ENV COUCHDB_VERSION=3.2.0
# Tue, 21 Dec 2021 10:45:03 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Tue, 21 Dec 2021 10:45:21 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Tue, 21 Dec 2021 10:45:22 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Tue, 21 Dec 2021 10:45:23 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Tue, 21 Dec 2021 10:45:24 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Tue, 21 Dec 2021 10:45:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Tue, 21 Dec 2021 10:45:25 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Tue, 21 Dec 2021 10:45:26 GMT
VOLUME [/opt/couchdb/data]
# Tue, 21 Dec 2021 10:45:27 GMT
EXPOSE 4369 5984 9100
# Tue, 21 Dec 2021 10:45:28 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:753408153c81560bc4244b14524c404cbf483c8afa8ac924272545400536a9d8`  
		Last Modified: Tue, 21 Dec 2021 01:49:44 GMT  
		Size: 25.9 MB (25923149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589f1cb358d3e3a123049341ce44cdc00d6c6484a66c1169425711e3d4e5ef61`  
		Last Modified: Tue, 21 Dec 2021 10:47:20 GMT  
		Size: 3.3 KB (3322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519ca2948856ed69aa492a4294b0510bcc03616eceac737dd2fe13ddbdad889d`  
		Last Modified: Tue, 21 Dec 2021 10:47:19 GMT  
		Size: 6.5 MB (6549891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d41232c99e6d3b4632a28126c15a9405dac5ec12ef1c3e71b47f7e455ed8bef7`  
		Last Modified: Tue, 21 Dec 2021 10:47:18 GMT  
		Size: 951.2 KB (951161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8413befe0746257456c09468b422890a186a8cf1a2868f008b8d56de24a7d815`  
		Last Modified: Tue, 21 Dec 2021 10:47:18 GMT  
		Size: 79.9 KB (79896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881e0db5b966260ec8900a1ed3580e995a95c4dc5080c6211050dfc9860f3d1c`  
		Last Modified: Tue, 21 Dec 2021 10:47:17 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025e09f93807f170da42d5be112a4f23ef5ac902b0beaa78c11c915805f0b1a9`  
		Last Modified: Tue, 21 Dec 2021 10:47:20 GMT  
		Size: 41.7 MB (41720123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde0b26399669e31d67674d81e379abf8ef313266494a9d475260b6a335625f3`  
		Last Modified: Tue, 21 Dec 2021 10:47:15 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402ec3e16c1dc98710c921b298b4ca7ca394a2dc0ca520cdd1c43ff281cc4957`  
		Last Modified: Tue, 21 Dec 2021 10:47:15 GMT  
		Size: 767.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc3cb611309b8ca0f28d85184acf44654e779f0bdddbc37dad0c41ad52adf34`  
		Last Modified: Tue, 21 Dec 2021 10:47:16 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3fdf7e2f3ce2dfd9e73da1db5bc4e20a67e2b21d05258e4ef11b690129988fa`  
		Last Modified: Tue, 21 Dec 2021 10:47:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
