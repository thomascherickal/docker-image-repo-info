## `varnish:stable`

```console
$ docker pull varnish@sha256:ffe65dd8757f7104cfa4148aefc2b77a56f22de5ab61ac6d2ca253903bb82de2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:stable` - linux; amd64

```console
$ docker pull varnish@sha256:f84787c44f51490b7ea7bf67a6048e844c7a9774353c05b2a6c529c62cb1a94e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.7 MB (100663637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4bca53c1704593ccd3d858ae3a915f614618c93c59a19415fdc14df71e34795`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 25 Oct 2022 01:43:53 GMT
ADD file:8644a8156a07a656a35c41e2b2a458befb660309f8592e3efd5b43d46156cec2 in / 
# Tue, 25 Oct 2022 01:43:53 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:11:00 GMT
ENV VARNISH_SIZE=100M
# Tue, 08 Nov 2022 19:05:17 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 08 Nov 2022 19:05:18 GMT
WORKDIR /etc/varnish
# Tue, 08 Nov 2022 19:05:18 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 08 Nov 2022 19:05:18 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 08 Nov 2022 19:05:18 GMT
EXPOSE 80 8443
# Tue, 08 Nov 2022 19:05:18 GMT
CMD []
```

-	Layers:
	-	`sha256:e9995326b091af7b3ce352fad4d76cf3a3cb62b7a0c35cc5f625e8e649d23c50`  
		Last Modified: Tue, 25 Oct 2022 01:47:55 GMT  
		Size: 31.4 MB (31420038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5ad496d7a71d7b593efa3fce9fb020a9a451fb2159f7c2108422908d254a28`  
		Last Modified: Tue, 08 Nov 2022 19:07:24 GMT  
		Size: 69.2 MB (69242895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4a2f33a68ff8c5b56a754bced7d172554c01325fe2f4cb12f2716062e73b57`  
		Last Modified: Tue, 08 Nov 2022 19:07:14 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; arm variant v7

```console
$ docker pull varnish@sha256:c6081657b8c569f194c038f83a7abebf3292f82ffca752aecc4415d8cfdfbba6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.2 MB (77228629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dbd43d3dc19aba4ef18adb91746dfdcf113b4b6ce71d8aa73daccafd0497f67`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 25 Oct 2022 03:14:27 GMT
ADD file:0d2a17d07f391dfbf63c00d2b826373c98aaf6ab777481e33d4bee6d57c4a0b0 in / 
# Tue, 25 Oct 2022 03:14:27 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 04:27:40 GMT
ENV VARNISH_SIZE=100M
# Wed, 09 Nov 2022 01:53:55 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 09 Nov 2022 01:53:56 GMT
WORKDIR /etc/varnish
# Wed, 09 Nov 2022 01:53:56 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 09 Nov 2022 01:53:56 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 09 Nov 2022 01:53:56 GMT
EXPOSE 80 8443
# Wed, 09 Nov 2022 01:53:56 GMT
CMD []
```

-	Layers:
	-	`sha256:e96255deabf6ae29e08aa044ffd2843f7a10c579cc8207bf0ddf13a90d192020`  
		Last Modified: Tue, 25 Oct 2022 03:21:16 GMT  
		Size: 26.6 MB (26579293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b2919d9dd637413ea69cdb230202c8f2b284314a8af2b1bfc67c1ae733c972`  
		Last Modified: Wed, 09 Nov 2022 01:56:50 GMT  
		Size: 50.6 MB (50648633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ccc6cdd8c2a698556e4c4fee6925e62fe0a0cc5b164193842c05ef7acfdeef`  
		Last Modified: Wed, 09 Nov 2022 01:56:41 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:ef363a1dd52f79d491b019247dce68b39edfedaf84c38b351959369a02acc442
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94718130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ed8cc05677668508268410d1bc85b9d4e26fcc9f3aae3e1cc9519b5c06102ce`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 25 Oct 2022 05:46:02 GMT
ADD file:d3de9d6279224464018a7153274276a9969483d143046bebe898b59aeaf3a518 in / 
# Tue, 25 Oct 2022 05:46:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 23:47:20 GMT
ENV VARNISH_SIZE=100M
# Tue, 08 Nov 2022 22:37:32 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 08 Nov 2022 22:37:33 GMT
WORKDIR /etc/varnish
# Tue, 08 Nov 2022 22:37:33 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 08 Nov 2022 22:37:33 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 08 Nov 2022 22:37:33 GMT
EXPOSE 80 8443
# Tue, 08 Nov 2022 22:37:33 GMT
CMD []
```

-	Layers:
	-	`sha256:dd6189d6fc13cb03db0f4a3d9659b6b6044fd5858019d659001eaf8367584d67`  
		Last Modified: Tue, 25 Oct 2022 05:49:06 GMT  
		Size: 30.1 MB (30063910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686826a08c5ee39c557d280190b500585e578a3c9fdfa78cf7cb9c3e57f5a040`  
		Last Modified: Tue, 08 Nov 2022 22:38:40 GMT  
		Size: 64.7 MB (64653517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25765452792ea6ec745992826728658de192db3d01a49662119add8dd898f8b`  
		Last Modified: Tue, 08 Nov 2022 22:38:33 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; 386

```console
$ docker pull varnish@sha256:4827a6a0be673a0f3dd7a653df1b1e9e27609192bda2748c14c4d3d86c0dcc83
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.1 MB (102083500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91f5a8ca94f5063364fa40d7546cd491108bf6df618e3ff74878b781adbb82cc`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 25 Oct 2022 02:22:34 GMT
ADD file:14adaece72e410cf04ac21a101e5b530aab1d5e5a189a2be72d195ec0ac5e6d4 in / 
# Tue, 25 Oct 2022 02:22:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 11:40:24 GMT
ENV VARNISH_SIZE=100M
# Sat, 12 Nov 2022 07:32:52 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Sat, 12 Nov 2022 07:32:52 GMT
WORKDIR /etc/varnish
# Sat, 12 Nov 2022 07:32:54 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Sat, 12 Nov 2022 07:32:54 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 12 Nov 2022 07:32:55 GMT
EXPOSE 80 8443
# Sat, 12 Nov 2022 07:32:56 GMT
CMD []
```

-	Layers:
	-	`sha256:3c83067056c0f1bc4e162249831ac686f3a9a9c64c5366b903581580de8fcac2`  
		Last Modified: Tue, 25 Oct 2022 02:28:26 GMT  
		Size: 32.4 MB (32396384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e4374bb892b78048ce15826020f5b219c15203010a9da2f6c9b1018427220d`  
		Last Modified: Sat, 12 Nov 2022 07:34:01 GMT  
		Size: 69.7 MB (69686413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e152cf2e5632f3e117907da64d5eabb13fb3f318a57b2cdb6eb3f9bc361cdcc`  
		Last Modified: Sat, 12 Nov 2022 07:33:52 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; ppc64le

```console
$ docker pull varnish@sha256:24acf9650a4b390e96c2fcbe2201757ec6d1ea1d1c0a4ecd94a028aa7fbb8ed9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.8 MB (99797505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aefb468478a0f9522019340bcb793ea58ba088549f814677afe86fe2b16f108`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 25 Oct 2022 03:13:50 GMT
ADD file:1f622759c37363caaa6e6b14831ec9369303345c096f3a018eba66a620b08d26 in / 
# Tue, 25 Oct 2022 03:13:52 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 09:22:35 GMT
ENV VARNISH_SIZE=100M
# Tue, 08 Nov 2022 22:40:01 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 08 Nov 2022 22:40:03 GMT
WORKDIR /etc/varnish
# Tue, 08 Nov 2022 22:40:04 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 08 Nov 2022 22:40:04 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 08 Nov 2022 22:40:04 GMT
EXPOSE 80 8443
# Tue, 08 Nov 2022 22:40:05 GMT
CMD []
```

-	Layers:
	-	`sha256:6d95b62526dd55d76e7ec2bd4015a327b5bb37161f2ffe8bc2bb08d34a677716`  
		Last Modified: Tue, 25 Oct 2022 03:19:31 GMT  
		Size: 35.3 MB (35290086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74743ca672ecc5c3052a063c5b2bc2eeb2acd774c54429dcebe2e54926498e30`  
		Last Modified: Tue, 08 Nov 2022 22:41:49 GMT  
		Size: 64.5 MB (64506714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6c06b4fd620e922b4e65ddbc467fdd4607ad7bccbabce797c06043f26d81db`  
		Last Modified: Tue, 08 Nov 2022 22:41:32 GMT  
		Size: 705.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; s390x

```console
$ docker pull varnish@sha256:56696516e927843ee570d49b487dcdb1f9bafbf699840e0fae822be3dd18aa12
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.0 MB (81005557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95550e2a0ac2a5d356dc655f1647581ec5a19251dce32c794c912b034476c669`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 25 Oct 2022 01:14:42 GMT
ADD file:1bb8efa7f80e494b9d2831490a7e74810350c1f9ee2d100596d2e1cb4c62f529 in / 
# Tue, 25 Oct 2022 01:14:44 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:54:13 GMT
ENV VARNISH_SIZE=100M
# Wed, 09 Nov 2022 02:48:48 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.11.tgz -o $tmpdir/orig.tgz;     echo "02f56f360c6bbed663e712edef961384e6003cfe73307c7ea50f805ac4b4df0d26958179170401a2254a69ab623acc172da42926d82189bfa724a4e8a78597ea  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.11|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Wed, 09 Nov 2022 02:48:54 GMT
WORKDIR /etc/varnish
# Wed, 09 Nov 2022 02:48:54 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 09 Nov 2022 02:48:54 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 09 Nov 2022 02:48:54 GMT
EXPOSE 80 8443
# Wed, 09 Nov 2022 02:48:55 GMT
CMD []
```

-	Layers:
	-	`sha256:abc14eb2518761d53b91fc564a31b657914f96b531f99a74ac8268f0717b007e`  
		Last Modified: Tue, 25 Oct 2022 01:19:01 GMT  
		Size: 29.7 MB (29650722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bf98babac41805a02077e85c96ba677903d740abedcc9abeca31f7f7bbd222`  
		Last Modified: Wed, 09 Nov 2022 02:49:53 GMT  
		Size: 51.4 MB (51354131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5098ef7a4293fa1a4f3b8db1a8cede3d7b7ccbb423ecaed5149bc5af120d8b`  
		Last Modified: Wed, 09 Nov 2022 02:49:46 GMT  
		Size: 704.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
