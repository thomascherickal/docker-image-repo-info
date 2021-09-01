<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `swipl`

-	[`swipl:8.2.4`](#swipl824)
-	[`swipl:8.3.29`](#swipl8329)
-	[`swipl:latest`](#swipllatest)
-	[`swipl:stable`](#swiplstable)

## `swipl:8.2.4`

```console
$ docker pull swipl@sha256:0ef14736125c5cd068eb22435b19c574e9e585de78896351f5577b753ed44c70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `swipl:8.2.4` - linux; amd64

```console
$ docker pull swipl@sha256:a3de56b9f0c0b04355f6227a142c7619309efbbd6537867f73d4769e90fbc36d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.3 MB (56278918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c604a2fce7caaded8063e1b174a84105fe5273734016012b067975fa2d2c4b13`
-	Default Command: `["swipl"]`

```dockerfile
# Tue, 17 Aug 2021 01:26:09 GMT
ADD file:f6c4487fa1f7a4e17f5d88fd0c91031a6efc7fa210d363a1d43d8b0f3a8d1d03 in / 
# Tue, 17 Aug 2021 01:26:09 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:41:06 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Michael Hendricks <michael@ndrix.org>
# Tue, 17 Aug 2021 09:41:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends     libtcmalloc-minimal4     libarchive13     libyaml-dev     libgmp10     libossp-uuid16     libssl1.1     ca-certificates     libdb5.3     libpcre3     libedit2     libgeos-c1v5     libspatialindex4v5     unixodbc     odbc-postgresql     tdsodbc     libmariadbclient18     libsqlite3-0     libserd-0-0     libraptor2-0 &&     dpkgArch="$(dpkg --print-architecture)" &&     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:41:29 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 10:28:15 GMT
RUN set -eux;     SWIPL_VER=8.2.4;     SWIPL_CHECKSUM=f4bcc78437f9080ab089762e9e6afa7071df7f584c14999b92b9a90a4efbd7d8;     BUILD_DEPS='make cmake ninja-build gcc g++ wget git autoconf libarchive-dev libgmp-dev libossp-uuid-dev libpcre3-dev libreadline-dev libedit-dev libssl-dev zlib1g-dev libdb-dev unixodbc-dev libsqlite3-dev libserd-dev libraptor2-dev libgeos++-dev libspatialindex-dev libgoogle-perftools-dev';     dpkgArch="$(dpkg --print-architecture)";     apt-get update; apt-get install -y --no-install-recommends $BUILD_DEPS; rm -rf /var/lib/apt/lists/*;     mkdir /tmp/src;     cd /tmp/src;     wget -q https://www.swi-prolog.org/download/stable/src/swipl-$SWIPL_VER.tar.gz;     echo "$SWIPL_CHECKSUM  swipl-$SWIPL_VER.tar.gz" >> swipl-$SWIPL_VER.tar.gz-CHECKSUM;     sha256sum -c swipl-$SWIPL_VER.tar.gz-CHECKSUM;     tar -xzf swipl-$SWIPL_VER.tar.gz;     mkdir swipl-$SWIPL_VER/build;     cd swipl-$SWIPL_VER/build;     cmake -DCMAKE_BUILD_TYPE=Release           -DSWIPL_PACKAGES_X=OFF 	  -DSWIPL_PACKAGES_JAVA=OFF 	  -DCMAKE_INSTALL_PREFIX=/usr 	  -G Ninja           ..;     ../scripts/pgo-compile.sh;     ninja;     ninja install;     rm -rf /tmp/src;     mkdir -p /usr/share/swi-prolog/pack;     cd /usr/share/swi-prolog/pack;     install_addin () {         git clone "$2" "$1";         git -C "$1" checkout -q "$3";         if [ "$1" = 'prosqlite' ]; then rm -rf "$1/lib"; fi;         swipl -g "pack_rebuild($1)" -t halt;         find "$1" -mindepth 1 -maxdepth 1 ! -name lib ! -name prolog ! -name pack.pl -exec rm -rf {} +;         find "$1" -name .git -exec rm -rf {} +;         find "$1" -name '*.so' -exec strip {} +;     };     dpkgArch="$(dpkg --print-architecture)";     install_addin space https://github.com/JanWielemaker/space.git cd6fefa63317a7a6effb61a1c5aee634ebe2ca05;     install_addin prosqlite https://github.com/nicos-angelopoulos/prosqlite.git cfd2f68709f5fb61833c0e2f8e9c6546e542009c;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] || install_addin rocksdb https://github.com/JanWielemaker/rocksdb.git f110766ee97cfbc6fddd4c33b7238f00e76ecc18;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] ||  install_addin hdt https://github.com/JanWielemaker/hdt.git e0a0eff87fc3318434cb493690c570e1255ed30e;     install_addin rserve_client https://github.com/JanWielemaker/rserve_client.git f8e83a4e1e4600baef4222dc4c2904a41a79a5ad;     apt-get purge -y --auto-remove $BUILD_DEPS
# Tue, 17 Aug 2021 10:28:16 GMT
CMD ["swipl"]
```

-	Layers:
	-	`sha256:33f99cea3b7da8c6e0143c9fd7590c6d56f7d310ddd59b11be4ad485ae4cab2a`  
		Last Modified: Tue, 17 Aug 2021 01:33:27 GMT  
		Size: 22.5 MB (22527748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e85f640db4abdf9e29f6550bd1443e98b32ad1665fb177c9cdaefa81b787ec5`  
		Last Modified: Tue, 17 Aug 2021 10:28:43 GMT  
		Size: 24.9 MB (24916406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaf6a6afb06aba7e6838aac7ba5e0d153c52e451c003063859aad62be235349`  
		Last Modified: Tue, 17 Aug 2021 10:28:54 GMT  
		Size: 8.8 MB (8834764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `swipl:8.2.4` - linux; arm variant v7

```console
$ docker pull swipl@sha256:138e37bed93e92604ea45cfc69e43757553a48cbec56a23770a265f7c2b5ace2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.4 MB (48395243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b362df7ac64629f990f90b140c67c8e60ee13b4cb191875eb01b4acec0bb648c`
-	Default Command: `["swipl"]`

```dockerfile
# Tue, 17 Aug 2021 02:19:36 GMT
ADD file:1719cfa11cf0f895b82719a2c082abb9f2d9b6dd6efc9e610e9732b97b31f56d in / 
# Tue, 17 Aug 2021 02:19:36 GMT
CMD ["bash"]
# Wed, 18 Aug 2021 02:16:54 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Michael Hendricks <michael@ndrix.org>
# Wed, 18 Aug 2021 02:17:30 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends     libtcmalloc-minimal4     libarchive13     libyaml-dev     libgmp10     libossp-uuid16     libssl1.1     ca-certificates     libdb5.3     libpcre3     libedit2     libgeos-c1v5     libspatialindex4v5     unixodbc     odbc-postgresql     tdsodbc     libmariadbclient18     libsqlite3-0     libserd-0-0     libraptor2-0 &&     dpkgArch="$(dpkg --print-architecture)" &&     rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 02:17:31 GMT
ENV LANG=C.UTF-8
# Wed, 18 Aug 2021 02:28:28 GMT
RUN set -eux;     SWIPL_VER=8.2.4;     SWIPL_CHECKSUM=f4bcc78437f9080ab089762e9e6afa7071df7f584c14999b92b9a90a4efbd7d8;     BUILD_DEPS='make cmake ninja-build gcc g++ wget git autoconf libarchive-dev libgmp-dev libossp-uuid-dev libpcre3-dev libreadline-dev libedit-dev libssl-dev zlib1g-dev libdb-dev unixodbc-dev libsqlite3-dev libserd-dev libraptor2-dev libgeos++-dev libspatialindex-dev libgoogle-perftools-dev';     dpkgArch="$(dpkg --print-architecture)";     apt-get update; apt-get install -y --no-install-recommends $BUILD_DEPS; rm -rf /var/lib/apt/lists/*;     mkdir /tmp/src;     cd /tmp/src;     wget -q https://www.swi-prolog.org/download/stable/src/swipl-$SWIPL_VER.tar.gz;     echo "$SWIPL_CHECKSUM  swipl-$SWIPL_VER.tar.gz" >> swipl-$SWIPL_VER.tar.gz-CHECKSUM;     sha256sum -c swipl-$SWIPL_VER.tar.gz-CHECKSUM;     tar -xzf swipl-$SWIPL_VER.tar.gz;     mkdir swipl-$SWIPL_VER/build;     cd swipl-$SWIPL_VER/build;     cmake -DCMAKE_BUILD_TYPE=Release           -DSWIPL_PACKAGES_X=OFF 	  -DSWIPL_PACKAGES_JAVA=OFF 	  -DCMAKE_INSTALL_PREFIX=/usr 	  -G Ninja           ..;     ../scripts/pgo-compile.sh;     ninja;     ninja install;     rm -rf /tmp/src;     mkdir -p /usr/share/swi-prolog/pack;     cd /usr/share/swi-prolog/pack;     install_addin () {         git clone "$2" "$1";         git -C "$1" checkout -q "$3";         if [ "$1" = 'prosqlite' ]; then rm -rf "$1/lib"; fi;         swipl -g "pack_rebuild($1)" -t halt;         find "$1" -mindepth 1 -maxdepth 1 ! -name lib ! -name prolog ! -name pack.pl -exec rm -rf {} +;         find "$1" -name .git -exec rm -rf {} +;         find "$1" -name '*.so' -exec strip {} +;     };     dpkgArch="$(dpkg --print-architecture)";     install_addin space https://github.com/JanWielemaker/space.git cd6fefa63317a7a6effb61a1c5aee634ebe2ca05;     install_addin prosqlite https://github.com/nicos-angelopoulos/prosqlite.git cfd2f68709f5fb61833c0e2f8e9c6546e542009c;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] || install_addin rocksdb https://github.com/JanWielemaker/rocksdb.git f110766ee97cfbc6fddd4c33b7238f00e76ecc18;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] ||  install_addin hdt https://github.com/JanWielemaker/hdt.git e0a0eff87fc3318434cb493690c570e1255ed30e;     install_addin rserve_client https://github.com/JanWielemaker/rserve_client.git f8e83a4e1e4600baef4222dc4c2904a41a79a5ad;     apt-get purge -y --auto-remove $BUILD_DEPS
# Wed, 18 Aug 2021 02:28:28 GMT
CMD ["swipl"]
```

-	Layers:
	-	`sha256:d1f994b3d26e717ce6c4ff9f7b5af7dbc4a4c831977d207f3ab47f213a8287e4`  
		Last Modified: Tue, 17 Aug 2021 02:36:57 GMT  
		Size: 19.3 MB (19316532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c21268258313a91c90a253dd732460e59ecb13cefbf4627756eea8b2c1c417`  
		Last Modified: Wed, 18 Aug 2021 02:29:21 GMT  
		Size: 22.9 MB (22885810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d01ee7d370abf8ca3634333401f7dc847e7e1e5b43380f416acfab48f33e220`  
		Last Modified: Wed, 18 Aug 2021 02:29:39 GMT  
		Size: 6.2 MB (6192901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `swipl:8.2.4` - linux; arm64 variant v8

```console
$ docker pull swipl@sha256:1d8e19b60b7a675013ec350d2ea188f740a1ebdd95f6c7875434db2e6c95587b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52712495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4e7f77d4c814ee8c5a62cc156e014719ced76ab002d04668043ba02cc42efe2`
-	Default Command: `["swipl"]`

```dockerfile
# Tue, 17 Aug 2021 01:48:32 GMT
ADD file:5cd26935234cc0540158a144066c0341b46a0caeb0a80db0355eeb8cfaf4fc0d in / 
# Tue, 17 Aug 2021 01:48:32 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 08:21:10 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Michael Hendricks <michael@ndrix.org>
# Tue, 17 Aug 2021 08:21:23 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends     libtcmalloc-minimal4     libarchive13     libyaml-dev     libgmp10     libossp-uuid16     libssl1.1     ca-certificates     libdb5.3     libpcre3     libedit2     libgeos-c1v5     libspatialindex4v5     unixodbc     odbc-postgresql     tdsodbc     libmariadbclient18     libsqlite3-0     libserd-0-0     libraptor2-0 &&     dpkgArch="$(dpkg --print-architecture)" &&     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 08:21:23 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 08:57:22 GMT
RUN set -eux;     SWIPL_VER=8.2.4;     SWIPL_CHECKSUM=f4bcc78437f9080ab089762e9e6afa7071df7f584c14999b92b9a90a4efbd7d8;     BUILD_DEPS='make cmake ninja-build gcc g++ wget git autoconf libarchive-dev libgmp-dev libossp-uuid-dev libpcre3-dev libreadline-dev libedit-dev libssl-dev zlib1g-dev libdb-dev unixodbc-dev libsqlite3-dev libserd-dev libraptor2-dev libgeos++-dev libspatialindex-dev libgoogle-perftools-dev';     dpkgArch="$(dpkg --print-architecture)";     apt-get update; apt-get install -y --no-install-recommends $BUILD_DEPS; rm -rf /var/lib/apt/lists/*;     mkdir /tmp/src;     cd /tmp/src;     wget -q https://www.swi-prolog.org/download/stable/src/swipl-$SWIPL_VER.tar.gz;     echo "$SWIPL_CHECKSUM  swipl-$SWIPL_VER.tar.gz" >> swipl-$SWIPL_VER.tar.gz-CHECKSUM;     sha256sum -c swipl-$SWIPL_VER.tar.gz-CHECKSUM;     tar -xzf swipl-$SWIPL_VER.tar.gz;     mkdir swipl-$SWIPL_VER/build;     cd swipl-$SWIPL_VER/build;     cmake -DCMAKE_BUILD_TYPE=Release           -DSWIPL_PACKAGES_X=OFF 	  -DSWIPL_PACKAGES_JAVA=OFF 	  -DCMAKE_INSTALL_PREFIX=/usr 	  -G Ninja           ..;     ../scripts/pgo-compile.sh;     ninja;     ninja install;     rm -rf /tmp/src;     mkdir -p /usr/share/swi-prolog/pack;     cd /usr/share/swi-prolog/pack;     install_addin () {         git clone "$2" "$1";         git -C "$1" checkout -q "$3";         if [ "$1" = 'prosqlite' ]; then rm -rf "$1/lib"; fi;         swipl -g "pack_rebuild($1)" -t halt;         find "$1" -mindepth 1 -maxdepth 1 ! -name lib ! -name prolog ! -name pack.pl -exec rm -rf {} +;         find "$1" -name .git -exec rm -rf {} +;         find "$1" -name '*.so' -exec strip {} +;     };     dpkgArch="$(dpkg --print-architecture)";     install_addin space https://github.com/JanWielemaker/space.git cd6fefa63317a7a6effb61a1c5aee634ebe2ca05;     install_addin prosqlite https://github.com/nicos-angelopoulos/prosqlite.git cfd2f68709f5fb61833c0e2f8e9c6546e542009c;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] || install_addin rocksdb https://github.com/JanWielemaker/rocksdb.git f110766ee97cfbc6fddd4c33b7238f00e76ecc18;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] ||  install_addin hdt https://github.com/JanWielemaker/hdt.git e0a0eff87fc3318434cb493690c570e1255ed30e;     install_addin rserve_client https://github.com/JanWielemaker/rserve_client.git f8e83a4e1e4600baef4222dc4c2904a41a79a5ad;     apt-get purge -y --auto-remove $BUILD_DEPS
# Tue, 17 Aug 2021 08:57:22 GMT
CMD ["swipl"]
```

-	Layers:
	-	`sha256:f862659192cd149f96ede75854bd3ebf59937831d3e4103087ae62df34ef1a29`  
		Last Modified: Tue, 17 Aug 2021 01:58:00 GMT  
		Size: 20.4 MB (20389447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8beb98d3b1ec04f952556f25e826cf5c6a4ea615fa9e736a5dcb072a06ea69`  
		Last Modified: Tue, 17 Aug 2021 08:57:47 GMT  
		Size: 23.8 MB (23758267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64679e4533072214d9f2286220168c09bdb2eb8647145d799d077d18a7f62ef`  
		Last Modified: Tue, 17 Aug 2021 08:57:59 GMT  
		Size: 8.6 MB (8564781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swipl:8.3.29`

```console
$ docker pull swipl@sha256:abaf3152b0b1bada16d4b99aa5fe9c4207034d1ba7e36b461063f531e6e58381
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `swipl:8.3.29` - linux; amd64

```console
$ docker pull swipl@sha256:148c8e0ff14e0b77ba9cd9db4ea3ea2914501a2d26560231126498e097b1610e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.6 MB (56601211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28089afa01487a996f7faaf2a2a1042d4421af1ac02ed40e60fa156d357d14b3`
-	Default Command: `["swipl"]`

```dockerfile
# Tue, 17 Aug 2021 01:26:09 GMT
ADD file:f6c4487fa1f7a4e17f5d88fd0c91031a6efc7fa210d363a1d43d8b0f3a8d1d03 in / 
# Tue, 17 Aug 2021 01:26:09 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:41:06 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Michael Hendricks <michael@ndrix.org>
# Tue, 17 Aug 2021 09:41:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends     libtcmalloc-minimal4     libarchive13     libyaml-dev     libgmp10     libossp-uuid16     libssl1.1     ca-certificates     libdb5.3     libpcre3     libedit2     libgeos-c1v5     libspatialindex4v5     unixodbc     odbc-postgresql     tdsodbc     libmariadbclient18     libsqlite3-0     libserd-0-0     libraptor2-0 &&     dpkgArch="$(dpkg --print-architecture)" &&     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:41:29 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 19:36:22 GMT
RUN set -eux;     SWIPL_VER=8.3.29;     SWIPL_CHECKSUM=4e15d8bde2d9da4fd504e17e10cbd7a7c3a77104972f10772396bad5015a9ee0;     BUILD_DEPS='make cmake ninja-build gcc g++ wget git autoconf libarchive-dev libgmp-dev libossp-uuid-dev libpcre3-dev libreadline-dev libedit-dev libssl-dev zlib1g-dev libdb-dev unixodbc-dev libsqlite3-dev libserd-dev libraptor2-dev libgeos++-dev libspatialindex-dev libgoogle-perftools-dev';     dpkgArch="$(dpkg --print-architecture)";     apt-get update; apt-get install -y --no-install-recommends $BUILD_DEPS; rm -rf /var/lib/apt/lists/*;     mkdir /tmp/src;     cd /tmp/src;     wget -q https://www.swi-prolog.org/download/devel/src/swipl-$SWIPL_VER.tar.gz;     echo "$SWIPL_CHECKSUM  swipl-$SWIPL_VER.tar.gz" >> swipl-$SWIPL_VER.tar.gz-CHECKSUM;     sha256sum -c swipl-$SWIPL_VER.tar.gz-CHECKSUM;     tar -xzf swipl-$SWIPL_VER.tar.gz;     mkdir swipl-$SWIPL_VER/build;     touch swipl-$SWIPL_VER/man/pl2xpce;     cd swipl-$SWIPL_VER/build;     cmake -DCMAKE_BUILD_TYPE=PGO           -DSWIPL_PACKAGES_X=OFF 	  -DSWIPL_PACKAGES_JAVA=OFF 	  -DCMAKE_INSTALL_PREFIX=/usr 	  -G Ninja           ..;     ninja;     ninja install;     rm -rf /tmp/src;     mkdir -p /usr/share/swi-prolog/pack;     cd /usr/share/swi-prolog/pack;     install_addin () {         git clone "$2" "$1";         git -C "$1" checkout -q "$3";         if [ "$1" = 'prosqlite' ]; then rm -rf "$1/lib"; fi;         swipl -g "pack_rebuild($1)" -t halt;         find "$1" -mindepth 1 -maxdepth 1 ! -name lib ! -name prolog ! -name pack.pl -exec rm -rf {} +;         find "$1" -name .git -exec rm -rf {} +;         find "$1" -name '*.so' -exec strip {} +;     };     dpkgArch="$(dpkg --print-architecture)";     install_addin space https://github.com/JanWielemaker/space.git cd6fefa63317a7a6effb61a1c5aee634ebe2ca05;     install_addin prosqlite https://github.com/nicos-angelopoulos/prosqlite.git cfd2f68709f5fb61833c0e2f8e9c6546e542009c;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] || install_addin rocksdb https://github.com/JanWielemaker/rocksdb.git f110766ee97cfbc6fddd4c33b7238f00e76ecc18;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] ||  install_addin hdt https://github.com/JanWielemaker/hdt.git e0a0eff87fc3318434cb493690c570e1255ed30e;     install_addin rserve_client https://github.com/JanWielemaker/rserve_client.git f8e83a4e1e4600baef4222dc4c2904a41a79a5ad;     apt-get purge -y --auto-remove $BUILD_DEPS
# Wed, 01 Sep 2021 19:36:22 GMT
CMD ["swipl"]
```

-	Layers:
	-	`sha256:33f99cea3b7da8c6e0143c9fd7590c6d56f7d310ddd59b11be4ad485ae4cab2a`  
		Last Modified: Tue, 17 Aug 2021 01:33:27 GMT  
		Size: 22.5 MB (22527748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e85f640db4abdf9e29f6550bd1443e98b32ad1665fb177c9cdaefa81b787ec5`  
		Last Modified: Tue, 17 Aug 2021 10:28:43 GMT  
		Size: 24.9 MB (24916406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e078f1e7b31d85f7b01ffee1a82ec6ad9f871c3dc51f0e5000d6c01f721c3260`  
		Last Modified: Wed, 01 Sep 2021 19:36:46 GMT  
		Size: 9.2 MB (9157057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `swipl:8.3.29` - linux; arm64 variant v8

```console
$ docker pull swipl@sha256:5c3d4d1e5c5169c2aef04b3e259bc2ff6fd7d21db8d01890874cb91ccfac9182
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (53038572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5edfd0f071fb0bc065cb08f0dc1c7ccbf1f9d0b9a1f8628b3fd278538235f7a0`
-	Default Command: `["swipl"]`

```dockerfile
# Tue, 17 Aug 2021 01:48:32 GMT
ADD file:5cd26935234cc0540158a144066c0341b46a0caeb0a80db0355eeb8cfaf4fc0d in / 
# Tue, 17 Aug 2021 01:48:32 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 08:21:10 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Michael Hendricks <michael@ndrix.org>
# Tue, 17 Aug 2021 08:21:23 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends     libtcmalloc-minimal4     libarchive13     libyaml-dev     libgmp10     libossp-uuid16     libssl1.1     ca-certificates     libdb5.3     libpcre3     libedit2     libgeos-c1v5     libspatialindex4v5     unixodbc     odbc-postgresql     tdsodbc     libmariadbclient18     libsqlite3-0     libserd-0-0     libraptor2-0 &&     dpkgArch="$(dpkg --print-architecture)" &&     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 08:21:23 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 19:57:43 GMT
RUN set -eux;     SWIPL_VER=8.3.29;     SWIPL_CHECKSUM=4e15d8bde2d9da4fd504e17e10cbd7a7c3a77104972f10772396bad5015a9ee0;     BUILD_DEPS='make cmake ninja-build gcc g++ wget git autoconf libarchive-dev libgmp-dev libossp-uuid-dev libpcre3-dev libreadline-dev libedit-dev libssl-dev zlib1g-dev libdb-dev unixodbc-dev libsqlite3-dev libserd-dev libraptor2-dev libgeos++-dev libspatialindex-dev libgoogle-perftools-dev';     dpkgArch="$(dpkg --print-architecture)";     apt-get update; apt-get install -y --no-install-recommends $BUILD_DEPS; rm -rf /var/lib/apt/lists/*;     mkdir /tmp/src;     cd /tmp/src;     wget -q https://www.swi-prolog.org/download/devel/src/swipl-$SWIPL_VER.tar.gz;     echo "$SWIPL_CHECKSUM  swipl-$SWIPL_VER.tar.gz" >> swipl-$SWIPL_VER.tar.gz-CHECKSUM;     sha256sum -c swipl-$SWIPL_VER.tar.gz-CHECKSUM;     tar -xzf swipl-$SWIPL_VER.tar.gz;     mkdir swipl-$SWIPL_VER/build;     touch swipl-$SWIPL_VER/man/pl2xpce;     cd swipl-$SWIPL_VER/build;     cmake -DCMAKE_BUILD_TYPE=PGO           -DSWIPL_PACKAGES_X=OFF 	  -DSWIPL_PACKAGES_JAVA=OFF 	  -DCMAKE_INSTALL_PREFIX=/usr 	  -G Ninja           ..;     ninja;     ninja install;     rm -rf /tmp/src;     mkdir -p /usr/share/swi-prolog/pack;     cd /usr/share/swi-prolog/pack;     install_addin () {         git clone "$2" "$1";         git -C "$1" checkout -q "$3";         if [ "$1" = 'prosqlite' ]; then rm -rf "$1/lib"; fi;         swipl -g "pack_rebuild($1)" -t halt;         find "$1" -mindepth 1 -maxdepth 1 ! -name lib ! -name prolog ! -name pack.pl -exec rm -rf {} +;         find "$1" -name .git -exec rm -rf {} +;         find "$1" -name '*.so' -exec strip {} +;     };     dpkgArch="$(dpkg --print-architecture)";     install_addin space https://github.com/JanWielemaker/space.git cd6fefa63317a7a6effb61a1c5aee634ebe2ca05;     install_addin prosqlite https://github.com/nicos-angelopoulos/prosqlite.git cfd2f68709f5fb61833c0e2f8e9c6546e542009c;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] || install_addin rocksdb https://github.com/JanWielemaker/rocksdb.git f110766ee97cfbc6fddd4c33b7238f00e76ecc18;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] ||  install_addin hdt https://github.com/JanWielemaker/hdt.git e0a0eff87fc3318434cb493690c570e1255ed30e;     install_addin rserve_client https://github.com/JanWielemaker/rserve_client.git f8e83a4e1e4600baef4222dc4c2904a41a79a5ad;     apt-get purge -y --auto-remove $BUILD_DEPS
# Wed, 01 Sep 2021 19:57:43 GMT
CMD ["swipl"]
```

-	Layers:
	-	`sha256:f862659192cd149f96ede75854bd3ebf59937831d3e4103087ae62df34ef1a29`  
		Last Modified: Tue, 17 Aug 2021 01:58:00 GMT  
		Size: 20.4 MB (20389447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8beb98d3b1ec04f952556f25e826cf5c6a4ea615fa9e736a5dcb072a06ea69`  
		Last Modified: Tue, 17 Aug 2021 08:57:47 GMT  
		Size: 23.8 MB (23758267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae843c475885f3309e9c2278b8776f69a65a5e42cede8669d0b3e08943571e50`  
		Last Modified: Wed, 01 Sep 2021 19:58:19 GMT  
		Size: 8.9 MB (8890858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swipl:latest`

```console
$ docker pull swipl@sha256:86bed406abb1288293e398e5228bc03487d0fa5129529e8d0dd077790bf32f88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `swipl:latest` - linux; amd64

```console
$ docker pull swipl@sha256:148c8e0ff14e0b77ba9cd9db4ea3ea2914501a2d26560231126498e097b1610e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.6 MB (56601211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28089afa01487a996f7faaf2a2a1042d4421af1ac02ed40e60fa156d357d14b3`
-	Default Command: `["swipl"]`

```dockerfile
# Tue, 17 Aug 2021 01:26:09 GMT
ADD file:f6c4487fa1f7a4e17f5d88fd0c91031a6efc7fa210d363a1d43d8b0f3a8d1d03 in / 
# Tue, 17 Aug 2021 01:26:09 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:41:06 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Michael Hendricks <michael@ndrix.org>
# Tue, 17 Aug 2021 09:41:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends     libtcmalloc-minimal4     libarchive13     libyaml-dev     libgmp10     libossp-uuid16     libssl1.1     ca-certificates     libdb5.3     libpcre3     libedit2     libgeos-c1v5     libspatialindex4v5     unixodbc     odbc-postgresql     tdsodbc     libmariadbclient18     libsqlite3-0     libserd-0-0     libraptor2-0 &&     dpkgArch="$(dpkg --print-architecture)" &&     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:41:29 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 19:36:22 GMT
RUN set -eux;     SWIPL_VER=8.3.29;     SWIPL_CHECKSUM=4e15d8bde2d9da4fd504e17e10cbd7a7c3a77104972f10772396bad5015a9ee0;     BUILD_DEPS='make cmake ninja-build gcc g++ wget git autoconf libarchive-dev libgmp-dev libossp-uuid-dev libpcre3-dev libreadline-dev libedit-dev libssl-dev zlib1g-dev libdb-dev unixodbc-dev libsqlite3-dev libserd-dev libraptor2-dev libgeos++-dev libspatialindex-dev libgoogle-perftools-dev';     dpkgArch="$(dpkg --print-architecture)";     apt-get update; apt-get install -y --no-install-recommends $BUILD_DEPS; rm -rf /var/lib/apt/lists/*;     mkdir /tmp/src;     cd /tmp/src;     wget -q https://www.swi-prolog.org/download/devel/src/swipl-$SWIPL_VER.tar.gz;     echo "$SWIPL_CHECKSUM  swipl-$SWIPL_VER.tar.gz" >> swipl-$SWIPL_VER.tar.gz-CHECKSUM;     sha256sum -c swipl-$SWIPL_VER.tar.gz-CHECKSUM;     tar -xzf swipl-$SWIPL_VER.tar.gz;     mkdir swipl-$SWIPL_VER/build;     touch swipl-$SWIPL_VER/man/pl2xpce;     cd swipl-$SWIPL_VER/build;     cmake -DCMAKE_BUILD_TYPE=PGO           -DSWIPL_PACKAGES_X=OFF 	  -DSWIPL_PACKAGES_JAVA=OFF 	  -DCMAKE_INSTALL_PREFIX=/usr 	  -G Ninja           ..;     ninja;     ninja install;     rm -rf /tmp/src;     mkdir -p /usr/share/swi-prolog/pack;     cd /usr/share/swi-prolog/pack;     install_addin () {         git clone "$2" "$1";         git -C "$1" checkout -q "$3";         if [ "$1" = 'prosqlite' ]; then rm -rf "$1/lib"; fi;         swipl -g "pack_rebuild($1)" -t halt;         find "$1" -mindepth 1 -maxdepth 1 ! -name lib ! -name prolog ! -name pack.pl -exec rm -rf {} +;         find "$1" -name .git -exec rm -rf {} +;         find "$1" -name '*.so' -exec strip {} +;     };     dpkgArch="$(dpkg --print-architecture)";     install_addin space https://github.com/JanWielemaker/space.git cd6fefa63317a7a6effb61a1c5aee634ebe2ca05;     install_addin prosqlite https://github.com/nicos-angelopoulos/prosqlite.git cfd2f68709f5fb61833c0e2f8e9c6546e542009c;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] || install_addin rocksdb https://github.com/JanWielemaker/rocksdb.git f110766ee97cfbc6fddd4c33b7238f00e76ecc18;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] ||  install_addin hdt https://github.com/JanWielemaker/hdt.git e0a0eff87fc3318434cb493690c570e1255ed30e;     install_addin rserve_client https://github.com/JanWielemaker/rserve_client.git f8e83a4e1e4600baef4222dc4c2904a41a79a5ad;     apt-get purge -y --auto-remove $BUILD_DEPS
# Wed, 01 Sep 2021 19:36:22 GMT
CMD ["swipl"]
```

-	Layers:
	-	`sha256:33f99cea3b7da8c6e0143c9fd7590c6d56f7d310ddd59b11be4ad485ae4cab2a`  
		Last Modified: Tue, 17 Aug 2021 01:33:27 GMT  
		Size: 22.5 MB (22527748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e85f640db4abdf9e29f6550bd1443e98b32ad1665fb177c9cdaefa81b787ec5`  
		Last Modified: Tue, 17 Aug 2021 10:28:43 GMT  
		Size: 24.9 MB (24916406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e078f1e7b31d85f7b01ffee1a82ec6ad9f871c3dc51f0e5000d6c01f721c3260`  
		Last Modified: Wed, 01 Sep 2021 19:36:46 GMT  
		Size: 9.2 MB (9157057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `swipl:latest` - linux; arm variant v7

```console
$ docker pull swipl@sha256:530fd948da8996808a5ef7116de7b7b97d3904c43d2ebf13f0c578a09a556457
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48591126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a00f42fd2c738469906a22c692d5912a221c7fe7294bd9051ce54a40064de60`
-	Default Command: `["swipl"]`

```dockerfile
# Tue, 17 Aug 2021 02:19:36 GMT
ADD file:1719cfa11cf0f895b82719a2c082abb9f2d9b6dd6efc9e610e9732b97b31f56d in / 
# Tue, 17 Aug 2021 02:19:36 GMT
CMD ["bash"]
# Wed, 18 Aug 2021 02:16:54 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Michael Hendricks <michael@ndrix.org>
# Wed, 18 Aug 2021 02:17:30 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends     libtcmalloc-minimal4     libarchive13     libyaml-dev     libgmp10     libossp-uuid16     libssl1.1     ca-certificates     libdb5.3     libpcre3     libedit2     libgeos-c1v5     libspatialindex4v5     unixodbc     odbc-postgresql     tdsodbc     libmariadbclient18     libsqlite3-0     libserd-0-0     libraptor2-0 &&     dpkgArch="$(dpkg --print-architecture)" &&     rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 02:17:31 GMT
ENV LANG=C.UTF-8
# Wed, 18 Aug 2021 02:22:47 GMT
RUN set -eux;     SWIPL_VER=8.3.26;     SWIPL_CHECKSUM=41d554d23137d2bedddf366ac43e0293068fd07f359f0e0546e771edb7a10962;     BUILD_DEPS='make cmake ninja-build gcc g++ wget git autoconf libarchive-dev libgmp-dev libossp-uuid-dev libpcre3-dev libreadline-dev libedit-dev libssl-dev zlib1g-dev libdb-dev unixodbc-dev libsqlite3-dev libserd-dev libraptor2-dev libgeos++-dev libspatialindex-dev libgoogle-perftools-dev';     dpkgArch="$(dpkg --print-architecture)";     apt-get update; apt-get install -y --no-install-recommends $BUILD_DEPS; rm -rf /var/lib/apt/lists/*;     mkdir /tmp/src;     cd /tmp/src;     wget -q https://www.swi-prolog.org/download/devel/src/swipl-$SWIPL_VER.tar.gz;     echo "$SWIPL_CHECKSUM  swipl-$SWIPL_VER.tar.gz" >> swipl-$SWIPL_VER.tar.gz-CHECKSUM;     sha256sum -c swipl-$SWIPL_VER.tar.gz-CHECKSUM;     tar -xzf swipl-$SWIPL_VER.tar.gz;     mkdir swipl-$SWIPL_VER/build;     cd swipl-$SWIPL_VER/build;     cmake -DCMAKE_BUILD_TYPE=Release           -DSWIPL_PACKAGES_X=OFF 	  -DSWIPL_PACKAGES_JAVA=OFF 	  -DCMAKE_INSTALL_PREFIX=/usr 	  -G Ninja           ..;     ../scripts/pgo-compile.sh;     ninja;     ninja install;     rm -rf /tmp/src;     mkdir -p /usr/share/swi-prolog/pack;     cd /usr/share/swi-prolog/pack;     install_addin () {         git clone "$2" "$1";         git -C "$1" checkout -q "$3";         if [ "$1" = 'prosqlite' ]; then rm -rf "$1/lib"; fi;         swipl -g "pack_rebuild($1)" -t halt;         find "$1" -mindepth 1 -maxdepth 1 ! -name lib ! -name prolog ! -name pack.pl -exec rm -rf {} +;         find "$1" -name .git -exec rm -rf {} +;         find "$1" -name '*.so' -exec strip {} +;     };     dpkgArch="$(dpkg --print-architecture)";     install_addin space https://github.com/JanWielemaker/space.git cd6fefa63317a7a6effb61a1c5aee634ebe2ca05;     install_addin prosqlite https://github.com/nicos-angelopoulos/prosqlite.git cfd2f68709f5fb61833c0e2f8e9c6546e542009c;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] || install_addin rocksdb https://github.com/JanWielemaker/rocksdb.git f110766ee97cfbc6fddd4c33b7238f00e76ecc18;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] ||  install_addin hdt https://github.com/JanWielemaker/hdt.git e0a0eff87fc3318434cb493690c570e1255ed30e;     install_addin rserve_client https://github.com/JanWielemaker/rserve_client.git f8e83a4e1e4600baef4222dc4c2904a41a79a5ad;     apt-get purge -y --auto-remove $BUILD_DEPS
# Wed, 18 Aug 2021 02:22:48 GMT
CMD ["swipl"]
```

-	Layers:
	-	`sha256:d1f994b3d26e717ce6c4ff9f7b5af7dbc4a4c831977d207f3ab47f213a8287e4`  
		Last Modified: Tue, 17 Aug 2021 02:36:57 GMT  
		Size: 19.3 MB (19316532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c21268258313a91c90a253dd732460e59ecb13cefbf4627756eea8b2c1c417`  
		Last Modified: Wed, 18 Aug 2021 02:29:21 GMT  
		Size: 22.9 MB (22885810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928b1d19df0617ba6965fd2028a6286d5c044dc91905db6b17bb2ba0e7027a54`  
		Last Modified: Wed, 18 Aug 2021 02:29:14 GMT  
		Size: 6.4 MB (6388784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `swipl:latest` - linux; arm64 variant v8

```console
$ docker pull swipl@sha256:5c3d4d1e5c5169c2aef04b3e259bc2ff6fd7d21db8d01890874cb91ccfac9182
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (53038572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5edfd0f071fb0bc065cb08f0dc1c7ccbf1f9d0b9a1f8628b3fd278538235f7a0`
-	Default Command: `["swipl"]`

```dockerfile
# Tue, 17 Aug 2021 01:48:32 GMT
ADD file:5cd26935234cc0540158a144066c0341b46a0caeb0a80db0355eeb8cfaf4fc0d in / 
# Tue, 17 Aug 2021 01:48:32 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 08:21:10 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Michael Hendricks <michael@ndrix.org>
# Tue, 17 Aug 2021 08:21:23 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends     libtcmalloc-minimal4     libarchive13     libyaml-dev     libgmp10     libossp-uuid16     libssl1.1     ca-certificates     libdb5.3     libpcre3     libedit2     libgeos-c1v5     libspatialindex4v5     unixodbc     odbc-postgresql     tdsodbc     libmariadbclient18     libsqlite3-0     libserd-0-0     libraptor2-0 &&     dpkgArch="$(dpkg --print-architecture)" &&     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 08:21:23 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 19:57:43 GMT
RUN set -eux;     SWIPL_VER=8.3.29;     SWIPL_CHECKSUM=4e15d8bde2d9da4fd504e17e10cbd7a7c3a77104972f10772396bad5015a9ee0;     BUILD_DEPS='make cmake ninja-build gcc g++ wget git autoconf libarchive-dev libgmp-dev libossp-uuid-dev libpcre3-dev libreadline-dev libedit-dev libssl-dev zlib1g-dev libdb-dev unixodbc-dev libsqlite3-dev libserd-dev libraptor2-dev libgeos++-dev libspatialindex-dev libgoogle-perftools-dev';     dpkgArch="$(dpkg --print-architecture)";     apt-get update; apt-get install -y --no-install-recommends $BUILD_DEPS; rm -rf /var/lib/apt/lists/*;     mkdir /tmp/src;     cd /tmp/src;     wget -q https://www.swi-prolog.org/download/devel/src/swipl-$SWIPL_VER.tar.gz;     echo "$SWIPL_CHECKSUM  swipl-$SWIPL_VER.tar.gz" >> swipl-$SWIPL_VER.tar.gz-CHECKSUM;     sha256sum -c swipl-$SWIPL_VER.tar.gz-CHECKSUM;     tar -xzf swipl-$SWIPL_VER.tar.gz;     mkdir swipl-$SWIPL_VER/build;     touch swipl-$SWIPL_VER/man/pl2xpce;     cd swipl-$SWIPL_VER/build;     cmake -DCMAKE_BUILD_TYPE=PGO           -DSWIPL_PACKAGES_X=OFF 	  -DSWIPL_PACKAGES_JAVA=OFF 	  -DCMAKE_INSTALL_PREFIX=/usr 	  -G Ninja           ..;     ninja;     ninja install;     rm -rf /tmp/src;     mkdir -p /usr/share/swi-prolog/pack;     cd /usr/share/swi-prolog/pack;     install_addin () {         git clone "$2" "$1";         git -C "$1" checkout -q "$3";         if [ "$1" = 'prosqlite' ]; then rm -rf "$1/lib"; fi;         swipl -g "pack_rebuild($1)" -t halt;         find "$1" -mindepth 1 -maxdepth 1 ! -name lib ! -name prolog ! -name pack.pl -exec rm -rf {} +;         find "$1" -name .git -exec rm -rf {} +;         find "$1" -name '*.so' -exec strip {} +;     };     dpkgArch="$(dpkg --print-architecture)";     install_addin space https://github.com/JanWielemaker/space.git cd6fefa63317a7a6effb61a1c5aee634ebe2ca05;     install_addin prosqlite https://github.com/nicos-angelopoulos/prosqlite.git cfd2f68709f5fb61833c0e2f8e9c6546e542009c;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] || install_addin rocksdb https://github.com/JanWielemaker/rocksdb.git f110766ee97cfbc6fddd4c33b7238f00e76ecc18;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] ||  install_addin hdt https://github.com/JanWielemaker/hdt.git e0a0eff87fc3318434cb493690c570e1255ed30e;     install_addin rserve_client https://github.com/JanWielemaker/rserve_client.git f8e83a4e1e4600baef4222dc4c2904a41a79a5ad;     apt-get purge -y --auto-remove $BUILD_DEPS
# Wed, 01 Sep 2021 19:57:43 GMT
CMD ["swipl"]
```

-	Layers:
	-	`sha256:f862659192cd149f96ede75854bd3ebf59937831d3e4103087ae62df34ef1a29`  
		Last Modified: Tue, 17 Aug 2021 01:58:00 GMT  
		Size: 20.4 MB (20389447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8beb98d3b1ec04f952556f25e826cf5c6a4ea615fa9e736a5dcb072a06ea69`  
		Last Modified: Tue, 17 Aug 2021 08:57:47 GMT  
		Size: 23.8 MB (23758267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae843c475885f3309e9c2278b8776f69a65a5e42cede8669d0b3e08943571e50`  
		Last Modified: Wed, 01 Sep 2021 19:58:19 GMT  
		Size: 8.9 MB (8890858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `swipl:stable`

```console
$ docker pull swipl@sha256:0ef14736125c5cd068eb22435b19c574e9e585de78896351f5577b753ed44c70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `swipl:stable` - linux; amd64

```console
$ docker pull swipl@sha256:a3de56b9f0c0b04355f6227a142c7619309efbbd6537867f73d4769e90fbc36d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.3 MB (56278918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c604a2fce7caaded8063e1b174a84105fe5273734016012b067975fa2d2c4b13`
-	Default Command: `["swipl"]`

```dockerfile
# Tue, 17 Aug 2021 01:26:09 GMT
ADD file:f6c4487fa1f7a4e17f5d88fd0c91031a6efc7fa210d363a1d43d8b0f3a8d1d03 in / 
# Tue, 17 Aug 2021 01:26:09 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:41:06 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Michael Hendricks <michael@ndrix.org>
# Tue, 17 Aug 2021 09:41:29 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends     libtcmalloc-minimal4     libarchive13     libyaml-dev     libgmp10     libossp-uuid16     libssl1.1     ca-certificates     libdb5.3     libpcre3     libedit2     libgeos-c1v5     libspatialindex4v5     unixodbc     odbc-postgresql     tdsodbc     libmariadbclient18     libsqlite3-0     libserd-0-0     libraptor2-0 &&     dpkgArch="$(dpkg --print-architecture)" &&     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:41:29 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 10:28:15 GMT
RUN set -eux;     SWIPL_VER=8.2.4;     SWIPL_CHECKSUM=f4bcc78437f9080ab089762e9e6afa7071df7f584c14999b92b9a90a4efbd7d8;     BUILD_DEPS='make cmake ninja-build gcc g++ wget git autoconf libarchive-dev libgmp-dev libossp-uuid-dev libpcre3-dev libreadline-dev libedit-dev libssl-dev zlib1g-dev libdb-dev unixodbc-dev libsqlite3-dev libserd-dev libraptor2-dev libgeos++-dev libspatialindex-dev libgoogle-perftools-dev';     dpkgArch="$(dpkg --print-architecture)";     apt-get update; apt-get install -y --no-install-recommends $BUILD_DEPS; rm -rf /var/lib/apt/lists/*;     mkdir /tmp/src;     cd /tmp/src;     wget -q https://www.swi-prolog.org/download/stable/src/swipl-$SWIPL_VER.tar.gz;     echo "$SWIPL_CHECKSUM  swipl-$SWIPL_VER.tar.gz" >> swipl-$SWIPL_VER.tar.gz-CHECKSUM;     sha256sum -c swipl-$SWIPL_VER.tar.gz-CHECKSUM;     tar -xzf swipl-$SWIPL_VER.tar.gz;     mkdir swipl-$SWIPL_VER/build;     cd swipl-$SWIPL_VER/build;     cmake -DCMAKE_BUILD_TYPE=Release           -DSWIPL_PACKAGES_X=OFF 	  -DSWIPL_PACKAGES_JAVA=OFF 	  -DCMAKE_INSTALL_PREFIX=/usr 	  -G Ninja           ..;     ../scripts/pgo-compile.sh;     ninja;     ninja install;     rm -rf /tmp/src;     mkdir -p /usr/share/swi-prolog/pack;     cd /usr/share/swi-prolog/pack;     install_addin () {         git clone "$2" "$1";         git -C "$1" checkout -q "$3";         if [ "$1" = 'prosqlite' ]; then rm -rf "$1/lib"; fi;         swipl -g "pack_rebuild($1)" -t halt;         find "$1" -mindepth 1 -maxdepth 1 ! -name lib ! -name prolog ! -name pack.pl -exec rm -rf {} +;         find "$1" -name .git -exec rm -rf {} +;         find "$1" -name '*.so' -exec strip {} +;     };     dpkgArch="$(dpkg --print-architecture)";     install_addin space https://github.com/JanWielemaker/space.git cd6fefa63317a7a6effb61a1c5aee634ebe2ca05;     install_addin prosqlite https://github.com/nicos-angelopoulos/prosqlite.git cfd2f68709f5fb61833c0e2f8e9c6546e542009c;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] || install_addin rocksdb https://github.com/JanWielemaker/rocksdb.git f110766ee97cfbc6fddd4c33b7238f00e76ecc18;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] ||  install_addin hdt https://github.com/JanWielemaker/hdt.git e0a0eff87fc3318434cb493690c570e1255ed30e;     install_addin rserve_client https://github.com/JanWielemaker/rserve_client.git f8e83a4e1e4600baef4222dc4c2904a41a79a5ad;     apt-get purge -y --auto-remove $BUILD_DEPS
# Tue, 17 Aug 2021 10:28:16 GMT
CMD ["swipl"]
```

-	Layers:
	-	`sha256:33f99cea3b7da8c6e0143c9fd7590c6d56f7d310ddd59b11be4ad485ae4cab2a`  
		Last Modified: Tue, 17 Aug 2021 01:33:27 GMT  
		Size: 22.5 MB (22527748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e85f640db4abdf9e29f6550bd1443e98b32ad1665fb177c9cdaefa81b787ec5`  
		Last Modified: Tue, 17 Aug 2021 10:28:43 GMT  
		Size: 24.9 MB (24916406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eaf6a6afb06aba7e6838aac7ba5e0d153c52e451c003063859aad62be235349`  
		Last Modified: Tue, 17 Aug 2021 10:28:54 GMT  
		Size: 8.8 MB (8834764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `swipl:stable` - linux; arm variant v7

```console
$ docker pull swipl@sha256:138e37bed93e92604ea45cfc69e43757553a48cbec56a23770a265f7c2b5ace2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.4 MB (48395243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b362df7ac64629f990f90b140c67c8e60ee13b4cb191875eb01b4acec0bb648c`
-	Default Command: `["swipl"]`

```dockerfile
# Tue, 17 Aug 2021 02:19:36 GMT
ADD file:1719cfa11cf0f895b82719a2c082abb9f2d9b6dd6efc9e610e9732b97b31f56d in / 
# Tue, 17 Aug 2021 02:19:36 GMT
CMD ["bash"]
# Wed, 18 Aug 2021 02:16:54 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Michael Hendricks <michael@ndrix.org>
# Wed, 18 Aug 2021 02:17:30 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends     libtcmalloc-minimal4     libarchive13     libyaml-dev     libgmp10     libossp-uuid16     libssl1.1     ca-certificates     libdb5.3     libpcre3     libedit2     libgeos-c1v5     libspatialindex4v5     unixodbc     odbc-postgresql     tdsodbc     libmariadbclient18     libsqlite3-0     libserd-0-0     libraptor2-0 &&     dpkgArch="$(dpkg --print-architecture)" &&     rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 02:17:31 GMT
ENV LANG=C.UTF-8
# Wed, 18 Aug 2021 02:28:28 GMT
RUN set -eux;     SWIPL_VER=8.2.4;     SWIPL_CHECKSUM=f4bcc78437f9080ab089762e9e6afa7071df7f584c14999b92b9a90a4efbd7d8;     BUILD_DEPS='make cmake ninja-build gcc g++ wget git autoconf libarchive-dev libgmp-dev libossp-uuid-dev libpcre3-dev libreadline-dev libedit-dev libssl-dev zlib1g-dev libdb-dev unixodbc-dev libsqlite3-dev libserd-dev libraptor2-dev libgeos++-dev libspatialindex-dev libgoogle-perftools-dev';     dpkgArch="$(dpkg --print-architecture)";     apt-get update; apt-get install -y --no-install-recommends $BUILD_DEPS; rm -rf /var/lib/apt/lists/*;     mkdir /tmp/src;     cd /tmp/src;     wget -q https://www.swi-prolog.org/download/stable/src/swipl-$SWIPL_VER.tar.gz;     echo "$SWIPL_CHECKSUM  swipl-$SWIPL_VER.tar.gz" >> swipl-$SWIPL_VER.tar.gz-CHECKSUM;     sha256sum -c swipl-$SWIPL_VER.tar.gz-CHECKSUM;     tar -xzf swipl-$SWIPL_VER.tar.gz;     mkdir swipl-$SWIPL_VER/build;     cd swipl-$SWIPL_VER/build;     cmake -DCMAKE_BUILD_TYPE=Release           -DSWIPL_PACKAGES_X=OFF 	  -DSWIPL_PACKAGES_JAVA=OFF 	  -DCMAKE_INSTALL_PREFIX=/usr 	  -G Ninja           ..;     ../scripts/pgo-compile.sh;     ninja;     ninja install;     rm -rf /tmp/src;     mkdir -p /usr/share/swi-prolog/pack;     cd /usr/share/swi-prolog/pack;     install_addin () {         git clone "$2" "$1";         git -C "$1" checkout -q "$3";         if [ "$1" = 'prosqlite' ]; then rm -rf "$1/lib"; fi;         swipl -g "pack_rebuild($1)" -t halt;         find "$1" -mindepth 1 -maxdepth 1 ! -name lib ! -name prolog ! -name pack.pl -exec rm -rf {} +;         find "$1" -name .git -exec rm -rf {} +;         find "$1" -name '*.so' -exec strip {} +;     };     dpkgArch="$(dpkg --print-architecture)";     install_addin space https://github.com/JanWielemaker/space.git cd6fefa63317a7a6effb61a1c5aee634ebe2ca05;     install_addin prosqlite https://github.com/nicos-angelopoulos/prosqlite.git cfd2f68709f5fb61833c0e2f8e9c6546e542009c;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] || install_addin rocksdb https://github.com/JanWielemaker/rocksdb.git f110766ee97cfbc6fddd4c33b7238f00e76ecc18;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] ||  install_addin hdt https://github.com/JanWielemaker/hdt.git e0a0eff87fc3318434cb493690c570e1255ed30e;     install_addin rserve_client https://github.com/JanWielemaker/rserve_client.git f8e83a4e1e4600baef4222dc4c2904a41a79a5ad;     apt-get purge -y --auto-remove $BUILD_DEPS
# Wed, 18 Aug 2021 02:28:28 GMT
CMD ["swipl"]
```

-	Layers:
	-	`sha256:d1f994b3d26e717ce6c4ff9f7b5af7dbc4a4c831977d207f3ab47f213a8287e4`  
		Last Modified: Tue, 17 Aug 2021 02:36:57 GMT  
		Size: 19.3 MB (19316532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c21268258313a91c90a253dd732460e59ecb13cefbf4627756eea8b2c1c417`  
		Last Modified: Wed, 18 Aug 2021 02:29:21 GMT  
		Size: 22.9 MB (22885810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d01ee7d370abf8ca3634333401f7dc847e7e1e5b43380f416acfab48f33e220`  
		Last Modified: Wed, 18 Aug 2021 02:29:39 GMT  
		Size: 6.2 MB (6192901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `swipl:stable` - linux; arm64 variant v8

```console
$ docker pull swipl@sha256:1d8e19b60b7a675013ec350d2ea188f740a1ebdd95f6c7875434db2e6c95587b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52712495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4e7f77d4c814ee8c5a62cc156e014719ced76ab002d04668043ba02cc42efe2`
-	Default Command: `["swipl"]`

```dockerfile
# Tue, 17 Aug 2021 01:48:32 GMT
ADD file:5cd26935234cc0540158a144066c0341b46a0caeb0a80db0355eeb8cfaf4fc0d in / 
# Tue, 17 Aug 2021 01:48:32 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 08:21:10 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Michael Hendricks <michael@ndrix.org>
# Tue, 17 Aug 2021 08:21:23 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends     libtcmalloc-minimal4     libarchive13     libyaml-dev     libgmp10     libossp-uuid16     libssl1.1     ca-certificates     libdb5.3     libpcre3     libedit2     libgeos-c1v5     libspatialindex4v5     unixodbc     odbc-postgresql     tdsodbc     libmariadbclient18     libsqlite3-0     libserd-0-0     libraptor2-0 &&     dpkgArch="$(dpkg --print-architecture)" &&     rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 08:21:23 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 08:57:22 GMT
RUN set -eux;     SWIPL_VER=8.2.4;     SWIPL_CHECKSUM=f4bcc78437f9080ab089762e9e6afa7071df7f584c14999b92b9a90a4efbd7d8;     BUILD_DEPS='make cmake ninja-build gcc g++ wget git autoconf libarchive-dev libgmp-dev libossp-uuid-dev libpcre3-dev libreadline-dev libedit-dev libssl-dev zlib1g-dev libdb-dev unixodbc-dev libsqlite3-dev libserd-dev libraptor2-dev libgeos++-dev libspatialindex-dev libgoogle-perftools-dev';     dpkgArch="$(dpkg --print-architecture)";     apt-get update; apt-get install -y --no-install-recommends $BUILD_DEPS; rm -rf /var/lib/apt/lists/*;     mkdir /tmp/src;     cd /tmp/src;     wget -q https://www.swi-prolog.org/download/stable/src/swipl-$SWIPL_VER.tar.gz;     echo "$SWIPL_CHECKSUM  swipl-$SWIPL_VER.tar.gz" >> swipl-$SWIPL_VER.tar.gz-CHECKSUM;     sha256sum -c swipl-$SWIPL_VER.tar.gz-CHECKSUM;     tar -xzf swipl-$SWIPL_VER.tar.gz;     mkdir swipl-$SWIPL_VER/build;     cd swipl-$SWIPL_VER/build;     cmake -DCMAKE_BUILD_TYPE=Release           -DSWIPL_PACKAGES_X=OFF 	  -DSWIPL_PACKAGES_JAVA=OFF 	  -DCMAKE_INSTALL_PREFIX=/usr 	  -G Ninja           ..;     ../scripts/pgo-compile.sh;     ninja;     ninja install;     rm -rf /tmp/src;     mkdir -p /usr/share/swi-prolog/pack;     cd /usr/share/swi-prolog/pack;     install_addin () {         git clone "$2" "$1";         git -C "$1" checkout -q "$3";         if [ "$1" = 'prosqlite' ]; then rm -rf "$1/lib"; fi;         swipl -g "pack_rebuild($1)" -t halt;         find "$1" -mindepth 1 -maxdepth 1 ! -name lib ! -name prolog ! -name pack.pl -exec rm -rf {} +;         find "$1" -name .git -exec rm -rf {} +;         find "$1" -name '*.so' -exec strip {} +;     };     dpkgArch="$(dpkg --print-architecture)";     install_addin space https://github.com/JanWielemaker/space.git cd6fefa63317a7a6effb61a1c5aee634ebe2ca05;     install_addin prosqlite https://github.com/nicos-angelopoulos/prosqlite.git cfd2f68709f5fb61833c0e2f8e9c6546e542009c;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] || install_addin rocksdb https://github.com/JanWielemaker/rocksdb.git f110766ee97cfbc6fddd4c33b7238f00e76ecc18;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] ||  install_addin hdt https://github.com/JanWielemaker/hdt.git e0a0eff87fc3318434cb493690c570e1255ed30e;     install_addin rserve_client https://github.com/JanWielemaker/rserve_client.git f8e83a4e1e4600baef4222dc4c2904a41a79a5ad;     apt-get purge -y --auto-remove $BUILD_DEPS
# Tue, 17 Aug 2021 08:57:22 GMT
CMD ["swipl"]
```

-	Layers:
	-	`sha256:f862659192cd149f96ede75854bd3ebf59937831d3e4103087ae62df34ef1a29`  
		Last Modified: Tue, 17 Aug 2021 01:58:00 GMT  
		Size: 20.4 MB (20389447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c8beb98d3b1ec04f952556f25e826cf5c6a4ea615fa9e736a5dcb072a06ea69`  
		Last Modified: Tue, 17 Aug 2021 08:57:47 GMT  
		Size: 23.8 MB (23758267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64679e4533072214d9f2286220168c09bdb2eb8647145d799d077d18a7f62ef`  
		Last Modified: Tue, 17 Aug 2021 08:57:59 GMT  
		Size: 8.6 MB (8564781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
