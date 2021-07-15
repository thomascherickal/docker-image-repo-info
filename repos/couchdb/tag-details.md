<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `couchdb`

-	[`couchdb:2`](#couchdb2)
-	[`couchdb:2.3`](#couchdb23)
-	[`couchdb:2.3.1`](#couchdb231)
-	[`couchdb:3`](#couchdb3)
-	[`couchdb:3.1`](#couchdb31)
-	[`couchdb:3.1.1`](#couchdb311)
-	[`couchdb:latest`](#couchdblatest)

## `couchdb:2`

```console
$ docker pull couchdb@sha256:5f38ddf66f8965dd54109bc5d7cd66a6b2fedf6c6550ea606d28e77bdcb24a5b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2` - linux; amd64

```console
$ docker pull couchdb@sha256:7915f17c6eef82a1318d7be9b2a1164ea7e809b3946fe3eacce5e746adc6c9ad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84508798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49e61de30c53d2c41bf71105914825ed5c180d0c936b21dc6acc834073be9643`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:51:13 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 23 Jun 2021 05:51:15 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 23 Jun 2021 05:51:26 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 07 Jul 2021 23:19:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 07 Jul 2021 23:19:41 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 07 Jul 2021 23:19:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 07 Jul 2021 23:20:12 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 07 Jul 2021 23:20:13 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 07 Jul 2021 23:20:31 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 07 Jul 2021 23:20:32 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 07 Jul 2021 23:20:32 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 07 Jul 2021 23:20:33 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 07 Jul 2021 23:20:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 07 Jul 2021 23:20:34 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 07 Jul 2021 23:20:34 GMT
VOLUME [/opt/couchdb/data]
# Wed, 07 Jul 2021 23:20:34 GMT
EXPOSE 4369 5984 9100
# Wed, 07 Jul 2021 23:20:35 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56acda79979ecba61f07d80188fac6ac183186a686d5f95008434ec065f41fa`  
		Last Modified: Wed, 23 Jun 2021 05:57:01 GMT  
		Size: 3.4 KB (3417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dae9ebd0dd45384cfce6054637761697cc472c88ecf98d3b65ebb821582ed6c`  
		Last Modified: Wed, 23 Jun 2021 05:57:00 GMT  
		Size: 6.7 MB (6690646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5d42f37b9396588987617303dc24662fb0e1f43459f5b4e2b05e069cd69d40`  
		Last Modified: Wed, 07 Jul 2021 23:20:52 GMT  
		Size: 1.3 MB (1258367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980f06759da554159a56f68854a642196e3db0300281f142d17c4d10be0a0881`  
		Last Modified: Wed, 07 Jul 2021 23:20:52 GMT  
		Size: 293.0 KB (293008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1543d07e7709248446a176c8cdab37c46584afb092578ad1034bbdbacbd87cf5`  
		Last Modified: Wed, 07 Jul 2021 23:21:15 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057931a446afd67aba58b7ced44de72b2bbb4d89da8b5ed36239366ec0d3c312`  
		Last Modified: Wed, 07 Jul 2021 23:21:19 GMT  
		Size: 49.1 MB (49113897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36814e6f1d7df65a0652520403064364757bf64c11875a8a8f5bbcddb29eac5`  
		Last Modified: Wed, 07 Jul 2021 23:21:13 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a077feefb03f8e9a3d53fb3cab8cf4c2130610f2b14c651b6ecab22b52fc1c`  
		Last Modified: Wed, 07 Jul 2021 23:21:13 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154f17865ac577c94ab20ba6a1d069e8358c737b35c901986668e9766111f173`  
		Last Modified: Wed, 07 Jul 2021 23:21:14 GMT  
		Size: 2.1 KB (2061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6542f38ef9fe4406e7dc448a70ba4f4a2439f4c1a2045fda001de0dca1d407d`  
		Last Modified: Wed, 07 Jul 2021 23:21:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:e0d961b53c2954b9b06b0f8b65abd7909c47e32604263dfeb165b1fb7845fd12
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72941386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5d8afbe45a9a4db6168d660ea5c4816e78c95b1c88d6d4a96b3ded9f63ad846`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:18:07 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 23 Jun 2021 00:18:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 23 Jun 2021 00:18:15 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 01:05:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 08 Jul 2021 01:05:23 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 08 Jul 2021 01:05:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 01:05:55 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Thu, 08 Jul 2021 01:05:56 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 08 Jul 2021 01:06:09 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 08 Jul 2021 01:06:09 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Thu, 08 Jul 2021 01:06:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 08 Jul 2021 01:06:10 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Thu, 08 Jul 2021 01:06:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 08 Jul 2021 01:06:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 01:06:11 GMT
VOLUME [/opt/couchdb/data]
# Thu, 08 Jul 2021 01:06:12 GMT
EXPOSE 4369 5984 9100
# Thu, 08 Jul 2021 01:06:12 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:339ec36e3b140be1528e45b20e2377aac8adcf3fe37d032e6eb9ee4dad84b53b`  
		Last Modified: Wed, 23 Jun 2021 00:21:32 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e09e9e959b7859e40642c2da7ea73345d2adba18d781d6d4bba0e3c9a4fcd4`  
		Last Modified: Wed, 23 Jun 2021 00:21:31 GMT  
		Size: 6.6 MB (6550152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cae01982b2316cf8b0c31b05b2a9f35981ea5e6e5a0b27cb387d8ca466901e9`  
		Last Modified: Thu, 08 Jul 2021 01:06:40 GMT  
		Size: 1.2 MB (1163469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ca64335472f92842e639e6af3b3b73fce01075ebffeaad8b0db79c2b410b30`  
		Last Modified: Thu, 08 Jul 2021 01:06:40 GMT  
		Size: 292.9 KB (292882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:545112f24e032933f069ae6781b25f9a262e7024dbd91722ec3146e02801b0c1`  
		Last Modified: Thu, 08 Jul 2021 01:07:07 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75747d3f6ce9eb71caaf609c78983eb73b6fcc38f05c869554458971d8f84fa3`  
		Last Modified: Thu, 08 Jul 2021 01:07:10 GMT  
		Size: 39.0 MB (39012845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a058f637ac6b0bb7a63a3d06a1ffeb479132e3805bf1d847f8fe06ab2da62d7a`  
		Last Modified: Thu, 08 Jul 2021 01:07:05 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13c76be4357c902544032954ca18b8dd15cf5a1c629ccf2d40fa0b4f0fd8a7e`  
		Last Modified: Thu, 08 Jul 2021 01:07:05 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b9de3a880ce25c24fbbcb1b8c37eb616781c5f94522677f552c5e8ac142718`  
		Last Modified: Thu, 08 Jul 2021 01:07:04 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f44a51c68d8ebce28a2968c51160202fe904fa726d7e04db859bd004f48c08d`  
		Last Modified: Thu, 08 Jul 2021 01:07:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3`

```console
$ docker pull couchdb@sha256:5f38ddf66f8965dd54109bc5d7cd66a6b2fedf6c6550ea606d28e77bdcb24a5b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3` - linux; amd64

```console
$ docker pull couchdb@sha256:7915f17c6eef82a1318d7be9b2a1164ea7e809b3946fe3eacce5e746adc6c9ad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84508798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49e61de30c53d2c41bf71105914825ed5c180d0c936b21dc6acc834073be9643`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:51:13 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 23 Jun 2021 05:51:15 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 23 Jun 2021 05:51:26 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 07 Jul 2021 23:19:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 07 Jul 2021 23:19:41 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 07 Jul 2021 23:19:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 07 Jul 2021 23:20:12 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 07 Jul 2021 23:20:13 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 07 Jul 2021 23:20:31 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 07 Jul 2021 23:20:32 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 07 Jul 2021 23:20:32 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 07 Jul 2021 23:20:33 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 07 Jul 2021 23:20:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 07 Jul 2021 23:20:34 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 07 Jul 2021 23:20:34 GMT
VOLUME [/opt/couchdb/data]
# Wed, 07 Jul 2021 23:20:34 GMT
EXPOSE 4369 5984 9100
# Wed, 07 Jul 2021 23:20:35 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56acda79979ecba61f07d80188fac6ac183186a686d5f95008434ec065f41fa`  
		Last Modified: Wed, 23 Jun 2021 05:57:01 GMT  
		Size: 3.4 KB (3417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dae9ebd0dd45384cfce6054637761697cc472c88ecf98d3b65ebb821582ed6c`  
		Last Modified: Wed, 23 Jun 2021 05:57:00 GMT  
		Size: 6.7 MB (6690646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5d42f37b9396588987617303dc24662fb0e1f43459f5b4e2b05e069cd69d40`  
		Last Modified: Wed, 07 Jul 2021 23:20:52 GMT  
		Size: 1.3 MB (1258367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980f06759da554159a56f68854a642196e3db0300281f142d17c4d10be0a0881`  
		Last Modified: Wed, 07 Jul 2021 23:20:52 GMT  
		Size: 293.0 KB (293008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1543d07e7709248446a176c8cdab37c46584afb092578ad1034bbdbacbd87cf5`  
		Last Modified: Wed, 07 Jul 2021 23:21:15 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057931a446afd67aba58b7ced44de72b2bbb4d89da8b5ed36239366ec0d3c312`  
		Last Modified: Wed, 07 Jul 2021 23:21:19 GMT  
		Size: 49.1 MB (49113897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36814e6f1d7df65a0652520403064364757bf64c11875a8a8f5bbcddb29eac5`  
		Last Modified: Wed, 07 Jul 2021 23:21:13 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a077feefb03f8e9a3d53fb3cab8cf4c2130610f2b14c651b6ecab22b52fc1c`  
		Last Modified: Wed, 07 Jul 2021 23:21:13 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154f17865ac577c94ab20ba6a1d069e8358c737b35c901986668e9766111f173`  
		Last Modified: Wed, 07 Jul 2021 23:21:14 GMT  
		Size: 2.1 KB (2061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6542f38ef9fe4406e7dc448a70ba4f4a2439f4c1a2045fda001de0dca1d407d`  
		Last Modified: Wed, 07 Jul 2021 23:21:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:e0d961b53c2954b9b06b0f8b65abd7909c47e32604263dfeb165b1fb7845fd12
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72941386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5d8afbe45a9a4db6168d660ea5c4816e78c95b1c88d6d4a96b3ded9f63ad846`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:18:07 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 23 Jun 2021 00:18:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 23 Jun 2021 00:18:15 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 01:05:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 08 Jul 2021 01:05:23 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 08 Jul 2021 01:05:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 01:05:55 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Thu, 08 Jul 2021 01:05:56 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 08 Jul 2021 01:06:09 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 08 Jul 2021 01:06:09 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Thu, 08 Jul 2021 01:06:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 08 Jul 2021 01:06:10 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Thu, 08 Jul 2021 01:06:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 08 Jul 2021 01:06:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 01:06:11 GMT
VOLUME [/opt/couchdb/data]
# Thu, 08 Jul 2021 01:06:12 GMT
EXPOSE 4369 5984 9100
# Thu, 08 Jul 2021 01:06:12 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:339ec36e3b140be1528e45b20e2377aac8adcf3fe37d032e6eb9ee4dad84b53b`  
		Last Modified: Wed, 23 Jun 2021 00:21:32 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e09e9e959b7859e40642c2da7ea73345d2adba18d781d6d4bba0e3c9a4fcd4`  
		Last Modified: Wed, 23 Jun 2021 00:21:31 GMT  
		Size: 6.6 MB (6550152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cae01982b2316cf8b0c31b05b2a9f35981ea5e6e5a0b27cb387d8ca466901e9`  
		Last Modified: Thu, 08 Jul 2021 01:06:40 GMT  
		Size: 1.2 MB (1163469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ca64335472f92842e639e6af3b3b73fce01075ebffeaad8b0db79c2b410b30`  
		Last Modified: Thu, 08 Jul 2021 01:06:40 GMT  
		Size: 292.9 KB (292882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:545112f24e032933f069ae6781b25f9a262e7024dbd91722ec3146e02801b0c1`  
		Last Modified: Thu, 08 Jul 2021 01:07:07 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75747d3f6ce9eb71caaf609c78983eb73b6fcc38f05c869554458971d8f84fa3`  
		Last Modified: Thu, 08 Jul 2021 01:07:10 GMT  
		Size: 39.0 MB (39012845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a058f637ac6b0bb7a63a3d06a1ffeb479132e3805bf1d847f8fe06ab2da62d7a`  
		Last Modified: Thu, 08 Jul 2021 01:07:05 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13c76be4357c902544032954ca18b8dd15cf5a1c629ccf2d40fa0b4f0fd8a7e`  
		Last Modified: Thu, 08 Jul 2021 01:07:05 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b9de3a880ce25c24fbbcb1b8c37eb616781c5f94522677f552c5e8ac142718`  
		Last Modified: Thu, 08 Jul 2021 01:07:04 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f44a51c68d8ebce28a2968c51160202fe904fa726d7e04db859bd004f48c08d`  
		Last Modified: Thu, 08 Jul 2021 01:07:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:2.3.1`

```console
$ docker pull couchdb@sha256:5f38ddf66f8965dd54109bc5d7cd66a6b2fedf6c6550ea606d28e77bdcb24a5b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:2.3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:7915f17c6eef82a1318d7be9b2a1164ea7e809b3946fe3eacce5e746adc6c9ad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84508798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49e61de30c53d2c41bf71105914825ed5c180d0c936b21dc6acc834073be9643`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:51:13 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 23 Jun 2021 05:51:15 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 23 Jun 2021 05:51:26 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 07 Jul 2021 23:19:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 07 Jul 2021 23:19:41 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 07 Jul 2021 23:19:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 07 Jul 2021 23:20:12 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Wed, 07 Jul 2021 23:20:13 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 07 Jul 2021 23:20:31 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 07 Jul 2021 23:20:32 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Wed, 07 Jul 2021 23:20:32 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 07 Jul 2021 23:20:33 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Wed, 07 Jul 2021 23:20:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 07 Jul 2021 23:20:34 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 07 Jul 2021 23:20:34 GMT
VOLUME [/opt/couchdb/data]
# Wed, 07 Jul 2021 23:20:34 GMT
EXPOSE 4369 5984 9100
# Wed, 07 Jul 2021 23:20:35 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56acda79979ecba61f07d80188fac6ac183186a686d5f95008434ec065f41fa`  
		Last Modified: Wed, 23 Jun 2021 05:57:01 GMT  
		Size: 3.4 KB (3417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dae9ebd0dd45384cfce6054637761697cc472c88ecf98d3b65ebb821582ed6c`  
		Last Modified: Wed, 23 Jun 2021 05:57:00 GMT  
		Size: 6.7 MB (6690646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5d42f37b9396588987617303dc24662fb0e1f43459f5b4e2b05e069cd69d40`  
		Last Modified: Wed, 07 Jul 2021 23:20:52 GMT  
		Size: 1.3 MB (1258367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980f06759da554159a56f68854a642196e3db0300281f142d17c4d10be0a0881`  
		Last Modified: Wed, 07 Jul 2021 23:20:52 GMT  
		Size: 293.0 KB (293008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1543d07e7709248446a176c8cdab37c46584afb092578ad1034bbdbacbd87cf5`  
		Last Modified: Wed, 07 Jul 2021 23:21:15 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057931a446afd67aba58b7ced44de72b2bbb4d89da8b5ed36239366ec0d3c312`  
		Last Modified: Wed, 07 Jul 2021 23:21:19 GMT  
		Size: 49.1 MB (49113897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36814e6f1d7df65a0652520403064364757bf64c11875a8a8f5bbcddb29eac5`  
		Last Modified: Wed, 07 Jul 2021 23:21:13 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a077feefb03f8e9a3d53fb3cab8cf4c2130610f2b14c651b6ecab22b52fc1c`  
		Last Modified: Wed, 07 Jul 2021 23:21:13 GMT  
		Size: 766.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154f17865ac577c94ab20ba6a1d069e8358c737b35c901986668e9766111f173`  
		Last Modified: Wed, 07 Jul 2021 23:21:14 GMT  
		Size: 2.1 KB (2061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6542f38ef9fe4406e7dc448a70ba4f4a2439f4c1a2045fda001de0dca1d407d`  
		Last Modified: Wed, 07 Jul 2021 23:21:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:2.3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:e0d961b53c2954b9b06b0f8b65abd7909c47e32604263dfeb165b1fb7845fd12
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72941386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5d8afbe45a9a4db6168d660ea5c4816e78c95b1c88d6d4a96b3ded9f63ad846`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:18:07 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 23 Jun 2021 00:18:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 23 Jun 2021 00:18:15 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 01:05:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 08 Jul 2021 01:05:23 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 08 Jul 2021 01:05:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 01:05:55 GMT
ENV COUCHDB_VERSION=2.3.1-1
# Thu, 08 Jul 2021 01:05:56 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 08 Jul 2021 01:06:09 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 08 Jul 2021 01:06:09 GMT
COPY --chown=couchdb:couchdbfile:74a26e2e31f9b408e93e4a065004a86e00211d06a4ce6ab1fbc23640bd92a929 in /opt/couchdb/etc/default.d/ 
# Thu, 08 Jul 2021 01:06:10 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 08 Jul 2021 01:06:10 GMT
COPY file:a03eff89f810529ca878388de0c227b20fb661957d2117d1664d535138fc12e6 in /usr/local/bin 
# Thu, 08 Jul 2021 01:06:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 08 Jul 2021 01:06:11 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 01:06:11 GMT
VOLUME [/opt/couchdb/data]
# Thu, 08 Jul 2021 01:06:12 GMT
EXPOSE 4369 5984 9100
# Thu, 08 Jul 2021 01:06:12 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:339ec36e3b140be1528e45b20e2377aac8adcf3fe37d032e6eb9ee4dad84b53b`  
		Last Modified: Wed, 23 Jun 2021 00:21:32 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e09e9e959b7859e40642c2da7ea73345d2adba18d781d6d4bba0e3c9a4fcd4`  
		Last Modified: Wed, 23 Jun 2021 00:21:31 GMT  
		Size: 6.6 MB (6550152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cae01982b2316cf8b0c31b05b2a9f35981ea5e6e5a0b27cb387d8ca466901e9`  
		Last Modified: Thu, 08 Jul 2021 01:06:40 GMT  
		Size: 1.2 MB (1163469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ca64335472f92842e639e6af3b3b73fce01075ebffeaad8b0db79c2b410b30`  
		Last Modified: Thu, 08 Jul 2021 01:06:40 GMT  
		Size: 292.9 KB (292882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:545112f24e032933f069ae6781b25f9a262e7024dbd91722ec3146e02801b0c1`  
		Last Modified: Thu, 08 Jul 2021 01:07:07 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75747d3f6ce9eb71caaf609c78983eb73b6fcc38f05c869554458971d8f84fa3`  
		Last Modified: Thu, 08 Jul 2021 01:07:10 GMT  
		Size: 39.0 MB (39012845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a058f637ac6b0bb7a63a3d06a1ffeb479132e3805bf1d847f8fe06ab2da62d7a`  
		Last Modified: Thu, 08 Jul 2021 01:07:05 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13c76be4357c902544032954ca18b8dd15cf5a1c629ccf2d40fa0b4f0fd8a7e`  
		Last Modified: Thu, 08 Jul 2021 01:07:05 GMT  
		Size: 765.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b9de3a880ce25c24fbbcb1b8c37eb616781c5f94522677f552c5e8ac142718`  
		Last Modified: Thu, 08 Jul 2021 01:07:04 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f44a51c68d8ebce28a2968c51160202fe904fa726d7e04db859bd004f48c08d`  
		Last Modified: Thu, 08 Jul 2021 01:07:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3`

```console
$ docker pull couchdb@sha256:be1c514761299cfc4e6afd19c637318a52741eb034fca69f5ba22647d64db984
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3` - linux; amd64

```console
$ docker pull couchdb@sha256:4ba37b549dca789a41e9e53cea46c949efe6f310c4c6e965ca73c9eccea0658f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.8 MB (83771461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d8a9c5436cca6d4759501c2931b9a875f58c4f30e41d189f18c7c964c73ec65`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:51:13 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 23 Jun 2021 05:51:15 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 23 Jun 2021 05:51:26 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 07 Jul 2021 23:19:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 07 Jul 2021 23:19:41 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 07 Jul 2021 23:19:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 07 Jul 2021 23:19:49 GMT
ENV COUCHDB_VERSION=3.1.1
# Wed, 07 Jul 2021 23:19:50 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 07 Jul 2021 23:20:04 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 07 Jul 2021 23:20:05 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 07 Jul 2021 23:20:05 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 07 Jul 2021 23:20:05 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 07 Jul 2021 23:20:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 07 Jul 2021 23:20:06 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 07 Jul 2021 23:20:07 GMT
VOLUME [/opt/couchdb/data]
# Wed, 07 Jul 2021 23:20:07 GMT
EXPOSE 4369 5984 9100
# Wed, 07 Jul 2021 23:20:07 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56acda79979ecba61f07d80188fac6ac183186a686d5f95008434ec065f41fa`  
		Last Modified: Wed, 23 Jun 2021 05:57:01 GMT  
		Size: 3.4 KB (3417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dae9ebd0dd45384cfce6054637761697cc472c88ecf98d3b65ebb821582ed6c`  
		Last Modified: Wed, 23 Jun 2021 05:57:00 GMT  
		Size: 6.7 MB (6690646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5d42f37b9396588987617303dc24662fb0e1f43459f5b4e2b05e069cd69d40`  
		Last Modified: Wed, 07 Jul 2021 23:20:52 GMT  
		Size: 1.3 MB (1258367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980f06759da554159a56f68854a642196e3db0300281f142d17c4d10be0a0881`  
		Last Modified: Wed, 07 Jul 2021 23:20:52 GMT  
		Size: 293.0 KB (293008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d27807f2cfda3753166970f8fbebf6061d633127f1ff8793a9af7cad2b33dd`  
		Last Modified: Wed, 07 Jul 2021 23:20:51 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10cc8ca2490ffb0c54f4d3340ab4df2f428aa8728ce940b89c934171b7761c47`  
		Last Modified: Wed, 07 Jul 2021 23:20:56 GMT  
		Size: 48.4 MB (48376573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6146c21667282fc1cab60dbe45ac415385d272e1df17e8cd967d703bc7822aca`  
		Last Modified: Wed, 07 Jul 2021 23:20:49 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b51caf4fd989fe545edf4a10ff550ce111ddc9117b2821b025d246d6d22138b`  
		Last Modified: Wed, 07 Jul 2021 23:20:49 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b4750c473a84b5ddbac67ea2afcc0b0cf32b13b5b43d0534d6ab906b4c31e8`  
		Last Modified: Wed, 07 Jul 2021 23:20:49 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f194c11d1136db653c5f738ff388aa94294e14d3f8e7910797bdf216265773f`  
		Last Modified: Wed, 07 Jul 2021 23:20:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:2eb6c0aa24fb433a23918bc5f6c3807707b5c4771592dac47801a07d4dd28854
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.8 MB (78787743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cec3671d2e2377def4770df15d7d7b63b73da46594654e293e73f67bfae3214`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:18:07 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 23 Jun 2021 00:18:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 23 Jun 2021 00:18:15 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 01:05:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 08 Jul 2021 01:05:23 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 08 Jul 2021 01:05:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 01:05:30 GMT
ENV COUCHDB_VERSION=3.1.1
# Thu, 08 Jul 2021 01:05:31 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 08 Jul 2021 01:05:44 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 08 Jul 2021 01:05:44 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 08 Jul 2021 01:05:45 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 08 Jul 2021 01:05:45 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Thu, 08 Jul 2021 01:05:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 08 Jul 2021 01:05:46 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 01:05:46 GMT
VOLUME [/opt/couchdb/data]
# Thu, 08 Jul 2021 01:05:46 GMT
EXPOSE 4369 5984 9100
# Thu, 08 Jul 2021 01:05:47 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:339ec36e3b140be1528e45b20e2377aac8adcf3fe37d032e6eb9ee4dad84b53b`  
		Last Modified: Wed, 23 Jun 2021 00:21:32 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e09e9e959b7859e40642c2da7ea73345d2adba18d781d6d4bba0e3c9a4fcd4`  
		Last Modified: Wed, 23 Jun 2021 00:21:31 GMT  
		Size: 6.6 MB (6550152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cae01982b2316cf8b0c31b05b2a9f35981ea5e6e5a0b27cb387d8ca466901e9`  
		Last Modified: Thu, 08 Jul 2021 01:06:40 GMT  
		Size: 1.2 MB (1163469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ca64335472f92842e639e6af3b3b73fce01075ebffeaad8b0db79c2b410b30`  
		Last Modified: Thu, 08 Jul 2021 01:06:40 GMT  
		Size: 292.9 KB (292882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4321bdb7fcc81167226de264982a5462af45f4d38375de39f2dc2bb6bafd8b88`  
		Last Modified: Thu, 08 Jul 2021 01:06:40 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a304fa9d63785e9f6f800236fccb71c359255744f1e98e89e60f86840439e9c`  
		Last Modified: Thu, 08 Jul 2021 01:06:43 GMT  
		Size: 44.9 MB (44859208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b5c6080f1616f5a51a2b7c967373e6d528548700cc3e629a5c8e0aa1dbf181`  
		Last Modified: Thu, 08 Jul 2021 01:06:37 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1922cac36934974f90895eba44af9a1bed372a1b25b26fc1231bd98a9890565c`  
		Last Modified: Thu, 08 Jul 2021 01:06:37 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5630fa08fca2df79f60665e134866137f9302bb029661f95613aadd702e4c7`  
		Last Modified: Thu, 08 Jul 2021 01:06:37 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a433c7e6e8e80f93a06c4e0554d70efedacf8730409b6c299ccd803b452677`  
		Last Modified: Thu, 08 Jul 2021 01:06:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1`

```console
$ docker pull couchdb@sha256:be1c514761299cfc4e6afd19c637318a52741eb034fca69f5ba22647d64db984
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1` - linux; amd64

```console
$ docker pull couchdb@sha256:4ba37b549dca789a41e9e53cea46c949efe6f310c4c6e965ca73c9eccea0658f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.8 MB (83771461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d8a9c5436cca6d4759501c2931b9a875f58c4f30e41d189f18c7c964c73ec65`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:51:13 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 23 Jun 2021 05:51:15 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 23 Jun 2021 05:51:26 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 07 Jul 2021 23:19:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 07 Jul 2021 23:19:41 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 07 Jul 2021 23:19:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 07 Jul 2021 23:19:49 GMT
ENV COUCHDB_VERSION=3.1.1
# Wed, 07 Jul 2021 23:19:50 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 07 Jul 2021 23:20:04 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 07 Jul 2021 23:20:05 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 07 Jul 2021 23:20:05 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 07 Jul 2021 23:20:05 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 07 Jul 2021 23:20:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 07 Jul 2021 23:20:06 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 07 Jul 2021 23:20:07 GMT
VOLUME [/opt/couchdb/data]
# Wed, 07 Jul 2021 23:20:07 GMT
EXPOSE 4369 5984 9100
# Wed, 07 Jul 2021 23:20:07 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56acda79979ecba61f07d80188fac6ac183186a686d5f95008434ec065f41fa`  
		Last Modified: Wed, 23 Jun 2021 05:57:01 GMT  
		Size: 3.4 KB (3417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dae9ebd0dd45384cfce6054637761697cc472c88ecf98d3b65ebb821582ed6c`  
		Last Modified: Wed, 23 Jun 2021 05:57:00 GMT  
		Size: 6.7 MB (6690646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5d42f37b9396588987617303dc24662fb0e1f43459f5b4e2b05e069cd69d40`  
		Last Modified: Wed, 07 Jul 2021 23:20:52 GMT  
		Size: 1.3 MB (1258367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980f06759da554159a56f68854a642196e3db0300281f142d17c4d10be0a0881`  
		Last Modified: Wed, 07 Jul 2021 23:20:52 GMT  
		Size: 293.0 KB (293008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d27807f2cfda3753166970f8fbebf6061d633127f1ff8793a9af7cad2b33dd`  
		Last Modified: Wed, 07 Jul 2021 23:20:51 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10cc8ca2490ffb0c54f4d3340ab4df2f428aa8728ce940b89c934171b7761c47`  
		Last Modified: Wed, 07 Jul 2021 23:20:56 GMT  
		Size: 48.4 MB (48376573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6146c21667282fc1cab60dbe45ac415385d272e1df17e8cd967d703bc7822aca`  
		Last Modified: Wed, 07 Jul 2021 23:20:49 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b51caf4fd989fe545edf4a10ff550ce111ddc9117b2821b025d246d6d22138b`  
		Last Modified: Wed, 07 Jul 2021 23:20:49 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b4750c473a84b5ddbac67ea2afcc0b0cf32b13b5b43d0534d6ab906b4c31e8`  
		Last Modified: Wed, 07 Jul 2021 23:20:49 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f194c11d1136db653c5f738ff388aa94294e14d3f8e7910797bdf216265773f`  
		Last Modified: Wed, 07 Jul 2021 23:20:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:2eb6c0aa24fb433a23918bc5f6c3807707b5c4771592dac47801a07d4dd28854
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.8 MB (78787743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cec3671d2e2377def4770df15d7d7b63b73da46594654e293e73f67bfae3214`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:18:07 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 23 Jun 2021 00:18:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 23 Jun 2021 00:18:15 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 01:05:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 08 Jul 2021 01:05:23 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 08 Jul 2021 01:05:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 01:05:30 GMT
ENV COUCHDB_VERSION=3.1.1
# Thu, 08 Jul 2021 01:05:31 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 08 Jul 2021 01:05:44 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 08 Jul 2021 01:05:44 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 08 Jul 2021 01:05:45 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 08 Jul 2021 01:05:45 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Thu, 08 Jul 2021 01:05:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 08 Jul 2021 01:05:46 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 01:05:46 GMT
VOLUME [/opt/couchdb/data]
# Thu, 08 Jul 2021 01:05:46 GMT
EXPOSE 4369 5984 9100
# Thu, 08 Jul 2021 01:05:47 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:339ec36e3b140be1528e45b20e2377aac8adcf3fe37d032e6eb9ee4dad84b53b`  
		Last Modified: Wed, 23 Jun 2021 00:21:32 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e09e9e959b7859e40642c2da7ea73345d2adba18d781d6d4bba0e3c9a4fcd4`  
		Last Modified: Wed, 23 Jun 2021 00:21:31 GMT  
		Size: 6.6 MB (6550152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cae01982b2316cf8b0c31b05b2a9f35981ea5e6e5a0b27cb387d8ca466901e9`  
		Last Modified: Thu, 08 Jul 2021 01:06:40 GMT  
		Size: 1.2 MB (1163469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ca64335472f92842e639e6af3b3b73fce01075ebffeaad8b0db79c2b410b30`  
		Last Modified: Thu, 08 Jul 2021 01:06:40 GMT  
		Size: 292.9 KB (292882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4321bdb7fcc81167226de264982a5462af45f4d38375de39f2dc2bb6bafd8b88`  
		Last Modified: Thu, 08 Jul 2021 01:06:40 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a304fa9d63785e9f6f800236fccb71c359255744f1e98e89e60f86840439e9c`  
		Last Modified: Thu, 08 Jul 2021 01:06:43 GMT  
		Size: 44.9 MB (44859208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b5c6080f1616f5a51a2b7c967373e6d528548700cc3e629a5c8e0aa1dbf181`  
		Last Modified: Thu, 08 Jul 2021 01:06:37 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1922cac36934974f90895eba44af9a1bed372a1b25b26fc1231bd98a9890565c`  
		Last Modified: Thu, 08 Jul 2021 01:06:37 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5630fa08fca2df79f60665e134866137f9302bb029661f95613aadd702e4c7`  
		Last Modified: Thu, 08 Jul 2021 01:06:37 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a433c7e6e8e80f93a06c4e0554d70efedacf8730409b6c299ccd803b452677`  
		Last Modified: Thu, 08 Jul 2021 01:06:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:3.1.1`

```console
$ docker pull couchdb@sha256:be1c514761299cfc4e6afd19c637318a52741eb034fca69f5ba22647d64db984
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:3.1.1` - linux; amd64

```console
$ docker pull couchdb@sha256:4ba37b549dca789a41e9e53cea46c949efe6f310c4c6e965ca73c9eccea0658f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.8 MB (83771461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d8a9c5436cca6d4759501c2931b9a875f58c4f30e41d189f18c7c964c73ec65`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:51:13 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 23 Jun 2021 05:51:15 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 23 Jun 2021 05:51:26 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 07 Jul 2021 23:19:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 07 Jul 2021 23:19:41 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 07 Jul 2021 23:19:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 07 Jul 2021 23:19:49 GMT
ENV COUCHDB_VERSION=3.1.1
# Wed, 07 Jul 2021 23:19:50 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 07 Jul 2021 23:20:04 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 07 Jul 2021 23:20:05 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 07 Jul 2021 23:20:05 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 07 Jul 2021 23:20:05 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 07 Jul 2021 23:20:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 07 Jul 2021 23:20:06 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 07 Jul 2021 23:20:07 GMT
VOLUME [/opt/couchdb/data]
# Wed, 07 Jul 2021 23:20:07 GMT
EXPOSE 4369 5984 9100
# Wed, 07 Jul 2021 23:20:07 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56acda79979ecba61f07d80188fac6ac183186a686d5f95008434ec065f41fa`  
		Last Modified: Wed, 23 Jun 2021 05:57:01 GMT  
		Size: 3.4 KB (3417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dae9ebd0dd45384cfce6054637761697cc472c88ecf98d3b65ebb821582ed6c`  
		Last Modified: Wed, 23 Jun 2021 05:57:00 GMT  
		Size: 6.7 MB (6690646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5d42f37b9396588987617303dc24662fb0e1f43459f5b4e2b05e069cd69d40`  
		Last Modified: Wed, 07 Jul 2021 23:20:52 GMT  
		Size: 1.3 MB (1258367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980f06759da554159a56f68854a642196e3db0300281f142d17c4d10be0a0881`  
		Last Modified: Wed, 07 Jul 2021 23:20:52 GMT  
		Size: 293.0 KB (293008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d27807f2cfda3753166970f8fbebf6061d633127f1ff8793a9af7cad2b33dd`  
		Last Modified: Wed, 07 Jul 2021 23:20:51 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10cc8ca2490ffb0c54f4d3340ab4df2f428aa8728ce940b89c934171b7761c47`  
		Last Modified: Wed, 07 Jul 2021 23:20:56 GMT  
		Size: 48.4 MB (48376573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6146c21667282fc1cab60dbe45ac415385d272e1df17e8cd967d703bc7822aca`  
		Last Modified: Wed, 07 Jul 2021 23:20:49 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b51caf4fd989fe545edf4a10ff550ce111ddc9117b2821b025d246d6d22138b`  
		Last Modified: Wed, 07 Jul 2021 23:20:49 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b4750c473a84b5ddbac67ea2afcc0b0cf32b13b5b43d0534d6ab906b4c31e8`  
		Last Modified: Wed, 07 Jul 2021 23:20:49 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f194c11d1136db653c5f738ff388aa94294e14d3f8e7910797bdf216265773f`  
		Last Modified: Wed, 07 Jul 2021 23:20:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:3.1.1` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:2eb6c0aa24fb433a23918bc5f6c3807707b5c4771592dac47801a07d4dd28854
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.8 MB (78787743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cec3671d2e2377def4770df15d7d7b63b73da46594654e293e73f67bfae3214`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:18:07 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 23 Jun 2021 00:18:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 23 Jun 2021 00:18:15 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 01:05:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 08 Jul 2021 01:05:23 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 08 Jul 2021 01:05:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 01:05:30 GMT
ENV COUCHDB_VERSION=3.1.1
# Thu, 08 Jul 2021 01:05:31 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 08 Jul 2021 01:05:44 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 08 Jul 2021 01:05:44 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 08 Jul 2021 01:05:45 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 08 Jul 2021 01:05:45 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Thu, 08 Jul 2021 01:05:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 08 Jul 2021 01:05:46 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 01:05:46 GMT
VOLUME [/opt/couchdb/data]
# Thu, 08 Jul 2021 01:05:46 GMT
EXPOSE 4369 5984 9100
# Thu, 08 Jul 2021 01:05:47 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:339ec36e3b140be1528e45b20e2377aac8adcf3fe37d032e6eb9ee4dad84b53b`  
		Last Modified: Wed, 23 Jun 2021 00:21:32 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e09e9e959b7859e40642c2da7ea73345d2adba18d781d6d4bba0e3c9a4fcd4`  
		Last Modified: Wed, 23 Jun 2021 00:21:31 GMT  
		Size: 6.6 MB (6550152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cae01982b2316cf8b0c31b05b2a9f35981ea5e6e5a0b27cb387d8ca466901e9`  
		Last Modified: Thu, 08 Jul 2021 01:06:40 GMT  
		Size: 1.2 MB (1163469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ca64335472f92842e639e6af3b3b73fce01075ebffeaad8b0db79c2b410b30`  
		Last Modified: Thu, 08 Jul 2021 01:06:40 GMT  
		Size: 292.9 KB (292882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4321bdb7fcc81167226de264982a5462af45f4d38375de39f2dc2bb6bafd8b88`  
		Last Modified: Thu, 08 Jul 2021 01:06:40 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a304fa9d63785e9f6f800236fccb71c359255744f1e98e89e60f86840439e9c`  
		Last Modified: Thu, 08 Jul 2021 01:06:43 GMT  
		Size: 44.9 MB (44859208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b5c6080f1616f5a51a2b7c967373e6d528548700cc3e629a5c8e0aa1dbf181`  
		Last Modified: Thu, 08 Jul 2021 01:06:37 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1922cac36934974f90895eba44af9a1bed372a1b25b26fc1231bd98a9890565c`  
		Last Modified: Thu, 08 Jul 2021 01:06:37 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5630fa08fca2df79f60665e134866137f9302bb029661f95613aadd702e4c7`  
		Last Modified: Thu, 08 Jul 2021 01:06:37 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a433c7e6e8e80f93a06c4e0554d70efedacf8730409b6c299ccd803b452677`  
		Last Modified: Thu, 08 Jul 2021 01:06:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchdb:latest`

```console
$ docker pull couchdb@sha256:be1c514761299cfc4e6afd19c637318a52741eb034fca69f5ba22647d64db984
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchdb:latest` - linux; amd64

```console
$ docker pull couchdb@sha256:4ba37b549dca789a41e9e53cea46c949efe6f310c4c6e965ca73c9eccea0658f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.8 MB (83771461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d8a9c5436cca6d4759501c2931b9a875f58c4f30e41d189f18c7c964c73ec65`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:51:13 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 23 Jun 2021 05:51:15 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 23 Jun 2021 05:51:26 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Wed, 07 Jul 2021 23:19:41 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Wed, 07 Jul 2021 23:19:41 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Wed, 07 Jul 2021 23:19:49 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Wed, 07 Jul 2021 23:19:49 GMT
ENV COUCHDB_VERSION=3.1.1
# Wed, 07 Jul 2021 23:19:50 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Wed, 07 Jul 2021 23:20:04 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Wed, 07 Jul 2021 23:20:05 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Wed, 07 Jul 2021 23:20:05 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Wed, 07 Jul 2021 23:20:05 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Wed, 07 Jul 2021 23:20:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Wed, 07 Jul 2021 23:20:06 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Wed, 07 Jul 2021 23:20:07 GMT
VOLUME [/opt/couchdb/data]
# Wed, 07 Jul 2021 23:20:07 GMT
EXPOSE 4369 5984 9100
# Wed, 07 Jul 2021 23:20:07 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56acda79979ecba61f07d80188fac6ac183186a686d5f95008434ec065f41fa`  
		Last Modified: Wed, 23 Jun 2021 05:57:01 GMT  
		Size: 3.4 KB (3417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dae9ebd0dd45384cfce6054637761697cc472c88ecf98d3b65ebb821582ed6c`  
		Last Modified: Wed, 23 Jun 2021 05:57:00 GMT  
		Size: 6.7 MB (6690646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5d42f37b9396588987617303dc24662fb0e1f43459f5b4e2b05e069cd69d40`  
		Last Modified: Wed, 07 Jul 2021 23:20:52 GMT  
		Size: 1.3 MB (1258367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980f06759da554159a56f68854a642196e3db0300281f142d17c4d10be0a0881`  
		Last Modified: Wed, 07 Jul 2021 23:20:52 GMT  
		Size: 293.0 KB (293008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d27807f2cfda3753166970f8fbebf6061d633127f1ff8793a9af7cad2b33dd`  
		Last Modified: Wed, 07 Jul 2021 23:20:51 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10cc8ca2490ffb0c54f4d3340ab4df2f428aa8728ce940b89c934171b7761c47`  
		Last Modified: Wed, 07 Jul 2021 23:20:56 GMT  
		Size: 48.4 MB (48376573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6146c21667282fc1cab60dbe45ac415385d272e1df17e8cd967d703bc7822aca`  
		Last Modified: Wed, 07 Jul 2021 23:20:49 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b51caf4fd989fe545edf4a10ff550ce111ddc9117b2821b025d246d6d22138b`  
		Last Modified: Wed, 07 Jul 2021 23:20:49 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b4750c473a84b5ddbac67ea2afcc0b0cf32b13b5b43d0534d6ab906b4c31e8`  
		Last Modified: Wed, 07 Jul 2021 23:20:49 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f194c11d1136db653c5f738ff388aa94294e14d3f8e7910797bdf216265773f`  
		Last Modified: Wed, 07 Jul 2021 23:20:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchdb:latest` - linux; arm64 variant v8

```console
$ docker pull couchdb@sha256:2eb6c0aa24fb433a23918bc5f6c3807707b5c4771592dac47801a07d4dd28854
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.8 MB (78787743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cec3671d2e2377def4770df15d7d7b63b73da46594654e293e73f67bfae3214`
-	Entrypoint: `["tini","--","\/docker-entrypoint.sh"]`
-	Default Command: `["\/opt\/couchdb\/bin\/couchdb"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:18:07 GMT
LABEL maintainer=CouchDB Developers dev@couchdb.apache.org
# Wed, 23 Jun 2021 00:18:08 GMT
RUN groupadd -g 5984 -r couchdb && useradd -u 5984 -d /opt/couchdb -g couchdb couchdb
# Wed, 23 Jun 2021 00:18:15 GMT
RUN set -ex;     apt-get update;     apt-get install -y --no-install-recommends         apt-transport-https         ca-certificates         dirmngr         gnupg      ;     rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 01:05:22 GMT
RUN set -eux;     apt-get update;     apt-get install -y --no-install-recommends gosu tini;     rm -rf /var/lib/apt/lists/*;     gosu nobody true;     tini --version
# Thu, 08 Jul 2021 01:05:23 GMT
ENV GPG_COUCH_KEY=390EF70BB1EA12B2773962950EE62FB37A00258D
# Thu, 08 Jul 2021 01:05:30 GMT
RUN set -eux;     apt-get update;     apt-get install -y curl;     export GNUPGHOME="$(mktemp -d)";     curl -fL -o keys.asc https://couchdb.apache.org/repo/keys.asc;     gpg --batch --import keys.asc;     gpg --batch --export "${GPG_COUCH_KEY}" > /usr/share/keyrings/couchdb-archive-keyring.gpg;     command -v gpgconf && gpgconf --kill all || :;     rm -rf "$GNUPGHOME";     apt-key list;     apt purge -y --autoremove curl;     rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 01:05:30 GMT
ENV COUCHDB_VERSION=3.1.1
# Thu, 08 Jul 2021 01:05:31 GMT
RUN . /etc/os-release;     echo "deb [signed-by=/usr/share/keyrings/couchdb-archive-keyring.gpg] https://apache.jfrog.io/artifactory/couchdb-deb/ ${VERSION_CODENAME} main" |         tee /etc/apt/sources.list.d/couchdb.list >/dev/null
# Thu, 08 Jul 2021 01:05:44 GMT
RUN set -eux;     apt-get update;         echo "couchdb couchdb/mode select none" | debconf-set-selections;     DEBIAN_FRONTEND=noninteractive apt-get install -y --allow-downgrades --allow-remove-essential --allow-change-held-packages             couchdb="$COUCHDB_VERSION"~buster     ;     rmdir /var/lib/couchdb /var/log/couchdb;     rm /opt/couchdb/data /opt/couchdb/var/log;     mkdir -p /opt/couchdb/data /opt/couchdb/var/log;     chown couchdb:couchdb /opt/couchdb/data /opt/couchdb/var/log;     chmod 777 /opt/couchdb/data /opt/couchdb/var/log;     rm /opt/couchdb/etc/default.d/10-filelog.ini;     find /opt/couchdb \! \( -user couchdb -group couchdb \) -exec chown -f couchdb:couchdb '{}' +;     find /opt/couchdb/etc -type d ! -perm 0755 -exec chmod -f 0755 '{}' +;     find /opt/couchdb/etc -type f ! -perm 0644 -exec chmod -f 0644 '{}' +;     chmod -f 0777 /opt/couchdb/etc/local.d;     rm -rf /var/lib/apt/lists/*;
# Thu, 08 Jul 2021 01:05:44 GMT
COPY --chown=couchdb:couchdbfile:459581cb8ff69dbc1cb246db7b488d5b6127e57fcbb0d0df1288722b5cd25111 in /opt/couchdb/etc/default.d/ 
# Thu, 08 Jul 2021 01:05:45 GMT
COPY --chown=couchdb:couchdbfile:f98e48e4254cb3ec4a766f3b9bd3260f16676a310eb0356ee9775c62edb3e8f3 in /opt/couchdb/etc/ 
# Thu, 08 Jul 2021 01:05:45 GMT
COPY file:5f96ca1bf2f6f650a65a16c93abec310412df7ca501bf32df2ac20f99b1a0742 in /usr/local/bin 
# Thu, 08 Jul 2021 01:05:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /docker-entrypoint.sh # backwards compat
# Thu, 08 Jul 2021 01:05:46 GMT
ENTRYPOINT ["tini" "--" "/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 01:05:46 GMT
VOLUME [/opt/couchdb/data]
# Thu, 08 Jul 2021 01:05:46 GMT
EXPOSE 4369 5984 9100
# Thu, 08 Jul 2021 01:05:47 GMT
CMD ["/opt/couchdb/bin/couchdb"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:339ec36e3b140be1528e45b20e2377aac8adcf3fe37d032e6eb9ee4dad84b53b`  
		Last Modified: Wed, 23 Jun 2021 00:21:32 GMT  
		Size: 3.4 KB (3438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e09e9e959b7859e40642c2da7ea73345d2adba18d781d6d4bba0e3c9a4fcd4`  
		Last Modified: Wed, 23 Jun 2021 00:21:31 GMT  
		Size: 6.6 MB (6550152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cae01982b2316cf8b0c31b05b2a9f35981ea5e6e5a0b27cb387d8ca466901e9`  
		Last Modified: Thu, 08 Jul 2021 01:06:40 GMT  
		Size: 1.2 MB (1163469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ca64335472f92842e639e6af3b3b73fce01075ebffeaad8b0db79c2b410b30`  
		Last Modified: Thu, 08 Jul 2021 01:06:40 GMT  
		Size: 292.9 KB (292882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4321bdb7fcc81167226de264982a5462af45f4d38375de39f2dc2bb6bafd8b88`  
		Last Modified: Thu, 08 Jul 2021 01:06:40 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a304fa9d63785e9f6f800236fccb71c359255744f1e98e89e60f86840439e9c`  
		Last Modified: Thu, 08 Jul 2021 01:06:43 GMT  
		Size: 44.9 MB (44859208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b5c6080f1616f5a51a2b7c967373e6d528548700cc3e629a5c8e0aa1dbf181`  
		Last Modified: Thu, 08 Jul 2021 01:06:37 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1922cac36934974f90895eba44af9a1bed372a1b25b26fc1231bd98a9890565c`  
		Last Modified: Thu, 08 Jul 2021 01:06:37 GMT  
		Size: 764.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5630fa08fca2df79f60665e134866137f9302bb029661f95613aadd702e4c7`  
		Last Modified: Thu, 08 Jul 2021 01:06:37 GMT  
		Size: 2.1 KB (2059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a433c7e6e8e80f93a06c4e0554d70efedacf8730409b6c299ccd803b452677`  
		Last Modified: Thu, 08 Jul 2021 01:06:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
