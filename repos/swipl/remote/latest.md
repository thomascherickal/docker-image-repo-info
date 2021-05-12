## `swipl:latest`

```console
$ docker pull swipl@sha256:3bc19c2832dcc3e7825b99325ac0fae644dddcf2137943d3902bd611c273790c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `swipl:latest` - linux; amd64

```console
$ docker pull swipl@sha256:4e4dc53df15e3a79a4cacc7442b0cc6764d6b5a541bb2d9cd7307bc94ddeb182
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.4 MB (56391667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74a66a369a24ac619ed70d34eb584b788ce640b14e8eff4d0854678e6d842de8`
-	Default Command: `["swipl"]`

```dockerfile
# Sat, 10 Apr 2021 01:21:54 GMT
ADD file:70cd6967491943999563ddd3ab9abae33791ac320cdc846dc57503cc44f25600 in / 
# Sat, 10 Apr 2021 01:21:54 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 17:50:40 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Michael Hendricks <michael@ndrix.org>
# Sat, 10 Apr 2021 17:50:53 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends     libtcmalloc-minimal4     libarchive13     libyaml-dev     libgmp10     libossp-uuid16     libssl1.1     ca-certificates     libdb5.3     libpcre3     libedit2     libgeos-c1v5     libspatialindex4v5     unixodbc     odbc-postgresql     tdsodbc     libmariadbclient18     libsqlite3-0     libserd-0-0     libraptor2-0 &&     dpkgArch="$(dpkg --print-architecture)" &&     rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:50:53 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 18:08:59 GMT
RUN set -eux;     SWIPL_VER=8.3.18;     SWIPL_CHECKSUM=528349b353b36dde3d57d1de366a45e4fbbb89d4a96de907b9a0497e601be768;     BUILD_DEPS='make cmake ninja-build gcc g++ wget git autoconf libarchive-dev libgmp-dev libossp-uuid-dev libpcre3-dev libreadline-dev libedit-dev libssl-dev zlib1g-dev libdb-dev unixodbc-dev libsqlite3-dev libserd-dev libraptor2-dev libgeos++-dev libspatialindex-dev libgoogle-perftools-dev';     dpkgArch="$(dpkg --print-architecture)";     apt-get update; apt-get install -y --no-install-recommends $BUILD_DEPS; rm -rf /var/lib/apt/lists/*;     mkdir /tmp/src;     cd /tmp/src;     wget -q https://www.swi-prolog.org/download/devel/src/swipl-$SWIPL_VER.tar.gz;     echo "$SWIPL_CHECKSUM  swipl-$SWIPL_VER.tar.gz" >> swipl-$SWIPL_VER.tar.gz-CHECKSUM;     sha256sum -c swipl-$SWIPL_VER.tar.gz-CHECKSUM;     tar -xzf swipl-$SWIPL_VER.tar.gz;     mkdir swipl-$SWIPL_VER/build;     cd swipl-$SWIPL_VER/build;     cmake -DCMAKE_BUILD_TYPE=Release           -DSWIPL_PACKAGES_X=OFF 	  -DSWIPL_PACKAGES_JAVA=OFF 	  -DCMAKE_INSTALL_PREFIX=/usr 	  -G Ninja           ..;     ../scripts/pgo-compile.sh;     ninja;     ninja install;     rm -rf /tmp/src;     mkdir -p /usr/share/swi-prolog/pack;     cd /usr/share/swi-prolog/pack;     install_addin () {         git clone "$2" "$1";         git -C "$1" checkout -q "$3";         if [ "$1" = 'prosqlite' ]; then rm -rf "$1/lib"; fi;         swipl -g "pack_rebuild($1)" -t halt;         find "$1" -mindepth 1 -maxdepth 1 ! -name lib ! -name prolog ! -name pack.pl -exec rm -rf {} +;         find "$1" -name .git -exec rm -rf {} +;         find "$1" -name '*.so' -exec strip {} +;     };     dpkgArch="$(dpkg --print-architecture)";     install_addin space https://github.com/JanWielemaker/space.git cd6fefa63317a7a6effb61a1c5aee634ebe2ca05;     install_addin prosqlite https://github.com/nicos-angelopoulos/prosqlite.git cfd2f68709f5fb61833c0e2f8e9c6546e542009c;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] || install_addin rocksdb https://github.com/JanWielemaker/rocksdb.git f110766ee97cfbc6fddd4c33b7238f00e76ecc18;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] ||  install_addin hdt https://github.com/JanWielemaker/hdt.git e0a0eff87fc3318434cb493690c570e1255ed30e;     install_addin rserve_client https://github.com/JanWielemaker/rserve_client.git f8e83a4e1e4600baef4222dc4c2904a41a79a5ad;     apt-get purge -y --auto-remove $BUILD_DEPS
# Sat, 10 Apr 2021 18:09:00 GMT
CMD ["swipl"]
```

-	Layers:
	-	`sha256:62deabe7a6db312ed773ccd640cd7cfbf51c22bf466886345684558f1036e358`  
		Last Modified: Sat, 10 Apr 2021 01:28:26 GMT  
		Size: 22.5 MB (22528265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0db3d44d840cb5cac9613fcb8e3edfa8587f9be5fb0a23b88bd9d5980d02fbc`  
		Last Modified: Sat, 10 Apr 2021 18:27:13 GMT  
		Size: 24.9 MB (24920421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8758420d64fa565f26120781d6ca7ae700547db437ca9bddfcf6d9633ad3d064`  
		Last Modified: Sat, 10 Apr 2021 18:27:12 GMT  
		Size: 8.9 MB (8942981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `swipl:latest` - linux; arm variant v7

```console
$ docker pull swipl@sha256:1cc10fb26018c1a155fcc9b40bb905ce11384b20f3ef20bf49be88f56d9094c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.5 MB (48495292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:591d7b7b23f22cd6e595e6fbcb1c194646dc3a55d459fdd3d0896b1e824c53a9`
-	Default Command: `["swipl"]`

```dockerfile
# Wed, 12 May 2021 01:13:00 GMT
ADD file:3a0c44e2f78c31814d76ce91706cea345d424f8b49631a1e01dbfe768d244d48 in / 
# Wed, 12 May 2021 01:13:05 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:07:55 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Michael Hendricks <michael@ndrix.org>
# Wed, 12 May 2021 02:08:33 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends     libtcmalloc-minimal4     libarchive13     libyaml-dev     libgmp10     libossp-uuid16     libssl1.1     ca-certificates     libdb5.3     libpcre3     libedit2     libgeos-c1v5     libspatialindex4v5     unixodbc     odbc-postgresql     tdsodbc     libmariadbclient18     libsqlite3-0     libserd-0-0     libraptor2-0 &&     dpkgArch="$(dpkg --print-architecture)" &&     rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 02:08:35 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 02:13:31 GMT
RUN set -eux;     SWIPL_VER=8.3.18;     SWIPL_CHECKSUM=528349b353b36dde3d57d1de366a45e4fbbb89d4a96de907b9a0497e601be768;     BUILD_DEPS='make cmake ninja-build gcc g++ wget git autoconf libarchive-dev libgmp-dev libossp-uuid-dev libpcre3-dev libreadline-dev libedit-dev libssl-dev zlib1g-dev libdb-dev unixodbc-dev libsqlite3-dev libserd-dev libraptor2-dev libgeos++-dev libspatialindex-dev libgoogle-perftools-dev';     dpkgArch="$(dpkg --print-architecture)";     apt-get update; apt-get install -y --no-install-recommends $BUILD_DEPS; rm -rf /var/lib/apt/lists/*;     mkdir /tmp/src;     cd /tmp/src;     wget -q https://www.swi-prolog.org/download/devel/src/swipl-$SWIPL_VER.tar.gz;     echo "$SWIPL_CHECKSUM  swipl-$SWIPL_VER.tar.gz" >> swipl-$SWIPL_VER.tar.gz-CHECKSUM;     sha256sum -c swipl-$SWIPL_VER.tar.gz-CHECKSUM;     tar -xzf swipl-$SWIPL_VER.tar.gz;     mkdir swipl-$SWIPL_VER/build;     cd swipl-$SWIPL_VER/build;     cmake -DCMAKE_BUILD_TYPE=Release           -DSWIPL_PACKAGES_X=OFF 	  -DSWIPL_PACKAGES_JAVA=OFF 	  -DCMAKE_INSTALL_PREFIX=/usr 	  -G Ninja           ..;     ../scripts/pgo-compile.sh;     ninja;     ninja install;     rm -rf /tmp/src;     mkdir -p /usr/share/swi-prolog/pack;     cd /usr/share/swi-prolog/pack;     install_addin () {         git clone "$2" "$1";         git -C "$1" checkout -q "$3";         if [ "$1" = 'prosqlite' ]; then rm -rf "$1/lib"; fi;         swipl -g "pack_rebuild($1)" -t halt;         find "$1" -mindepth 1 -maxdepth 1 ! -name lib ! -name prolog ! -name pack.pl -exec rm -rf {} +;         find "$1" -name .git -exec rm -rf {} +;         find "$1" -name '*.so' -exec strip {} +;     };     dpkgArch="$(dpkg --print-architecture)";     install_addin space https://github.com/JanWielemaker/space.git cd6fefa63317a7a6effb61a1c5aee634ebe2ca05;     install_addin prosqlite https://github.com/nicos-angelopoulos/prosqlite.git cfd2f68709f5fb61833c0e2f8e9c6546e542009c;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] || install_addin rocksdb https://github.com/JanWielemaker/rocksdb.git f110766ee97cfbc6fddd4c33b7238f00e76ecc18;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] ||  install_addin hdt https://github.com/JanWielemaker/hdt.git e0a0eff87fc3318434cb493690c570e1255ed30e;     install_addin rserve_client https://github.com/JanWielemaker/rserve_client.git f8e83a4e1e4600baef4222dc4c2904a41a79a5ad;     apt-get purge -y --auto-remove $BUILD_DEPS
# Wed, 12 May 2021 02:13:32 GMT
CMD ["swipl"]
```

-	Layers:
	-	`sha256:ce2b35672977ffba9f48ce0726706cd15d926482c1008f69213433c61ba44966`  
		Last Modified: Wed, 12 May 2021 01:21:44 GMT  
		Size: 19.3 MB (19315154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed932ba77efb460bd98cf545ca0150d01189e662f4d5966acc78445f28dc2c49`  
		Last Modified: Wed, 12 May 2021 02:19:06 GMT  
		Size: 22.9 MB (22880842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19748fd7b144fbaff4becfedcfc95e24b1916d53fa59335a968daccc513b1d08`  
		Last Modified: Wed, 12 May 2021 02:19:02 GMT  
		Size: 6.3 MB (6299296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `swipl:latest` - linux; arm64 variant v8

```console
$ docker pull swipl@sha256:eff51544e45a4118848a5694c1b0cb7d53fa5235105d8330791b4a988bd5484f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52805552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d600567e658e720949418d644c409a66c9bcc5a7543e0b3c6d23a81e2b410027`
-	Default Command: `["swipl"]`

```dockerfile
# Sat, 10 Apr 2021 00:44:13 GMT
ADD file:a74d7856e70f2e18d2509edd9f0527254a69e9d1347715149c772a0d4ca7d509 in / 
# Sat, 10 Apr 2021 00:44:14 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 17:04:23 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Michael Hendricks <michael@ndrix.org>
# Sat, 10 Apr 2021 17:04:58 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends     libtcmalloc-minimal4     libarchive13     libyaml-dev     libgmp10     libossp-uuid16     libssl1.1     ca-certificates     libdb5.3     libpcre3     libedit2     libgeos-c1v5     libspatialindex4v5     unixodbc     odbc-postgresql     tdsodbc     libmariadbclient18     libsqlite3-0     libserd-0-0     libraptor2-0 &&     dpkgArch="$(dpkg --print-architecture)" &&     rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:05:00 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 17:37:32 GMT
RUN set -eux;     SWIPL_VER=8.3.18;     SWIPL_CHECKSUM=528349b353b36dde3d57d1de366a45e4fbbb89d4a96de907b9a0497e601be768;     BUILD_DEPS='make cmake ninja-build gcc g++ wget git autoconf libarchive-dev libgmp-dev libossp-uuid-dev libpcre3-dev libreadline-dev libedit-dev libssl-dev zlib1g-dev libdb-dev unixodbc-dev libsqlite3-dev libserd-dev libraptor2-dev libgeos++-dev libspatialindex-dev libgoogle-perftools-dev';     dpkgArch="$(dpkg --print-architecture)";     apt-get update; apt-get install -y --no-install-recommends $BUILD_DEPS; rm -rf /var/lib/apt/lists/*;     mkdir /tmp/src;     cd /tmp/src;     wget -q https://www.swi-prolog.org/download/devel/src/swipl-$SWIPL_VER.tar.gz;     echo "$SWIPL_CHECKSUM  swipl-$SWIPL_VER.tar.gz" >> swipl-$SWIPL_VER.tar.gz-CHECKSUM;     sha256sum -c swipl-$SWIPL_VER.tar.gz-CHECKSUM;     tar -xzf swipl-$SWIPL_VER.tar.gz;     mkdir swipl-$SWIPL_VER/build;     cd swipl-$SWIPL_VER/build;     cmake -DCMAKE_BUILD_TYPE=Release           -DSWIPL_PACKAGES_X=OFF 	  -DSWIPL_PACKAGES_JAVA=OFF 	  -DCMAKE_INSTALL_PREFIX=/usr 	  -G Ninja           ..;     ../scripts/pgo-compile.sh;     ninja;     ninja install;     rm -rf /tmp/src;     mkdir -p /usr/share/swi-prolog/pack;     cd /usr/share/swi-prolog/pack;     install_addin () {         git clone "$2" "$1";         git -C "$1" checkout -q "$3";         if [ "$1" = 'prosqlite' ]; then rm -rf "$1/lib"; fi;         swipl -g "pack_rebuild($1)" -t halt;         find "$1" -mindepth 1 -maxdepth 1 ! -name lib ! -name prolog ! -name pack.pl -exec rm -rf {} +;         find "$1" -name .git -exec rm -rf {} +;         find "$1" -name '*.so' -exec strip {} +;     };     dpkgArch="$(dpkg --print-architecture)";     install_addin space https://github.com/JanWielemaker/space.git cd6fefa63317a7a6effb61a1c5aee634ebe2ca05;     install_addin prosqlite https://github.com/nicos-angelopoulos/prosqlite.git cfd2f68709f5fb61833c0e2f8e9c6546e542009c;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] || install_addin rocksdb https://github.com/JanWielemaker/rocksdb.git f110766ee97cfbc6fddd4c33b7238f00e76ecc18;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] ||  install_addin hdt https://github.com/JanWielemaker/hdt.git e0a0eff87fc3318434cb493690c570e1255ed30e;     install_addin rserve_client https://github.com/JanWielemaker/rserve_client.git f8e83a4e1e4600baef4222dc4c2904a41a79a5ad;     apt-get purge -y --auto-remove $BUILD_DEPS
# Sat, 10 Apr 2021 17:37:35 GMT
CMD ["swipl"]
```

-	Layers:
	-	`sha256:bc16ed4a30c7b74efb2ba46d7df8a6591a02826832c27a5cf55cc6e06111a5a6`  
		Last Modified: Sat, 10 Apr 2021 00:50:10 GMT  
		Size: 20.4 MB (20389366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5439c83741649ea579ed349c18294c3c8abd9ac28499cee8f824f2b2c7e5a14b`  
		Last Modified: Sat, 10 Apr 2021 18:11:03 GMT  
		Size: 23.7 MB (23742631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cfb8a6e45baaa72e8ae3ad9592ef42191027a45ffe3cb5d955427fae9681f0`  
		Last Modified: Sat, 10 Apr 2021 18:11:00 GMT  
		Size: 8.7 MB (8673555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
