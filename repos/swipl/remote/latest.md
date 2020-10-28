## `swipl:latest`

```console
$ docker pull swipl@sha256:3667688c4e884701323cb84c8dfc8be89a195a18a8ff2f39873c61384bc11f70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `swipl:latest` - linux; amd64

```console
$ docker pull swipl@sha256:fa0aa5ad0d414b1dfb072d4e6d44079db2bba5f1d70a362c5ddcf5673d4b1b60
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.2 MB (56227893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2756fb4fce12deca9e07a2fb3692b48c90735c4ebb05ba073b278ab8ecfdd53e`
-	Default Command: `["swipl"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:45 GMT
ADD file:4453535d387fcb17ead2026c72c05444e7558aa4736e3c0cdfb87cf20eaa5a9f in / 
# Tue, 13 Oct 2020 01:44:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 22:19:51 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Michael Hendricks <michael@ndrix.org>
# Tue, 13 Oct 2020 22:20:07 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends     libtcmalloc-minimal4     libarchive13     libyaml-dev     libgmp10     libossp-uuid16     libssl1.1     ca-certificates     libdb5.3     libpcre3     libedit2     libgeos-c1v5     libspatialindex4v5     unixodbc     odbc-postgresql     tdsodbc     libmariadbclient18     libsqlite3-0     libserd-0-0     libraptor2-0 &&     dpkgArch="$(dpkg --print-architecture)" &&     rm -rf /var/lib/apt/lists/*
# Wed, 28 Oct 2020 18:20:52 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 18:39:26 GMT
RUN set -eux;     SWIPL_VER=8.2.2;     SWIPL_CHECKSUM=35ca864cfd257e3e59ebe8f01e186f8959a8b4d42f17a9a6c04ecdfa5d1e164b;     BUILD_DEPS='make cmake ninja-build gcc g++ wget git autoconf libarchive-dev libgmp-dev libossp-uuid-dev libpcre3-dev libreadline-dev libedit-dev libssl-dev zlib1g-dev libdb-dev unixodbc-dev libsqlite3-dev libserd-dev libraptor2-dev libgeos++-dev libspatialindex-dev libgoogle-perftools-dev';     dpkgArch="$(dpkg --print-architecture)";     apt-get update; apt-get install -y --no-install-recommends $BUILD_DEPS; rm -rf /var/lib/apt/lists/*;     mkdir /tmp/src;     cd /tmp/src;     wget -q https://www.swi-prolog.org/download/stable/src/swipl-$SWIPL_VER.tar.gz;     echo "$SWIPL_CHECKSUM  swipl-$SWIPL_VER.tar.gz" >> swipl-$SWIPL_VER.tar.gz-CHECKSUM;     sha256sum -c swipl-$SWIPL_VER.tar.gz-CHECKSUM;     tar -xzf swipl-$SWIPL_VER.tar.gz;     mkdir swipl-$SWIPL_VER/build;     cd swipl-$SWIPL_VER/build;     cmake -DCMAKE_BUILD_TYPE=Release           -DSWIPL_PACKAGES_X=OFF 	  -DSWIPL_PACKAGES_JAVA=OFF 	  -DCMAKE_INSTALL_PREFIX=/usr 	  -G Ninja           ..;     ../scripts/pgo-compile.sh;     ninja;     ninja install;     rm -rf /tmp/src;     mkdir -p /usr/share/swi-prolog/pack;     cd /usr/share/swi-prolog/pack;     install_addin () {         git clone "$2" "$1";         git -C "$1" checkout -q "$3";         if [ "$1" = 'prosqlite' ]; then rm -rf "$1/lib"; fi;         swipl -g "pack_rebuild($1)" -t halt;         find "$1" -mindepth 1 -maxdepth 1 ! -name lib ! -name prolog ! -name pack.pl -exec rm -rf {} +;         find "$1" -name .git -exec rm -rf {} +;         find "$1" -name '*.so' -exec strip {} +;     };     dpkgArch="$(dpkg --print-architecture)";     install_addin space https://github.com/JanWielemaker/space.git cd6fefa63317a7a6effb61a1c5aee634ebe2ca05;     install_addin prosqlite https://github.com/nicos-angelopoulos/prosqlite.git cfd2f68709f5fb61833c0e2f8e9c6546e542009c;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] || install_addin rocksdb https://github.com/JanWielemaker/rocksdb.git f110766ee97cfbc6fddd4c33b7238f00e76ecc18;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] ||  install_addin hdt https://github.com/JanWielemaker/hdt.git e0a0eff87fc3318434cb493690c570e1255ed30e;     install_addin rserve_client https://github.com/JanWielemaker/rserve_client.git f8e83a4e1e4600baef4222dc4c2904a41a79a5ad;     apt-get purge -y --auto-remove $BUILD_DEPS
# Wed, 28 Oct 2020 18:39:27 GMT
CMD ["swipl"]
```

-	Layers:
	-	`sha256:babf97a3f00ae0a4d59c1a0f88918d8f7aa0f0758380258b2016f0cd17e97202`  
		Last Modified: Tue, 13 Oct 2020 01:51:03 GMT  
		Size: 22.5 MB (22522093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2a798fd94916786141463c4a57e34f752605ec873ba2a00c0b823e1b0c7315`  
		Last Modified: Tue, 13 Oct 2020 22:42:24 GMT  
		Size: 24.9 MB (24879827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be92d72fd49a91ee50f2a967d89893131dfa4970510c99fa88264a9f91918bd2`  
		Last Modified: Wed, 28 Oct 2020 18:39:46 GMT  
		Size: 8.8 MB (8825973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `swipl:latest` - linux; arm variant v7

```console
$ docker pull swipl@sha256:73a9a12d8b29ca0b363d02e588f0a64beee4d3f0cc0e5855d9240759689a0fdd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.3 MB (48343499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f28e73e4e5976503708181d3eef47a9c10ea20a4654c615ac71e56e54a30a4c`
-	Default Command: `["swipl"]`

```dockerfile
# Tue, 13 Oct 2020 01:04:30 GMT
ADD file:d204a257433edcd6f9ddd2c769b9e187c408eb4972203a5daab60214b5b576bc in / 
# Tue, 13 Oct 2020 01:04:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 19:34:23 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Michael Hendricks <michael@ndrix.org>
# Tue, 13 Oct 2020 19:35:24 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends     libtcmalloc-minimal4     libarchive13     libyaml-dev     libgmp10     libossp-uuid16     libssl1.1     ca-certificates     libdb5.3     libpcre3     libedit2     libgeos-c1v5     libspatialindex4v5     unixodbc     odbc-postgresql     tdsodbc     libmariadbclient18     libsqlite3-0     libserd-0-0     libraptor2-0 &&     dpkgArch="$(dpkg --print-architecture)" &&     rm -rf /var/lib/apt/lists/*
# Wed, 28 Oct 2020 18:06:57 GMT
ENV LANG=C.UTF-8
# Wed, 28 Oct 2020 18:11:37 GMT
RUN set -eux;     SWIPL_VER=8.2.2;     SWIPL_CHECKSUM=35ca864cfd257e3e59ebe8f01e186f8959a8b4d42f17a9a6c04ecdfa5d1e164b;     BUILD_DEPS='make cmake ninja-build gcc g++ wget git autoconf libarchive-dev libgmp-dev libossp-uuid-dev libpcre3-dev libreadline-dev libedit-dev libssl-dev zlib1g-dev libdb-dev unixodbc-dev libsqlite3-dev libserd-dev libraptor2-dev libgeos++-dev libspatialindex-dev libgoogle-perftools-dev';     dpkgArch="$(dpkg --print-architecture)";     apt-get update; apt-get install -y --no-install-recommends $BUILD_DEPS; rm -rf /var/lib/apt/lists/*;     mkdir /tmp/src;     cd /tmp/src;     wget -q https://www.swi-prolog.org/download/stable/src/swipl-$SWIPL_VER.tar.gz;     echo "$SWIPL_CHECKSUM  swipl-$SWIPL_VER.tar.gz" >> swipl-$SWIPL_VER.tar.gz-CHECKSUM;     sha256sum -c swipl-$SWIPL_VER.tar.gz-CHECKSUM;     tar -xzf swipl-$SWIPL_VER.tar.gz;     mkdir swipl-$SWIPL_VER/build;     cd swipl-$SWIPL_VER/build;     cmake -DCMAKE_BUILD_TYPE=Release           -DSWIPL_PACKAGES_X=OFF 	  -DSWIPL_PACKAGES_JAVA=OFF 	  -DCMAKE_INSTALL_PREFIX=/usr 	  -G Ninja           ..;     ../scripts/pgo-compile.sh;     ninja;     ninja install;     rm -rf /tmp/src;     mkdir -p /usr/share/swi-prolog/pack;     cd /usr/share/swi-prolog/pack;     install_addin () {         git clone "$2" "$1";         git -C "$1" checkout -q "$3";         if [ "$1" = 'prosqlite' ]; then rm -rf "$1/lib"; fi;         swipl -g "pack_rebuild($1)" -t halt;         find "$1" -mindepth 1 -maxdepth 1 ! -name lib ! -name prolog ! -name pack.pl -exec rm -rf {} +;         find "$1" -name .git -exec rm -rf {} +;         find "$1" -name '*.so' -exec strip {} +;     };     dpkgArch="$(dpkg --print-architecture)";     install_addin space https://github.com/JanWielemaker/space.git cd6fefa63317a7a6effb61a1c5aee634ebe2ca05;     install_addin prosqlite https://github.com/nicos-angelopoulos/prosqlite.git cfd2f68709f5fb61833c0e2f8e9c6546e542009c;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] || install_addin rocksdb https://github.com/JanWielemaker/rocksdb.git f110766ee97cfbc6fddd4c33b7238f00e76ecc18;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] ||  install_addin hdt https://github.com/JanWielemaker/hdt.git e0a0eff87fc3318434cb493690c570e1255ed30e;     install_addin rserve_client https://github.com/JanWielemaker/rserve_client.git f8e83a4e1e4600baef4222dc4c2904a41a79a5ad;     apt-get purge -y --auto-remove $BUILD_DEPS
# Wed, 28 Oct 2020 18:11:38 GMT
CMD ["swipl"]
```

-	Layers:
	-	`sha256:cc11be355171b10881b3ed16be16ceb2d7787cd459c6489d83bac55ee5824b35`  
		Last Modified: Tue, 13 Oct 2020 01:12:46 GMT  
		Size: 19.3 MB (19304540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6edb6a09248f1deb471bc643f50b41d86e1cc4617a6861e40fcce489655ec2fd`  
		Last Modified: Tue, 13 Oct 2020 19:42:05 GMT  
		Size: 22.9 MB (22861621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d0369800afb52ef78675f3b6f67e48fe4aea541c0db46c8137a70a2161ae59`  
		Last Modified: Wed, 28 Oct 2020 18:11:56 GMT  
		Size: 6.2 MB (6177338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `swipl:latest` - linux; arm64 variant v8

```console
$ docker pull swipl@sha256:b7eda684aeee1f2be9f7c331c44abfd71966b979f5b7c54d7bd599ed42386b43
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.6 MB (52581180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4f76e26c2b0431162079b2b0400fc1908ef3260aad102484da2f799762fea94`
-	Default Command: `["swipl"]`

```dockerfile
# Tue, 13 Oct 2020 01:44:21 GMT
ADD file:1783101ec41dba711940487fb45a9287f74a0639658051ad8bc9b2618a15be61 in / 
# Tue, 13 Oct 2020 01:44:22 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 18:40:15 GMT
LABEL maintainer=Dave Curylo <dave@curylo.org>, Michael Hendricks <michael@ndrix.org>
# Tue, 13 Oct 2020 18:41:03 GMT
RUN apt-get update &&     apt-get install -y --no-install-recommends     libtcmalloc-minimal4     libarchive13     libyaml-dev     libgmp10     libossp-uuid16     libssl1.1     ca-certificates     libdb5.3     libpcre3     libedit2     libgeos-c1v5     libspatialindex4v5     unixodbc     odbc-postgresql     tdsodbc     libmariadbclient18     libsqlite3-0     libserd-0-0     libraptor2-0 &&     dpkgArch="$(dpkg --print-architecture)" &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 19:14:18 GMT
RUN set -eux;     SWIPL_VER=8.2.0;     SWIPL_CHECKSUM=d8c9f3adb9cd997a5fed7b5f5dbfe971d2defda969b9066ada158e4202c09c3c;     BUILD_DEPS='make cmake ninja-build gcc g++ wget git autoconf libarchive-dev libgmp-dev libossp-uuid-dev libpcre3-dev libreadline-dev libedit-dev libssl-dev zlib1g-dev libdb-dev unixodbc-dev libsqlite3-dev libserd-dev libraptor2-dev libgeos++-dev libspatialindex-dev libgoogle-perftools-dev';     dpkgArch="$(dpkg --print-architecture)";     apt-get update; apt-get install -y --no-install-recommends $BUILD_DEPS; rm -rf /var/lib/apt/lists/*;     mkdir /tmp/src;     cd /tmp/src;     wget -q https://www.swi-prolog.org/download/stable/src/swipl-$SWIPL_VER.tar.gz;     echo "$SWIPL_CHECKSUM  swipl-$SWIPL_VER.tar.gz" >> swipl-$SWIPL_VER.tar.gz-CHECKSUM;     sha256sum -c swipl-$SWIPL_VER.tar.gz-CHECKSUM;     tar -xzf swipl-$SWIPL_VER.tar.gz;     mkdir swipl-$SWIPL_VER/build;     cd swipl-$SWIPL_VER/build;     cmake -DCMAKE_BUILD_TYPE=Release           -DSWIPL_PACKAGES_X=OFF 	  -DSWIPL_PACKAGES_JAVA=OFF 	  -DCMAKE_INSTALL_PREFIX=/usr 	  -G Ninja           ..;     LANG=C.UTF8 ../scripts/pgo-compile.sh;     LANG=C.UTF8 ninja;     LANG=C.UTF8 ninja install;     rm -rf /tmp/src;     mkdir -p /usr/share/swi-prolog/pack;     cd /usr/share/swi-prolog/pack;     install_addin () {         git clone "$2" "$1";         git -C "$1" checkout -q "$3";         if [ "$1" = 'prosqlite' ]; then rm -rf "$1/lib"; fi;         swipl -g "pack_rebuild($1)" -t halt;         find "$1" -mindepth 1 -maxdepth 1 ! -name lib ! -name prolog ! -name pack.pl -exec rm -rf {} +;         find "$1" -name .git -exec rm -rf {} +;         find "$1" -name '*.so' -exec strip {} +;     };     dpkgArch="$(dpkg --print-architecture)";     install_addin space https://github.com/JanWielemaker/space.git cd6fefa63317a7a6effb61a1c5aee634ebe2ca05;     install_addin prosqlite https://github.com/nicos-angelopoulos/prosqlite.git 816cb2e45a5fb53290a763a3306e430b72c40794;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] || install_addin rocksdb https://github.com/JanWielemaker/rocksdb.git f110766ee97cfbc6fddd4c33b7238f00e76ecc18;     [ "$dpkgArch" = 'armhf' ] || [ "$dpkgArch" = 'armel' ] ||  install_addin hdt https://github.com/JanWielemaker/hdt.git e0a0eff87fc3318434cb493690c570e1255ed30e;     install_addin rserve_client https://github.com/JanWielemaker/rserve_client.git 2af6c08fb1b59709dbc48b44f339b06f1217b4a5;     apt-get purge -y --auto-remove $BUILD_DEPS
# Tue, 13 Oct 2020 19:14:28 GMT
ENV LANG=C.UTF-8
# Tue, 13 Oct 2020 19:14:35 GMT
CMD ["swipl"]
```

-	Layers:
	-	`sha256:f4bec48cdb322f1180477bdd362bcd92d70a1ab628fc36319017bf4e8058d9ee`  
		Last Modified: Tue, 13 Oct 2020 01:51:12 GMT  
		Size: 20.4 MB (20376997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122cc8adb8198c9705ff7752c3e4b2f6db95cd84c210f19e5137b5c80d8b5e20`  
		Last Modified: Tue, 13 Oct 2020 19:14:56 GMT  
		Size: 23.7 MB (23739243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bbf58e8bb7d51aa6a59abb1b28329213a88e1ead48df659cd98faad3f0dd34`  
		Last Modified: Tue, 13 Oct 2020 19:14:52 GMT  
		Size: 8.5 MB (8464940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
