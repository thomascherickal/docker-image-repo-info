<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `varnish`

-	[`varnish:6.0`](#varnish60)
-	[`varnish:6.0.12`](#varnish6012)
-	[`varnish:7.3`](#varnish73)
-	[`varnish:7.3-alpine`](#varnish73-alpine)
-	[`varnish:7.3.1`](#varnish731)
-	[`varnish:7.3.1-alpine`](#varnish731-alpine)
-	[`varnish:7.4`](#varnish74)
-	[`varnish:7.4-alpine`](#varnish74-alpine)
-	[`varnish:7.4.2`](#varnish742)
-	[`varnish:7.4.2-alpine`](#varnish742-alpine)
-	[`varnish:alpine`](#varnishalpine)
-	[`varnish:fresh`](#varnishfresh)
-	[`varnish:fresh-alpine`](#varnishfresh-alpine)
-	[`varnish:latest`](#varnishlatest)
-	[`varnish:old`](#varnishold)
-	[`varnish:old-alpine`](#varnishold-alpine)
-	[`varnish:stable`](#varnishstable)

## `varnish:6.0`

```console
$ docker pull varnish@sha256:83a590c5be4d9e7bd66b7b90c78b786914a52661680ac88a7416cef15249d16b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:6.0` - linux; amd64

```console
$ docker pull varnish@sha256:b87136ceca6dbbb6c043856b46dc6f2868b19f8b590d6854b390c7299efc3943
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95851971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53f22488e835db5b05edaddd6831ee21b3d5abcc6c5ab96b5011ac4cb93a97ca`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 01:20:50 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Tue, 19 Dec 2023 01:20:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:05:59 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 08:07:40 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.12.tgz -o $tmpdir/orig.tgz;     echo "d80abb42380e85bc4be02278b3620b0a66d182465945146eecb2cdc022e77945ad815e897a5ed0bec2f458471617f647a80c743c0f72e73334ad92d3ac298af4  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.12|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 19 Dec 2023 08:07:40 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 08:07:40 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 19 Dec 2023 08:07:40 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 08:07:41 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 08:07:41 GMT
CMD []
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6eccc4b0a9abfc48ce57a783112f8f97d60f34816565535ed611d487b742d2`  
		Last Modified: Tue, 19 Dec 2023 08:09:01 GMT  
		Size: 64.4 MB (64433396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b919dc92685b5d4f6647a892025e8bdc664e1ab313fd22b26aadbe53f5f136bd`  
		Last Modified: Tue, 19 Dec 2023 08:08:53 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; arm variant v7

```console
$ docker pull varnish@sha256:b7a60981b3fc7fc22a6a065e5ea164928e3fc454e2acfc4ad830a29b4ce1d41e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72850985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5d33c2240e6f7289ba573e1d41811d6662ad39a5710f8973cea25ca2281559d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 02:08:09 GMT
ADD file:496e70a34ff4dabb4eefdf40e4e2f0563bea0c120bb43206f8f52ab5a887b637 in / 
# Tue, 19 Dec 2023 02:08:09 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:17:55 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 08:19:39 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.12.tgz -o $tmpdir/orig.tgz;     echo "d80abb42380e85bc4be02278b3620b0a66d182465945146eecb2cdc022e77945ad815e897a5ed0bec2f458471617f647a80c743c0f72e73334ad92d3ac298af4  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.12|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 19 Dec 2023 08:19:39 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 08:19:40 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 19 Dec 2023 08:19:40 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 08:19:40 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 08:19:40 GMT
CMD []
```

-	Layers:
	-	`sha256:19ccf4d6cc6956e4a5522352be94632923aa376a9939a4f45428a4f304c73bc8`  
		Last Modified: Tue, 19 Dec 2023 02:12:33 GMT  
		Size: 26.6 MB (26578972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105ed2a8f3cdbfeed8a77fff5c85b3bbfeeaf6ed56a514bafbca125b3e19b0e6`  
		Last Modified: Tue, 19 Dec 2023 08:20:49 GMT  
		Size: 46.3 MB (46271310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ddfe0f63afa45573e2077350d693f7508d0a5ac6e440990c4b23983848cfb6`  
		Last Modified: Tue, 19 Dec 2023 08:20:43 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:c66151b20502d18818ba7c51903d1a8742b3c23c1d148d8a6de6eb7d44fad343
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.9 MB (89947531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:642c464bc8bb3d14e8fafb63d1c048b2dc6c018d73d75cceb57fdf7a6cfeae8e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 21:21:40 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 21:23:04 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.12.tgz -o $tmpdir/orig.tgz;     echo "d80abb42380e85bc4be02278b3620b0a66d182465945146eecb2cdc022e77945ad815e897a5ed0bec2f458471617f647a80c743c0f72e73334ad92d3ac298af4  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.12|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 21 Nov 2023 21:23:04 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 21:23:04 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 21 Nov 2023 21:23:04 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 21:23:05 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 21:23:05 GMT
CMD []
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c54fe601a038c4d89325227f48596a94a4e44b39870a11399952782daa5f3c`  
		Last Modified: Tue, 21 Nov 2023 21:24:17 GMT  
		Size: 59.9 MB (59882708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f896890a1244055bc5bb66ea669ea2e0d1f6f6c82dcd1de073b3ef0885dc810f`  
		Last Modified: Tue, 21 Nov 2023 21:24:10 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; 386

```console
$ docker pull varnish@sha256:b842943e7429125c62902f678680031c957134e780aa6a48987613a05c2cbaa4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.1 MB (97117939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f96d47bae6ce87e0790321c40cc2ab5911bae135d4660b8588780fb7702b9ef4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 04:40:15 GMT
ADD file:7de881b584405a880c4d02778056aaa81bb5dd5d1af65b3086d66aed9ff0ad4b in / 
# Tue, 21 Nov 2023 04:40:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 15:18:48 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 15:20:59 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.12.tgz -o $tmpdir/orig.tgz;     echo "d80abb42380e85bc4be02278b3620b0a66d182465945146eecb2cdc022e77945ad815e897a5ed0bec2f458471617f647a80c743c0f72e73334ad92d3ac298af4  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.12|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 21 Nov 2023 15:21:00 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 15:21:00 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 21 Nov 2023 15:21:00 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 15:21:01 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 15:21:01 GMT
CMD []
```

-	Layers:
	-	`sha256:75c11612678b54e79a38118fe66e532c61b3d0798afb741007b4cd3209c0ec4e`  
		Last Modified: Tue, 21 Nov 2023 04:45:24 GMT  
		Size: 32.4 MB (32402632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92ff281c7632f3cc43de9266bd270b60c9947c71d8ecd4447a642432aa474a2`  
		Last Modified: Tue, 21 Nov 2023 15:22:37 GMT  
		Size: 64.7 MB (64714607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42e11325b795fce4ed6da4516d07a680b0fed89bf469efa769f3bdd733bdd505`  
		Last Modified: Tue, 21 Nov 2023 15:22:24 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; ppc64le

```console
$ docker pull varnish@sha256:eae28db647a78e9c81e7a12d56a54ddb38acc4196be62bd474fc6065f09c5260
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.6 MB (94635754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbb31ef67ecd67eeae948cbf7035f3a62f9b306540d58cfdfb8cf6e6544f6a5e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 04:24:43 GMT
ADD file:b0d18f2d04821eb50d1faecc1a64916f5c63dd386ae71a3b2cb1d6c4aac6e1c4 in / 
# Tue, 21 Nov 2023 04:24:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 12:58:32 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 13:01:18 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.12.tgz -o $tmpdir/orig.tgz;     echo "d80abb42380e85bc4be02278b3620b0a66d182465945146eecb2cdc022e77945ad815e897a5ed0bec2f458471617f647a80c743c0f72e73334ad92d3ac298af4  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.12|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 21 Nov 2023 13:01:21 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 13:01:21 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 21 Nov 2023 13:01:21 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 13:01:21 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 13:01:21 GMT
CMD []
```

-	Layers:
	-	`sha256:60239a74847cd7e9a928353188f3cf096ca8cf648e2b27c765058e169d568fd9`  
		Last Modified: Tue, 21 Nov 2023 04:29:47 GMT  
		Size: 35.3 MB (35293727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569c6d4e2d1dbb35d3b9ee83520833f8382e7eb87b7e6962c8d2e4c0be7806dd`  
		Last Modified: Tue, 21 Nov 2023 13:02:46 GMT  
		Size: 59.3 MB (59341325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448e034f0cac91c1eefcc5bec2f728aa50eb54a22d0abb010d4f5a8e3ad28047`  
		Last Modified: Tue, 21 Nov 2023 13:02:36 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0` - linux; s390x

```console
$ docker pull varnish@sha256:1afbcc817848afe7c42f083bf59bb6924839dbe7876bbd67969a4fe4138e0293
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76249533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e26b3d40fd7d0d13dd16d991a8913dbae2a3e5c7c1607b401be603ecacc8845`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 01:43:11 GMT
ADD file:36a070457acddafcd6cdda22a3c41efcbd4e2b1694831eb74c8143520ebf1cf2 in / 
# Tue, 19 Dec 2023 01:43:14 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 10:00:12 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 10:01:34 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.12.tgz -o $tmpdir/orig.tgz;     echo "d80abb42380e85bc4be02278b3620b0a66d182465945146eecb2cdc022e77945ad815e897a5ed0bec2f458471617f647a80c743c0f72e73334ad92d3ac298af4  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.12|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 19 Dec 2023 10:01:37 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 10:01:37 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 19 Dec 2023 10:01:37 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 10:01:37 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 10:01:37 GMT
CMD []
```

-	Layers:
	-	`sha256:eff2a4367cf88d5103011eba9299da2b4d173b0bde5dc0455020febf72b9b1c4`  
		Last Modified: Tue, 19 Dec 2023 01:48:08 GMT  
		Size: 29.7 MB (29657006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e08bddb91ea3ca1853adfc84a048668d647ae7fcde9dccca2f849a8b14f192`  
		Last Modified: Tue, 19 Dec 2023 10:02:47 GMT  
		Size: 46.6 MB (46591826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9818963852ea1e4abd0b87c001745b3c7ca8b6dfd2f9abf946875c1c50dc629`  
		Last Modified: Tue, 19 Dec 2023 10:02:41 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:6.0.12`

```console
$ docker pull varnish@sha256:83a590c5be4d9e7bd66b7b90c78b786914a52661680ac88a7416cef15249d16b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:6.0.12` - linux; amd64

```console
$ docker pull varnish@sha256:b87136ceca6dbbb6c043856b46dc6f2868b19f8b590d6854b390c7299efc3943
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95851971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53f22488e835db5b05edaddd6831ee21b3d5abcc6c5ab96b5011ac4cb93a97ca`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 01:20:50 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Tue, 19 Dec 2023 01:20:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:05:59 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 08:07:40 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.12.tgz -o $tmpdir/orig.tgz;     echo "d80abb42380e85bc4be02278b3620b0a66d182465945146eecb2cdc022e77945ad815e897a5ed0bec2f458471617f647a80c743c0f72e73334ad92d3ac298af4  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.12|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 19 Dec 2023 08:07:40 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 08:07:40 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 19 Dec 2023 08:07:40 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 08:07:41 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 08:07:41 GMT
CMD []
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6eccc4b0a9abfc48ce57a783112f8f97d60f34816565535ed611d487b742d2`  
		Last Modified: Tue, 19 Dec 2023 08:09:01 GMT  
		Size: 64.4 MB (64433396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b919dc92685b5d4f6647a892025e8bdc664e1ab313fd22b26aadbe53f5f136bd`  
		Last Modified: Tue, 19 Dec 2023 08:08:53 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.12` - linux; arm variant v7

```console
$ docker pull varnish@sha256:b7a60981b3fc7fc22a6a065e5ea164928e3fc454e2acfc4ad830a29b4ce1d41e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72850985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5d33c2240e6f7289ba573e1d41811d6662ad39a5710f8973cea25ca2281559d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 02:08:09 GMT
ADD file:496e70a34ff4dabb4eefdf40e4e2f0563bea0c120bb43206f8f52ab5a887b637 in / 
# Tue, 19 Dec 2023 02:08:09 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:17:55 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 08:19:39 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.12.tgz -o $tmpdir/orig.tgz;     echo "d80abb42380e85bc4be02278b3620b0a66d182465945146eecb2cdc022e77945ad815e897a5ed0bec2f458471617f647a80c743c0f72e73334ad92d3ac298af4  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.12|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 19 Dec 2023 08:19:39 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 08:19:40 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 19 Dec 2023 08:19:40 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 08:19:40 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 08:19:40 GMT
CMD []
```

-	Layers:
	-	`sha256:19ccf4d6cc6956e4a5522352be94632923aa376a9939a4f45428a4f304c73bc8`  
		Last Modified: Tue, 19 Dec 2023 02:12:33 GMT  
		Size: 26.6 MB (26578972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105ed2a8f3cdbfeed8a77fff5c85b3bbfeeaf6ed56a514bafbca125b3e19b0e6`  
		Last Modified: Tue, 19 Dec 2023 08:20:49 GMT  
		Size: 46.3 MB (46271310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ddfe0f63afa45573e2077350d693f7508d0a5ac6e440990c4b23983848cfb6`  
		Last Modified: Tue, 19 Dec 2023 08:20:43 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.12` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:c66151b20502d18818ba7c51903d1a8742b3c23c1d148d8a6de6eb7d44fad343
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.9 MB (89947531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:642c464bc8bb3d14e8fafb63d1c048b2dc6c018d73d75cceb57fdf7a6cfeae8e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 21:21:40 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 21:23:04 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.12.tgz -o $tmpdir/orig.tgz;     echo "d80abb42380e85bc4be02278b3620b0a66d182465945146eecb2cdc022e77945ad815e897a5ed0bec2f458471617f647a80c743c0f72e73334ad92d3ac298af4  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.12|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 21 Nov 2023 21:23:04 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 21:23:04 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 21 Nov 2023 21:23:04 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 21:23:05 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 21:23:05 GMT
CMD []
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c54fe601a038c4d89325227f48596a94a4e44b39870a11399952782daa5f3c`  
		Last Modified: Tue, 21 Nov 2023 21:24:17 GMT  
		Size: 59.9 MB (59882708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f896890a1244055bc5bb66ea669ea2e0d1f6f6c82dcd1de073b3ef0885dc810f`  
		Last Modified: Tue, 21 Nov 2023 21:24:10 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.12` - linux; 386

```console
$ docker pull varnish@sha256:b842943e7429125c62902f678680031c957134e780aa6a48987613a05c2cbaa4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.1 MB (97117939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f96d47bae6ce87e0790321c40cc2ab5911bae135d4660b8588780fb7702b9ef4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 04:40:15 GMT
ADD file:7de881b584405a880c4d02778056aaa81bb5dd5d1af65b3086d66aed9ff0ad4b in / 
# Tue, 21 Nov 2023 04:40:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 15:18:48 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 15:20:59 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.12.tgz -o $tmpdir/orig.tgz;     echo "d80abb42380e85bc4be02278b3620b0a66d182465945146eecb2cdc022e77945ad815e897a5ed0bec2f458471617f647a80c743c0f72e73334ad92d3ac298af4  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.12|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 21 Nov 2023 15:21:00 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 15:21:00 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 21 Nov 2023 15:21:00 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 15:21:01 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 15:21:01 GMT
CMD []
```

-	Layers:
	-	`sha256:75c11612678b54e79a38118fe66e532c61b3d0798afb741007b4cd3209c0ec4e`  
		Last Modified: Tue, 21 Nov 2023 04:45:24 GMT  
		Size: 32.4 MB (32402632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92ff281c7632f3cc43de9266bd270b60c9947c71d8ecd4447a642432aa474a2`  
		Last Modified: Tue, 21 Nov 2023 15:22:37 GMT  
		Size: 64.7 MB (64714607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42e11325b795fce4ed6da4516d07a680b0fed89bf469efa769f3bdd733bdd505`  
		Last Modified: Tue, 21 Nov 2023 15:22:24 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.12` - linux; ppc64le

```console
$ docker pull varnish@sha256:eae28db647a78e9c81e7a12d56a54ddb38acc4196be62bd474fc6065f09c5260
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.6 MB (94635754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbb31ef67ecd67eeae948cbf7035f3a62f9b306540d58cfdfb8cf6e6544f6a5e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 04:24:43 GMT
ADD file:b0d18f2d04821eb50d1faecc1a64916f5c63dd386ae71a3b2cb1d6c4aac6e1c4 in / 
# Tue, 21 Nov 2023 04:24:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 12:58:32 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 13:01:18 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.12.tgz -o $tmpdir/orig.tgz;     echo "d80abb42380e85bc4be02278b3620b0a66d182465945146eecb2cdc022e77945ad815e897a5ed0bec2f458471617f647a80c743c0f72e73334ad92d3ac298af4  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.12|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 21 Nov 2023 13:01:21 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 13:01:21 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 21 Nov 2023 13:01:21 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 13:01:21 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 13:01:21 GMT
CMD []
```

-	Layers:
	-	`sha256:60239a74847cd7e9a928353188f3cf096ca8cf648e2b27c765058e169d568fd9`  
		Last Modified: Tue, 21 Nov 2023 04:29:47 GMT  
		Size: 35.3 MB (35293727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569c6d4e2d1dbb35d3b9ee83520833f8382e7eb87b7e6962c8d2e4c0be7806dd`  
		Last Modified: Tue, 21 Nov 2023 13:02:46 GMT  
		Size: 59.3 MB (59341325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448e034f0cac91c1eefcc5bec2f728aa50eb54a22d0abb010d4f5a8e3ad28047`  
		Last Modified: Tue, 21 Nov 2023 13:02:36 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:6.0.12` - linux; s390x

```console
$ docker pull varnish@sha256:1afbcc817848afe7c42f083bf59bb6924839dbe7876bbd67969a4fe4138e0293
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76249533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e26b3d40fd7d0d13dd16d991a8913dbae2a3e5c7c1607b401be603ecacc8845`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 01:43:11 GMT
ADD file:36a070457acddafcd6cdda22a3c41efcbd4e2b1694831eb74c8143520ebf1cf2 in / 
# Tue, 19 Dec 2023 01:43:14 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 10:00:12 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 10:01:34 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.12.tgz -o $tmpdir/orig.tgz;     echo "d80abb42380e85bc4be02278b3620b0a66d182465945146eecb2cdc022e77945ad815e897a5ed0bec2f458471617f647a80c743c0f72e73334ad92d3ac298af4  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.12|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 19 Dec 2023 10:01:37 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 10:01:37 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 19 Dec 2023 10:01:37 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 10:01:37 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 10:01:37 GMT
CMD []
```

-	Layers:
	-	`sha256:eff2a4367cf88d5103011eba9299da2b4d173b0bde5dc0455020febf72b9b1c4`  
		Last Modified: Tue, 19 Dec 2023 01:48:08 GMT  
		Size: 29.7 MB (29657006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e08bddb91ea3ca1853adfc84a048668d647ae7fcde9dccca2f849a8b14f192`  
		Last Modified: Tue, 19 Dec 2023 10:02:47 GMT  
		Size: 46.6 MB (46591826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9818963852ea1e4abd0b87c001745b3c7ca8b6dfd2f9abf946875c1c50dc629`  
		Last Modified: Tue, 19 Dec 2023 10:02:41 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.3`

```console
$ docker pull varnish@sha256:87dffb5c48c83cdcf12a3efeb6457d9e178f29604494e32b51701e1b2aa27cb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.3` - linux; amd64

```console
$ docker pull varnish@sha256:df9b1ecb6e4ca0e98f9dbdf680885e16c7e510e2de4ddabc59ae2982e8c8cf99
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101966885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac6fda6c72241a94c1e31ff26a39609231e0b895e083619d8286a89b39030028`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 01:20:50 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Tue, 19 Dec 2023 01:20:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:03:02 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 19 Dec 2023 08:03:02 GMT
ARG VARNISH_VERSION=7.3.1
# Tue, 19 Dec 2023 08:03:02 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Tue, 19 Dec 2023 08:03:03 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 19 Dec 2023 08:03:03 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 19 Dec 2023 08:03:03 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 19 Dec 2023 08:03:03 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 19 Dec 2023 08:03:03 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 19 Dec 2023 08:03:03 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 19 Dec 2023 08:03:03 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 19 Dec 2023 08:03:03 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 08:05:41 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.1.tgz -o $tmpdir/orig.tgz;     echo "57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 19 Dec 2023 08:05:42 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 08:05:42 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 19 Dec 2023 08:05:42 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 08:05:42 GMT
USER varnish
# Tue, 19 Dec 2023 08:05:42 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 08:05:42 GMT
CMD []
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e37b9699670384020e902a0ae2f3c71ef125515c77fb7f57f956fe2ab064bc8`  
		Last Modified: Tue, 19 Dec 2023 08:08:41 GMT  
		Size: 70.5 MB (70548520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbc9ee7e56bac88b0277ca7cd2409fa0ea1152bcdf965d290cd039497678c49`  
		Last Modified: Tue, 19 Dec 2023 08:08:32 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3` - linux; arm variant v7

```console
$ docker pull varnish@sha256:ad549d82c4744321f31d836fa2757228ec9c6ee28a2fe56905d8606424ce55f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.8 MB (78751981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:580eedff14a9163d5717e74e0654d277448fd09bed4c6672badbf8cbbd32236f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 02:08:09 GMT
ADD file:496e70a34ff4dabb4eefdf40e4e2f0563bea0c120bb43206f8f52ab5a887b637 in / 
# Tue, 19 Dec 2023 02:08:09 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:15:00 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 19 Dec 2023 08:15:00 GMT
ARG VARNISH_VERSION=7.3.1
# Tue, 19 Dec 2023 08:15:00 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Tue, 19 Dec 2023 08:15:00 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 19 Dec 2023 08:15:01 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 19 Dec 2023 08:15:01 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 19 Dec 2023 08:15:01 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 19 Dec 2023 08:15:01 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 19 Dec 2023 08:15:01 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 19 Dec 2023 08:15:01 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 19 Dec 2023 08:15:01 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 08:17:37 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.1.tgz -o $tmpdir/orig.tgz;     echo "57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 19 Dec 2023 08:17:37 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 08:17:37 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 19 Dec 2023 08:17:38 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 08:17:38 GMT
USER varnish
# Tue, 19 Dec 2023 08:17:38 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 08:17:38 GMT
CMD []
```

-	Layers:
	-	`sha256:19ccf4d6cc6956e4a5522352be94632923aa376a9939a4f45428a4f304c73bc8`  
		Last Modified: Tue, 19 Dec 2023 02:12:33 GMT  
		Size: 26.6 MB (26578972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8d700fb01496fa8c844f9ebb7e2c0de1106588b482a0aef5209b031c470c89`  
		Last Modified: Tue, 19 Dec 2023 08:20:32 GMT  
		Size: 52.2 MB (52172516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa853700f1de2e0c582912f1a2175a3c69c30b2cd96cf0db35fb599a9d9bd9c7`  
		Last Modified: Tue, 19 Dec 2023 08:20:25 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:32014d110bbaffe0743bdc54c6c9d439532cf91ad71fbcdbdb7ae00779b18d62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.8 MB (95781809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66a11569b230dc214d07fcb99a041dcdfe426ea3ca30a6c31410230131217503`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 21:19:16 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 21 Nov 2023 21:19:16 GMT
ARG VARNISH_VERSION=7.3.1
# Tue, 21 Nov 2023 21:19:16 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Tue, 21 Nov 2023 21:19:16 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 21 Nov 2023 21:19:16 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 21 Nov 2023 21:19:16 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 21 Nov 2023 21:19:16 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 21 Nov 2023 21:19:16 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 21 Nov 2023 21:19:16 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 21 Nov 2023 21:19:16 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 21 Nov 2023 21:19:16 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 21:21:25 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.1.tgz -o $tmpdir/orig.tgz;     echo "57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 21 Nov 2023 21:21:26 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 21:21:26 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 21 Nov 2023 21:21:26 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 21:21:26 GMT
USER varnish
# Tue, 21 Nov 2023 21:21:26 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 21:21:26 GMT
CMD []
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc98e65c086f4b548a2e982f49352b25a0cd9922c2f9a98330b42163385f0d4`  
		Last Modified: Tue, 21 Nov 2023 21:23:59 GMT  
		Size: 65.7 MB (65717192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff1904762c1d07cd5329fe0e393c0598fdbac6a204808c4e326bd44f6f505eb`  
		Last Modified: Tue, 21 Nov 2023 21:23:52 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3` - linux; 386

```console
$ docker pull varnish@sha256:522eb24b5d28a7295ce65f1086e33d5d85beaf7c9c65b3c60759498baeb3d4e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.2 MB (103212796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b70fc90e400e9dfbd466ceab45b7e7287a51be25ddbbc35bb9b1668978ffda0d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 04:40:15 GMT
ADD file:7de881b584405a880c4d02778056aaa81bb5dd5d1af65b3086d66aed9ff0ad4b in / 
# Tue, 21 Nov 2023 04:40:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 15:15:08 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 21 Nov 2023 15:15:08 GMT
ARG VARNISH_VERSION=7.3.1
# Tue, 21 Nov 2023 15:15:08 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Tue, 21 Nov 2023 15:15:08 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 21 Nov 2023 15:15:09 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 21 Nov 2023 15:15:09 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 21 Nov 2023 15:15:09 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 21 Nov 2023 15:15:09 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 21 Nov 2023 15:15:09 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 21 Nov 2023 15:15:09 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 21 Nov 2023 15:15:09 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 15:18:32 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.1.tgz -o $tmpdir/orig.tgz;     echo "57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 21 Nov 2023 15:18:33 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 15:18:33 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 21 Nov 2023 15:18:33 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 15:18:34 GMT
USER varnish
# Tue, 21 Nov 2023 15:18:34 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 15:18:34 GMT
CMD []
```

-	Layers:
	-	`sha256:75c11612678b54e79a38118fe66e532c61b3d0798afb741007b4cd3209c0ec4e`  
		Last Modified: Tue, 21 Nov 2023 04:45:24 GMT  
		Size: 32.4 MB (32402632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae3bc414da66bdd2d32a046a233e988a45ad7faaa11b96e0f5e55973fa16073`  
		Last Modified: Tue, 21 Nov 2023 15:22:12 GMT  
		Size: 70.8 MB (70809672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d549858933a493ec89c83cb3fafe3fec83022f9eae66525cdcbdf30fc7e49c92`  
		Last Modified: Tue, 21 Nov 2023 15:21:58 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3` - linux; ppc64le

```console
$ docker pull varnish@sha256:66a0133569e260a895c68333c0426c77cdaa6c2f4dcb29b8f24906c16932c150
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.9 MB (100887371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc4919272c647cb21a3aee48eb9f1a2e0a70f042c7da2e16ef2463f7cf62433b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 04:24:43 GMT
ADD file:b0d18f2d04821eb50d1faecc1a64916f5c63dd386ae71a3b2cb1d6c4aac6e1c4 in / 
# Tue, 21 Nov 2023 04:24:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 12:54:35 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 21 Nov 2023 12:54:35 GMT
ARG VARNISH_VERSION=7.3.1
# Tue, 21 Nov 2023 12:54:36 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Tue, 21 Nov 2023 12:54:36 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 21 Nov 2023 12:54:36 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 21 Nov 2023 12:54:37 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 21 Nov 2023 12:54:37 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 21 Nov 2023 12:54:37 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 21 Nov 2023 12:54:37 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 21 Nov 2023 12:54:38 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 21 Nov 2023 12:54:38 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 12:58:17 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.1.tgz -o $tmpdir/orig.tgz;     echo "57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 21 Nov 2023 12:58:19 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 12:58:19 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 21 Nov 2023 12:58:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 12:58:20 GMT
USER varnish
# Tue, 21 Nov 2023 12:58:20 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 12:58:20 GMT
CMD []
```

-	Layers:
	-	`sha256:60239a74847cd7e9a928353188f3cf096ca8cf648e2b27c765058e169d568fd9`  
		Last Modified: Tue, 21 Nov 2023 04:29:47 GMT  
		Size: 35.3 MB (35293727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef474112e53d3cd9414bbc58b355c42c87c37b9296900ac553800b9812b43a51`  
		Last Modified: Tue, 21 Nov 2023 13:02:23 GMT  
		Size: 65.6 MB (65593153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72377d237fe1a86489eea9d2d9f72ba19b74303b09593612e4f440d909932fc`  
		Last Modified: Tue, 21 Nov 2023 13:02:12 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3` - linux; s390x

```console
$ docker pull varnish@sha256:0ab6caa4ba596675fb6506e80cd6416e352dc89123bce57cd6a750c5e9162e99
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.3 MB (82337376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77957464272e0f2a1870b20c4bd51bf9af77a796e6053701d2cc4d533ee2cc88`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 01:43:11 GMT
ADD file:36a070457acddafcd6cdda22a3c41efcbd4e2b1694831eb74c8143520ebf1cf2 in / 
# Tue, 19 Dec 2023 01:43:14 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 09:57:28 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 19 Dec 2023 09:57:28 GMT
ARG VARNISH_VERSION=7.3.1
# Tue, 19 Dec 2023 09:57:28 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Tue, 19 Dec 2023 09:57:29 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 19 Dec 2023 09:57:29 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 19 Dec 2023 09:57:30 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 19 Dec 2023 09:57:30 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 19 Dec 2023 09:57:30 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 19 Dec 2023 09:57:31 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 19 Dec 2023 09:57:31 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 19 Dec 2023 09:57:31 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 09:59:40 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.1.tgz -o $tmpdir/orig.tgz;     echo "57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 19 Dec 2023 09:59:43 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 09:59:43 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 19 Dec 2023 09:59:43 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 09:59:44 GMT
USER varnish
# Tue, 19 Dec 2023 09:59:44 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 09:59:44 GMT
CMD []
```

-	Layers:
	-	`sha256:eff2a4367cf88d5103011eba9299da2b4d173b0bde5dc0455020febf72b9b1c4`  
		Last Modified: Tue, 19 Dec 2023 01:48:08 GMT  
		Size: 29.7 MB (29657006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973b42ff7f83f76b123f93bf3b16fc127a7cc9fe1475d16b393a84485a77e625`  
		Last Modified: Tue, 19 Dec 2023 10:02:30 GMT  
		Size: 52.7 MB (52679878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e8e963aca39b2ea7900e6590a2e12624c36457b736760d4d9eb8d5289d9da7`  
		Last Modified: Tue, 19 Dec 2023 10:02:23 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.3-alpine`

```console
$ docker pull varnish@sha256:7aacc92711bb4c55276bcd32206e3a3f872f0a45b9f4a620843f81c5d676ac57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.3-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:a660b85166043d82783fefc5da6e563dd3baddbd57f85142037f982e902bfe0f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72971654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22258995a868639c834b5ee85a5c1679cc4ff4a424d12549e212ce22893c3d49`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:20:49 GMT
ADD file:1f4eb46669b5b6275af19eb7471a6899a61c276aa7d925b8ae99310b14b75b92 in / 
# Fri, 08 Dec 2023 01:20:49 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 17:29:13 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Mon, 11 Dec 2023 17:29:13 GMT
ARG VARNISH_VERSION=7.3.1
# Mon, 11 Dec 2023 17:29:13 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Mon, 11 Dec 2023 17:29:13 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 17:29:13 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 17:29:13 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Mon, 11 Dec 2023 17:29:13 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Mon, 11 Dec 2023 17:29:13 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Mon, 11 Dec 2023 17:29:13 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 17:29:13 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 17:29:14 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 17:30:32 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 17:30:32 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 17:30:32 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 17:30:32 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 17:30:32 GMT
USER varnish
# Mon, 11 Dec 2023 17:30:32 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 17:30:32 GMT
CMD []
```

-	Layers:
	-	`sha256:661ff4d9561e3fd050929ee5097067c34bafc523ee60f5294a37fd08056a73ca`  
		Last Modified: Fri, 08 Dec 2023 01:21:10 GMT  
		Size: 3.4 MB (3408480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df54af4bcc97a93a4bd34d0e0a186b4643293a0b4e9b118bb5fd66e7ff3a678`  
		Last Modified: Mon, 11 Dec 2023 17:31:23 GMT  
		Size: 69.6 MB (69562679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1c4c6bbeee3080ea2c25f71ad2659e1800e05df9cb4040bb500ea920d75038`  
		Last Modified: Mon, 11 Dec 2023 17:31:13 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:6263e0f2a246117ad4a109b963cd07c7d0d046bcc7cd22e2433a380f326e152a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.2 MB (57173570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21da2e0d838632cb4b57d2a16f3f84df85831022148ef32ee8b33b64913dc17f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:57:20 GMT
ADD file:13b9291053208eec61cd7c97bac2fa154380ad8d10182567763eea3e10c5882f in / 
# Fri, 08 Dec 2023 01:57:20 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 20:35:53 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Mon, 11 Dec 2023 20:35:53 GMT
ARG VARNISH_VERSION=7.3.1
# Mon, 11 Dec 2023 20:35:54 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Mon, 11 Dec 2023 20:35:54 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 20:35:54 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 20:35:54 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Mon, 11 Dec 2023 20:35:54 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Mon, 11 Dec 2023 20:35:54 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Mon, 11 Dec 2023 20:35:54 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 20:35:54 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 20:35:54 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 20:37:10 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 20:37:10 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 20:37:10 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 20:37:10 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 20:37:10 GMT
USER varnish
# Mon, 11 Dec 2023 20:37:10 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 20:37:11 GMT
CMD []
```

-	Layers:
	-	`sha256:1086c24c41097f090ce847d192c11307e1715eeb563a2cf4f410b2a199ae1942`  
		Last Modified: Fri, 08 Dec 2023 01:57:36 GMT  
		Size: 2.9 MB (2918701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c23e83961531cd3bf4404f796467444964e4ad11f8a736b70489b794a148810`  
		Last Modified: Mon, 11 Dec 2023 20:39:58 GMT  
		Size: 54.3 MB (54254374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52917b5a405d3bd4ee7ca2f070f6435b1099aee4e248f9c2e1c6ee9662be3001`  
		Last Modified: Mon, 11 Dec 2023 20:39:52 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:212fc3b9e2ae991b2d5398dbb64a8bd7fa6f89ce994f70c6705b127da860b723
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69670674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d26d4bdefa37aa5cbbabe0839fc9ee9ed1e23ce42b5bdbaa8a0619a63147e42a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:39:30 GMT
ADD file:8182c73f869a899cf624a59c400acb8226776d15e4d3a0d240a94e65340540d0 in / 
# Fri, 08 Dec 2023 01:39:30 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:17:05 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Mon, 11 Dec 2023 19:17:05 GMT
ARG VARNISH_VERSION=7.3.1
# Mon, 11 Dec 2023 19:17:06 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Mon, 11 Dec 2023 19:17:06 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 19:17:06 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 19:17:06 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Mon, 11 Dec 2023 19:17:06 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Mon, 11 Dec 2023 19:17:06 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Mon, 11 Dec 2023 19:17:06 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 19:17:06 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 19:17:06 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 19:18:16 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 19:18:17 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 19:18:17 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 19:18:17 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 19:18:17 GMT
USER varnish
# Mon, 11 Dec 2023 19:18:17 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 19:18:17 GMT
CMD []
```

-	Layers:
	-	`sha256:c303524923177661067f7eb378c3dd5277088c2676ebd1cd78e68397bb80fdbf`  
		Last Modified: Fri, 08 Dec 2023 01:39:48 GMT  
		Size: 3.3 MB (3347794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f90173f8b57807827483acedf8c853c481199ecb51a4797e033af8de7fa8a4`  
		Last Modified: Mon, 11 Dec 2023 19:19:12 GMT  
		Size: 66.3 MB (66322385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430ac4e33922777503f5d5f1ac2d2b199f4e9ca70758e3e94f23a9dd4d755c39`  
		Last Modified: Mon, 11 Dec 2023 19:19:06 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3-alpine` - linux; 386

```console
$ docker pull varnish@sha256:144593b4ae2f9889676979af92e6655686ec14070d3715973aaae1d2c004ad1b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (75000229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13ad0500a3c76c97cd544861eb007b787ea85320e31e8c2a3a4e74d818d5a47e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:38:25 GMT
ADD file:bd52540f209ba362654d795d7893669c819d35011a16f9f319301727a33b3bd9 in / 
# Fri, 08 Dec 2023 01:38:25 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 17:41:19 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Mon, 11 Dec 2023 17:41:19 GMT
ARG VARNISH_VERSION=7.3.1
# Mon, 11 Dec 2023 17:41:19 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Mon, 11 Dec 2023 17:41:19 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 17:41:19 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 17:41:19 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Mon, 11 Dec 2023 17:41:19 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Mon, 11 Dec 2023 17:41:20 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Mon, 11 Dec 2023 17:41:20 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 17:41:20 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 17:41:20 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 17:43:20 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 17:43:20 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 17:43:20 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 17:43:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 17:43:20 GMT
USER varnish
# Mon, 11 Dec 2023 17:43:21 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 17:43:21 GMT
CMD []
```

-	Layers:
	-	`sha256:9acd8b4c9d4385585f74dabb4bc6b3351888710ae37ec5dbd9ea950281b8f9bb`  
		Last Modified: Fri, 08 Dec 2023 01:38:43 GMT  
		Size: 3.2 MB (3244115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ef2537002ecb2bb3abded65d6356f3692fda99b626ea47de362a0110b0b5b5`  
		Last Modified: Mon, 11 Dec 2023 17:44:21 GMT  
		Size: 71.8 MB (71755614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e61ec8d102709660006ff1fcde698d488782452a4493a0eae31ed253ef2bce7`  
		Last Modified: Mon, 11 Dec 2023 17:44:07 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:a76ce382abf1217b12fa2bf3e1e795b0431efa83fdcbeeb8f7fd50124327baf4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.5 MB (70485288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cb51e4e5c8495d2d3a90e2274b3a1ba12e2541fc87085ca17e4f0092b93702b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:22:51 GMT
ADD file:052421189f8d269382daaaa8beb63c687e4d8ca908c421abdce53bcc627a40b4 in / 
# Fri, 08 Dec 2023 01:22:51 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 17:25:41 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Mon, 11 Dec 2023 17:25:43 GMT
ARG VARNISH_VERSION=7.3.1
# Mon, 11 Dec 2023 17:25:43 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Mon, 11 Dec 2023 17:25:44 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 17:25:44 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 17:25:44 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Mon, 11 Dec 2023 17:25:45 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Mon, 11 Dec 2023 17:25:45 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Mon, 11 Dec 2023 17:25:45 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 17:25:45 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 17:25:46 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 17:27:08 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 17:27:11 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 17:27:11 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 17:27:12 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 17:27:13 GMT
USER varnish
# Mon, 11 Dec 2023 17:27:13 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 17:27:13 GMT
CMD []
```

-	Layers:
	-	`sha256:243ac51c334a47917a84be93e972ee6378987e9b3b917a5a8df29025e161c1f3`  
		Last Modified: Fri, 08 Dec 2023 01:23:14 GMT  
		Size: 3.4 MB (3358233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42894c6396857cddc9334f3f02e9b3a4fe9e83a14200487428ee54247e804ade`  
		Last Modified: Mon, 11 Dec 2023 17:28:11 GMT  
		Size: 67.1 MB (67126559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86af6ac0c31af7d9ef2235797afd83c075764dac4f8b2af2ea00d996fd202644`  
		Last Modified: Mon, 11 Dec 2023 17:28:00 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:12ceacf7e0b60a469d0bb4588a8fce08904d2076e215786778a3db5b8625db26
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64858338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2b460b5437dfface2a98ed7a3c28597b4530d8a6e501b486153d9958d1c58e7`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:41:50 GMT
ADD file:47e0982fc3ae485c06d46f3c0022afd39ed7ec95fe755c2391e6b0cfcae65dfc in / 
# Fri, 08 Dec 2023 01:41:51 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:54:01 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Mon, 11 Dec 2023 19:54:01 GMT
ARG VARNISH_VERSION=7.3.1
# Mon, 11 Dec 2023 19:54:01 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Mon, 11 Dec 2023 19:54:01 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 19:54:01 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 19:54:02 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Mon, 11 Dec 2023 19:54:02 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Mon, 11 Dec 2023 19:54:02 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Mon, 11 Dec 2023 19:54:02 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 19:54:02 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 19:54:02 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 19:55:21 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 19:55:25 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 19:55:25 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 19:55:25 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 19:55:25 GMT
USER varnish
# Mon, 11 Dec 2023 19:55:25 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 19:55:25 GMT
CMD []
```

-	Layers:
	-	`sha256:0fca3ee44ced87b7184bc23390283fdf10cfae0e844a25b785dd11c463815227`  
		Last Modified: Fri, 08 Dec 2023 01:42:30 GMT  
		Size: 3.2 MB (3242332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de618724c4df65b558efa8979cd6a8db37714a1bc88b90d86d2c7ae78629b3fd`  
		Last Modified: Mon, 11 Dec 2023 19:56:31 GMT  
		Size: 61.6 MB (61615510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57580a9d987d8a4e6b62eaa72d36e8665a06835e8fb63ee71d17edfd3c531a0a`  
		Last Modified: Mon, 11 Dec 2023 19:56:24 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.3.1`

```console
$ docker pull varnish@sha256:87dffb5c48c83cdcf12a3efeb6457d9e178f29604494e32b51701e1b2aa27cb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.3.1` - linux; amd64

```console
$ docker pull varnish@sha256:df9b1ecb6e4ca0e98f9dbdf680885e16c7e510e2de4ddabc59ae2982e8c8cf99
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101966885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac6fda6c72241a94c1e31ff26a39609231e0b895e083619d8286a89b39030028`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 01:20:50 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Tue, 19 Dec 2023 01:20:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:03:02 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 19 Dec 2023 08:03:02 GMT
ARG VARNISH_VERSION=7.3.1
# Tue, 19 Dec 2023 08:03:02 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Tue, 19 Dec 2023 08:03:03 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 19 Dec 2023 08:03:03 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 19 Dec 2023 08:03:03 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 19 Dec 2023 08:03:03 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 19 Dec 2023 08:03:03 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 19 Dec 2023 08:03:03 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 19 Dec 2023 08:03:03 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 19 Dec 2023 08:03:03 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 08:05:41 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.1.tgz -o $tmpdir/orig.tgz;     echo "57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 19 Dec 2023 08:05:42 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 08:05:42 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 19 Dec 2023 08:05:42 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 08:05:42 GMT
USER varnish
# Tue, 19 Dec 2023 08:05:42 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 08:05:42 GMT
CMD []
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e37b9699670384020e902a0ae2f3c71ef125515c77fb7f57f956fe2ab064bc8`  
		Last Modified: Tue, 19 Dec 2023 08:08:41 GMT  
		Size: 70.5 MB (70548520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbc9ee7e56bac88b0277ca7cd2409fa0ea1152bcdf965d290cd039497678c49`  
		Last Modified: Tue, 19 Dec 2023 08:08:32 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3.1` - linux; arm variant v7

```console
$ docker pull varnish@sha256:ad549d82c4744321f31d836fa2757228ec9c6ee28a2fe56905d8606424ce55f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.8 MB (78751981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:580eedff14a9163d5717e74e0654d277448fd09bed4c6672badbf8cbbd32236f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 02:08:09 GMT
ADD file:496e70a34ff4dabb4eefdf40e4e2f0563bea0c120bb43206f8f52ab5a887b637 in / 
# Tue, 19 Dec 2023 02:08:09 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:15:00 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 19 Dec 2023 08:15:00 GMT
ARG VARNISH_VERSION=7.3.1
# Tue, 19 Dec 2023 08:15:00 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Tue, 19 Dec 2023 08:15:00 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 19 Dec 2023 08:15:01 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 19 Dec 2023 08:15:01 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 19 Dec 2023 08:15:01 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 19 Dec 2023 08:15:01 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 19 Dec 2023 08:15:01 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 19 Dec 2023 08:15:01 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 19 Dec 2023 08:15:01 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 08:17:37 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.1.tgz -o $tmpdir/orig.tgz;     echo "57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 19 Dec 2023 08:17:37 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 08:17:37 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 19 Dec 2023 08:17:38 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 08:17:38 GMT
USER varnish
# Tue, 19 Dec 2023 08:17:38 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 08:17:38 GMT
CMD []
```

-	Layers:
	-	`sha256:19ccf4d6cc6956e4a5522352be94632923aa376a9939a4f45428a4f304c73bc8`  
		Last Modified: Tue, 19 Dec 2023 02:12:33 GMT  
		Size: 26.6 MB (26578972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8d700fb01496fa8c844f9ebb7e2c0de1106588b482a0aef5209b031c470c89`  
		Last Modified: Tue, 19 Dec 2023 08:20:32 GMT  
		Size: 52.2 MB (52172516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa853700f1de2e0c582912f1a2175a3c69c30b2cd96cf0db35fb599a9d9bd9c7`  
		Last Modified: Tue, 19 Dec 2023 08:20:25 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3.1` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:32014d110bbaffe0743bdc54c6c9d439532cf91ad71fbcdbdb7ae00779b18d62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.8 MB (95781809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66a11569b230dc214d07fcb99a041dcdfe426ea3ca30a6c31410230131217503`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 21:19:16 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 21 Nov 2023 21:19:16 GMT
ARG VARNISH_VERSION=7.3.1
# Tue, 21 Nov 2023 21:19:16 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Tue, 21 Nov 2023 21:19:16 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 21 Nov 2023 21:19:16 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 21 Nov 2023 21:19:16 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 21 Nov 2023 21:19:16 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 21 Nov 2023 21:19:16 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 21 Nov 2023 21:19:16 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 21 Nov 2023 21:19:16 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 21 Nov 2023 21:19:16 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 21:21:25 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.1.tgz -o $tmpdir/orig.tgz;     echo "57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 21 Nov 2023 21:21:26 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 21:21:26 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 21 Nov 2023 21:21:26 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 21:21:26 GMT
USER varnish
# Tue, 21 Nov 2023 21:21:26 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 21:21:26 GMT
CMD []
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc98e65c086f4b548a2e982f49352b25a0cd9922c2f9a98330b42163385f0d4`  
		Last Modified: Tue, 21 Nov 2023 21:23:59 GMT  
		Size: 65.7 MB (65717192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff1904762c1d07cd5329fe0e393c0598fdbac6a204808c4e326bd44f6f505eb`  
		Last Modified: Tue, 21 Nov 2023 21:23:52 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3.1` - linux; 386

```console
$ docker pull varnish@sha256:522eb24b5d28a7295ce65f1086e33d5d85beaf7c9c65b3c60759498baeb3d4e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.2 MB (103212796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b70fc90e400e9dfbd466ceab45b7e7287a51be25ddbbc35bb9b1668978ffda0d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 04:40:15 GMT
ADD file:7de881b584405a880c4d02778056aaa81bb5dd5d1af65b3086d66aed9ff0ad4b in / 
# Tue, 21 Nov 2023 04:40:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 15:15:08 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 21 Nov 2023 15:15:08 GMT
ARG VARNISH_VERSION=7.3.1
# Tue, 21 Nov 2023 15:15:08 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Tue, 21 Nov 2023 15:15:08 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 21 Nov 2023 15:15:09 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 21 Nov 2023 15:15:09 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 21 Nov 2023 15:15:09 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 21 Nov 2023 15:15:09 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 21 Nov 2023 15:15:09 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 21 Nov 2023 15:15:09 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 21 Nov 2023 15:15:09 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 15:18:32 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.1.tgz -o $tmpdir/orig.tgz;     echo "57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 21 Nov 2023 15:18:33 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 15:18:33 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 21 Nov 2023 15:18:33 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 15:18:34 GMT
USER varnish
# Tue, 21 Nov 2023 15:18:34 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 15:18:34 GMT
CMD []
```

-	Layers:
	-	`sha256:75c11612678b54e79a38118fe66e532c61b3d0798afb741007b4cd3209c0ec4e`  
		Last Modified: Tue, 21 Nov 2023 04:45:24 GMT  
		Size: 32.4 MB (32402632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae3bc414da66bdd2d32a046a233e988a45ad7faaa11b96e0f5e55973fa16073`  
		Last Modified: Tue, 21 Nov 2023 15:22:12 GMT  
		Size: 70.8 MB (70809672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d549858933a493ec89c83cb3fafe3fec83022f9eae66525cdcbdf30fc7e49c92`  
		Last Modified: Tue, 21 Nov 2023 15:21:58 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3.1` - linux; ppc64le

```console
$ docker pull varnish@sha256:66a0133569e260a895c68333c0426c77cdaa6c2f4dcb29b8f24906c16932c150
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.9 MB (100887371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc4919272c647cb21a3aee48eb9f1a2e0a70f042c7da2e16ef2463f7cf62433b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 04:24:43 GMT
ADD file:b0d18f2d04821eb50d1faecc1a64916f5c63dd386ae71a3b2cb1d6c4aac6e1c4 in / 
# Tue, 21 Nov 2023 04:24:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 12:54:35 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 21 Nov 2023 12:54:35 GMT
ARG VARNISH_VERSION=7.3.1
# Tue, 21 Nov 2023 12:54:36 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Tue, 21 Nov 2023 12:54:36 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 21 Nov 2023 12:54:36 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 21 Nov 2023 12:54:37 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 21 Nov 2023 12:54:37 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 21 Nov 2023 12:54:37 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 21 Nov 2023 12:54:37 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 21 Nov 2023 12:54:38 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 21 Nov 2023 12:54:38 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 12:58:17 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.1.tgz -o $tmpdir/orig.tgz;     echo "57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 21 Nov 2023 12:58:19 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 12:58:19 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 21 Nov 2023 12:58:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 12:58:20 GMT
USER varnish
# Tue, 21 Nov 2023 12:58:20 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 12:58:20 GMT
CMD []
```

-	Layers:
	-	`sha256:60239a74847cd7e9a928353188f3cf096ca8cf648e2b27c765058e169d568fd9`  
		Last Modified: Tue, 21 Nov 2023 04:29:47 GMT  
		Size: 35.3 MB (35293727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef474112e53d3cd9414bbc58b355c42c87c37b9296900ac553800b9812b43a51`  
		Last Modified: Tue, 21 Nov 2023 13:02:23 GMT  
		Size: 65.6 MB (65593153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72377d237fe1a86489eea9d2d9f72ba19b74303b09593612e4f440d909932fc`  
		Last Modified: Tue, 21 Nov 2023 13:02:12 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3.1` - linux; s390x

```console
$ docker pull varnish@sha256:0ab6caa4ba596675fb6506e80cd6416e352dc89123bce57cd6a750c5e9162e99
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.3 MB (82337376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77957464272e0f2a1870b20c4bd51bf9af77a796e6053701d2cc4d533ee2cc88`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 01:43:11 GMT
ADD file:36a070457acddafcd6cdda22a3c41efcbd4e2b1694831eb74c8143520ebf1cf2 in / 
# Tue, 19 Dec 2023 01:43:14 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 09:57:28 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 19 Dec 2023 09:57:28 GMT
ARG VARNISH_VERSION=7.3.1
# Tue, 19 Dec 2023 09:57:28 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Tue, 19 Dec 2023 09:57:29 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 19 Dec 2023 09:57:29 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 19 Dec 2023 09:57:30 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 19 Dec 2023 09:57:30 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 19 Dec 2023 09:57:30 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 19 Dec 2023 09:57:31 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 19 Dec 2023 09:57:31 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 19 Dec 2023 09:57:31 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 09:59:40 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.1.tgz -o $tmpdir/orig.tgz;     echo "57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 19 Dec 2023 09:59:43 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 09:59:43 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 19 Dec 2023 09:59:43 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 09:59:44 GMT
USER varnish
# Tue, 19 Dec 2023 09:59:44 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 09:59:44 GMT
CMD []
```

-	Layers:
	-	`sha256:eff2a4367cf88d5103011eba9299da2b4d173b0bde5dc0455020febf72b9b1c4`  
		Last Modified: Tue, 19 Dec 2023 01:48:08 GMT  
		Size: 29.7 MB (29657006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973b42ff7f83f76b123f93bf3b16fc127a7cc9fe1475d16b393a84485a77e625`  
		Last Modified: Tue, 19 Dec 2023 10:02:30 GMT  
		Size: 52.7 MB (52679878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e8e963aca39b2ea7900e6590a2e12624c36457b736760d4d9eb8d5289d9da7`  
		Last Modified: Tue, 19 Dec 2023 10:02:23 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.3.1-alpine`

```console
$ docker pull varnish@sha256:7aacc92711bb4c55276bcd32206e3a3f872f0a45b9f4a620843f81c5d676ac57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.3.1-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:a660b85166043d82783fefc5da6e563dd3baddbd57f85142037f982e902bfe0f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72971654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22258995a868639c834b5ee85a5c1679cc4ff4a424d12549e212ce22893c3d49`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:20:49 GMT
ADD file:1f4eb46669b5b6275af19eb7471a6899a61c276aa7d925b8ae99310b14b75b92 in / 
# Fri, 08 Dec 2023 01:20:49 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 17:29:13 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Mon, 11 Dec 2023 17:29:13 GMT
ARG VARNISH_VERSION=7.3.1
# Mon, 11 Dec 2023 17:29:13 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Mon, 11 Dec 2023 17:29:13 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 17:29:13 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 17:29:13 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Mon, 11 Dec 2023 17:29:13 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Mon, 11 Dec 2023 17:29:13 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Mon, 11 Dec 2023 17:29:13 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 17:29:13 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 17:29:14 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 17:30:32 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 17:30:32 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 17:30:32 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 17:30:32 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 17:30:32 GMT
USER varnish
# Mon, 11 Dec 2023 17:30:32 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 17:30:32 GMT
CMD []
```

-	Layers:
	-	`sha256:661ff4d9561e3fd050929ee5097067c34bafc523ee60f5294a37fd08056a73ca`  
		Last Modified: Fri, 08 Dec 2023 01:21:10 GMT  
		Size: 3.4 MB (3408480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df54af4bcc97a93a4bd34d0e0a186b4643293a0b4e9b118bb5fd66e7ff3a678`  
		Last Modified: Mon, 11 Dec 2023 17:31:23 GMT  
		Size: 69.6 MB (69562679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1c4c6bbeee3080ea2c25f71ad2659e1800e05df9cb4040bb500ea920d75038`  
		Last Modified: Mon, 11 Dec 2023 17:31:13 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3.1-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:6263e0f2a246117ad4a109b963cd07c7d0d046bcc7cd22e2433a380f326e152a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.2 MB (57173570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21da2e0d838632cb4b57d2a16f3f84df85831022148ef32ee8b33b64913dc17f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:57:20 GMT
ADD file:13b9291053208eec61cd7c97bac2fa154380ad8d10182567763eea3e10c5882f in / 
# Fri, 08 Dec 2023 01:57:20 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 20:35:53 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Mon, 11 Dec 2023 20:35:53 GMT
ARG VARNISH_VERSION=7.3.1
# Mon, 11 Dec 2023 20:35:54 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Mon, 11 Dec 2023 20:35:54 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 20:35:54 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 20:35:54 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Mon, 11 Dec 2023 20:35:54 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Mon, 11 Dec 2023 20:35:54 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Mon, 11 Dec 2023 20:35:54 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 20:35:54 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 20:35:54 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 20:37:10 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 20:37:10 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 20:37:10 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 20:37:10 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 20:37:10 GMT
USER varnish
# Mon, 11 Dec 2023 20:37:10 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 20:37:11 GMT
CMD []
```

-	Layers:
	-	`sha256:1086c24c41097f090ce847d192c11307e1715eeb563a2cf4f410b2a199ae1942`  
		Last Modified: Fri, 08 Dec 2023 01:57:36 GMT  
		Size: 2.9 MB (2918701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c23e83961531cd3bf4404f796467444964e4ad11f8a736b70489b794a148810`  
		Last Modified: Mon, 11 Dec 2023 20:39:58 GMT  
		Size: 54.3 MB (54254374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52917b5a405d3bd4ee7ca2f070f6435b1099aee4e248f9c2e1c6ee9662be3001`  
		Last Modified: Mon, 11 Dec 2023 20:39:52 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3.1-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:212fc3b9e2ae991b2d5398dbb64a8bd7fa6f89ce994f70c6705b127da860b723
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69670674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d26d4bdefa37aa5cbbabe0839fc9ee9ed1e23ce42b5bdbaa8a0619a63147e42a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:39:30 GMT
ADD file:8182c73f869a899cf624a59c400acb8226776d15e4d3a0d240a94e65340540d0 in / 
# Fri, 08 Dec 2023 01:39:30 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:17:05 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Mon, 11 Dec 2023 19:17:05 GMT
ARG VARNISH_VERSION=7.3.1
# Mon, 11 Dec 2023 19:17:06 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Mon, 11 Dec 2023 19:17:06 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 19:17:06 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 19:17:06 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Mon, 11 Dec 2023 19:17:06 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Mon, 11 Dec 2023 19:17:06 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Mon, 11 Dec 2023 19:17:06 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 19:17:06 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 19:17:06 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 19:18:16 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 19:18:17 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 19:18:17 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 19:18:17 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 19:18:17 GMT
USER varnish
# Mon, 11 Dec 2023 19:18:17 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 19:18:17 GMT
CMD []
```

-	Layers:
	-	`sha256:c303524923177661067f7eb378c3dd5277088c2676ebd1cd78e68397bb80fdbf`  
		Last Modified: Fri, 08 Dec 2023 01:39:48 GMT  
		Size: 3.3 MB (3347794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f90173f8b57807827483acedf8c853c481199ecb51a4797e033af8de7fa8a4`  
		Last Modified: Mon, 11 Dec 2023 19:19:12 GMT  
		Size: 66.3 MB (66322385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430ac4e33922777503f5d5f1ac2d2b199f4e9ca70758e3e94f23a9dd4d755c39`  
		Last Modified: Mon, 11 Dec 2023 19:19:06 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3.1-alpine` - linux; 386

```console
$ docker pull varnish@sha256:144593b4ae2f9889676979af92e6655686ec14070d3715973aaae1d2c004ad1b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (75000229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13ad0500a3c76c97cd544861eb007b787ea85320e31e8c2a3a4e74d818d5a47e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:38:25 GMT
ADD file:bd52540f209ba362654d795d7893669c819d35011a16f9f319301727a33b3bd9 in / 
# Fri, 08 Dec 2023 01:38:25 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 17:41:19 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Mon, 11 Dec 2023 17:41:19 GMT
ARG VARNISH_VERSION=7.3.1
# Mon, 11 Dec 2023 17:41:19 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Mon, 11 Dec 2023 17:41:19 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 17:41:19 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 17:41:19 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Mon, 11 Dec 2023 17:41:19 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Mon, 11 Dec 2023 17:41:20 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Mon, 11 Dec 2023 17:41:20 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 17:41:20 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 17:41:20 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 17:43:20 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 17:43:20 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 17:43:20 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 17:43:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 17:43:20 GMT
USER varnish
# Mon, 11 Dec 2023 17:43:21 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 17:43:21 GMT
CMD []
```

-	Layers:
	-	`sha256:9acd8b4c9d4385585f74dabb4bc6b3351888710ae37ec5dbd9ea950281b8f9bb`  
		Last Modified: Fri, 08 Dec 2023 01:38:43 GMT  
		Size: 3.2 MB (3244115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ef2537002ecb2bb3abded65d6356f3692fda99b626ea47de362a0110b0b5b5`  
		Last Modified: Mon, 11 Dec 2023 17:44:21 GMT  
		Size: 71.8 MB (71755614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e61ec8d102709660006ff1fcde698d488782452a4493a0eae31ed253ef2bce7`  
		Last Modified: Mon, 11 Dec 2023 17:44:07 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3.1-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:a76ce382abf1217b12fa2bf3e1e795b0431efa83fdcbeeb8f7fd50124327baf4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.5 MB (70485288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cb51e4e5c8495d2d3a90e2274b3a1ba12e2541fc87085ca17e4f0092b93702b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:22:51 GMT
ADD file:052421189f8d269382daaaa8beb63c687e4d8ca908c421abdce53bcc627a40b4 in / 
# Fri, 08 Dec 2023 01:22:51 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 17:25:41 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Mon, 11 Dec 2023 17:25:43 GMT
ARG VARNISH_VERSION=7.3.1
# Mon, 11 Dec 2023 17:25:43 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Mon, 11 Dec 2023 17:25:44 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 17:25:44 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 17:25:44 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Mon, 11 Dec 2023 17:25:45 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Mon, 11 Dec 2023 17:25:45 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Mon, 11 Dec 2023 17:25:45 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 17:25:45 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 17:25:46 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 17:27:08 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 17:27:11 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 17:27:11 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 17:27:12 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 17:27:13 GMT
USER varnish
# Mon, 11 Dec 2023 17:27:13 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 17:27:13 GMT
CMD []
```

-	Layers:
	-	`sha256:243ac51c334a47917a84be93e972ee6378987e9b3b917a5a8df29025e161c1f3`  
		Last Modified: Fri, 08 Dec 2023 01:23:14 GMT  
		Size: 3.4 MB (3358233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42894c6396857cddc9334f3f02e9b3a4fe9e83a14200487428ee54247e804ade`  
		Last Modified: Mon, 11 Dec 2023 17:28:11 GMT  
		Size: 67.1 MB (67126559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86af6ac0c31af7d9ef2235797afd83c075764dac4f8b2af2ea00d996fd202644`  
		Last Modified: Mon, 11 Dec 2023 17:28:00 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.3.1-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:12ceacf7e0b60a469d0bb4588a8fce08904d2076e215786778a3db5b8625db26
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64858338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2b460b5437dfface2a98ed7a3c28597b4530d8a6e501b486153d9958d1c58e7`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:41:50 GMT
ADD file:47e0982fc3ae485c06d46f3c0022afd39ed7ec95fe755c2391e6b0cfcae65dfc in / 
# Fri, 08 Dec 2023 01:41:51 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:54:01 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Mon, 11 Dec 2023 19:54:01 GMT
ARG VARNISH_VERSION=7.3.1
# Mon, 11 Dec 2023 19:54:01 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Mon, 11 Dec 2023 19:54:01 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 19:54:01 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 19:54:02 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Mon, 11 Dec 2023 19:54:02 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Mon, 11 Dec 2023 19:54:02 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Mon, 11 Dec 2023 19:54:02 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 19:54:02 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 19:54:02 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 19:55:21 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 19:55:25 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 19:55:25 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 19:55:25 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 19:55:25 GMT
USER varnish
# Mon, 11 Dec 2023 19:55:25 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 19:55:25 GMT
CMD []
```

-	Layers:
	-	`sha256:0fca3ee44ced87b7184bc23390283fdf10cfae0e844a25b785dd11c463815227`  
		Last Modified: Fri, 08 Dec 2023 01:42:30 GMT  
		Size: 3.2 MB (3242332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de618724c4df65b558efa8979cd6a8db37714a1bc88b90d86d2c7ae78629b3fd`  
		Last Modified: Mon, 11 Dec 2023 19:56:31 GMT  
		Size: 61.6 MB (61615510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57580a9d987d8a4e6b62eaa72d36e8665a06835e8fb63ee71d17edfd3c531a0a`  
		Last Modified: Mon, 11 Dec 2023 19:56:24 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.4`

```console
$ docker pull varnish@sha256:74f3de816160fb949b01111c302f4d37a49b45b1a754d1e145e8d3d7dc94cfb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.4` - linux; amd64

```console
$ docker pull varnish@sha256:eadc1f8f442bb86961c300d37a64bb51b2658b8f6bed39c21fdd85405775c144
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134738894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e44717a97df19098a313b57e48e02fe1b413b2d92fe2eb3e6350c5f85ed591df`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 01:20:27 GMT
ADD file:ac3cd70031d35e46d86b876934946ffc8756de4de065fbc926dce642dac07ff3 in / 
# Tue, 19 Dec 2023 01:20:28 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:59:51 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Tue, 19 Dec 2023 07:59:51 GMT
ARG VARNISH_VERSION=7.4.2
# Tue, 19 Dec 2023 07:59:51 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Tue, 19 Dec 2023 07:59:51 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 19 Dec 2023 07:59:52 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 19 Dec 2023 07:59:52 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Tue, 19 Dec 2023 07:59:52 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Tue, 19 Dec 2023 07:59:52 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Tue, 19 Dec 2023 07:59:52 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 19 Dec 2023 07:59:52 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 19 Dec 2023 07:59:52 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 08:02:47 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.2.tgz -o $tmpdir/orig.tgz;     echo "acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 19 Dec 2023 08:02:48 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 08:02:48 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 19 Dec 2023 08:02:48 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 08:02:48 GMT
USER varnish
# Tue, 19 Dec 2023 08:02:48 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 08:02:49 GMT
CMD []
```

-	Layers:
	-	`sha256:af107e978371b6cd6339127a05502c5eacd1e6b0e9eb7b2f4aa7b6fc87e2dd81`  
		Last Modified: Tue, 19 Dec 2023 01:24:59 GMT  
		Size: 29.1 MB (29125963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b1c37f74eda351d5d18bd05ac7a597435e4dcc3dca90495bfb8704d7030f37`  
		Last Modified: Tue, 19 Dec 2023 08:08:18 GMT  
		Size: 105.6 MB (105612439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98889ac1ccb507f3093353ef6ddc3ca2dae1063b5323bb989732b0271c784f40`  
		Last Modified: Tue, 19 Dec 2023 08:08:03 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4` - linux; arm variant v7

```console
$ docker pull varnish@sha256:0b0725305bd25fb5c7804c983f3a03f5c358908c150b56e6fc7754762d2fad7f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104987802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36b50ea5a138f4de8b6fb2c81a616b546478c36e122bd5e421db168ef5ad924c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 02:07:50 GMT
ADD file:aef112919e7924ad6da32181b1df5099cd692680c104118da3a24cd4dfe55a1d in / 
# Tue, 19 Dec 2023 02:07:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:11:51 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Tue, 19 Dec 2023 08:11:51 GMT
ARG VARNISH_VERSION=7.4.2
# Tue, 19 Dec 2023 08:11:51 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Tue, 19 Dec 2023 08:11:51 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 19 Dec 2023 08:11:51 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 19 Dec 2023 08:11:51 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Tue, 19 Dec 2023 08:11:51 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Tue, 19 Dec 2023 08:11:52 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Tue, 19 Dec 2023 08:11:52 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 19 Dec 2023 08:11:52 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 19 Dec 2023 08:11:52 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 08:14:41 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.2.tgz -o $tmpdir/orig.tgz;     echo "acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 19 Dec 2023 08:14:42 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 08:14:42 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 19 Dec 2023 08:14:42 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 08:14:42 GMT
USER varnish
# Tue, 19 Dec 2023 08:14:42 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 08:14:43 GMT
CMD []
```

-	Layers:
	-	`sha256:65ab19615c01a3b542f77fadb3bd27872b6a20cba3e9269fb951de36d8fa6805`  
		Last Modified: Tue, 19 Dec 2023 02:11:52 GMT  
		Size: 24.7 MB (24718157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0329b82b2a3ad7a3589db33efac87f48ea52033e08b8fb622036d689eac669e`  
		Last Modified: Tue, 19 Dec 2023 08:20:12 GMT  
		Size: 80.3 MB (80269153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:873759df9ef5bea1a9b39771cb9f95f002aab5fcac9279141c11bad88f032d9a`  
		Last Modified: Tue, 19 Dec 2023 08:20:00 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:7b765c330312fbd652f5811c86c4c6b3e88e2e2c24d7e16f83f4b1782bd8cb90
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.2 MB (129246108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23a72da26db114f62729359648ac0a655eb843e6245e8c01514293bbfcb75b91`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 21:16:36 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Tue, 21 Nov 2023 21:16:36 GMT
ARG VARNISH_VERSION=7.4.2
# Tue, 21 Nov 2023 21:16:37 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Tue, 21 Nov 2023 21:16:37 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 21 Nov 2023 21:16:37 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 21 Nov 2023 21:16:37 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Tue, 21 Nov 2023 21:16:37 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Tue, 21 Nov 2023 21:16:37 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Tue, 21 Nov 2023 21:16:37 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 21 Nov 2023 21:16:37 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 21 Nov 2023 21:16:37 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 21:19:02 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.2.tgz -o $tmpdir/orig.tgz;     echo "acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 21 Nov 2023 21:19:04 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 21:19:04 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 21 Nov 2023 21:19:04 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 21:19:04 GMT
USER varnish
# Tue, 21 Nov 2023 21:19:04 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 21:19:04 GMT
CMD []
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4c433f9fe1b4c04daf893df7f3dde2d25de13ed8474ae8887c623dbb3b0d5f`  
		Last Modified: Tue, 21 Nov 2023 21:23:39 GMT  
		Size: 100.1 MB (100066338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700ba44dbd53506d34d537e4614e9fb6a06b8a9aa2797b7e028061bc36b56044`  
		Last Modified: Tue, 21 Nov 2023 21:23:28 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4` - linux; 386

```console
$ docker pull varnish@sha256:f7094353a24b15c6f1dc90d7efd0fd58cbeba2336184d3b5eedca4b98da770a4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131941018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e481519ab9391779d3c4321f01ff5a60343ba4a44a01e1184384da4fd9eacc19`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 04:39:53 GMT
ADD file:930e1b9d85b6927c4d3046f7c75de2f3bfc6ec29100c314d0ab2b780ea30e962 in / 
# Tue, 21 Nov 2023 04:39:53 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 15:11:13 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Tue, 21 Nov 2023 15:11:13 GMT
ARG VARNISH_VERSION=7.4.2
# Tue, 21 Nov 2023 15:11:13 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Tue, 21 Nov 2023 15:11:13 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 21 Nov 2023 15:11:13 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 21 Nov 2023 15:11:13 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Tue, 21 Nov 2023 15:11:13 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Tue, 21 Nov 2023 15:11:14 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Tue, 21 Nov 2023 15:11:14 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 21 Nov 2023 15:11:14 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 21 Nov 2023 15:11:14 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 15:14:49 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.2.tgz -o $tmpdir/orig.tgz;     echo "acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 21 Nov 2023 15:14:50 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 15:14:51 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 21 Nov 2023 15:14:51 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 15:14:51 GMT
USER varnish
# Tue, 21 Nov 2023 15:14:51 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 15:14:51 GMT
CMD []
```

-	Layers:
	-	`sha256:c0734eabce8885d8904dbd11b77aa97c2d2b04bc8e2af9e89d47c4bda590dd8e`  
		Last Modified: Tue, 21 Nov 2023 04:44:34 GMT  
		Size: 30.2 MB (30164109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebaa590b85c3666b3aa98d7f7f7d5e957400d175de18f1a103ee9fc72f3ff1e`  
		Last Modified: Tue, 21 Nov 2023 15:21:44 GMT  
		Size: 101.8 MB (101776416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb43c8e9e7fcf7c7d91ab556103770f53e487c54d5b6d3a5e6eae1531dabb03c`  
		Last Modified: Tue, 21 Nov 2023 15:21:22 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4` - linux; ppc64le

```console
$ docker pull varnish@sha256:2393ba60ad3c5b5c3b8dc33eecd5388405e067b6c7b6aa6614d4c0e22d8cb740
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.7 MB (137679921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11d740886e444fe4a948031256adfe8d9d4148f985a3451ff9217f8b3b02084b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 12:50:24 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Tue, 21 Nov 2023 12:50:24 GMT
ARG VARNISH_VERSION=7.4.2
# Tue, 21 Nov 2023 12:50:24 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Tue, 21 Nov 2023 12:50:24 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 21 Nov 2023 12:50:25 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 21 Nov 2023 12:50:25 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Tue, 21 Nov 2023 12:50:25 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Tue, 21 Nov 2023 12:50:25 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Tue, 21 Nov 2023 12:50:25 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 21 Nov 2023 12:50:26 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 21 Nov 2023 12:50:26 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 12:54:18 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.2.tgz -o $tmpdir/orig.tgz;     echo "acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 21 Nov 2023 12:54:22 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 12:54:23 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 21 Nov 2023 12:54:23 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 12:54:23 GMT
USER varnish
# Tue, 21 Nov 2023 12:54:23 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 12:54:24 GMT
CMD []
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53276baea44ef2eb7632af8b3e497190197e059d4973c54c393e8e514579fee6`  
		Last Modified: Tue, 21 Nov 2023 13:01:56 GMT  
		Size: 104.5 MB (104537822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e228724f48a9283f83071d90b2ad5ea3adbd7aa8db408cf9cc17907d068aefd9`  
		Last Modified: Tue, 21 Nov 2023 13:01:38 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4` - linux; s390x

```console
$ docker pull varnish@sha256:6c7d0645cb3a69ac8d8f1550498bd4d8cdea53596dec94bcb46dd960a79f7032
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112324108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a720df683a8465e59eb06466380c0e7aa703e6e2adeafe901b372ac4a969610`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 01:42:37 GMT
ADD file:f06f12fa5a93afc3a79ac4371d24b0a471a5a1818cf34c1d90004c8f410914b9 in / 
# Tue, 19 Dec 2023 01:42:39 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 09:54:42 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Tue, 19 Dec 2023 09:54:43 GMT
ARG VARNISH_VERSION=7.4.2
# Tue, 19 Dec 2023 09:54:43 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Tue, 19 Dec 2023 09:54:43 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 19 Dec 2023 09:54:43 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 19 Dec 2023 09:54:43 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Tue, 19 Dec 2023 09:54:43 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Tue, 19 Dec 2023 09:54:43 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Tue, 19 Dec 2023 09:54:43 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 19 Dec 2023 09:54:43 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 19 Dec 2023 09:54:44 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 09:57:01 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.2.tgz -o $tmpdir/orig.tgz;     echo "acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 19 Dec 2023 09:57:06 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 09:57:06 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 19 Dec 2023 09:57:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 09:57:06 GMT
USER varnish
# Tue, 19 Dec 2023 09:57:07 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 09:57:07 GMT
CMD []
```

-	Layers:
	-	`sha256:bc6b1888979d3ceb063da848b2034e980e2c2613642159c1e856550b79aa620c`  
		Last Modified: Tue, 19 Dec 2023 01:47:38 GMT  
		Size: 27.5 MB (27491874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3940bd8b958075529145975f552f030ebc62a56083ae9e2ec9058a92ea0ab779`  
		Last Modified: Tue, 19 Dec 2023 10:02:14 GMT  
		Size: 84.8 MB (84831742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb1488658ec91ebf7b68fc1fb93f9c1b080f2aa4dd7407cfe14422af0a66a9f`  
		Last Modified: Tue, 19 Dec 2023 10:02:02 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.4-alpine`

```console
$ docker pull varnish@sha256:dccb7bbef9e81823cff443fb4a939c7b4f8c12e7ebd7e4ccf6f61d160a7f1697
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.4-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:b5eac55ba74a47af082bddac8f75de72ab56c24b23dff05b3bed748daa07e97f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73099369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c47739cdf917b26886e22b56f88ed349bd402588e139d368a79c43130e0edb81`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:20:49 GMT
ADD file:1f4eb46669b5b6275af19eb7471a6899a61c276aa7d925b8ae99310b14b75b92 in / 
# Fri, 08 Dec 2023 01:20:49 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 17:27:32 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Mon, 11 Dec 2023 17:27:32 GMT
ARG VARNISH_VERSION=7.4.2
# Mon, 11 Dec 2023 17:27:32 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Mon, 11 Dec 2023 17:27:32 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 17:27:32 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 17:27:32 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Mon, 11 Dec 2023 17:27:32 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Mon, 11 Dec 2023 17:27:32 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Mon, 11 Dec 2023 17:27:32 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 17:27:32 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 17:27:32 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 17:28:57 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 17:28:57 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 17:28:57 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 17:28:57 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 17:28:57 GMT
USER varnish
# Mon, 11 Dec 2023 17:28:57 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 17:28:57 GMT
CMD []
```

-	Layers:
	-	`sha256:661ff4d9561e3fd050929ee5097067c34bafc523ee60f5294a37fd08056a73ca`  
		Last Modified: Fri, 08 Dec 2023 01:21:10 GMT  
		Size: 3.4 MB (3408480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596ff0f1e45ff73a12d763f801097546e24d971a656c1e6c500464e3d9dc93d1`  
		Last Modified: Mon, 11 Dec 2023 17:30:59 GMT  
		Size: 69.7 MB (69690393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c9254892d8bb199804b7583c9d4976bb18fc6ffd3f835b13a09661f7f44eec`  
		Last Modified: Mon, 11 Dec 2023 17:30:50 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:87a53efcd35a17d5bfd0e5c7c785d5763c252ed86ec36857dac3fe45d93a33b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.3 MB (57297011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b2c19442982ba0e6c0be7f492a6ec1ada91fcc8a5ba1969f78b73a95d385b49`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:57:20 GMT
ADD file:13b9291053208eec61cd7c97bac2fa154380ad8d10182567763eea3e10c5882f in / 
# Fri, 08 Dec 2023 01:57:20 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 20:34:14 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Mon, 11 Dec 2023 20:34:14 GMT
ARG VARNISH_VERSION=7.4.2
# Mon, 11 Dec 2023 20:34:14 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Mon, 11 Dec 2023 20:34:14 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 20:34:14 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 20:34:15 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Mon, 11 Dec 2023 20:34:15 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Mon, 11 Dec 2023 20:34:15 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Mon, 11 Dec 2023 20:34:15 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 20:34:15 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 20:34:15 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 20:35:49 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 20:35:49 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 20:35:49 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 20:35:49 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 20:35:50 GMT
USER varnish
# Mon, 11 Dec 2023 20:35:50 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 20:35:50 GMT
CMD []
```

-	Layers:
	-	`sha256:1086c24c41097f090ce847d192c11307e1715eeb563a2cf4f410b2a199ae1942`  
		Last Modified: Fri, 08 Dec 2023 01:57:36 GMT  
		Size: 2.9 MB (2918701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c36cad4b93a74bd362b04d858cd9d78544bbb44bf895d4f6f5af8579139a2c7`  
		Last Modified: Mon, 11 Dec 2023 20:38:54 GMT  
		Size: 54.4 MB (54377812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a48e0aa1dee5bbd35355dac977a62f98ae8d12c24cf4ff2840627e55f9e3af`  
		Last Modified: Mon, 11 Dec 2023 20:38:48 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:c3a738cfcba71417cb1dbd6d79c584cf8ab596101cec9da60ae7550d322ff93a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69801066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd43f5c0e3e024f3ba7432e4d185a26e5527662f7ef11c692005bf9c34994822`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:39:30 GMT
ADD file:8182c73f869a899cf624a59c400acb8226776d15e4d3a0d240a94e65340540d0 in / 
# Fri, 08 Dec 2023 01:39:30 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:15:41 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Mon, 11 Dec 2023 19:15:41 GMT
ARG VARNISH_VERSION=7.4.2
# Mon, 11 Dec 2023 19:15:41 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Mon, 11 Dec 2023 19:15:41 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 19:15:41 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 19:15:41 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Mon, 11 Dec 2023 19:15:41 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Mon, 11 Dec 2023 19:15:41 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Mon, 11 Dec 2023 19:15:41 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 19:15:41 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 19:15:41 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 19:16:58 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 19:16:58 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 19:16:59 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 19:16:59 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 19:16:59 GMT
USER varnish
# Mon, 11 Dec 2023 19:16:59 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 19:16:59 GMT
CMD []
```

-	Layers:
	-	`sha256:c303524923177661067f7eb378c3dd5277088c2676ebd1cd78e68397bb80fdbf`  
		Last Modified: Fri, 08 Dec 2023 01:39:48 GMT  
		Size: 3.3 MB (3347794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62285e0f2c1fa910fd125cc6c60e04450bca85c9ae1dfc3e94e75962246bed4`  
		Last Modified: Mon, 11 Dec 2023 19:18:53 GMT  
		Size: 66.5 MB (66452773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88163622582d5ecfa15893cced49ef724d3bbcbc6a809c3eb87c3e8434a0ed8`  
		Last Modified: Mon, 11 Dec 2023 19:18:46 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4-alpine` - linux; 386

```console
$ docker pull varnish@sha256:a79e39ac0276a1a34a258fbeeb02ac4b8b9e1c671b97f7a074fd2b6b4ae61023
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75122339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d691498e2889909c12cf91c9d555aed1a790d657a76cbc91c6b8d70a09ac4f25`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:38:25 GMT
ADD file:bd52540f209ba362654d795d7893669c819d35011a16f9f319301727a33b3bd9 in / 
# Fri, 08 Dec 2023 01:38:25 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 17:38:39 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Mon, 11 Dec 2023 17:38:39 GMT
ARG VARNISH_VERSION=7.4.2
# Mon, 11 Dec 2023 17:38:39 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Mon, 11 Dec 2023 17:38:39 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 17:38:39 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 17:38:40 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Mon, 11 Dec 2023 17:38:40 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Mon, 11 Dec 2023 17:38:40 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Mon, 11 Dec 2023 17:38:40 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 17:38:40 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 17:38:40 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 17:41:07 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 17:41:07 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 17:41:07 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 17:41:07 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 17:41:08 GMT
USER varnish
# Mon, 11 Dec 2023 17:41:08 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 17:41:08 GMT
CMD []
```

-	Layers:
	-	`sha256:9acd8b4c9d4385585f74dabb4bc6b3351888710ae37ec5dbd9ea950281b8f9bb`  
		Last Modified: Fri, 08 Dec 2023 01:38:43 GMT  
		Size: 3.2 MB (3244115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238a34d823f5a0cc31c7c355c956fd3e368a725f030f90a9e5d7df163792781d`  
		Last Modified: Mon, 11 Dec 2023 17:43:54 GMT  
		Size: 71.9 MB (71877729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57837da0913799765f0e9fd3302510c33ad5687b16eba780a53df338bc424d68`  
		Last Modified: Mon, 11 Dec 2023 17:43:40 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:b1b11ea19fa1b2687950414bb42591a92a3393f5395012ddc49e30e188233c95
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70614826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0564114572d93006a1a5cdd6ad53c188754e8c924236219640b9da35370cc7c3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:22:51 GMT
ADD file:052421189f8d269382daaaa8beb63c687e4d8ca908c421abdce53bcc627a40b4 in / 
# Fri, 08 Dec 2023 01:22:51 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 17:23:45 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Mon, 11 Dec 2023 17:23:45 GMT
ARG VARNISH_VERSION=7.4.2
# Mon, 11 Dec 2023 17:23:46 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Mon, 11 Dec 2023 17:23:46 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 17:23:46 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 17:23:47 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Mon, 11 Dec 2023 17:23:47 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Mon, 11 Dec 2023 17:23:47 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Mon, 11 Dec 2023 17:23:47 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 17:23:47 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 17:23:48 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 17:25:32 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 17:25:35 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 17:25:35 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 17:25:35 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 17:25:35 GMT
USER varnish
# Mon, 11 Dec 2023 17:25:36 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 17:25:36 GMT
CMD []
```

-	Layers:
	-	`sha256:243ac51c334a47917a84be93e972ee6378987e9b3b917a5a8df29025e161c1f3`  
		Last Modified: Fri, 08 Dec 2023 01:23:14 GMT  
		Size: 3.4 MB (3358233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3df8df9f5a4588e06e3e5398e16334f14812f2fdf045fd348b76a021da038d2`  
		Last Modified: Mon, 11 Dec 2023 17:27:46 GMT  
		Size: 67.3 MB (67256096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a44bfc4f6b4cc77283fb963e01fa094f85bf552a7514cb05c8c37783a83ff005`  
		Last Modified: Mon, 11 Dec 2023 17:27:35 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:2cea98b4853ec31e2735aca0c3e36d4f79721ea90b05a682e8a3a3701b334c9d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (64983529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dca28acdd122e49a4f4ebe4f0c061684c2798f776cc451771e4a27ea500fd75`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:41:50 GMT
ADD file:47e0982fc3ae485c06d46f3c0022afd39ed7ec95fe755c2391e6b0cfcae65dfc in / 
# Fri, 08 Dec 2023 01:41:51 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:52:03 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Mon, 11 Dec 2023 19:52:03 GMT
ARG VARNISH_VERSION=7.4.2
# Mon, 11 Dec 2023 19:52:04 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Mon, 11 Dec 2023 19:52:04 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 19:52:04 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 19:52:05 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Mon, 11 Dec 2023 19:52:05 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Mon, 11 Dec 2023 19:52:05 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Mon, 11 Dec 2023 19:52:06 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 19:52:06 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 19:52:06 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 19:53:37 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 19:53:40 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 19:53:40 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 19:53:41 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 19:53:41 GMT
USER varnish
# Mon, 11 Dec 2023 19:53:41 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 19:53:41 GMT
CMD []
```

-	Layers:
	-	`sha256:0fca3ee44ced87b7184bc23390283fdf10cfae0e844a25b785dd11c463815227`  
		Last Modified: Fri, 08 Dec 2023 01:42:30 GMT  
		Size: 3.2 MB (3242332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebca86ea5cb356f01dcce8ee2acb336ac6e346114eee85687c7bdbe3b09f508`  
		Last Modified: Mon, 11 Dec 2023 19:56:11 GMT  
		Size: 61.7 MB (61740701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15fe8e4d2daf80c7668faf912a02bf7be20425091121a2bd932d5025606840b`  
		Last Modified: Mon, 11 Dec 2023 19:56:02 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.4.2`

```console
$ docker pull varnish@sha256:74f3de816160fb949b01111c302f4d37a49b45b1a754d1e145e8d3d7dc94cfb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.4.2` - linux; amd64

```console
$ docker pull varnish@sha256:eadc1f8f442bb86961c300d37a64bb51b2658b8f6bed39c21fdd85405775c144
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134738894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e44717a97df19098a313b57e48e02fe1b413b2d92fe2eb3e6350c5f85ed591df`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 01:20:27 GMT
ADD file:ac3cd70031d35e46d86b876934946ffc8756de4de065fbc926dce642dac07ff3 in / 
# Tue, 19 Dec 2023 01:20:28 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:59:51 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Tue, 19 Dec 2023 07:59:51 GMT
ARG VARNISH_VERSION=7.4.2
# Tue, 19 Dec 2023 07:59:51 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Tue, 19 Dec 2023 07:59:51 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 19 Dec 2023 07:59:52 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 19 Dec 2023 07:59:52 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Tue, 19 Dec 2023 07:59:52 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Tue, 19 Dec 2023 07:59:52 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Tue, 19 Dec 2023 07:59:52 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 19 Dec 2023 07:59:52 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 19 Dec 2023 07:59:52 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 08:02:47 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.2.tgz -o $tmpdir/orig.tgz;     echo "acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 19 Dec 2023 08:02:48 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 08:02:48 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 19 Dec 2023 08:02:48 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 08:02:48 GMT
USER varnish
# Tue, 19 Dec 2023 08:02:48 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 08:02:49 GMT
CMD []
```

-	Layers:
	-	`sha256:af107e978371b6cd6339127a05502c5eacd1e6b0e9eb7b2f4aa7b6fc87e2dd81`  
		Last Modified: Tue, 19 Dec 2023 01:24:59 GMT  
		Size: 29.1 MB (29125963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b1c37f74eda351d5d18bd05ac7a597435e4dcc3dca90495bfb8704d7030f37`  
		Last Modified: Tue, 19 Dec 2023 08:08:18 GMT  
		Size: 105.6 MB (105612439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98889ac1ccb507f3093353ef6ddc3ca2dae1063b5323bb989732b0271c784f40`  
		Last Modified: Tue, 19 Dec 2023 08:08:03 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4.2` - linux; arm variant v7

```console
$ docker pull varnish@sha256:0b0725305bd25fb5c7804c983f3a03f5c358908c150b56e6fc7754762d2fad7f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104987802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36b50ea5a138f4de8b6fb2c81a616b546478c36e122bd5e421db168ef5ad924c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 02:07:50 GMT
ADD file:aef112919e7924ad6da32181b1df5099cd692680c104118da3a24cd4dfe55a1d in / 
# Tue, 19 Dec 2023 02:07:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:11:51 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Tue, 19 Dec 2023 08:11:51 GMT
ARG VARNISH_VERSION=7.4.2
# Tue, 19 Dec 2023 08:11:51 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Tue, 19 Dec 2023 08:11:51 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 19 Dec 2023 08:11:51 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 19 Dec 2023 08:11:51 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Tue, 19 Dec 2023 08:11:51 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Tue, 19 Dec 2023 08:11:52 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Tue, 19 Dec 2023 08:11:52 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 19 Dec 2023 08:11:52 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 19 Dec 2023 08:11:52 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 08:14:41 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.2.tgz -o $tmpdir/orig.tgz;     echo "acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 19 Dec 2023 08:14:42 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 08:14:42 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 19 Dec 2023 08:14:42 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 08:14:42 GMT
USER varnish
# Tue, 19 Dec 2023 08:14:42 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 08:14:43 GMT
CMD []
```

-	Layers:
	-	`sha256:65ab19615c01a3b542f77fadb3bd27872b6a20cba3e9269fb951de36d8fa6805`  
		Last Modified: Tue, 19 Dec 2023 02:11:52 GMT  
		Size: 24.7 MB (24718157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0329b82b2a3ad7a3589db33efac87f48ea52033e08b8fb622036d689eac669e`  
		Last Modified: Tue, 19 Dec 2023 08:20:12 GMT  
		Size: 80.3 MB (80269153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:873759df9ef5bea1a9b39771cb9f95f002aab5fcac9279141c11bad88f032d9a`  
		Last Modified: Tue, 19 Dec 2023 08:20:00 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4.2` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:7b765c330312fbd652f5811c86c4c6b3e88e2e2c24d7e16f83f4b1782bd8cb90
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.2 MB (129246108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23a72da26db114f62729359648ac0a655eb843e6245e8c01514293bbfcb75b91`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 21:16:36 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Tue, 21 Nov 2023 21:16:36 GMT
ARG VARNISH_VERSION=7.4.2
# Tue, 21 Nov 2023 21:16:37 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Tue, 21 Nov 2023 21:16:37 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 21 Nov 2023 21:16:37 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 21 Nov 2023 21:16:37 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Tue, 21 Nov 2023 21:16:37 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Tue, 21 Nov 2023 21:16:37 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Tue, 21 Nov 2023 21:16:37 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 21 Nov 2023 21:16:37 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 21 Nov 2023 21:16:37 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 21:19:02 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.2.tgz -o $tmpdir/orig.tgz;     echo "acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 21 Nov 2023 21:19:04 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 21:19:04 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 21 Nov 2023 21:19:04 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 21:19:04 GMT
USER varnish
# Tue, 21 Nov 2023 21:19:04 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 21:19:04 GMT
CMD []
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4c433f9fe1b4c04daf893df7f3dde2d25de13ed8474ae8887c623dbb3b0d5f`  
		Last Modified: Tue, 21 Nov 2023 21:23:39 GMT  
		Size: 100.1 MB (100066338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700ba44dbd53506d34d537e4614e9fb6a06b8a9aa2797b7e028061bc36b56044`  
		Last Modified: Tue, 21 Nov 2023 21:23:28 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4.2` - linux; 386

```console
$ docker pull varnish@sha256:f7094353a24b15c6f1dc90d7efd0fd58cbeba2336184d3b5eedca4b98da770a4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131941018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e481519ab9391779d3c4321f01ff5a60343ba4a44a01e1184384da4fd9eacc19`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 04:39:53 GMT
ADD file:930e1b9d85b6927c4d3046f7c75de2f3bfc6ec29100c314d0ab2b780ea30e962 in / 
# Tue, 21 Nov 2023 04:39:53 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 15:11:13 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Tue, 21 Nov 2023 15:11:13 GMT
ARG VARNISH_VERSION=7.4.2
# Tue, 21 Nov 2023 15:11:13 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Tue, 21 Nov 2023 15:11:13 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 21 Nov 2023 15:11:13 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 21 Nov 2023 15:11:13 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Tue, 21 Nov 2023 15:11:13 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Tue, 21 Nov 2023 15:11:14 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Tue, 21 Nov 2023 15:11:14 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 21 Nov 2023 15:11:14 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 21 Nov 2023 15:11:14 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 15:14:49 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.2.tgz -o $tmpdir/orig.tgz;     echo "acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 21 Nov 2023 15:14:50 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 15:14:51 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 21 Nov 2023 15:14:51 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 15:14:51 GMT
USER varnish
# Tue, 21 Nov 2023 15:14:51 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 15:14:51 GMT
CMD []
```

-	Layers:
	-	`sha256:c0734eabce8885d8904dbd11b77aa97c2d2b04bc8e2af9e89d47c4bda590dd8e`  
		Last Modified: Tue, 21 Nov 2023 04:44:34 GMT  
		Size: 30.2 MB (30164109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebaa590b85c3666b3aa98d7f7f7d5e957400d175de18f1a103ee9fc72f3ff1e`  
		Last Modified: Tue, 21 Nov 2023 15:21:44 GMT  
		Size: 101.8 MB (101776416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb43c8e9e7fcf7c7d91ab556103770f53e487c54d5b6d3a5e6eae1531dabb03c`  
		Last Modified: Tue, 21 Nov 2023 15:21:22 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4.2` - linux; ppc64le

```console
$ docker pull varnish@sha256:2393ba60ad3c5b5c3b8dc33eecd5388405e067b6c7b6aa6614d4c0e22d8cb740
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.7 MB (137679921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11d740886e444fe4a948031256adfe8d9d4148f985a3451ff9217f8b3b02084b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 12:50:24 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Tue, 21 Nov 2023 12:50:24 GMT
ARG VARNISH_VERSION=7.4.2
# Tue, 21 Nov 2023 12:50:24 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Tue, 21 Nov 2023 12:50:24 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 21 Nov 2023 12:50:25 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 21 Nov 2023 12:50:25 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Tue, 21 Nov 2023 12:50:25 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Tue, 21 Nov 2023 12:50:25 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Tue, 21 Nov 2023 12:50:25 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 21 Nov 2023 12:50:26 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 21 Nov 2023 12:50:26 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 12:54:18 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.2.tgz -o $tmpdir/orig.tgz;     echo "acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 21 Nov 2023 12:54:22 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 12:54:23 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 21 Nov 2023 12:54:23 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 12:54:23 GMT
USER varnish
# Tue, 21 Nov 2023 12:54:23 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 12:54:24 GMT
CMD []
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53276baea44ef2eb7632af8b3e497190197e059d4973c54c393e8e514579fee6`  
		Last Modified: Tue, 21 Nov 2023 13:01:56 GMT  
		Size: 104.5 MB (104537822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e228724f48a9283f83071d90b2ad5ea3adbd7aa8db408cf9cc17907d068aefd9`  
		Last Modified: Tue, 21 Nov 2023 13:01:38 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4.2` - linux; s390x

```console
$ docker pull varnish@sha256:6c7d0645cb3a69ac8d8f1550498bd4d8cdea53596dec94bcb46dd960a79f7032
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112324108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a720df683a8465e59eb06466380c0e7aa703e6e2adeafe901b372ac4a969610`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 01:42:37 GMT
ADD file:f06f12fa5a93afc3a79ac4371d24b0a471a5a1818cf34c1d90004c8f410914b9 in / 
# Tue, 19 Dec 2023 01:42:39 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 09:54:42 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Tue, 19 Dec 2023 09:54:43 GMT
ARG VARNISH_VERSION=7.4.2
# Tue, 19 Dec 2023 09:54:43 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Tue, 19 Dec 2023 09:54:43 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 19 Dec 2023 09:54:43 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 19 Dec 2023 09:54:43 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Tue, 19 Dec 2023 09:54:43 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Tue, 19 Dec 2023 09:54:43 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Tue, 19 Dec 2023 09:54:43 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 19 Dec 2023 09:54:43 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 19 Dec 2023 09:54:44 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 09:57:01 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.2.tgz -o $tmpdir/orig.tgz;     echo "acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 19 Dec 2023 09:57:06 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 09:57:06 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 19 Dec 2023 09:57:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 09:57:06 GMT
USER varnish
# Tue, 19 Dec 2023 09:57:07 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 09:57:07 GMT
CMD []
```

-	Layers:
	-	`sha256:bc6b1888979d3ceb063da848b2034e980e2c2613642159c1e856550b79aa620c`  
		Last Modified: Tue, 19 Dec 2023 01:47:38 GMT  
		Size: 27.5 MB (27491874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3940bd8b958075529145975f552f030ebc62a56083ae9e2ec9058a92ea0ab779`  
		Last Modified: Tue, 19 Dec 2023 10:02:14 GMT  
		Size: 84.8 MB (84831742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb1488658ec91ebf7b68fc1fb93f9c1b080f2aa4dd7407cfe14422af0a66a9f`  
		Last Modified: Tue, 19 Dec 2023 10:02:02 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:7.4.2-alpine`

```console
$ docker pull varnish@sha256:dccb7bbef9e81823cff443fb4a939c7b4f8c12e7ebd7e4ccf6f61d160a7f1697
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:7.4.2-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:b5eac55ba74a47af082bddac8f75de72ab56c24b23dff05b3bed748daa07e97f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73099369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c47739cdf917b26886e22b56f88ed349bd402588e139d368a79c43130e0edb81`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:20:49 GMT
ADD file:1f4eb46669b5b6275af19eb7471a6899a61c276aa7d925b8ae99310b14b75b92 in / 
# Fri, 08 Dec 2023 01:20:49 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 17:27:32 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Mon, 11 Dec 2023 17:27:32 GMT
ARG VARNISH_VERSION=7.4.2
# Mon, 11 Dec 2023 17:27:32 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Mon, 11 Dec 2023 17:27:32 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 17:27:32 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 17:27:32 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Mon, 11 Dec 2023 17:27:32 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Mon, 11 Dec 2023 17:27:32 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Mon, 11 Dec 2023 17:27:32 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 17:27:32 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 17:27:32 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 17:28:57 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 17:28:57 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 17:28:57 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 17:28:57 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 17:28:57 GMT
USER varnish
# Mon, 11 Dec 2023 17:28:57 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 17:28:57 GMT
CMD []
```

-	Layers:
	-	`sha256:661ff4d9561e3fd050929ee5097067c34bafc523ee60f5294a37fd08056a73ca`  
		Last Modified: Fri, 08 Dec 2023 01:21:10 GMT  
		Size: 3.4 MB (3408480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596ff0f1e45ff73a12d763f801097546e24d971a656c1e6c500464e3d9dc93d1`  
		Last Modified: Mon, 11 Dec 2023 17:30:59 GMT  
		Size: 69.7 MB (69690393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c9254892d8bb199804b7583c9d4976bb18fc6ffd3f835b13a09661f7f44eec`  
		Last Modified: Mon, 11 Dec 2023 17:30:50 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4.2-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:87a53efcd35a17d5bfd0e5c7c785d5763c252ed86ec36857dac3fe45d93a33b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.3 MB (57297011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b2c19442982ba0e6c0be7f492a6ec1ada91fcc8a5ba1969f78b73a95d385b49`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:57:20 GMT
ADD file:13b9291053208eec61cd7c97bac2fa154380ad8d10182567763eea3e10c5882f in / 
# Fri, 08 Dec 2023 01:57:20 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 20:34:14 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Mon, 11 Dec 2023 20:34:14 GMT
ARG VARNISH_VERSION=7.4.2
# Mon, 11 Dec 2023 20:34:14 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Mon, 11 Dec 2023 20:34:14 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 20:34:14 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 20:34:15 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Mon, 11 Dec 2023 20:34:15 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Mon, 11 Dec 2023 20:34:15 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Mon, 11 Dec 2023 20:34:15 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 20:34:15 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 20:34:15 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 20:35:49 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 20:35:49 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 20:35:49 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 20:35:49 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 20:35:50 GMT
USER varnish
# Mon, 11 Dec 2023 20:35:50 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 20:35:50 GMT
CMD []
```

-	Layers:
	-	`sha256:1086c24c41097f090ce847d192c11307e1715eeb563a2cf4f410b2a199ae1942`  
		Last Modified: Fri, 08 Dec 2023 01:57:36 GMT  
		Size: 2.9 MB (2918701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c36cad4b93a74bd362b04d858cd9d78544bbb44bf895d4f6f5af8579139a2c7`  
		Last Modified: Mon, 11 Dec 2023 20:38:54 GMT  
		Size: 54.4 MB (54377812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a48e0aa1dee5bbd35355dac977a62f98ae8d12c24cf4ff2840627e55f9e3af`  
		Last Modified: Mon, 11 Dec 2023 20:38:48 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4.2-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:c3a738cfcba71417cb1dbd6d79c584cf8ab596101cec9da60ae7550d322ff93a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69801066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd43f5c0e3e024f3ba7432e4d185a26e5527662f7ef11c692005bf9c34994822`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:39:30 GMT
ADD file:8182c73f869a899cf624a59c400acb8226776d15e4d3a0d240a94e65340540d0 in / 
# Fri, 08 Dec 2023 01:39:30 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:15:41 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Mon, 11 Dec 2023 19:15:41 GMT
ARG VARNISH_VERSION=7.4.2
# Mon, 11 Dec 2023 19:15:41 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Mon, 11 Dec 2023 19:15:41 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 19:15:41 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 19:15:41 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Mon, 11 Dec 2023 19:15:41 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Mon, 11 Dec 2023 19:15:41 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Mon, 11 Dec 2023 19:15:41 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 19:15:41 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 19:15:41 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 19:16:58 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 19:16:58 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 19:16:59 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 19:16:59 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 19:16:59 GMT
USER varnish
# Mon, 11 Dec 2023 19:16:59 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 19:16:59 GMT
CMD []
```

-	Layers:
	-	`sha256:c303524923177661067f7eb378c3dd5277088c2676ebd1cd78e68397bb80fdbf`  
		Last Modified: Fri, 08 Dec 2023 01:39:48 GMT  
		Size: 3.3 MB (3347794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62285e0f2c1fa910fd125cc6c60e04450bca85c9ae1dfc3e94e75962246bed4`  
		Last Modified: Mon, 11 Dec 2023 19:18:53 GMT  
		Size: 66.5 MB (66452773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88163622582d5ecfa15893cced49ef724d3bbcbc6a809c3eb87c3e8434a0ed8`  
		Last Modified: Mon, 11 Dec 2023 19:18:46 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4.2-alpine` - linux; 386

```console
$ docker pull varnish@sha256:a79e39ac0276a1a34a258fbeeb02ac4b8b9e1c671b97f7a074fd2b6b4ae61023
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75122339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d691498e2889909c12cf91c9d555aed1a790d657a76cbc91c6b8d70a09ac4f25`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:38:25 GMT
ADD file:bd52540f209ba362654d795d7893669c819d35011a16f9f319301727a33b3bd9 in / 
# Fri, 08 Dec 2023 01:38:25 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 17:38:39 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Mon, 11 Dec 2023 17:38:39 GMT
ARG VARNISH_VERSION=7.4.2
# Mon, 11 Dec 2023 17:38:39 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Mon, 11 Dec 2023 17:38:39 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 17:38:39 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 17:38:40 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Mon, 11 Dec 2023 17:38:40 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Mon, 11 Dec 2023 17:38:40 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Mon, 11 Dec 2023 17:38:40 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 17:38:40 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 17:38:40 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 17:41:07 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 17:41:07 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 17:41:07 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 17:41:07 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 17:41:08 GMT
USER varnish
# Mon, 11 Dec 2023 17:41:08 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 17:41:08 GMT
CMD []
```

-	Layers:
	-	`sha256:9acd8b4c9d4385585f74dabb4bc6b3351888710ae37ec5dbd9ea950281b8f9bb`  
		Last Modified: Fri, 08 Dec 2023 01:38:43 GMT  
		Size: 3.2 MB (3244115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238a34d823f5a0cc31c7c355c956fd3e368a725f030f90a9e5d7df163792781d`  
		Last Modified: Mon, 11 Dec 2023 17:43:54 GMT  
		Size: 71.9 MB (71877729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57837da0913799765f0e9fd3302510c33ad5687b16eba780a53df338bc424d68`  
		Last Modified: Mon, 11 Dec 2023 17:43:40 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4.2-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:b1b11ea19fa1b2687950414bb42591a92a3393f5395012ddc49e30e188233c95
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70614826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0564114572d93006a1a5cdd6ad53c188754e8c924236219640b9da35370cc7c3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:22:51 GMT
ADD file:052421189f8d269382daaaa8beb63c687e4d8ca908c421abdce53bcc627a40b4 in / 
# Fri, 08 Dec 2023 01:22:51 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 17:23:45 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Mon, 11 Dec 2023 17:23:45 GMT
ARG VARNISH_VERSION=7.4.2
# Mon, 11 Dec 2023 17:23:46 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Mon, 11 Dec 2023 17:23:46 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 17:23:46 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 17:23:47 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Mon, 11 Dec 2023 17:23:47 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Mon, 11 Dec 2023 17:23:47 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Mon, 11 Dec 2023 17:23:47 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 17:23:47 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 17:23:48 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 17:25:32 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 17:25:35 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 17:25:35 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 17:25:35 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 17:25:35 GMT
USER varnish
# Mon, 11 Dec 2023 17:25:36 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 17:25:36 GMT
CMD []
```

-	Layers:
	-	`sha256:243ac51c334a47917a84be93e972ee6378987e9b3b917a5a8df29025e161c1f3`  
		Last Modified: Fri, 08 Dec 2023 01:23:14 GMT  
		Size: 3.4 MB (3358233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3df8df9f5a4588e06e3e5398e16334f14812f2fdf045fd348b76a021da038d2`  
		Last Modified: Mon, 11 Dec 2023 17:27:46 GMT  
		Size: 67.3 MB (67256096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a44bfc4f6b4cc77283fb963e01fa094f85bf552a7514cb05c8c37783a83ff005`  
		Last Modified: Mon, 11 Dec 2023 17:27:35 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:7.4.2-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:2cea98b4853ec31e2735aca0c3e36d4f79721ea90b05a682e8a3a3701b334c9d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (64983529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dca28acdd122e49a4f4ebe4f0c061684c2798f776cc451771e4a27ea500fd75`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:41:50 GMT
ADD file:47e0982fc3ae485c06d46f3c0022afd39ed7ec95fe755c2391e6b0cfcae65dfc in / 
# Fri, 08 Dec 2023 01:41:51 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:52:03 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Mon, 11 Dec 2023 19:52:03 GMT
ARG VARNISH_VERSION=7.4.2
# Mon, 11 Dec 2023 19:52:04 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Mon, 11 Dec 2023 19:52:04 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 19:52:04 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 19:52:05 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Mon, 11 Dec 2023 19:52:05 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Mon, 11 Dec 2023 19:52:05 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Mon, 11 Dec 2023 19:52:06 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 19:52:06 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 19:52:06 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 19:53:37 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 19:53:40 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 19:53:40 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 19:53:41 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 19:53:41 GMT
USER varnish
# Mon, 11 Dec 2023 19:53:41 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 19:53:41 GMT
CMD []
```

-	Layers:
	-	`sha256:0fca3ee44ced87b7184bc23390283fdf10cfae0e844a25b785dd11c463815227`  
		Last Modified: Fri, 08 Dec 2023 01:42:30 GMT  
		Size: 3.2 MB (3242332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebca86ea5cb356f01dcce8ee2acb336ac6e346114eee85687c7bdbe3b09f508`  
		Last Modified: Mon, 11 Dec 2023 19:56:11 GMT  
		Size: 61.7 MB (61740701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15fe8e4d2daf80c7668faf912a02bf7be20425091121a2bd932d5025606840b`  
		Last Modified: Mon, 11 Dec 2023 19:56:02 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:alpine`

```console
$ docker pull varnish@sha256:dccb7bbef9e81823cff443fb4a939c7b4f8c12e7ebd7e4ccf6f61d160a7f1697
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:alpine` - linux; amd64

```console
$ docker pull varnish@sha256:b5eac55ba74a47af082bddac8f75de72ab56c24b23dff05b3bed748daa07e97f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73099369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c47739cdf917b26886e22b56f88ed349bd402588e139d368a79c43130e0edb81`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:20:49 GMT
ADD file:1f4eb46669b5b6275af19eb7471a6899a61c276aa7d925b8ae99310b14b75b92 in / 
# Fri, 08 Dec 2023 01:20:49 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 17:27:32 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Mon, 11 Dec 2023 17:27:32 GMT
ARG VARNISH_VERSION=7.4.2
# Mon, 11 Dec 2023 17:27:32 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Mon, 11 Dec 2023 17:27:32 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 17:27:32 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 17:27:32 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Mon, 11 Dec 2023 17:27:32 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Mon, 11 Dec 2023 17:27:32 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Mon, 11 Dec 2023 17:27:32 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 17:27:32 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 17:27:32 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 17:28:57 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 17:28:57 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 17:28:57 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 17:28:57 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 17:28:57 GMT
USER varnish
# Mon, 11 Dec 2023 17:28:57 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 17:28:57 GMT
CMD []
```

-	Layers:
	-	`sha256:661ff4d9561e3fd050929ee5097067c34bafc523ee60f5294a37fd08056a73ca`  
		Last Modified: Fri, 08 Dec 2023 01:21:10 GMT  
		Size: 3.4 MB (3408480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596ff0f1e45ff73a12d763f801097546e24d971a656c1e6c500464e3d9dc93d1`  
		Last Modified: Mon, 11 Dec 2023 17:30:59 GMT  
		Size: 69.7 MB (69690393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c9254892d8bb199804b7583c9d4976bb18fc6ffd3f835b13a09661f7f44eec`  
		Last Modified: Mon, 11 Dec 2023 17:30:50 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:87a53efcd35a17d5bfd0e5c7c785d5763c252ed86ec36857dac3fe45d93a33b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.3 MB (57297011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b2c19442982ba0e6c0be7f492a6ec1ada91fcc8a5ba1969f78b73a95d385b49`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:57:20 GMT
ADD file:13b9291053208eec61cd7c97bac2fa154380ad8d10182567763eea3e10c5882f in / 
# Fri, 08 Dec 2023 01:57:20 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 20:34:14 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Mon, 11 Dec 2023 20:34:14 GMT
ARG VARNISH_VERSION=7.4.2
# Mon, 11 Dec 2023 20:34:14 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Mon, 11 Dec 2023 20:34:14 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 20:34:14 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 20:34:15 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Mon, 11 Dec 2023 20:34:15 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Mon, 11 Dec 2023 20:34:15 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Mon, 11 Dec 2023 20:34:15 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 20:34:15 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 20:34:15 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 20:35:49 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 20:35:49 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 20:35:49 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 20:35:49 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 20:35:50 GMT
USER varnish
# Mon, 11 Dec 2023 20:35:50 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 20:35:50 GMT
CMD []
```

-	Layers:
	-	`sha256:1086c24c41097f090ce847d192c11307e1715eeb563a2cf4f410b2a199ae1942`  
		Last Modified: Fri, 08 Dec 2023 01:57:36 GMT  
		Size: 2.9 MB (2918701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c36cad4b93a74bd362b04d858cd9d78544bbb44bf895d4f6f5af8579139a2c7`  
		Last Modified: Mon, 11 Dec 2023 20:38:54 GMT  
		Size: 54.4 MB (54377812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a48e0aa1dee5bbd35355dac977a62f98ae8d12c24cf4ff2840627e55f9e3af`  
		Last Modified: Mon, 11 Dec 2023 20:38:48 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:c3a738cfcba71417cb1dbd6d79c584cf8ab596101cec9da60ae7550d322ff93a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69801066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd43f5c0e3e024f3ba7432e4d185a26e5527662f7ef11c692005bf9c34994822`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:39:30 GMT
ADD file:8182c73f869a899cf624a59c400acb8226776d15e4d3a0d240a94e65340540d0 in / 
# Fri, 08 Dec 2023 01:39:30 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:15:41 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Mon, 11 Dec 2023 19:15:41 GMT
ARG VARNISH_VERSION=7.4.2
# Mon, 11 Dec 2023 19:15:41 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Mon, 11 Dec 2023 19:15:41 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 19:15:41 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 19:15:41 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Mon, 11 Dec 2023 19:15:41 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Mon, 11 Dec 2023 19:15:41 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Mon, 11 Dec 2023 19:15:41 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 19:15:41 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 19:15:41 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 19:16:58 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 19:16:58 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 19:16:59 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 19:16:59 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 19:16:59 GMT
USER varnish
# Mon, 11 Dec 2023 19:16:59 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 19:16:59 GMT
CMD []
```

-	Layers:
	-	`sha256:c303524923177661067f7eb378c3dd5277088c2676ebd1cd78e68397bb80fdbf`  
		Last Modified: Fri, 08 Dec 2023 01:39:48 GMT  
		Size: 3.3 MB (3347794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62285e0f2c1fa910fd125cc6c60e04450bca85c9ae1dfc3e94e75962246bed4`  
		Last Modified: Mon, 11 Dec 2023 19:18:53 GMT  
		Size: 66.5 MB (66452773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88163622582d5ecfa15893cced49ef724d3bbcbc6a809c3eb87c3e8434a0ed8`  
		Last Modified: Mon, 11 Dec 2023 19:18:46 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; 386

```console
$ docker pull varnish@sha256:a79e39ac0276a1a34a258fbeeb02ac4b8b9e1c671b97f7a074fd2b6b4ae61023
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75122339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d691498e2889909c12cf91c9d555aed1a790d657a76cbc91c6b8d70a09ac4f25`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:38:25 GMT
ADD file:bd52540f209ba362654d795d7893669c819d35011a16f9f319301727a33b3bd9 in / 
# Fri, 08 Dec 2023 01:38:25 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 17:38:39 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Mon, 11 Dec 2023 17:38:39 GMT
ARG VARNISH_VERSION=7.4.2
# Mon, 11 Dec 2023 17:38:39 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Mon, 11 Dec 2023 17:38:39 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 17:38:39 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 17:38:40 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Mon, 11 Dec 2023 17:38:40 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Mon, 11 Dec 2023 17:38:40 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Mon, 11 Dec 2023 17:38:40 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 17:38:40 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 17:38:40 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 17:41:07 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 17:41:07 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 17:41:07 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 17:41:07 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 17:41:08 GMT
USER varnish
# Mon, 11 Dec 2023 17:41:08 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 17:41:08 GMT
CMD []
```

-	Layers:
	-	`sha256:9acd8b4c9d4385585f74dabb4bc6b3351888710ae37ec5dbd9ea950281b8f9bb`  
		Last Modified: Fri, 08 Dec 2023 01:38:43 GMT  
		Size: 3.2 MB (3244115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238a34d823f5a0cc31c7c355c956fd3e368a725f030f90a9e5d7df163792781d`  
		Last Modified: Mon, 11 Dec 2023 17:43:54 GMT  
		Size: 71.9 MB (71877729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57837da0913799765f0e9fd3302510c33ad5687b16eba780a53df338bc424d68`  
		Last Modified: Mon, 11 Dec 2023 17:43:40 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:b1b11ea19fa1b2687950414bb42591a92a3393f5395012ddc49e30e188233c95
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70614826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0564114572d93006a1a5cdd6ad53c188754e8c924236219640b9da35370cc7c3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:22:51 GMT
ADD file:052421189f8d269382daaaa8beb63c687e4d8ca908c421abdce53bcc627a40b4 in / 
# Fri, 08 Dec 2023 01:22:51 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 17:23:45 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Mon, 11 Dec 2023 17:23:45 GMT
ARG VARNISH_VERSION=7.4.2
# Mon, 11 Dec 2023 17:23:46 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Mon, 11 Dec 2023 17:23:46 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 17:23:46 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 17:23:47 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Mon, 11 Dec 2023 17:23:47 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Mon, 11 Dec 2023 17:23:47 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Mon, 11 Dec 2023 17:23:47 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 17:23:47 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 17:23:48 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 17:25:32 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 17:25:35 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 17:25:35 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 17:25:35 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 17:25:35 GMT
USER varnish
# Mon, 11 Dec 2023 17:25:36 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 17:25:36 GMT
CMD []
```

-	Layers:
	-	`sha256:243ac51c334a47917a84be93e972ee6378987e9b3b917a5a8df29025e161c1f3`  
		Last Modified: Fri, 08 Dec 2023 01:23:14 GMT  
		Size: 3.4 MB (3358233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3df8df9f5a4588e06e3e5398e16334f14812f2fdf045fd348b76a021da038d2`  
		Last Modified: Mon, 11 Dec 2023 17:27:46 GMT  
		Size: 67.3 MB (67256096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a44bfc4f6b4cc77283fb963e01fa094f85bf552a7514cb05c8c37783a83ff005`  
		Last Modified: Mon, 11 Dec 2023 17:27:35 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:alpine` - linux; s390x

```console
$ docker pull varnish@sha256:2cea98b4853ec31e2735aca0c3e36d4f79721ea90b05a682e8a3a3701b334c9d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (64983529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dca28acdd122e49a4f4ebe4f0c061684c2798f776cc451771e4a27ea500fd75`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:41:50 GMT
ADD file:47e0982fc3ae485c06d46f3c0022afd39ed7ec95fe755c2391e6b0cfcae65dfc in / 
# Fri, 08 Dec 2023 01:41:51 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:52:03 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Mon, 11 Dec 2023 19:52:03 GMT
ARG VARNISH_VERSION=7.4.2
# Mon, 11 Dec 2023 19:52:04 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Mon, 11 Dec 2023 19:52:04 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 19:52:04 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 19:52:05 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Mon, 11 Dec 2023 19:52:05 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Mon, 11 Dec 2023 19:52:05 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Mon, 11 Dec 2023 19:52:06 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 19:52:06 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 19:52:06 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 19:53:37 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 19:53:40 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 19:53:40 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 19:53:41 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 19:53:41 GMT
USER varnish
# Mon, 11 Dec 2023 19:53:41 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 19:53:41 GMT
CMD []
```

-	Layers:
	-	`sha256:0fca3ee44ced87b7184bc23390283fdf10cfae0e844a25b785dd11c463815227`  
		Last Modified: Fri, 08 Dec 2023 01:42:30 GMT  
		Size: 3.2 MB (3242332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebca86ea5cb356f01dcce8ee2acb336ac6e346114eee85687c7bdbe3b09f508`  
		Last Modified: Mon, 11 Dec 2023 19:56:11 GMT  
		Size: 61.7 MB (61740701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15fe8e4d2daf80c7668faf912a02bf7be20425091121a2bd932d5025606840b`  
		Last Modified: Mon, 11 Dec 2023 19:56:02 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:fresh`

```console
$ docker pull varnish@sha256:74f3de816160fb949b01111c302f4d37a49b45b1a754d1e145e8d3d7dc94cfb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:fresh` - linux; amd64

```console
$ docker pull varnish@sha256:eadc1f8f442bb86961c300d37a64bb51b2658b8f6bed39c21fdd85405775c144
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134738894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e44717a97df19098a313b57e48e02fe1b413b2d92fe2eb3e6350c5f85ed591df`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 01:20:27 GMT
ADD file:ac3cd70031d35e46d86b876934946ffc8756de4de065fbc926dce642dac07ff3 in / 
# Tue, 19 Dec 2023 01:20:28 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:59:51 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Tue, 19 Dec 2023 07:59:51 GMT
ARG VARNISH_VERSION=7.4.2
# Tue, 19 Dec 2023 07:59:51 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Tue, 19 Dec 2023 07:59:51 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 19 Dec 2023 07:59:52 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 19 Dec 2023 07:59:52 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Tue, 19 Dec 2023 07:59:52 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Tue, 19 Dec 2023 07:59:52 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Tue, 19 Dec 2023 07:59:52 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 19 Dec 2023 07:59:52 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 19 Dec 2023 07:59:52 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 08:02:47 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.2.tgz -o $tmpdir/orig.tgz;     echo "acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 19 Dec 2023 08:02:48 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 08:02:48 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 19 Dec 2023 08:02:48 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 08:02:48 GMT
USER varnish
# Tue, 19 Dec 2023 08:02:48 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 08:02:49 GMT
CMD []
```

-	Layers:
	-	`sha256:af107e978371b6cd6339127a05502c5eacd1e6b0e9eb7b2f4aa7b6fc87e2dd81`  
		Last Modified: Tue, 19 Dec 2023 01:24:59 GMT  
		Size: 29.1 MB (29125963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b1c37f74eda351d5d18bd05ac7a597435e4dcc3dca90495bfb8704d7030f37`  
		Last Modified: Tue, 19 Dec 2023 08:08:18 GMT  
		Size: 105.6 MB (105612439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98889ac1ccb507f3093353ef6ddc3ca2dae1063b5323bb989732b0271c784f40`  
		Last Modified: Tue, 19 Dec 2023 08:08:03 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; arm variant v7

```console
$ docker pull varnish@sha256:0b0725305bd25fb5c7804c983f3a03f5c358908c150b56e6fc7754762d2fad7f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104987802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36b50ea5a138f4de8b6fb2c81a616b546478c36e122bd5e421db168ef5ad924c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 02:07:50 GMT
ADD file:aef112919e7924ad6da32181b1df5099cd692680c104118da3a24cd4dfe55a1d in / 
# Tue, 19 Dec 2023 02:07:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:11:51 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Tue, 19 Dec 2023 08:11:51 GMT
ARG VARNISH_VERSION=7.4.2
# Tue, 19 Dec 2023 08:11:51 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Tue, 19 Dec 2023 08:11:51 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 19 Dec 2023 08:11:51 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 19 Dec 2023 08:11:51 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Tue, 19 Dec 2023 08:11:51 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Tue, 19 Dec 2023 08:11:52 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Tue, 19 Dec 2023 08:11:52 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 19 Dec 2023 08:11:52 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 19 Dec 2023 08:11:52 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 08:14:41 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.2.tgz -o $tmpdir/orig.tgz;     echo "acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 19 Dec 2023 08:14:42 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 08:14:42 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 19 Dec 2023 08:14:42 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 08:14:42 GMT
USER varnish
# Tue, 19 Dec 2023 08:14:42 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 08:14:43 GMT
CMD []
```

-	Layers:
	-	`sha256:65ab19615c01a3b542f77fadb3bd27872b6a20cba3e9269fb951de36d8fa6805`  
		Last Modified: Tue, 19 Dec 2023 02:11:52 GMT  
		Size: 24.7 MB (24718157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0329b82b2a3ad7a3589db33efac87f48ea52033e08b8fb622036d689eac669e`  
		Last Modified: Tue, 19 Dec 2023 08:20:12 GMT  
		Size: 80.3 MB (80269153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:873759df9ef5bea1a9b39771cb9f95f002aab5fcac9279141c11bad88f032d9a`  
		Last Modified: Tue, 19 Dec 2023 08:20:00 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:7b765c330312fbd652f5811c86c4c6b3e88e2e2c24d7e16f83f4b1782bd8cb90
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.2 MB (129246108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23a72da26db114f62729359648ac0a655eb843e6245e8c01514293bbfcb75b91`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 21:16:36 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Tue, 21 Nov 2023 21:16:36 GMT
ARG VARNISH_VERSION=7.4.2
# Tue, 21 Nov 2023 21:16:37 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Tue, 21 Nov 2023 21:16:37 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 21 Nov 2023 21:16:37 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 21 Nov 2023 21:16:37 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Tue, 21 Nov 2023 21:16:37 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Tue, 21 Nov 2023 21:16:37 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Tue, 21 Nov 2023 21:16:37 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 21 Nov 2023 21:16:37 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 21 Nov 2023 21:16:37 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 21:19:02 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.2.tgz -o $tmpdir/orig.tgz;     echo "acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 21 Nov 2023 21:19:04 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 21:19:04 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 21 Nov 2023 21:19:04 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 21:19:04 GMT
USER varnish
# Tue, 21 Nov 2023 21:19:04 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 21:19:04 GMT
CMD []
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4c433f9fe1b4c04daf893df7f3dde2d25de13ed8474ae8887c623dbb3b0d5f`  
		Last Modified: Tue, 21 Nov 2023 21:23:39 GMT  
		Size: 100.1 MB (100066338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700ba44dbd53506d34d537e4614e9fb6a06b8a9aa2797b7e028061bc36b56044`  
		Last Modified: Tue, 21 Nov 2023 21:23:28 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; 386

```console
$ docker pull varnish@sha256:f7094353a24b15c6f1dc90d7efd0fd58cbeba2336184d3b5eedca4b98da770a4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131941018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e481519ab9391779d3c4321f01ff5a60343ba4a44a01e1184384da4fd9eacc19`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 04:39:53 GMT
ADD file:930e1b9d85b6927c4d3046f7c75de2f3bfc6ec29100c314d0ab2b780ea30e962 in / 
# Tue, 21 Nov 2023 04:39:53 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 15:11:13 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Tue, 21 Nov 2023 15:11:13 GMT
ARG VARNISH_VERSION=7.4.2
# Tue, 21 Nov 2023 15:11:13 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Tue, 21 Nov 2023 15:11:13 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 21 Nov 2023 15:11:13 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 21 Nov 2023 15:11:13 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Tue, 21 Nov 2023 15:11:13 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Tue, 21 Nov 2023 15:11:14 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Tue, 21 Nov 2023 15:11:14 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 21 Nov 2023 15:11:14 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 21 Nov 2023 15:11:14 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 15:14:49 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.2.tgz -o $tmpdir/orig.tgz;     echo "acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 21 Nov 2023 15:14:50 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 15:14:51 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 21 Nov 2023 15:14:51 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 15:14:51 GMT
USER varnish
# Tue, 21 Nov 2023 15:14:51 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 15:14:51 GMT
CMD []
```

-	Layers:
	-	`sha256:c0734eabce8885d8904dbd11b77aa97c2d2b04bc8e2af9e89d47c4bda590dd8e`  
		Last Modified: Tue, 21 Nov 2023 04:44:34 GMT  
		Size: 30.2 MB (30164109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebaa590b85c3666b3aa98d7f7f7d5e957400d175de18f1a103ee9fc72f3ff1e`  
		Last Modified: Tue, 21 Nov 2023 15:21:44 GMT  
		Size: 101.8 MB (101776416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb43c8e9e7fcf7c7d91ab556103770f53e487c54d5b6d3a5e6eae1531dabb03c`  
		Last Modified: Tue, 21 Nov 2023 15:21:22 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; ppc64le

```console
$ docker pull varnish@sha256:2393ba60ad3c5b5c3b8dc33eecd5388405e067b6c7b6aa6614d4c0e22d8cb740
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.7 MB (137679921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11d740886e444fe4a948031256adfe8d9d4148f985a3451ff9217f8b3b02084b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 12:50:24 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Tue, 21 Nov 2023 12:50:24 GMT
ARG VARNISH_VERSION=7.4.2
# Tue, 21 Nov 2023 12:50:24 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Tue, 21 Nov 2023 12:50:24 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 21 Nov 2023 12:50:25 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 21 Nov 2023 12:50:25 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Tue, 21 Nov 2023 12:50:25 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Tue, 21 Nov 2023 12:50:25 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Tue, 21 Nov 2023 12:50:25 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 21 Nov 2023 12:50:26 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 21 Nov 2023 12:50:26 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 12:54:18 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.2.tgz -o $tmpdir/orig.tgz;     echo "acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 21 Nov 2023 12:54:22 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 12:54:23 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 21 Nov 2023 12:54:23 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 12:54:23 GMT
USER varnish
# Tue, 21 Nov 2023 12:54:23 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 12:54:24 GMT
CMD []
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53276baea44ef2eb7632af8b3e497190197e059d4973c54c393e8e514579fee6`  
		Last Modified: Tue, 21 Nov 2023 13:01:56 GMT  
		Size: 104.5 MB (104537822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e228724f48a9283f83071d90b2ad5ea3adbd7aa8db408cf9cc17907d068aefd9`  
		Last Modified: Tue, 21 Nov 2023 13:01:38 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh` - linux; s390x

```console
$ docker pull varnish@sha256:6c7d0645cb3a69ac8d8f1550498bd4d8cdea53596dec94bcb46dd960a79f7032
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112324108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a720df683a8465e59eb06466380c0e7aa703e6e2adeafe901b372ac4a969610`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 01:42:37 GMT
ADD file:f06f12fa5a93afc3a79ac4371d24b0a471a5a1818cf34c1d90004c8f410914b9 in / 
# Tue, 19 Dec 2023 01:42:39 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 09:54:42 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Tue, 19 Dec 2023 09:54:43 GMT
ARG VARNISH_VERSION=7.4.2
# Tue, 19 Dec 2023 09:54:43 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Tue, 19 Dec 2023 09:54:43 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 19 Dec 2023 09:54:43 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 19 Dec 2023 09:54:43 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Tue, 19 Dec 2023 09:54:43 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Tue, 19 Dec 2023 09:54:43 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Tue, 19 Dec 2023 09:54:43 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 19 Dec 2023 09:54:43 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 19 Dec 2023 09:54:44 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 09:57:01 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.2.tgz -o $tmpdir/orig.tgz;     echo "acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 19 Dec 2023 09:57:06 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 09:57:06 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 19 Dec 2023 09:57:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 09:57:06 GMT
USER varnish
# Tue, 19 Dec 2023 09:57:07 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 09:57:07 GMT
CMD []
```

-	Layers:
	-	`sha256:bc6b1888979d3ceb063da848b2034e980e2c2613642159c1e856550b79aa620c`  
		Last Modified: Tue, 19 Dec 2023 01:47:38 GMT  
		Size: 27.5 MB (27491874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3940bd8b958075529145975f552f030ebc62a56083ae9e2ec9058a92ea0ab779`  
		Last Modified: Tue, 19 Dec 2023 10:02:14 GMT  
		Size: 84.8 MB (84831742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb1488658ec91ebf7b68fc1fb93f9c1b080f2aa4dd7407cfe14422af0a66a9f`  
		Last Modified: Tue, 19 Dec 2023 10:02:02 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:fresh-alpine`

```console
$ docker pull varnish@sha256:dccb7bbef9e81823cff443fb4a939c7b4f8c12e7ebd7e4ccf6f61d160a7f1697
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:fresh-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:b5eac55ba74a47af082bddac8f75de72ab56c24b23dff05b3bed748daa07e97f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73099369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c47739cdf917b26886e22b56f88ed349bd402588e139d368a79c43130e0edb81`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:20:49 GMT
ADD file:1f4eb46669b5b6275af19eb7471a6899a61c276aa7d925b8ae99310b14b75b92 in / 
# Fri, 08 Dec 2023 01:20:49 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 17:27:32 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Mon, 11 Dec 2023 17:27:32 GMT
ARG VARNISH_VERSION=7.4.2
# Mon, 11 Dec 2023 17:27:32 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Mon, 11 Dec 2023 17:27:32 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 17:27:32 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 17:27:32 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Mon, 11 Dec 2023 17:27:32 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Mon, 11 Dec 2023 17:27:32 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Mon, 11 Dec 2023 17:27:32 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 17:27:32 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 17:27:32 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 17:28:57 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 17:28:57 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 17:28:57 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 17:28:57 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 17:28:57 GMT
USER varnish
# Mon, 11 Dec 2023 17:28:57 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 17:28:57 GMT
CMD []
```

-	Layers:
	-	`sha256:661ff4d9561e3fd050929ee5097067c34bafc523ee60f5294a37fd08056a73ca`  
		Last Modified: Fri, 08 Dec 2023 01:21:10 GMT  
		Size: 3.4 MB (3408480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596ff0f1e45ff73a12d763f801097546e24d971a656c1e6c500464e3d9dc93d1`  
		Last Modified: Mon, 11 Dec 2023 17:30:59 GMT  
		Size: 69.7 MB (69690393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c9254892d8bb199804b7583c9d4976bb18fc6ffd3f835b13a09661f7f44eec`  
		Last Modified: Mon, 11 Dec 2023 17:30:50 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:87a53efcd35a17d5bfd0e5c7c785d5763c252ed86ec36857dac3fe45d93a33b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.3 MB (57297011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b2c19442982ba0e6c0be7f492a6ec1ada91fcc8a5ba1969f78b73a95d385b49`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:57:20 GMT
ADD file:13b9291053208eec61cd7c97bac2fa154380ad8d10182567763eea3e10c5882f in / 
# Fri, 08 Dec 2023 01:57:20 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 20:34:14 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Mon, 11 Dec 2023 20:34:14 GMT
ARG VARNISH_VERSION=7.4.2
# Mon, 11 Dec 2023 20:34:14 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Mon, 11 Dec 2023 20:34:14 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 20:34:14 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 20:34:15 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Mon, 11 Dec 2023 20:34:15 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Mon, 11 Dec 2023 20:34:15 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Mon, 11 Dec 2023 20:34:15 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 20:34:15 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 20:34:15 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 20:35:49 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 20:35:49 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 20:35:49 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 20:35:49 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 20:35:50 GMT
USER varnish
# Mon, 11 Dec 2023 20:35:50 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 20:35:50 GMT
CMD []
```

-	Layers:
	-	`sha256:1086c24c41097f090ce847d192c11307e1715eeb563a2cf4f410b2a199ae1942`  
		Last Modified: Fri, 08 Dec 2023 01:57:36 GMT  
		Size: 2.9 MB (2918701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c36cad4b93a74bd362b04d858cd9d78544bbb44bf895d4f6f5af8579139a2c7`  
		Last Modified: Mon, 11 Dec 2023 20:38:54 GMT  
		Size: 54.4 MB (54377812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a48e0aa1dee5bbd35355dac977a62f98ae8d12c24cf4ff2840627e55f9e3af`  
		Last Modified: Mon, 11 Dec 2023 20:38:48 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:c3a738cfcba71417cb1dbd6d79c584cf8ab596101cec9da60ae7550d322ff93a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69801066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd43f5c0e3e024f3ba7432e4d185a26e5527662f7ef11c692005bf9c34994822`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:39:30 GMT
ADD file:8182c73f869a899cf624a59c400acb8226776d15e4d3a0d240a94e65340540d0 in / 
# Fri, 08 Dec 2023 01:39:30 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:15:41 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Mon, 11 Dec 2023 19:15:41 GMT
ARG VARNISH_VERSION=7.4.2
# Mon, 11 Dec 2023 19:15:41 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Mon, 11 Dec 2023 19:15:41 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 19:15:41 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 19:15:41 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Mon, 11 Dec 2023 19:15:41 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Mon, 11 Dec 2023 19:15:41 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Mon, 11 Dec 2023 19:15:41 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 19:15:41 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 19:15:41 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 19:16:58 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 19:16:58 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 19:16:59 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 19:16:59 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 19:16:59 GMT
USER varnish
# Mon, 11 Dec 2023 19:16:59 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 19:16:59 GMT
CMD []
```

-	Layers:
	-	`sha256:c303524923177661067f7eb378c3dd5277088c2676ebd1cd78e68397bb80fdbf`  
		Last Modified: Fri, 08 Dec 2023 01:39:48 GMT  
		Size: 3.3 MB (3347794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62285e0f2c1fa910fd125cc6c60e04450bca85c9ae1dfc3e94e75962246bed4`  
		Last Modified: Mon, 11 Dec 2023 19:18:53 GMT  
		Size: 66.5 MB (66452773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88163622582d5ecfa15893cced49ef724d3bbcbc6a809c3eb87c3e8434a0ed8`  
		Last Modified: Mon, 11 Dec 2023 19:18:46 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; 386

```console
$ docker pull varnish@sha256:a79e39ac0276a1a34a258fbeeb02ac4b8b9e1c671b97f7a074fd2b6b4ae61023
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75122339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d691498e2889909c12cf91c9d555aed1a790d657a76cbc91c6b8d70a09ac4f25`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:38:25 GMT
ADD file:bd52540f209ba362654d795d7893669c819d35011a16f9f319301727a33b3bd9 in / 
# Fri, 08 Dec 2023 01:38:25 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 17:38:39 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Mon, 11 Dec 2023 17:38:39 GMT
ARG VARNISH_VERSION=7.4.2
# Mon, 11 Dec 2023 17:38:39 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Mon, 11 Dec 2023 17:38:39 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 17:38:39 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 17:38:40 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Mon, 11 Dec 2023 17:38:40 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Mon, 11 Dec 2023 17:38:40 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Mon, 11 Dec 2023 17:38:40 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 17:38:40 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 17:38:40 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 17:41:07 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 17:41:07 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 17:41:07 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 17:41:07 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 17:41:08 GMT
USER varnish
# Mon, 11 Dec 2023 17:41:08 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 17:41:08 GMT
CMD []
```

-	Layers:
	-	`sha256:9acd8b4c9d4385585f74dabb4bc6b3351888710ae37ec5dbd9ea950281b8f9bb`  
		Last Modified: Fri, 08 Dec 2023 01:38:43 GMT  
		Size: 3.2 MB (3244115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238a34d823f5a0cc31c7c355c956fd3e368a725f030f90a9e5d7df163792781d`  
		Last Modified: Mon, 11 Dec 2023 17:43:54 GMT  
		Size: 71.9 MB (71877729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57837da0913799765f0e9fd3302510c33ad5687b16eba780a53df338bc424d68`  
		Last Modified: Mon, 11 Dec 2023 17:43:40 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:b1b11ea19fa1b2687950414bb42591a92a3393f5395012ddc49e30e188233c95
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70614826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0564114572d93006a1a5cdd6ad53c188754e8c924236219640b9da35370cc7c3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:22:51 GMT
ADD file:052421189f8d269382daaaa8beb63c687e4d8ca908c421abdce53bcc627a40b4 in / 
# Fri, 08 Dec 2023 01:22:51 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 17:23:45 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Mon, 11 Dec 2023 17:23:45 GMT
ARG VARNISH_VERSION=7.4.2
# Mon, 11 Dec 2023 17:23:46 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Mon, 11 Dec 2023 17:23:46 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 17:23:46 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 17:23:47 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Mon, 11 Dec 2023 17:23:47 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Mon, 11 Dec 2023 17:23:47 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Mon, 11 Dec 2023 17:23:47 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 17:23:47 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 17:23:48 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 17:25:32 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 17:25:35 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 17:25:35 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 17:25:35 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 17:25:35 GMT
USER varnish
# Mon, 11 Dec 2023 17:25:36 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 17:25:36 GMT
CMD []
```

-	Layers:
	-	`sha256:243ac51c334a47917a84be93e972ee6378987e9b3b917a5a8df29025e161c1f3`  
		Last Modified: Fri, 08 Dec 2023 01:23:14 GMT  
		Size: 3.4 MB (3358233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3df8df9f5a4588e06e3e5398e16334f14812f2fdf045fd348b76a021da038d2`  
		Last Modified: Mon, 11 Dec 2023 17:27:46 GMT  
		Size: 67.3 MB (67256096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a44bfc4f6b4cc77283fb963e01fa094f85bf552a7514cb05c8c37783a83ff005`  
		Last Modified: Mon, 11 Dec 2023 17:27:35 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:fresh-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:2cea98b4853ec31e2735aca0c3e36d4f79721ea90b05a682e8a3a3701b334c9d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (64983529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dca28acdd122e49a4f4ebe4f0c061684c2798f776cc451771e4a27ea500fd75`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:41:50 GMT
ADD file:47e0982fc3ae485c06d46f3c0022afd39ed7ec95fe755c2391e6b0cfcae65dfc in / 
# Fri, 08 Dec 2023 01:41:51 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:52:03 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Mon, 11 Dec 2023 19:52:03 GMT
ARG VARNISH_VERSION=7.4.2
# Mon, 11 Dec 2023 19:52:04 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Mon, 11 Dec 2023 19:52:04 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 19:52:04 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 19:52:05 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Mon, 11 Dec 2023 19:52:05 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Mon, 11 Dec 2023 19:52:05 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Mon, 11 Dec 2023 19:52:06 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 19:52:06 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 19:52:06 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 19:53:37 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 19:53:40 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 19:53:40 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 19:53:41 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 19:53:41 GMT
USER varnish
# Mon, 11 Dec 2023 19:53:41 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 19:53:41 GMT
CMD []
```

-	Layers:
	-	`sha256:0fca3ee44ced87b7184bc23390283fdf10cfae0e844a25b785dd11c463815227`  
		Last Modified: Fri, 08 Dec 2023 01:42:30 GMT  
		Size: 3.2 MB (3242332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebca86ea5cb356f01dcce8ee2acb336ac6e346114eee85687c7bdbe3b09f508`  
		Last Modified: Mon, 11 Dec 2023 19:56:11 GMT  
		Size: 61.7 MB (61740701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15fe8e4d2daf80c7668faf912a02bf7be20425091121a2bd932d5025606840b`  
		Last Modified: Mon, 11 Dec 2023 19:56:02 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:latest`

```console
$ docker pull varnish@sha256:74f3de816160fb949b01111c302f4d37a49b45b1a754d1e145e8d3d7dc94cfb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:latest` - linux; amd64

```console
$ docker pull varnish@sha256:eadc1f8f442bb86961c300d37a64bb51b2658b8f6bed39c21fdd85405775c144
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.7 MB (134738894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e44717a97df19098a313b57e48e02fe1b413b2d92fe2eb3e6350c5f85ed591df`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 01:20:27 GMT
ADD file:ac3cd70031d35e46d86b876934946ffc8756de4de065fbc926dce642dac07ff3 in / 
# Tue, 19 Dec 2023 01:20:28 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 07:59:51 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Tue, 19 Dec 2023 07:59:51 GMT
ARG VARNISH_VERSION=7.4.2
# Tue, 19 Dec 2023 07:59:51 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Tue, 19 Dec 2023 07:59:51 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 19 Dec 2023 07:59:52 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 19 Dec 2023 07:59:52 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Tue, 19 Dec 2023 07:59:52 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Tue, 19 Dec 2023 07:59:52 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Tue, 19 Dec 2023 07:59:52 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 19 Dec 2023 07:59:52 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 19 Dec 2023 07:59:52 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 08:02:47 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.2.tgz -o $tmpdir/orig.tgz;     echo "acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 19 Dec 2023 08:02:48 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 08:02:48 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 19 Dec 2023 08:02:48 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 08:02:48 GMT
USER varnish
# Tue, 19 Dec 2023 08:02:48 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 08:02:49 GMT
CMD []
```

-	Layers:
	-	`sha256:af107e978371b6cd6339127a05502c5eacd1e6b0e9eb7b2f4aa7b6fc87e2dd81`  
		Last Modified: Tue, 19 Dec 2023 01:24:59 GMT  
		Size: 29.1 MB (29125963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b1c37f74eda351d5d18bd05ac7a597435e4dcc3dca90495bfb8704d7030f37`  
		Last Modified: Tue, 19 Dec 2023 08:08:18 GMT  
		Size: 105.6 MB (105612439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98889ac1ccb507f3093353ef6ddc3ca2dae1063b5323bb989732b0271c784f40`  
		Last Modified: Tue, 19 Dec 2023 08:08:03 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; arm variant v7

```console
$ docker pull varnish@sha256:0b0725305bd25fb5c7804c983f3a03f5c358908c150b56e6fc7754762d2fad7f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104987802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36b50ea5a138f4de8b6fb2c81a616b546478c36e122bd5e421db168ef5ad924c`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 02:07:50 GMT
ADD file:aef112919e7924ad6da32181b1df5099cd692680c104118da3a24cd4dfe55a1d in / 
# Tue, 19 Dec 2023 02:07:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:11:51 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Tue, 19 Dec 2023 08:11:51 GMT
ARG VARNISH_VERSION=7.4.2
# Tue, 19 Dec 2023 08:11:51 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Tue, 19 Dec 2023 08:11:51 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 19 Dec 2023 08:11:51 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 19 Dec 2023 08:11:51 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Tue, 19 Dec 2023 08:11:51 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Tue, 19 Dec 2023 08:11:52 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Tue, 19 Dec 2023 08:11:52 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 19 Dec 2023 08:11:52 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 19 Dec 2023 08:11:52 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 08:14:41 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.2.tgz -o $tmpdir/orig.tgz;     echo "acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 19 Dec 2023 08:14:42 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 08:14:42 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 19 Dec 2023 08:14:42 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 08:14:42 GMT
USER varnish
# Tue, 19 Dec 2023 08:14:42 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 08:14:43 GMT
CMD []
```

-	Layers:
	-	`sha256:65ab19615c01a3b542f77fadb3bd27872b6a20cba3e9269fb951de36d8fa6805`  
		Last Modified: Tue, 19 Dec 2023 02:11:52 GMT  
		Size: 24.7 MB (24718157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0329b82b2a3ad7a3589db33efac87f48ea52033e08b8fb622036d689eac669e`  
		Last Modified: Tue, 19 Dec 2023 08:20:12 GMT  
		Size: 80.3 MB (80269153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:873759df9ef5bea1a9b39771cb9f95f002aab5fcac9279141c11bad88f032d9a`  
		Last Modified: Tue, 19 Dec 2023 08:20:00 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:7b765c330312fbd652f5811c86c4c6b3e88e2e2c24d7e16f83f4b1782bd8cb90
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.2 MB (129246108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23a72da26db114f62729359648ac0a655eb843e6245e8c01514293bbfcb75b91`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 21:16:36 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Tue, 21 Nov 2023 21:16:36 GMT
ARG VARNISH_VERSION=7.4.2
# Tue, 21 Nov 2023 21:16:37 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Tue, 21 Nov 2023 21:16:37 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 21 Nov 2023 21:16:37 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 21 Nov 2023 21:16:37 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Tue, 21 Nov 2023 21:16:37 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Tue, 21 Nov 2023 21:16:37 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Tue, 21 Nov 2023 21:16:37 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 21 Nov 2023 21:16:37 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 21 Nov 2023 21:16:37 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 21:19:02 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.2.tgz -o $tmpdir/orig.tgz;     echo "acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 21 Nov 2023 21:19:04 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 21:19:04 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 21 Nov 2023 21:19:04 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 21:19:04 GMT
USER varnish
# Tue, 21 Nov 2023 21:19:04 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 21:19:04 GMT
CMD []
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4c433f9fe1b4c04daf893df7f3dde2d25de13ed8474ae8887c623dbb3b0d5f`  
		Last Modified: Tue, 21 Nov 2023 21:23:39 GMT  
		Size: 100.1 MB (100066338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700ba44dbd53506d34d537e4614e9fb6a06b8a9aa2797b7e028061bc36b56044`  
		Last Modified: Tue, 21 Nov 2023 21:23:28 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; 386

```console
$ docker pull varnish@sha256:f7094353a24b15c6f1dc90d7efd0fd58cbeba2336184d3b5eedca4b98da770a4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131941018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e481519ab9391779d3c4321f01ff5a60343ba4a44a01e1184384da4fd9eacc19`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 04:39:53 GMT
ADD file:930e1b9d85b6927c4d3046f7c75de2f3bfc6ec29100c314d0ab2b780ea30e962 in / 
# Tue, 21 Nov 2023 04:39:53 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 15:11:13 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Tue, 21 Nov 2023 15:11:13 GMT
ARG VARNISH_VERSION=7.4.2
# Tue, 21 Nov 2023 15:11:13 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Tue, 21 Nov 2023 15:11:13 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 21 Nov 2023 15:11:13 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 21 Nov 2023 15:11:13 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Tue, 21 Nov 2023 15:11:13 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Tue, 21 Nov 2023 15:11:14 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Tue, 21 Nov 2023 15:11:14 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 21 Nov 2023 15:11:14 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 21 Nov 2023 15:11:14 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 15:14:49 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.2.tgz -o $tmpdir/orig.tgz;     echo "acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 21 Nov 2023 15:14:50 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 15:14:51 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 21 Nov 2023 15:14:51 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 15:14:51 GMT
USER varnish
# Tue, 21 Nov 2023 15:14:51 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 15:14:51 GMT
CMD []
```

-	Layers:
	-	`sha256:c0734eabce8885d8904dbd11b77aa97c2d2b04bc8e2af9e89d47c4bda590dd8e`  
		Last Modified: Tue, 21 Nov 2023 04:44:34 GMT  
		Size: 30.2 MB (30164109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebaa590b85c3666b3aa98d7f7f7d5e957400d175de18f1a103ee9fc72f3ff1e`  
		Last Modified: Tue, 21 Nov 2023 15:21:44 GMT  
		Size: 101.8 MB (101776416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb43c8e9e7fcf7c7d91ab556103770f53e487c54d5b6d3a5e6eae1531dabb03c`  
		Last Modified: Tue, 21 Nov 2023 15:21:22 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; ppc64le

```console
$ docker pull varnish@sha256:2393ba60ad3c5b5c3b8dc33eecd5388405e067b6c7b6aa6614d4c0e22d8cb740
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.7 MB (137679921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11d740886e444fe4a948031256adfe8d9d4148f985a3451ff9217f8b3b02084b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 12:50:24 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Tue, 21 Nov 2023 12:50:24 GMT
ARG VARNISH_VERSION=7.4.2
# Tue, 21 Nov 2023 12:50:24 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Tue, 21 Nov 2023 12:50:24 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 21 Nov 2023 12:50:25 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 21 Nov 2023 12:50:25 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Tue, 21 Nov 2023 12:50:25 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Tue, 21 Nov 2023 12:50:25 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Tue, 21 Nov 2023 12:50:25 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 21 Nov 2023 12:50:26 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 21 Nov 2023 12:50:26 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 12:54:18 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.2.tgz -o $tmpdir/orig.tgz;     echo "acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 21 Nov 2023 12:54:22 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 12:54:23 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 21 Nov 2023 12:54:23 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 12:54:23 GMT
USER varnish
# Tue, 21 Nov 2023 12:54:23 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 12:54:24 GMT
CMD []
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53276baea44ef2eb7632af8b3e497190197e059d4973c54c393e8e514579fee6`  
		Last Modified: Tue, 21 Nov 2023 13:01:56 GMT  
		Size: 104.5 MB (104537822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e228724f48a9283f83071d90b2ad5ea3adbd7aa8db408cf9cc17907d068aefd9`  
		Last Modified: Tue, 21 Nov 2023 13:01:38 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:latest` - linux; s390x

```console
$ docker pull varnish@sha256:6c7d0645cb3a69ac8d8f1550498bd4d8cdea53596dec94bcb46dd960a79f7032
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112324108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a720df683a8465e59eb06466380c0e7aa703e6e2adeafe901b372ac4a969610`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 01:42:37 GMT
ADD file:f06f12fa5a93afc3a79ac4371d24b0a471a5a1818cf34c1d90004c8f410914b9 in / 
# Tue, 19 Dec 2023 01:42:39 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 09:54:42 GMT
ARG PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d
# Tue, 19 Dec 2023 09:54:43 GMT
ARG VARNISH_VERSION=7.4.2
# Tue, 19 Dec 2023 09:54:43 GMT
ARG DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971
# Tue, 19 Dec 2023 09:54:43 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 19 Dec 2023 09:54:43 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 19 Dec 2023 09:54:43 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0-1
# Tue, 19 Dec 2023 09:54:43 GMT
ARG VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9
# Tue, 19 Dec 2023 09:54:43 GMT
ARG VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1
# Tue, 19 Dec 2023 09:54:43 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 19 Dec 2023 09:54:43 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 19 Dec 2023 09:54:44 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 09:57:01 GMT
# ARGS: DIST_SHA512=acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971 PKG_COMMIT=cfa8cb3724e4ca6398f60b09157715bcb99d189d TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.4.2 VMOD_DYNAMIC_COMMIT=15e32fb8cf96752c90d895b0ca31451bd05d92d9 VMOD_DYNAMIC_SHA512SUM=d62d7af87770ef370c2e78e5b464f4f7712ebb50281728ca157ff38303f5455f1afdc0f8efaf0040febdf2d0aedbfa4c3369fe0f9d634ed34f185b54876cb4d1 VMOD_DYNAMIC_VERSION=2.8.0-1
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout cfa8cb3724e4ca6398f60b09157715bcb99d189d;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.4.2.tgz -o $tmpdir/orig.tgz;     echo "acd61a852ac7d66b268ab831d3a771d7a063a6a257b5e7c25c5a2ec9bccefa845279b9bd5fc85dd0b4f1d56da59164a13149355d1e6187e71ad76463687f7971  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 19 Dec 2023 09:57:06 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 09:57:06 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 19 Dec 2023 09:57:06 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 09:57:06 GMT
USER varnish
# Tue, 19 Dec 2023 09:57:07 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 09:57:07 GMT
CMD []
```

-	Layers:
	-	`sha256:bc6b1888979d3ceb063da848b2034e980e2c2613642159c1e856550b79aa620c`  
		Last Modified: Tue, 19 Dec 2023 01:47:38 GMT  
		Size: 27.5 MB (27491874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3940bd8b958075529145975f552f030ebc62a56083ae9e2ec9058a92ea0ab779`  
		Last Modified: Tue, 19 Dec 2023 10:02:14 GMT  
		Size: 84.8 MB (84831742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb1488658ec91ebf7b68fc1fb93f9c1b080f2aa4dd7407cfe14422af0a66a9f`  
		Last Modified: Tue, 19 Dec 2023 10:02:02 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:old`

```console
$ docker pull varnish@sha256:87dffb5c48c83cdcf12a3efeb6457d9e178f29604494e32b51701e1b2aa27cb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:old` - linux; amd64

```console
$ docker pull varnish@sha256:df9b1ecb6e4ca0e98f9dbdf680885e16c7e510e2de4ddabc59ae2982e8c8cf99
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101966885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac6fda6c72241a94c1e31ff26a39609231e0b895e083619d8286a89b39030028`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 01:20:50 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Tue, 19 Dec 2023 01:20:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:03:02 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 19 Dec 2023 08:03:02 GMT
ARG VARNISH_VERSION=7.3.1
# Tue, 19 Dec 2023 08:03:02 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Tue, 19 Dec 2023 08:03:03 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 19 Dec 2023 08:03:03 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 19 Dec 2023 08:03:03 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 19 Dec 2023 08:03:03 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 19 Dec 2023 08:03:03 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 19 Dec 2023 08:03:03 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 19 Dec 2023 08:03:03 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 19 Dec 2023 08:03:03 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 08:05:41 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.1.tgz -o $tmpdir/orig.tgz;     echo "57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 19 Dec 2023 08:05:42 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 08:05:42 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 19 Dec 2023 08:05:42 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 08:05:42 GMT
USER varnish
# Tue, 19 Dec 2023 08:05:42 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 08:05:42 GMT
CMD []
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e37b9699670384020e902a0ae2f3c71ef125515c77fb7f57f956fe2ab064bc8`  
		Last Modified: Tue, 19 Dec 2023 08:08:41 GMT  
		Size: 70.5 MB (70548520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbc9ee7e56bac88b0277ca7cd2409fa0ea1152bcdf965d290cd039497678c49`  
		Last Modified: Tue, 19 Dec 2023 08:08:32 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; arm variant v7

```console
$ docker pull varnish@sha256:ad549d82c4744321f31d836fa2757228ec9c6ee28a2fe56905d8606424ce55f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.8 MB (78751981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:580eedff14a9163d5717e74e0654d277448fd09bed4c6672badbf8cbbd32236f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 02:08:09 GMT
ADD file:496e70a34ff4dabb4eefdf40e4e2f0563bea0c120bb43206f8f52ab5a887b637 in / 
# Tue, 19 Dec 2023 02:08:09 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:15:00 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 19 Dec 2023 08:15:00 GMT
ARG VARNISH_VERSION=7.3.1
# Tue, 19 Dec 2023 08:15:00 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Tue, 19 Dec 2023 08:15:00 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 19 Dec 2023 08:15:01 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 19 Dec 2023 08:15:01 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 19 Dec 2023 08:15:01 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 19 Dec 2023 08:15:01 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 19 Dec 2023 08:15:01 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 19 Dec 2023 08:15:01 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 19 Dec 2023 08:15:01 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 08:17:37 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.1.tgz -o $tmpdir/orig.tgz;     echo "57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 19 Dec 2023 08:17:37 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 08:17:37 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 19 Dec 2023 08:17:38 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 08:17:38 GMT
USER varnish
# Tue, 19 Dec 2023 08:17:38 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 08:17:38 GMT
CMD []
```

-	Layers:
	-	`sha256:19ccf4d6cc6956e4a5522352be94632923aa376a9939a4f45428a4f304c73bc8`  
		Last Modified: Tue, 19 Dec 2023 02:12:33 GMT  
		Size: 26.6 MB (26578972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8d700fb01496fa8c844f9ebb7e2c0de1106588b482a0aef5209b031c470c89`  
		Last Modified: Tue, 19 Dec 2023 08:20:32 GMT  
		Size: 52.2 MB (52172516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa853700f1de2e0c582912f1a2175a3c69c30b2cd96cf0db35fb599a9d9bd9c7`  
		Last Modified: Tue, 19 Dec 2023 08:20:25 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:32014d110bbaffe0743bdc54c6c9d439532cf91ad71fbcdbdb7ae00779b18d62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.8 MB (95781809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66a11569b230dc214d07fcb99a041dcdfe426ea3ca30a6c31410230131217503`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 21:19:16 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 21 Nov 2023 21:19:16 GMT
ARG VARNISH_VERSION=7.3.1
# Tue, 21 Nov 2023 21:19:16 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Tue, 21 Nov 2023 21:19:16 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 21 Nov 2023 21:19:16 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 21 Nov 2023 21:19:16 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 21 Nov 2023 21:19:16 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 21 Nov 2023 21:19:16 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 21 Nov 2023 21:19:16 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 21 Nov 2023 21:19:16 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 21 Nov 2023 21:19:16 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 21:21:25 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.1.tgz -o $tmpdir/orig.tgz;     echo "57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 21 Nov 2023 21:21:26 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 21:21:26 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 21 Nov 2023 21:21:26 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 21:21:26 GMT
USER varnish
# Tue, 21 Nov 2023 21:21:26 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 21:21:26 GMT
CMD []
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc98e65c086f4b548a2e982f49352b25a0cd9922c2f9a98330b42163385f0d4`  
		Last Modified: Tue, 21 Nov 2023 21:23:59 GMT  
		Size: 65.7 MB (65717192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff1904762c1d07cd5329fe0e393c0598fdbac6a204808c4e326bd44f6f505eb`  
		Last Modified: Tue, 21 Nov 2023 21:23:52 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; 386

```console
$ docker pull varnish@sha256:522eb24b5d28a7295ce65f1086e33d5d85beaf7c9c65b3c60759498baeb3d4e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.2 MB (103212796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b70fc90e400e9dfbd466ceab45b7e7287a51be25ddbbc35bb9b1668978ffda0d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 04:40:15 GMT
ADD file:7de881b584405a880c4d02778056aaa81bb5dd5d1af65b3086d66aed9ff0ad4b in / 
# Tue, 21 Nov 2023 04:40:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 15:15:08 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 21 Nov 2023 15:15:08 GMT
ARG VARNISH_VERSION=7.3.1
# Tue, 21 Nov 2023 15:15:08 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Tue, 21 Nov 2023 15:15:08 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 21 Nov 2023 15:15:09 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 21 Nov 2023 15:15:09 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 21 Nov 2023 15:15:09 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 21 Nov 2023 15:15:09 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 21 Nov 2023 15:15:09 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 21 Nov 2023 15:15:09 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 21 Nov 2023 15:15:09 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 15:18:32 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.1.tgz -o $tmpdir/orig.tgz;     echo "57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 21 Nov 2023 15:18:33 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 15:18:33 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 21 Nov 2023 15:18:33 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 15:18:34 GMT
USER varnish
# Tue, 21 Nov 2023 15:18:34 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 15:18:34 GMT
CMD []
```

-	Layers:
	-	`sha256:75c11612678b54e79a38118fe66e532c61b3d0798afb741007b4cd3209c0ec4e`  
		Last Modified: Tue, 21 Nov 2023 04:45:24 GMT  
		Size: 32.4 MB (32402632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae3bc414da66bdd2d32a046a233e988a45ad7faaa11b96e0f5e55973fa16073`  
		Last Modified: Tue, 21 Nov 2023 15:22:12 GMT  
		Size: 70.8 MB (70809672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d549858933a493ec89c83cb3fafe3fec83022f9eae66525cdcbdf30fc7e49c92`  
		Last Modified: Tue, 21 Nov 2023 15:21:58 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; ppc64le

```console
$ docker pull varnish@sha256:66a0133569e260a895c68333c0426c77cdaa6c2f4dcb29b8f24906c16932c150
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.9 MB (100887371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc4919272c647cb21a3aee48eb9f1a2e0a70f042c7da2e16ef2463f7cf62433b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 04:24:43 GMT
ADD file:b0d18f2d04821eb50d1faecc1a64916f5c63dd386ae71a3b2cb1d6c4aac6e1c4 in / 
# Tue, 21 Nov 2023 04:24:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 12:54:35 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 21 Nov 2023 12:54:35 GMT
ARG VARNISH_VERSION=7.3.1
# Tue, 21 Nov 2023 12:54:36 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Tue, 21 Nov 2023 12:54:36 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 21 Nov 2023 12:54:36 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 21 Nov 2023 12:54:37 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 21 Nov 2023 12:54:37 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 21 Nov 2023 12:54:37 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 21 Nov 2023 12:54:37 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 21 Nov 2023 12:54:38 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 21 Nov 2023 12:54:38 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 12:58:17 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.1.tgz -o $tmpdir/orig.tgz;     echo "57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 21 Nov 2023 12:58:19 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 12:58:19 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 21 Nov 2023 12:58:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 12:58:20 GMT
USER varnish
# Tue, 21 Nov 2023 12:58:20 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 12:58:20 GMT
CMD []
```

-	Layers:
	-	`sha256:60239a74847cd7e9a928353188f3cf096ca8cf648e2b27c765058e169d568fd9`  
		Last Modified: Tue, 21 Nov 2023 04:29:47 GMT  
		Size: 35.3 MB (35293727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef474112e53d3cd9414bbc58b355c42c87c37b9296900ac553800b9812b43a51`  
		Last Modified: Tue, 21 Nov 2023 13:02:23 GMT  
		Size: 65.6 MB (65593153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72377d237fe1a86489eea9d2d9f72ba19b74303b09593612e4f440d909932fc`  
		Last Modified: Tue, 21 Nov 2023 13:02:12 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old` - linux; s390x

```console
$ docker pull varnish@sha256:0ab6caa4ba596675fb6506e80cd6416e352dc89123bce57cd6a750c5e9162e99
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.3 MB (82337376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77957464272e0f2a1870b20c4bd51bf9af77a796e6053701d2cc4d533ee2cc88`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 01:43:11 GMT
ADD file:36a070457acddafcd6cdda22a3c41efcbd4e2b1694831eb74c8143520ebf1cf2 in / 
# Tue, 19 Dec 2023 01:43:14 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 09:57:28 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Tue, 19 Dec 2023 09:57:28 GMT
ARG VARNISH_VERSION=7.3.1
# Tue, 19 Dec 2023 09:57:28 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Tue, 19 Dec 2023 09:57:29 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Tue, 19 Dec 2023 09:57:29 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Tue, 19 Dec 2023 09:57:30 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Tue, 19 Dec 2023 09:57:30 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Tue, 19 Dec 2023 09:57:30 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Tue, 19 Dec 2023 09:57:31 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Tue, 19 Dec 2023 09:57:31 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkg-config python3-sphinx
# Tue, 19 Dec 2023 09:57:31 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 09:59:40 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot libgetdns-dev";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     mkdir -p /work/varnish /pkgs;     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS libgetdns10;         adduser --uid 1000 --quiet --system --no-create-home --home /nonexistent --group varnish;     adduser --uid 1001 --quiet --system --no-create-home --home /nonexistent --ingroup varnish vcache;     adduser --uid 1002 --quiet --system --no-create-home --home /nonexistent --ingroup varnish varnishlog;         cd /work/varnish;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 712667312304cbb1798f131caa0a98b7697a2cd9;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-7.3.1.tgz -o $tmpdir/orig.tgz;     echo "57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|$VARNISH_VERSION|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     mv ../*dev*.deb /pkgs;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     rm -rf /var/lib/apt/lists/* /work/ /usr/lib/varnish/vmods/libvmod_*.la;     chown varnish /var/lib/varnish;
# Tue, 19 Dec 2023 09:59:43 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 09:59:43 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Tue, 19 Dec 2023 09:59:43 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 09:59:44 GMT
USER varnish
# Tue, 19 Dec 2023 09:59:44 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 09:59:44 GMT
CMD []
```

-	Layers:
	-	`sha256:eff2a4367cf88d5103011eba9299da2b4d173b0bde5dc0455020febf72b9b1c4`  
		Last Modified: Tue, 19 Dec 2023 01:48:08 GMT  
		Size: 29.7 MB (29657006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973b42ff7f83f76b123f93bf3b16fc127a7cc9fe1475d16b393a84485a77e625`  
		Last Modified: Tue, 19 Dec 2023 10:02:30 GMT  
		Size: 52.7 MB (52679878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e8e963aca39b2ea7900e6590a2e12624c36457b736760d4d9eb8d5289d9da7`  
		Last Modified: Tue, 19 Dec 2023 10:02:23 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:old-alpine`

```console
$ docker pull varnish@sha256:7aacc92711bb4c55276bcd32206e3a3f872f0a45b9f4a620843f81c5d676ac57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:old-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:a660b85166043d82783fefc5da6e563dd3baddbd57f85142037f982e902bfe0f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (72971654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22258995a868639c834b5ee85a5c1679cc4ff4a424d12549e212ce22893c3d49`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:20:49 GMT
ADD file:1f4eb46669b5b6275af19eb7471a6899a61c276aa7d925b8ae99310b14b75b92 in / 
# Fri, 08 Dec 2023 01:20:49 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 17:29:13 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Mon, 11 Dec 2023 17:29:13 GMT
ARG VARNISH_VERSION=7.3.1
# Mon, 11 Dec 2023 17:29:13 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Mon, 11 Dec 2023 17:29:13 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 17:29:13 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 17:29:13 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Mon, 11 Dec 2023 17:29:13 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Mon, 11 Dec 2023 17:29:13 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Mon, 11 Dec 2023 17:29:13 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 17:29:13 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 17:29:14 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 17:30:32 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 17:30:32 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 17:30:32 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 17:30:32 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 17:30:32 GMT
USER varnish
# Mon, 11 Dec 2023 17:30:32 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 17:30:32 GMT
CMD []
```

-	Layers:
	-	`sha256:661ff4d9561e3fd050929ee5097067c34bafc523ee60f5294a37fd08056a73ca`  
		Last Modified: Fri, 08 Dec 2023 01:21:10 GMT  
		Size: 3.4 MB (3408480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df54af4bcc97a93a4bd34d0e0a186b4643293a0b4e9b118bb5fd66e7ff3a678`  
		Last Modified: Mon, 11 Dec 2023 17:31:23 GMT  
		Size: 69.6 MB (69562679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1c4c6bbeee3080ea2c25f71ad2659e1800e05df9cb4040bb500ea920d75038`  
		Last Modified: Mon, 11 Dec 2023 17:31:13 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:6263e0f2a246117ad4a109b963cd07c7d0d046bcc7cd22e2433a380f326e152a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.2 MB (57173570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21da2e0d838632cb4b57d2a16f3f84df85831022148ef32ee8b33b64913dc17f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:57:20 GMT
ADD file:13b9291053208eec61cd7c97bac2fa154380ad8d10182567763eea3e10c5882f in / 
# Fri, 08 Dec 2023 01:57:20 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 20:35:53 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Mon, 11 Dec 2023 20:35:53 GMT
ARG VARNISH_VERSION=7.3.1
# Mon, 11 Dec 2023 20:35:54 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Mon, 11 Dec 2023 20:35:54 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 20:35:54 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 20:35:54 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Mon, 11 Dec 2023 20:35:54 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Mon, 11 Dec 2023 20:35:54 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Mon, 11 Dec 2023 20:35:54 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 20:35:54 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 20:35:54 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 20:37:10 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 20:37:10 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 20:37:10 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 20:37:10 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 20:37:10 GMT
USER varnish
# Mon, 11 Dec 2023 20:37:10 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 20:37:11 GMT
CMD []
```

-	Layers:
	-	`sha256:1086c24c41097f090ce847d192c11307e1715eeb563a2cf4f410b2a199ae1942`  
		Last Modified: Fri, 08 Dec 2023 01:57:36 GMT  
		Size: 2.9 MB (2918701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c23e83961531cd3bf4404f796467444964e4ad11f8a736b70489b794a148810`  
		Last Modified: Mon, 11 Dec 2023 20:39:58 GMT  
		Size: 54.3 MB (54254374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52917b5a405d3bd4ee7ca2f070f6435b1099aee4e248f9c2e1c6ee9662be3001`  
		Last Modified: Mon, 11 Dec 2023 20:39:52 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:212fc3b9e2ae991b2d5398dbb64a8bd7fa6f89ce994f70c6705b127da860b723
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69670674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d26d4bdefa37aa5cbbabe0839fc9ee9ed1e23ce42b5bdbaa8a0619a63147e42a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:39:30 GMT
ADD file:8182c73f869a899cf624a59c400acb8226776d15e4d3a0d240a94e65340540d0 in / 
# Fri, 08 Dec 2023 01:39:30 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:17:05 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Mon, 11 Dec 2023 19:17:05 GMT
ARG VARNISH_VERSION=7.3.1
# Mon, 11 Dec 2023 19:17:06 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Mon, 11 Dec 2023 19:17:06 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 19:17:06 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 19:17:06 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Mon, 11 Dec 2023 19:17:06 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Mon, 11 Dec 2023 19:17:06 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Mon, 11 Dec 2023 19:17:06 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 19:17:06 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 19:17:06 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 19:18:16 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 19:18:17 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 19:18:17 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 19:18:17 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 19:18:17 GMT
USER varnish
# Mon, 11 Dec 2023 19:18:17 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 19:18:17 GMT
CMD []
```

-	Layers:
	-	`sha256:c303524923177661067f7eb378c3dd5277088c2676ebd1cd78e68397bb80fdbf`  
		Last Modified: Fri, 08 Dec 2023 01:39:48 GMT  
		Size: 3.3 MB (3347794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f90173f8b57807827483acedf8c853c481199ecb51a4797e033af8de7fa8a4`  
		Last Modified: Mon, 11 Dec 2023 19:19:12 GMT  
		Size: 66.3 MB (66322385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430ac4e33922777503f5d5f1ac2d2b199f4e9ca70758e3e94f23a9dd4d755c39`  
		Last Modified: Mon, 11 Dec 2023 19:19:06 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; 386

```console
$ docker pull varnish@sha256:144593b4ae2f9889676979af92e6655686ec14070d3715973aaae1d2c004ad1b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (75000229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13ad0500a3c76c97cd544861eb007b787ea85320e31e8c2a3a4e74d818d5a47e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:38:25 GMT
ADD file:bd52540f209ba362654d795d7893669c819d35011a16f9f319301727a33b3bd9 in / 
# Fri, 08 Dec 2023 01:38:25 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 17:41:19 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Mon, 11 Dec 2023 17:41:19 GMT
ARG VARNISH_VERSION=7.3.1
# Mon, 11 Dec 2023 17:41:19 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Mon, 11 Dec 2023 17:41:19 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 17:41:19 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 17:41:19 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Mon, 11 Dec 2023 17:41:19 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Mon, 11 Dec 2023 17:41:20 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Mon, 11 Dec 2023 17:41:20 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 17:41:20 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 17:41:20 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 17:43:20 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 17:43:20 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 17:43:20 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 17:43:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 17:43:20 GMT
USER varnish
# Mon, 11 Dec 2023 17:43:21 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 17:43:21 GMT
CMD []
```

-	Layers:
	-	`sha256:9acd8b4c9d4385585f74dabb4bc6b3351888710ae37ec5dbd9ea950281b8f9bb`  
		Last Modified: Fri, 08 Dec 2023 01:38:43 GMT  
		Size: 3.2 MB (3244115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ef2537002ecb2bb3abded65d6356f3692fda99b626ea47de362a0110b0b5b5`  
		Last Modified: Mon, 11 Dec 2023 17:44:21 GMT  
		Size: 71.8 MB (71755614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e61ec8d102709660006ff1fcde698d488782452a4493a0eae31ed253ef2bce7`  
		Last Modified: Mon, 11 Dec 2023 17:44:07 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:a76ce382abf1217b12fa2bf3e1e795b0431efa83fdcbeeb8f7fd50124327baf4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.5 MB (70485288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cb51e4e5c8495d2d3a90e2274b3a1ba12e2541fc87085ca17e4f0092b93702b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:22:51 GMT
ADD file:052421189f8d269382daaaa8beb63c687e4d8ca908c421abdce53bcc627a40b4 in / 
# Fri, 08 Dec 2023 01:22:51 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 17:25:41 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Mon, 11 Dec 2023 17:25:43 GMT
ARG VARNISH_VERSION=7.3.1
# Mon, 11 Dec 2023 17:25:43 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Mon, 11 Dec 2023 17:25:44 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 17:25:44 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 17:25:44 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Mon, 11 Dec 2023 17:25:45 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Mon, 11 Dec 2023 17:25:45 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Mon, 11 Dec 2023 17:25:45 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 17:25:45 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 17:25:46 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 17:27:08 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 17:27:11 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 17:27:11 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 17:27:12 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 17:27:13 GMT
USER varnish
# Mon, 11 Dec 2023 17:27:13 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 17:27:13 GMT
CMD []
```

-	Layers:
	-	`sha256:243ac51c334a47917a84be93e972ee6378987e9b3b917a5a8df29025e161c1f3`  
		Last Modified: Fri, 08 Dec 2023 01:23:14 GMT  
		Size: 3.4 MB (3358233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42894c6396857cddc9334f3f02e9b3a4fe9e83a14200487428ee54247e804ade`  
		Last Modified: Mon, 11 Dec 2023 17:28:11 GMT  
		Size: 67.1 MB (67126559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86af6ac0c31af7d9ef2235797afd83c075764dac4f8b2af2ea00d996fd202644`  
		Last Modified: Mon, 11 Dec 2023 17:28:00 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:12ceacf7e0b60a469d0bb4588a8fce08904d2076e215786778a3db5b8625db26
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64858338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2b460b5437dfface2a98ed7a3c28597b4530d8a6e501b486153d9958d1c58e7`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 08 Dec 2023 01:41:50 GMT
ADD file:47e0982fc3ae485c06d46f3c0022afd39ed7ec95fe755c2391e6b0cfcae65dfc in / 
# Fri, 08 Dec 2023 01:41:51 GMT
CMD ["/bin/sh"]
# Mon, 11 Dec 2023 19:54:01 GMT
ARG PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9
# Mon, 11 Dec 2023 19:54:01 GMT
ARG VARNISH_VERSION=7.3.1
# Mon, 11 Dec 2023 19:54:01 GMT
ARG DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d
# Mon, 11 Dec 2023 19:54:01 GMT
ARG VARNISH_MODULES_VERSION=0.22.0
# Mon, 11 Dec 2023 19:54:01 GMT
ARG VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a
# Mon, 11 Dec 2023 19:54:02 GMT
ARG VMOD_DYNAMIC_VERSION=2.8.0
# Mon, 11 Dec 2023 19:54:02 GMT
ARG VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0
# Mon, 11 Dec 2023 19:54:02 GMT
ARG VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de
# Mon, 11 Dec 2023 19:54:02 GMT
ARG TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55
# Mon, 11 Dec 2023 19:54:02 GMT
ENV VMOD_DEPS=autoconf-archive automake curl libtool make pkgconfig py3-sphinx
# Mon, 11 Dec 2023 19:54:02 GMT
ENV VARNISH_SIZE=100M
# Mon, 11 Dec 2023 19:55:21 GMT
# ARGS: DIST_SHA512=57de14ff47038752a151b704d7f629438bba74e258e7d88c6ca58e8a10bfc89368f36b7f32d5525ff032033d941f3e48dde5ae090e44ca928110d2eeb1db589d PKG_COMMIT=712667312304cbb1798f131caa0a98b7697a2cd9 TOOLBOX_COMMIT=01ff3ec18a955f93880afe18167f17d0bc36cd55 VARNISH_MODULES_SHA512SUM=597ac1161224a25c11183fbaaf25412c8f8e0af3bf58fa76161328d8ae97aa7c485cfa6ed50e9f24ce73eca9ddeeb87ee4998427382c0fce633bf43eaf08068a VARNISH_MODULES_VERSION=0.22.0 VARNISH_VERSION=7.3.1 VMOD_DYNAMIC_COMMIT=af9c51cb53982b42eed6116960015c09171838b0 VMOD_DYNAMIC_SHA512SUM=4a91de4a1fc3e6eb925ac5e8c9d56d9786c368fbbb3b957285bd0edf4e955ee19ad1ee6b4b3c4754cf5885be6593c269419c19fea36760513397d92085e105de VMOD_DYNAMIC_VERSION=2.8.0
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo py3-docutils python3 autoconf automake libtool";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;         addgroup -g 1000 -S varnish;     adduser -u 1000 -S -D -H -s /sbin/nologin -G varnish -g varnish varnish;     adduser -u 1001 -S -D -H -s /sbin/nologin -G varnish -g varnish vcache;     adduser -u 1002 -S -D -H -s /sbin/nologin -G varnish -g varnish varnishlog;         adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers.d/builder;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";         git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout $PKG_COMMIT;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=$VARNISH_VERSION/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"$DIST_SHA512  varnish-\$pkgver.tgz\"/";         chown builder -R .;     su builder -c "abuild -r";     apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;         git clone https://github.com/varnish/toolbox.git;     cd toolbox;     git checkout $TOOLBOX_COMMIT;     cp install-vmod/install-vmod /usr/local/bin/;         install-vmod https://github.com/varnish/varnish-modules/releases/download/$VARNISH_MODULES_VERSION/varnish-modules-$VARNISH_MODULES_VERSION.tar.gz $VARNISH_MODULES_SHA512SUM;         install-vmod https://github.com/nigoroll/libvmod-dynamic/archive/$VMOD_DYNAMIC_COMMIT.tar.gz $VMOD_DYNAMIC_SHA512SUM;         apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache /varnish-modules /vmod-dynamic /etc/sudoers.d/builder;     deluser --remove-home builder;     chown varnish /var/lib/varnish;
# Mon, 11 Dec 2023 19:55:25 GMT
WORKDIR /etc/varnish
# Mon, 11 Dec 2023 19:55:25 GMT
COPY dir:6dcb75fa0bc26d4afaf5dc722b0827803ad6d52fba8af98ee9fcd0dd74a868f3 in /usr/local/bin/ 
# Mon, 11 Dec 2023 19:55:25 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Mon, 11 Dec 2023 19:55:25 GMT
USER varnish
# Mon, 11 Dec 2023 19:55:25 GMT
EXPOSE 80 8443
# Mon, 11 Dec 2023 19:55:25 GMT
CMD []
```

-	Layers:
	-	`sha256:0fca3ee44ced87b7184bc23390283fdf10cfae0e844a25b785dd11c463815227`  
		Last Modified: Fri, 08 Dec 2023 01:42:30 GMT  
		Size: 3.2 MB (3242332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de618724c4df65b558efa8979cd6a8db37714a1bc88b90d86d2c7ae78629b3fd`  
		Last Modified: Mon, 11 Dec 2023 19:56:31 GMT  
		Size: 61.6 MB (61615510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57580a9d987d8a4e6b62eaa72d36e8665a06835e8fb63ee71d17edfd3c531a0a`  
		Last Modified: Mon, 11 Dec 2023 19:56:24 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `varnish:stable`

```console
$ docker pull varnish@sha256:83a590c5be4d9e7bd66b7b90c78b786914a52661680ac88a7416cef15249d16b
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
$ docker pull varnish@sha256:b87136ceca6dbbb6c043856b46dc6f2868b19f8b590d6854b390c7299efc3943
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.9 MB (95851971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53f22488e835db5b05edaddd6831ee21b3d5abcc6c5ab96b5011ac4cb93a97ca`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 01:20:50 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Tue, 19 Dec 2023 01:20:50 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:05:59 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 08:07:40 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.12.tgz -o $tmpdir/orig.tgz;     echo "d80abb42380e85bc4be02278b3620b0a66d182465945146eecb2cdc022e77945ad815e897a5ed0bec2f458471617f647a80c743c0f72e73334ad92d3ac298af4  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.12|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 19 Dec 2023 08:07:40 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 08:07:40 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 19 Dec 2023 08:07:40 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 08:07:41 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 08:07:41 GMT
CMD []
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6eccc4b0a9abfc48ce57a783112f8f97d60f34816565535ed611d487b742d2`  
		Last Modified: Tue, 19 Dec 2023 08:09:01 GMT  
		Size: 64.4 MB (64433396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b919dc92685b5d4f6647a892025e8bdc664e1ab313fd22b26aadbe53f5f136bd`  
		Last Modified: Tue, 19 Dec 2023 08:08:53 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; arm variant v7

```console
$ docker pull varnish@sha256:b7a60981b3fc7fc22a6a065e5ea164928e3fc454e2acfc4ad830a29b4ce1d41e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72850985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5d33c2240e6f7289ba573e1d41811d6662ad39a5710f8973cea25ca2281559d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 02:08:09 GMT
ADD file:496e70a34ff4dabb4eefdf40e4e2f0563bea0c120bb43206f8f52ab5a887b637 in / 
# Tue, 19 Dec 2023 02:08:09 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 08:17:55 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 08:19:39 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.12.tgz -o $tmpdir/orig.tgz;     echo "d80abb42380e85bc4be02278b3620b0a66d182465945146eecb2cdc022e77945ad815e897a5ed0bec2f458471617f647a80c743c0f72e73334ad92d3ac298af4  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.12|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 19 Dec 2023 08:19:39 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 08:19:40 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 19 Dec 2023 08:19:40 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 08:19:40 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 08:19:40 GMT
CMD []
```

-	Layers:
	-	`sha256:19ccf4d6cc6956e4a5522352be94632923aa376a9939a4f45428a4f304c73bc8`  
		Last Modified: Tue, 19 Dec 2023 02:12:33 GMT  
		Size: 26.6 MB (26578972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105ed2a8f3cdbfeed8a77fff5c85b3bbfeeaf6ed56a514bafbca125b3e19b0e6`  
		Last Modified: Tue, 19 Dec 2023 08:20:49 GMT  
		Size: 46.3 MB (46271310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ddfe0f63afa45573e2077350d693f7508d0a5ac6e440990c4b23983848cfb6`  
		Last Modified: Tue, 19 Dec 2023 08:20:43 GMT  
		Size: 703.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:c66151b20502d18818ba7c51903d1a8742b3c23c1d148d8a6de6eb7d44fad343
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.9 MB (89947531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:642c464bc8bb3d14e8fafb63d1c048b2dc6c018d73d75cceb57fdf7a6cfeae8e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 21:21:40 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 21:23:04 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.12.tgz -o $tmpdir/orig.tgz;     echo "d80abb42380e85bc4be02278b3620b0a66d182465945146eecb2cdc022e77945ad815e897a5ed0bec2f458471617f647a80c743c0f72e73334ad92d3ac298af4  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.12|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 21 Nov 2023 21:23:04 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 21:23:04 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 21 Nov 2023 21:23:04 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 21:23:05 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 21:23:05 GMT
CMD []
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c54fe601a038c4d89325227f48596a94a4e44b39870a11399952782daa5f3c`  
		Last Modified: Tue, 21 Nov 2023 21:24:17 GMT  
		Size: 59.9 MB (59882708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f896890a1244055bc5bb66ea669ea2e0d1f6f6c82dcd1de073b3ef0885dc810f`  
		Last Modified: Tue, 21 Nov 2023 21:24:10 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; 386

```console
$ docker pull varnish@sha256:b842943e7429125c62902f678680031c957134e780aa6a48987613a05c2cbaa4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.1 MB (97117939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f96d47bae6ce87e0790321c40cc2ab5911bae135d4660b8588780fb7702b9ef4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 04:40:15 GMT
ADD file:7de881b584405a880c4d02778056aaa81bb5dd5d1af65b3086d66aed9ff0ad4b in / 
# Tue, 21 Nov 2023 04:40:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 15:18:48 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 15:20:59 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.12.tgz -o $tmpdir/orig.tgz;     echo "d80abb42380e85bc4be02278b3620b0a66d182465945146eecb2cdc022e77945ad815e897a5ed0bec2f458471617f647a80c743c0f72e73334ad92d3ac298af4  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.12|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 21 Nov 2023 15:21:00 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 15:21:00 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 21 Nov 2023 15:21:00 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 15:21:01 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 15:21:01 GMT
CMD []
```

-	Layers:
	-	`sha256:75c11612678b54e79a38118fe66e532c61b3d0798afb741007b4cd3209c0ec4e`  
		Last Modified: Tue, 21 Nov 2023 04:45:24 GMT  
		Size: 32.4 MB (32402632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92ff281c7632f3cc43de9266bd270b60c9947c71d8ecd4447a642432aa474a2`  
		Last Modified: Tue, 21 Nov 2023 15:22:37 GMT  
		Size: 64.7 MB (64714607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42e11325b795fce4ed6da4516d07a680b0fed89bf469efa769f3bdd733bdd505`  
		Last Modified: Tue, 21 Nov 2023 15:22:24 GMT  
		Size: 700.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; ppc64le

```console
$ docker pull varnish@sha256:eae28db647a78e9c81e7a12d56a54ddb38acc4196be62bd474fc6065f09c5260
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.6 MB (94635754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbb31ef67ecd67eeae948cbf7035f3a62f9b306540d58cfdfb8cf6e6544f6a5e`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 21 Nov 2023 04:24:43 GMT
ADD file:b0d18f2d04821eb50d1faecc1a64916f5c63dd386ae71a3b2cb1d6c4aac6e1c4 in / 
# Tue, 21 Nov 2023 04:24:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 12:58:32 GMT
ENV VARNISH_SIZE=100M
# Tue, 21 Nov 2023 13:01:18 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.12.tgz -o $tmpdir/orig.tgz;     echo "d80abb42380e85bc4be02278b3620b0a66d182465945146eecb2cdc022e77945ad815e897a5ed0bec2f458471617f647a80c743c0f72e73334ad92d3ac298af4  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.12|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 21 Nov 2023 13:01:21 GMT
WORKDIR /etc/varnish
# Tue, 21 Nov 2023 13:01:21 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 21 Nov 2023 13:01:21 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 21 Nov 2023 13:01:21 GMT
EXPOSE 80 8443
# Tue, 21 Nov 2023 13:01:21 GMT
CMD []
```

-	Layers:
	-	`sha256:60239a74847cd7e9a928353188f3cf096ca8cf648e2b27c765058e169d568fd9`  
		Last Modified: Tue, 21 Nov 2023 04:29:47 GMT  
		Size: 35.3 MB (35293727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569c6d4e2d1dbb35d3b9ee83520833f8382e7eb87b7e6962c8d2e4c0be7806dd`  
		Last Modified: Tue, 21 Nov 2023 13:02:46 GMT  
		Size: 59.3 MB (59341325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448e034f0cac91c1eefcc5bec2f728aa50eb54a22d0abb010d4f5a8e3ad28047`  
		Last Modified: Tue, 21 Nov 2023 13:02:36 GMT  
		Size: 702.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:stable` - linux; s390x

```console
$ docker pull varnish@sha256:1afbcc817848afe7c42f083bf59bb6924839dbe7876bbd67969a4fe4138e0293
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76249533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e26b3d40fd7d0d13dd16d991a8913dbae2a3e5c7c1607b401be603ecacc8845`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Tue, 19 Dec 2023 01:43:11 GMT
ADD file:36a070457acddafcd6cdda22a3c41efcbd4e2b1694831eb74c8143520ebf1cf2 in / 
# Tue, 19 Dec 2023 01:43:14 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 10:00:12 GMT
ENV VARNISH_SIZE=100M
# Tue, 19 Dec 2023 10:01:34 GMT
RUN set -e;     BASE_PKGS="curl dpkg-dev debhelper devscripts equivs git pkg-config apt-utils fakeroot";     export DEBIAN_FRONTEND=noninteractive;     export DEBCONF_NONINTERACTIVE_SEEN=true;     tmpdir="$(mktemp -d)";     cd "$tmpdir";     apt-get update;     apt-get install -y --no-install-recommends $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache;     git checkout 10da6a585eb7d8defe9d273a51df5b133500eb6b;     rm -rf .git;     curl -f https://varnish-cache.org/downloads/varnish-6.0.12.tgz -o $tmpdir/orig.tgz;     echo "d80abb42380e85bc4be02278b3620b0a66d182465945146eecb2cdc022e77945ad815e897a5ed0bec2f458471617f647a80c743c0f72e73334ad92d3ac298af4  $tmpdir/orig.tgz" | sha512sum -c -;     tar xavf $tmpdir/orig.tgz --strip 1;     sed -i -e "s|@VERSION@|6.0.12|"  "debian/changelog";     mk-build-deps --install --tool="apt-get -o Debug::pkgProblemResolver=yes --yes" debian/control;     sed -i '' debian/varnish*;     dpkg-buildpackage -us -uc -j"$(nproc)";     apt-get -y --no-install-recommends install ../*.deb;     apt-get -y purge --auto-remove varnish-build-deps $BASE_PKGS;     mkdir /pkgs;     mv ../*dev*.deb /pkgs;     rm -rf /var/lib/apt/lists/* "$tmpdir";
# Tue, 19 Dec 2023 10:01:37 GMT
WORKDIR /etc/varnish
# Tue, 19 Dec 2023 10:01:37 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Tue, 19 Dec 2023 10:01:37 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Tue, 19 Dec 2023 10:01:37 GMT
EXPOSE 80 8443
# Tue, 19 Dec 2023 10:01:37 GMT
CMD []
```

-	Layers:
	-	`sha256:eff2a4367cf88d5103011eba9299da2b4d173b0bde5dc0455020febf72b9b1c4`  
		Last Modified: Tue, 19 Dec 2023 01:48:08 GMT  
		Size: 29.7 MB (29657006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e08bddb91ea3ca1853adfc84a048668d647ae7fcde9dccca2f849a8b14f192`  
		Last Modified: Tue, 19 Dec 2023 10:02:47 GMT  
		Size: 46.6 MB (46591826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9818963852ea1e4abd0b87c001745b3c7ca8b6dfd2f9abf946875c1c50dc629`  
		Last Modified: Tue, 19 Dec 2023 10:02:41 GMT  
		Size: 701.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
